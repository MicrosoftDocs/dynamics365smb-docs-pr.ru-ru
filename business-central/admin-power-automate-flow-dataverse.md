---
title: Использование потока Power Automate для своевременной синхронизации изменений сущностей Dataverse
description: 'Узнайте, как создать поток в Power Automate, который оповестит вас, когда в среде Dataverse изменяется сущность.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'Power Automate, Flow, Dataverse'
ms.search.form: null
ms.date: 09/05/2022
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# <a name="use-a-power-automate-flow-to-timely-synchronize-dataverse-entity-changes"></a>Использование потока Power Automate для своевременной синхронизации изменений сущностей Dataverse

Администраторы могут создать автоматизированный поток в Power Automate, который уведомляет ваш [!INCLUDE[prod_short](includes/prod_short.md)] об изменениях в записях в вашей организации [!INCLUDE [cds_long_md](includes/cds_long_md.md)].

> [!NOTE]
> В этой статье предполагается, что вы подключили свою онлайн-версию [!INCLUDE[prod_short](includes/prod_short.md)] с [!INCLUDE [cds_long_md](includes/cds_long_md.md)] и запланированную синхронизацию двух приложений.

## <a name="import-the-flow-template"></a>Импорт шаблона потока

> [!TIP]
> Чтобы упростить настройку потока, мы создали шаблон, который определит для вас триггер потока и условие потока. Чтобы использовать шаблон, выполните действия, описанные в этом разделе. Чтобы создать поток самостоятельно, пропустите этот раздел и начните с шагов, описанных в разделе [Определение триггера потока](#define-the-flow-trigger).

1. Войдите в [Power Automate](https://powerautomate.microsoft.com).
2. Выберите **Шаблоны**, затем найдите **Уведомление Business Central**.

:::image type="content" source="media/power-automate-import-template.png" alt-text="Ключевые слова для поиска шаблона потока.":::
3. Выберите шаблон **Уведомить Business Central при изменении учетной записи**.
4. Далее переходите к шагам из раздела [Уведомить Business Central об изменении](#notify-business-central-about-a-change).

## <a name="define-the-flow-trigger"></a>Определение триггера потока

1. Войдите в [Power Automate](https://flow.microsoft.com).
2. Создайте автоматический облачный поток, который запускается, когда строка для сущности [!INCLUDE [cds_long_md](includes/cds_long_md.md)] добавляется, изменяется или удаляется. Для получения дополнительной информации см. раздел [Запуск потоков при добавлении, изменении или удалении строки](/power-automate/dataverse/create-update-delete-trigger). В этом примере используется сущность **Учетные записи**. На следующем изображении показаны настройки для первого шага определения триггера потока.

:::image type="content" source="media/power-automate-flow-dataverse-trigger.png" alt-text="Настройки триггера потока":::
3. Используйте кнопку **AssistEdit (...)** в правом верхнем углу, чтобы добавить подключение к вашей среде [!INCLUDE [cds_long_md](includes/cds_long_md.md)].
4. Выберите **Показать дополнительные параметры**, а в поле **Фильтр строк** введите **customertypecode eq 3** или **customertypecode eq 11** и **statecode eq 0**. Эти значения означают, что триггер будет срабатывать только при внесении изменений в активные учетные записи типа **клиент** или **поставщик**.

## <a name="define-the-flow-condition"></a>Определение условия потока

Данные синхронизируются между [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE [cds_long_md](includes/cds_long_md.md)] через учетную запись пользователя интеграции. Чтобы игнорировать изменения, внесенные при синхронизации, создайте в своем потоке шаг условия, исключающий изменения, внесенные учетной записью пользователя интеграции.  

1. Добавьте шаг **Получить строку по ID из Dataverse** после триггера потока со следующими настройками. Для получения дополнительной информации см. раздел [Получение строки по ID из Dataverse](/power-automate/dataverse/get-row-id).

    1. В поле **Имя таблицы** выберите **Пользователи**
    2. В поле **Идентификатор строки** выберите **Кем изменено (значение)** из триггера потока.  

2. Добавьте шаг условия со следующими параметрами **или** для идентификации учетной записи пользователя интеграции.
    1. **Основной адрес электронной почты** пользователя содержит **contoso.com**
    2. **Полное имя** пользователя содержит **[!INCLUDE[prod_short](includes/prod_short.md)]**.

3. Добавьте элемент управления «Завершить», чтобы остановить поток, если сущность была изменена учетной записью пользователя интеграции.

На следующем изображении показано, как определить триггер потока и условие потока.

:::image type="content" source="media/power-automate-flow-dataverse.png" alt-text="Обзор настроек триггера потока и условий":::

## <a name="notify-business-central-about-a-change"></a>Уведомление Business Central об изменении

Если поток не остановлен условием, вы должны уведомить [!INCLUDE[prod_short](includes/prod_short.md)], что произошло изменение. Для этого используйте соединитель [!INCLUDE[prod_short](includes/prod_short.md)].

1. В ветке **Нет** шага условия добавьте действие и найдите **Dynamics 365 [!INCLUDE[prod_short](includes/prod_short.md)]**. В списке выберите значок соединителя.
2. Выберите действие **Создать запись (V3)**.

:::image type="content" source="media/power-automate-flow-dataverse-connector.png" alt-text="Параметры соединителя [!INCLUDE[prod_short](includes/prod_short.md)]":::

3. Используйте кнопку **помощь в изменении (...)** в правом верхнем углу, чтобы добавить подключение к вашему [!INCLUDE[prod_short](includes/prod_short.md)].
4. При подключении заполните поля **Имя среды** и **Название компании**.
5. В поле **Категория API** введите **microsoft/dataverse/v1.0**.
6. В поле **Имя таблицы** введите **dataverseEntityChanges**.
7. В поле **entityName** введите **учетная запись**.
8. Сохраните поток.

На изображении ниже показано, как должен выглядеть ваш поток.

:::image type="content" source="media/power-automate-flow-dataverse-summary.png" alt-text="Обзор всех настроек потока":::

Когда вы добавляете, удаляете или изменяете учетную запись в среде [!INCLUDE [cds_long_md](includes/cds_long_md.md)], этот поток будет выполнять следующие действия:

1. Вызывать среду [!INCLUDE[prod_short](includes/prod_short.md)], которую вы указали в соединителе [!INCLUDE[prod_short](includes/prod_short.md)].
2. Использовать API [!INCLUDE[prod_short](includes/prod_short.md)] для вставки записи со значением **учетная запись** для параметра **entityName** в таблице **Изменение элемента Dataverse**. Этот параметр является точным названием сущности Dataverse, для которой создается поток.
3. [!INCLUDE[prod_short](includes/prod_short.md)] запустит элемент очереди заданий, который синхронизирует клиентов с учетными записями.

## <a name="see-also"></a>См. также

[Использование Business Central в потоках Power Automate](across-how-use-financials-data-source-flow.md)  
[Настройка автоматизированных рабочих процессов](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows)  
[Интеграция с Microsoft Dataverse](admin-common-data-service.md)  
[Синхронизация данных в Business Central с Microsoft Dataverse](admin-synchronizing-business-central-and-sales.md)  
