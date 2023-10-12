---
title: Интеграция с Dynamics 365 Sales
description: 'Узнайте, как подготовить Dynamics 365 Business Central к интеграции с Dynamics 365 Sales.'
author: brentholtorf
ms.topic: conceptual
ms.search.keywords: 'sales, crm, integration, integrating'
ms.date: 09/28/2023
ms.author: bholtorf
ms.custom: bap-template
---
# Интеграция с Dynamics 365 Sales

[!INCLUDE[azure-ad-to-microsoft-entra-id](~/../shared-content/shared/azure-ad-to-microsoft-entra-id.md)]

Роль менеджера по продажам часто рассматривается как самая направленная наружу должность в бизнесе. Однако может быть полезно для менеджеров по продажам посмотреть внутрь бизнеса и увидеть, что происходит на заднем дворе. Путем интеграции [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] вы можете дать своим продавцам эту информацию. Интеграция позволит людям просматривать информацию в [!INCLUDE[prod_short](includes/prod_short.md)] во время работы в [!INCLUDE[crm_md](includes/crm_md.md)]. Например, при подготовке предложения по продаже может быть полезно знать, имеется ли достаточно запасов для выполнения заказа. Дополнительные сведения см. в разделе [Использование Dynamics 365 Sales из Business Central](marketing-integrate-dynamicscrm.md).

> [!NOTE]
> В этом разделе описывается процесс интеграции сетевых версий [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[prod_short](includes/prod_short.md)] через [!INCLUDE[prod_short](includes/cds_long_md.md)]. Сведения о локальной конфигурации см. в разделе [Подготовка Dynamics 365 Sales к локальной интеграции](/dynamics365/business-central/dev-itpro/administration/prepare-dynamics-365-for-sales-for-integration).

## Интеграция через Dataverse
Чтобы упростить подключение и синхронизацию данных с другими приложениями Dynamics 365, [!INCLUDE[prod_short](includes/prod_short.md)] также интегрируется с [!INCLUDE[prod_short](includes/cds_long_md.md)]. Например, вы можете подключиться к [!INCLUDE[crm_md](includes/crm_md.md)] или даже к приложениям, которые вы создаете сами. Если вы впервые выполняете интеграцию, это следует сделать это через [!INCLUDE[prod_short](includes/cds_long_md.md)]. Дополнительные сведения см. в разделе [Интеграция с Dataverse](admin-common-data-service.md).

Если вы уже интегрировали [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[prod_short](includes/prod_short.md)], вы можете продолжить синхронизацию данных, используя ваши настройки. Однако, если вы обновите или выключите интеграцию [!INCLUDE[crm_md](includes/crm_md.md)], чтобы включить его снова, вы должны подключиться через [!INCLUDE[prod_short](includes/cds_long_md.md)]. Дополнительные сведения см. в разделе [Обновление интеграции с Dynamics 365 Sales](admin-upgrade-sales-to-cds.md).

> [!NOTE]
> При повторном подключении через [!INCLUDE[prod_short](includes/cds_long_md.md)] применяются настройки синхронизации по умолчанию и перезаписываются все ваши конфигурации. Например, будут применены сопоставления таблиц по умолчанию.

## Параметры интеграции, специфичные для интеграции [!INCLUDE[crm_md](includes/crm_md.md)]
Интеграция с [!INCLUDE[prod_short](includes/prod_short.md)] происходит через [!INCLUDE[prod_short](includes/cds_long_md.md)], предусмотрено множество стандартных настроек и таблиц. В дополнение к стандартным настройкам, есть некоторые, которые являются специфическими для [!INCLUDE[crm_md](includes/crm_md.md)]. Настройки перечислены в следующих разделах.

## Разрешения и роли безопасности для учетных записей пользователей в Sales
При установке решения интеграции разрешения для учетной записи пользователя интеграции настраиваются. Если эти разрешения изменены, вам может потребоваться сбросить их. Вы можете сделать это, переустановив решение интеграции, выбрав **Повторить развертывание решения интеграции** на странице **Настройка подключения Dynamics 365**. Развернуты следующие роли безопасности:

* Администратор интеграции Dynamics 365 Business Central
* Пользователь интеграции Dynamics 365 Business Central
* Пользователь наличия товара Dynamics 365 Business Central

### Настройки подключения в руководстве по установке
Вы можете использовать мастер настройки, чтобы быстро настроить подключение и указать расширенные функции, такие как связи между записями.

1. Выберите **Настройка и расширения**, затем выберите **Мастер настройки**.
2. Выберите **Настройка подключения к Dynamics 365 Sales**, чтобы запустить мастер настройки.
3. Заполните соответствующим образом поля.
4. При желании можно использовать расширенные параметры, которые могут повысить безопасность и предоставить дополнительные возможности. Расширенные параметры рассматриваются в таблице ниже.  

| Поле | Описанием |
|--|--|
| **Импорт решения Dynamics 365 Sales** | Установите и настройте решение интеграции в [!INCLUDE[crm_md](includes/crm_md.md)]. <!--For more information, see [About the Base CDS Integration Solution](admin-common-data-service.md#about-the-business-central-integration-solution). Need to add a new topic--> |
|**Автоматическая синхронизация наличия товаров**|Указывает, что очередь работ для наличия товаров должна быть запланирована. Очередь работы запускается каждые 30 минут и обновляет доступность связанных товаров.|
| **Включить интеграцию с заказом на продажу** | Когда сотрудники создают заказы на продажу в [!INCLUDE[crm_md](includes/crm_md.md)] и выполняют заказы в [!INCLUDE[prod_short](includes/prod_short.md)], эта настройка процесс в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Включение интеграции обработки заказов на продажу](/dynamics365/customer-engagement/sales-enterprise/developer/enable-sales-order-processing-integration). Вы должны предоставить учетные данные для учетной записи пользователя-администратора в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Обработка данных в заказах на продажу](marketing-integrate-dynamicscrm.md#handling-sales-order-data). |
|**Включить подключение к Dynamics 365 Sales** | Включите подключение к [!INCLUDE[crm_md](includes/crm_md.md)]. |
| **Версия SDK Dynamics 365** | Это необходимо только в том случае, если выполняется интеграция с локальной версией [!INCLUDE[crm_md](includes/crm_md.md)]. Этот SDK является комплектом разработки программного обеспечения Dynamics 365 (также называемый Xrm), который используется для подключения [!INCLUDE[prod_short](includes/prod_short.md)] к [!INCLUDE[crm_md](includes/crm_md.md)]. Версия должна быть совместима с версией пакета SDK, которая используется [!INCLUDE[crm_md](includes/crm_md.md)], и равна или новее версии, используемой [!INCLUDE[crm_md](includes/crm_md.md)]. |

### Параметры подключения на странице настройки подключения Microsoft Dynamics 365

Введите следующие сведения для подключения из [!INCLUDE[prod_short](includes/prod_short.md)] к [!INCLUDE[crm_md](includes/crm_md.md)].

| Поле | Описанием |
|--|--|
|**URL-адрес Dynamics 365 Sales**|URL-адрес вашего экземпляра [!INCLUDE[crm_md](includes/crm_md.md)]. Этот параметр позволяет пользователям открывать записи в [!INCLUDE[prod_short](includes/prod_short.md)], которые соответствуют записям в [!INCLUDE[crm_md](includes/crm_md.md)]. Например, счет или продукт. Записи [!INCLUDE[prod_short](includes/prod_short.md)] открываются в [!INCLUDE[prod_short](includes/prod_short.md)].|
|**Автоматическая синхронизация наличия товаров**|Указывает, что очередь работ для наличия товаров должна быть запланирована. Очередь работы запускается каждые 30 минут и обновляет доступность связанных товаров.|
|**Версия SDK Dynamics 365**|Если выполняется интеграция с локальной версией [!INCLUDE[crm_md](includes/crm_md.md)], следует использовать набор разработки программного обеспечения Dynamics 365 (также называемый Xrm) для подключения [!INCLUDE[prod_short](includes/prod_short.md)] к [!INCLUDE[crm_md](includes/crm_md.md)]. Выбранная версия должна быть совместима с версией SDK, которая используется приложением [!INCLUDE[crm_md](includes/crm_md.md)]. Эта версия равна или новее версии, используемой приложением [!INCLUDE[crm_md](includes/crm_md.md)].|

В дополнение к приведенным выше параметрам введите следующие настройки для [!INCLUDE[crm_md](includes/crm_md.md)].

| Поле | Описание |
|--|--|
| **Интеграция заказов на продажу разрешена** | Разрешите пользователям отправлять заказы на продажу и активированные предложения в [!INCLUDE[crm_md](includes/crm_md.md)] и затем просматривать и обрабатывать их в [!INCLUDE[prod_short](includes/prod_short.md)]. Эта настройка интегрирует процесс в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Включение интеграции обработки заказов на продажу](/dynamics365/customer-engagement/sales-enterprise/developer/enable-sales-order-processing-integration). |
| **Автоматически создавать заказы на продажу** | Создание заказов на продажу в [!INCLUDE[prod_short](includes/prod_short.md)], когда пользователь создает и отправляет заказ на продажу в [!INCLUDE[crm_md](includes/crm_md.md)]. |
| **Автоматически обрабатывать предложения по продаже** | Обработка предложения по продаже в [!INCLUDE[prod_short](includes/prod_short.md)], когда пользователь создает и активирует его в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Обработка данных в предложениях по продаже](/dynamics365/business-central/marketing-integrate-dynamicscrm?tabs=new-experience#handling-sales-quotes-data). |
|**Двунаправленная синхронизация заказов на продажу**|Синхронизируйте заказы на продажу в обоих направлениях. Например, если клиент передумал о продукте или количестве, которое он заказал в [!INCLUDE[crm_md](includes/crm_md.md)], вы можете архивировать документ продажи и создать новый в [!INCLUDE[prod_short](includes/prod_short.md)]. То же самое относится и к изменениям в [!INCLUDE[prod_short](includes/prod_short.md)]. Например, при изменении цен, сумм налогов или ожидаемых дат отгрузки эти изменения автоматически синхронизируются с [!INCLUDE[crm_md](includes/crm_md.md)]. Двунаправленная синхронизация помогает держать ваших продавцов в курсе последних изменений и статуса предложений и заказов.|

<!--
### User Account Settings
Integration with Business Central through Dataverse requires an administrator user account and an account that is used only for the connection between the apps. This account is called the "integration user." When you install the CDS Base Integration Solution, permissions for the integration user account are configured in [!INCLUDE[crm_md](includes/crm_md.md)]. If those permissions are changed you might need to reset them. You can do that by reinstalling the Integration Solution or by manually resetting them. The following tables list the minimum permissions for the user accounts in [!INCLUDE[crm_md](includes/crm_md.md)].  -->

### Сопоставление стандартных объектов Sales для синхронизации

Объекты в [!INCLUDE[crm_md](includes/crm_md.md)], например заказы, интегрируются с эквивалентными типами таблиц в [!INCLUDE[prod_short](includes/prod_short.md)], например заказы на продажу. Для работы с данными [!INCLUDE[crm_md](includes/crm_md.md)] нужно настроить ссылки, называемые связываниями, между таблицами в [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[prod_short](includes/prod_short.md)].

В следующей таблице перечислено стандартное соответствие между таблицами в [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[crm_md](includes/crm_md.md)], которое предоставляет [!INCLUDE[prod_short](includes/prod_short.md)].

| [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[crm_md](includes/crm_md.md)] | Направление синхронизации | Фильтр по умолчанию |
|--|--|--|--|
| Единица измерения | Группа единиц | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Товар | Продукт | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | Тип контактов Sales: **Тип продукта** — **Товарный запас** |
| Ресурс | Продукт | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | Тип контактов Sales: **Тип продукта** — **Услуги** |
| Единица измерения товара | CRM UOM |[!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
| Единица измерения ресурса | CRM UOM |[!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]||
| Группа единиц | CRM Uomschedule | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] ||
| Ценовая группа клиента | Прайс-лист | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Цена продажи | Прайс-лист на продукцию | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] | Фильтр контактов [!INCLUDE[prod_short](includes/prod_short.md)]: **Код продажи** не пустой, **Тип продажи** — **Ценовая группа клиента** |
| Возможная сделка | Возможная сделка | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] |  |
| Заголовок счета продажи | Счет | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Строка счета продажи | Продукт счета | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Заголовок заказа на продажу | Заказ на продажу | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] <br><br> Для синхронизации в обоих направлениях необходимо включить **Двунаправленная синхронизация заказов на продажу** на странице **Настройка подключения Dynamics 365**.| Фильтр заголовков продаж [!INCLUDE[prod_short](includes/prod_short.md)]: **Тип документа** — Заказ, **Статус** — Выпущено |
| Примечания заказа на продажу | Примечания заказа на продажу | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] |  |

> [!NOTE]
> Сопоставления для таблиц единиц измерения номенклатур, единицы измерения ресурсов и группы единиц доступны только в том случае, если ваш администратор включил **Обновление функции: синхронизация нескольких единиц измерения с Dynamics 365 Sales** на странице **Управление функциями**. Для получения дополнительной информации прочтите [Синхронизация номенклатур и ресурсов с товарами в разных единицах измерения](admin-prepare-dynamics-365-for-sales-for-integration.md#synchronizing-items-and-resources-with-products-with-different-units-of-measure).

## Синхронизация номенклатур и ресурсов с товарами с разными единицами измерения
Компании часто производят или покупают товары в одной единице измерения, а затем продают их в другой. Чтобы синхронизировать элементы, в которых используется несколько единиц измерения, необходимо включить **Обновление функции: синхронизация нескольких единиц измерения с Dynamics 365 Sales** на странице **Управление функциями**. 

Когда вы включите обновлений функций, создается новая таблица групп единиц, которая назначается каждому товару и ресурсу в [!INCLUDE[prod_short](includes/prod_short.md)]. Таблицы позволяют сопоставить таблицы «Группа единиц», «Единица измерения товара» и «Единица измерения ресурса» в [!INCLUDE[prod_short](includes/prod_short.md)] с группой единиц Dynamics 365 Sales в [!INCLUDE[crm_md](includes/crm_md.md)]. На следующем изображении показаны сопоставления.

:::image type="content" source="media/unit group 1.png" alt-text="Отображение таблиц для групп единиц":::

Вы можете создать несколько единиц измерения для каждой группы единиц и назначить группы для продуктов в [!INCLUDE[crm_md](includes/crm_md.md)]. После этого вы сможете синхронизировать продукты с товарами и ресурсами в [!INCLUDE[prod_short](includes/prod_short.md)]. Вы можете вручную связать единицы измерения товаров или единицы измерения ресурса с группой единиц. Когда вы это сделаете, если группа единиц для товара или ресурса не связана с группой единиц в [!INCLUDE[crm_md](includes/crm_md.md)], например, потому что группа единиц не существует, [!INCLUDE[prod_short](includes/prod_short.md)] автоматически создаст группу единиц в [!INCLUDE[crm_md](includes/crm_md.md)].

### Сопоставление товаров и ресурсов с продуктами
Когда вы включаете **Обновление функции: синхронизация нескольких единиц измерения с Dynamics 365 Sales**, происходит следующее:

* Новые сопоставления создаются для товаров и ресурсов.
* Существующие сопоставления удаляются. <!--which mappings?-->
* Обновление данных создает группы единиц для товаров и ресурсов.

Чтобы использовать новые сопоставления, необходимо синхронизировать группы единиц, единицу измерения товара и единицу измерения ресурса. Вы также должны повторно синхронизировать товары и ресурсы. 

> [!NOTE]
> [!INCLUDE[crm_md](includes/crm_md.md)] не позволяет изменять группу единиц продукта. Следовательно, вы должны списать свои продукты и отвязать товары и ресурсы, а затем синхронизировать, создав новые продукты в [!INCLUDE[crm_md](includes/crm_md.md)]. 

Следующие шаги описывают шаги для начала сопоставления групп единиц:

1. Убедитесь, что продукты в [!INCLUDE[crm_md](includes/crm_md.md)] не связаны с товарами или ресурсами в [!INCLUDE[prod_short](includes/prod_short.md)]. Если они связаны, перейдите на страницы **Продукты** и/или **Ресурсы** и используйте параметры фильтра, чтобы выбрать связанные записи. Затем выберите действие **Dynamics 365 Sales** и выберите **Отменить связывание**. Это действие планирует фоновое задание для разъединения записей. Пока задание выполняется, вы можете проверить его статус, используя действие **Журнал синхронизации**. Дополнительные сведения см. в разделе [Связывание и синхронизация](admin-how-to-couple-and-synchronize-records-manually.md). 
2. Поскольку что новые продукты будут создаваться в [!INCLUDE[crm_md](includes/crm_md.md)] с новыми группами единиц, чтобы избежать дублирования имен, выполните одно из следующих действий:
    
    * Переименуйте свои продукты, а затем удалите их в [!INCLUDE[crm_md](includes/crm_md.md)]. Для получения дополнительной информации см. [Списание продуктов (Центр продаж)](/dynamics365/sales-enterprise/retire-product). Для массового редактирования ваших продуктов в Microsoft Excel, войдите в Power Apps, выберите среду, перейдите в таблицу **Продукт** и выберите вкладку **Данные**. Удалите все примененные фильтры. В группе **Данные** выберите действие **Редактировать данные в Excel**. Добавьте префикс или суффикс к связанным продуктам, а затем удалите их.
    * Спишите свои продукты и удалите их. 

3. Выполните следующие действия для синхронизации **Группы единиц**, **Единица измерения**, **Товары** и **Ресурсы**:
    1. В [!INCLUDE[prod_short](includes/prod_short.md)] откройте страницу **Настройка подключения Dynamics 365 Sales**.
    2. Используйте действие **Запустить полную синхронизацию**, чтобы открыть страницу **Просмотр полной синхронизации Dataverse**.
    3. Для сопоставлений **UOM ТОВАРА**, **UOM РЕСУРСА** И **ГРУППА ЕДИНИЦ** выберите действие **Рекомендовать полную синхронизацию**.
    4. Выберите действие **Синхронизировать все**.

    > [!NOTE]
    > Для сопоставлений, которые еще не были полностью синхронизированы, это действие полностью синхронизирует их. Чтобы предотвратить синхронизацию этих сопоставлений, удалите сопоставления со страницы. Это только удаляет их из текущей полной синхронизации, но не удаляет сопоставления.
    
5. Выберите сопоставление **ТОВАР-ПРОДУКТ**, а затем выберите действие **Перезапустить**. Перезапуск создает новые продукты из товаров в [!INCLUDE[crm_md](includes/crm_md.md)] и назначает новую группу единиц, относящуюся к товару.
6. Выберите сопоставление **РЕСУРС-ПРОДУКТ**, а затем выберите действие **Перезапустить**. Перезапуск создает новые продукты из ресурсов в [!INCLUDE[crm_md](includes/crm_md.md)] и назначает новую группу единиц, относящуюся к ресурсам.

### Правила синхронизации

В следующей таблице перечислены правила, управляющие синхронизацией между [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[prod_short](includes/prod_short.md)]. Эти правила дополняют правила, определенные для Dataverse, которые также применяются. Дополнительные сведения см. в разделе [Сопоставление стандартных сущностей](admin-synchronizing-business-central-and-sales.md#standard-table-mapping-for-synchronization).

> [!NOTE]  
> Изменения данных, которые были сделаны в учетной записи пользователя интеграции, не синхронизируются. Поэтому рекомендуется не изменять данные при использовании этой учетной записи. Дополнительные сведения см. в разделе [Настройка учетных записей пользователей для интеграции с Dynamics 365 Sales](admin-setting-up-integration-with-dynamics-sales.md).

|Стол|Правило|
|-----|----|
|Единицы измерения|Единицы измерения синхронизируются с группами единиц в [!INCLUDE[crm_md](includes/crm_md.md)]. Для группы единиц может быть задана только одна единица измерения.|
|Товаров|При синхронизации товаров с продуктами [!INCLUDE[crm_md](includes/crm_md.md)], [!INCLUDE[prod_short](includes/prod_short.md)] автоматически создает прайс-лист в [!INCLUDE[crm_md](includes/crm_md.md)]. Чтобы избежать ошибок синхронизации, не следует изменять данный прайс-лист вручную.|
|Ресурсы|Ресурсы синхронизируются с продуктами [!INCLUDE[crm_md](includes/crm_md.md)], имеющими тип "Услуга".|
|Ценовые группы клиентов|Ценовые группы клиентов синхронизируются с прайс-листами Sales.|
|Цены продажи|Цены Sales с типом продажи "Ценовая группа клиента" и определенным кодом продаж, синхронизируются со строками прайс-листов [!INCLUDE[crm_md](includes/crm_md.md)].|
|Возможные сделки|Возможные сделки синхронизируются с возможными сделками [!INCLUDE[crm_md](includes/crm_md.md)]. Значение кода менеджера по продажам определяет владельца связанной таблицы в [!INCLUDE[crm_md](includes/crm_md.md)].|
|Учтенные счета продажи|Учтенные счета продажи синхронизируются со счетами продажи. Прежде чем счет можно будет синхронизировать, рекомендуется синхронизировать все остальные таблицы, которые могут быть использованы в нем, от менеджеров по продажам до прайс-листов. Значение кода менеджера по продажам в заголовке счета определяет владельца связанной таблицы в Sales.|
|Заказы на продажу|Когда включена интеграция заказов на продажу, заказы на продажу в [!INCLUDE[prod_short](includes/prod_short.md)], которые созданы из отправленных заказов на продажу в [!INCLUDE[crm_md](includes/crm_md.md)], синхронизируются с заказами на продажу в [!INCLUDE[crm_md](includes/crm_md.md)], когда они выпущены. Прежде чем синхронизировать заказы, рекомендуется сначала синхронизировать все таблицы, связанные с заказом, такие как продавцы и прайс-листы. Поле кода менеджера по продажам в заголовке заказа определяет владельца связанной таблицы в [!INCLUDE[crm_md](includes/crm_md.md)].|

### Задания синхронизации для интеграции Sales

Задания выполняются в следующем порядке во избежание зависимостей связывания между таблицами. Есть дополнительные задания, доступные из Dataverse. Дополнительные сведения см. в разделе [Использование очередей работ для планирования задач](./admin-job-queues-schedule-tasks.md).

1. Задание синхронизации "ЕДИНИЦА ИЗМЕРЕНИЯ — Dynamics 365 Sales"  
2. Задание синхронизации "РЕСУРС-ПРОДУКТ - Dynamics 365 Sales"  
3. Задание синхронизации "ТОВАР-ПРОДУКТ — Dynamics 365 Sales"  
4. Задание синхронизации "CUSTPRCGRP-PRICE — Dynamics 365 Sales".
5. Задание синхронизации "SALESPRC-PRODPRICE — Dynamics 365 Sales".
6. Задание синхронизации "POSTEDSALESINV-INV — Dynamics 365 Sales".

### Операции очереди заданий синхронизации по умолчанию

В следующей таблице описываются задания синхронизации по умолчанию для Sales.  

|Операция очереди работ|Описание|Направление|Сопоставление таблиц интеграции|Частота синхронизации по умолчанию (мин)|Время бездействия по умолчанию (мин)|  
|---------------------|---------------------------------------|---------------|-------------------------------|-----|-----|  
|Задание синхронизации "ЕДИНИЦА ИЗМЕРЕНИЯ — Dynamics 365 Sales"|Синхронизирует группы единиц [!INCLUDE[crm_md](includes/crm_md.md)] с единицами измерения [!INCLUDE[prod_short](includes/prod_short.md)].|Из [!INCLUDE[prod_short](includes/prod_short.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|ЕДИНИЦА ИЗМЕРЕНИЯ|30|720<br> (12 ч.)|
|Задание синхронизации "РЕСУРС-ПРОДУКТ - Dynamics 365 Sales"|Синхронизирует продукты [!INCLUDE[crm_md](includes/crm_md.md)] с ресурсами [!INCLUDE[prod_short](includes/prod_short.md)].|Из [!INCLUDE[prod_short](includes/prod_short.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|РЕСУРС-ПРОДУКТ|30|720<br> (12 ч.)|
|Задание синхронизации "ТОВАР-ПРОДУКТ — Dynamics 365 Sales"|Синхронизирует продукты [!INCLUDE[crm_md](includes/crm_md.md)] с товарами [!INCLUDE[prod_short](includes/prod_short.md)].|Из [!INCLUDE[prod_short](includes/prod_short.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|ТОВАР-ПРОДУКТ|30|1440<br> (24 ч.)|
|Задание синхронизации "CUSTPRCGRP-PRICE — Dynamics 365 Sales"|Синхронизирует прайс-листы продаж [!INCLUDE[crm_md](includes/crm_md.md)] с ценовыми группами клиентов [!INCLUDE[prod_short](includes/prod_short.md)].| |ЦЕНОВЫЕ ГРУППЫ КЛИЕНТОВ — ПРАЙС-ЛИСТЫ ПРОДАЖ|30|1440<br> (24 ч.)|
|Задание синхронизации "SALESPRC-PRODUCTPRICE — Dynamics 365 Sales"|Синхронизирует цены продуктов [!INCLUDE[crm_md](includes/crm_md.md)] с ценами продажи [!INCLUDE[prod_short](includes/prod_short.md)].||ЦЕНА ПРОДУКТА — ЦЕНА ПРОДАЖ|30|1440<br> (24 ч.)|
|Задание синхронизации "POSTEDSALESINV-INV — Dynamics 365 Sales"|Синхронизирует счета [!INCLUDE[crm_md](includes/crm_md.md)] с учтенными счетами продаж [!INCLUDE[prod_short](includes/prod_short.md)].|Из [!INCLUDE[prod_short](includes/prod_short.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|СЧЕТА — УЧТЕННЫЕ СЧЕТА ПРОДАЖ|30|1440<br> (24 ч.)|
|Синхронизация "Статистика по клиенту — Dynamics 365 Sales"|Обновление организаций [!INCLUDE[crm_md](includes/crm_md.md)] с новейшими данными клиентов [!INCLUDE[prod_short](includes/prod_short.md)]. В [!INCLUDE[crm_md](includes/crm_md.md)] данная информация отображается в форме быстрого просмотра **Статистика организации Business Central** организаций, которые связаны с клиентами [!INCLUDE[prod_short](includes/prod_short.md)].<br /><br /> Эти данные можно также обновлять вручную из каждой записи клиента. Дополнительные сведения см. в разделе [Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md). </BR></BR>**Примечание.** Эта запись очереди заданий используется только в случае установки решения интеграции [!INCLUDE[prod_short](includes/prod_short.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]. |Неприменимо|Неприменимо|30|Неприменимо| 

## Подключение к локальным версиям выпуска Business Central 2019, волны 1 и Microsoft Dynamics NAV 2018
Рабочая группа Microsoft Power Platform [объявила](/power-platform/important-changes-coming#deprecation-of-office365-authentication-type-and-organizationserviceproxy-class-for-connecting-to-dataverse), что она объявляет устаревшим тип проверки подлинности Office365. Если вы используете локальную версию [!INCLUDE[prod_short](includes/prod_short.md)], более раннюю, чем выпуск Business Central 2019 волны 1, необходимо использовать тип проверки подлинности OAuth для подключения к [!INCLUDE[crm_md](includes/crm_md.md)] Online. Шаги в этом разделе описывают, как подключить следующие версии продуктов:

* Выпуск Business Central 2019, волна 1
* Microsoft Dynamics NAV 2018

### Предварительные требования

- Вы должны иметь подписку Microsoft Azure. Пробная учетная запись будет работать для регистрации приложения.
- [!INCLUDE[crm_md](includes/crm_md.md)] настроен на использование одного из следующих типов аутентификации:

   - Office365 (устаревшая версия)

     > [!IMPORTANT]
     > С апреля 2022 года поддержка Office365 (устаревшая версия) будет прекращена. Дополнительные сведения см. в разделе [Запланированные важные изменения (устаревания) в Power Apps, Power Automate и приложениях для взаимодействия с клиентами](/power-platform/important-changes-coming#deprecation-of-office365-authentication-type-and-organizationserviceproxy-class-for-connecting-to-dataverse).

   - OAuth

### Для подключения выпуска Business Central 2019 волны 1 и Dynamics NAV 2018

1. Импортируйте решение интеграции Microsoft Dynamics 365 Business Central в вашу среду [!INCLUDE[crm_md](includes/crm_md.md)]. Решение интеграции доступно в папке CrmCustomization на установочном DVD-диске [!INCLUDE[prod_short](includes/prod_short.md)] или Dynamics NAV 2018. В зависимости от версии продукта импортируйте одно из следующих решений:

   * Для [!INCLUDE[prod_short](includes/prod_short.md)] папка содержит DynamicsNAVIntegrationSolution_v9 и DynamicsNAVIntegrationSolution_v91. решения. Решение, которое вы должны импортировать, зависит от версии [!INCLUDE[crm_md](includes/crm_md.md)], к которой вы подключаетесь. [!INCLUDE[crm_md](includes/crm_md.md)] Online требует решения интеграции DynamicsNAVIntegrationSolution_v91.
   * Для Dynamics NAV 2018 установите решение DynamicsNAVIntegrationSolution.

2. Создайте неинтерактивного пользователя интеграции в своей среде [!INCLUDE[crm_md](includes/crm_md.md)] и назначьте этому пользователю следующие роли безопасности. Дополнительные сведения см. в разделе [Создание неинтерактивной учетной записи пользователя](/power-platform/admin/create-users-assign-online-security-roles#create-a-non-interactive-user-account).

   * Администратор интеграции Dynamics 365 Business Central
   * Пользователь интеграции Dynamics 365 Business Central

   > [!Important]
   > У этого пользователя не должно быть роли безопасности системного администратора. Кроме того, вы не можете использовать учетную запись системного администратора в качестве пользователя интеграции.

3.  На портале Azure создайте регистрацию приложения для [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения см. в статье [Регистрация приложения в Microsoft Entra ID](/powerapps/developer/data-platform/walkthrough-register-app-azure-active-directory). 
  
   > [!NOTE]
   > Мы рекомендуем вам зарегистрировать приложение в том же клиенте, что и ваша среда Dataverse, поэтому вам не нужно давать согласие на доступ приложения к среде. Если вы регистрируете приложение в другой среде, вы должны войти в Microsoft Entra ID, используя учетную запись администратора для вашей среды Dataverse, и дать согласие.
   >
   > Кроме того, приложение, которое вы регистрируете, не должно иметь секрета. Подключение приложения с секретом к Dataverse доступно только в выпуске Business Central 2020 волны 1 и более поздних версиях.
  
4. В зависимости от версии продукта выполните одно из следующих действий:

    * В [!INCLUDE[prod_short](includes/prod_short.md)] найдите пункт **Настройка подключения Microsoft Dynamics 365**, затем выберите связанную ссылку. 
    * В Dynamics NAV 2018 найдите пункт **Настройка подключения Microsoft Dynamics 365 for Sales**, затем выберите связанную ссылку.

5. В поле **Тип аутентификации** выберите вариант для OAuth. 
6. Выберите версию CRM SDK, соответствующую версии решения, импортированного на шаге 1.

   > [!NOTE]
   > Этот шаг актуален только для [!INCLUDE[prod_short](includes/prod_short.md)].

7. Введите URL-адрес вашей среды [!INCLUDE[crm_md](includes/crm_md.md)], затем введите имя пользователя и пароль для пользователя интеграции. 

   * В [!INCLUDE[prod_short](includes/prod_short.md)] используйте поле **Адрес сервера**.
   * В Dynamics NAV 2018 используйте поле **URL-адрес Dynamics 365 Sales**.

8. В поле **Строка подключения** укажите идентификатор регистрации приложения. В этом поле есть два токена, в которых должен быть указан идентификатор вашего приложения.

   |Маркер           |Описание  |
   |----------------|-------------|
   |**AppId**       |Установите идентификатор приложения.      |
   |**RedirectUri** |Установите идентификатор приложения, но добавьте префикс **app://**.         |

    **Пример** В следующем примере показана строка подключения.

    ```
    AuthType=OAuth;Username=jsmith@contoso.onmicrosoft.com;Password=****;Url=https://contosotest.crm.dynamics.com;AppId=<your AppId>;RedirectUri=app://<your AppId>;TokenCacheStorePath=;LoginPrompt=Auto
    ```
9. Включите подключение.

> [!Note]
> Если вы хотите настроить подключение к экземпляру [!INCLUDE[crm_md](includes/crm_md.md)] с определенным типом проверки подлинности, заполните поля на экспресс-вкладке **Сведения о типе проверки подлинности**. Для получения дополнительной информации см. раздел [Аутентификация с веб-службами Microsoft Dataverse](/powerapps/developer/data-platform/authentication). Этот шаг не требуется при подключении к сетевой версии [!INCLUDE[prod_short](includes/prod_short.md)].

## См. также

[Настройка учетных записей пользователя для интеграции с [!INCLUDE[crm_md](includes/crm_md.md)]](admin-setting-up-integration-with-dynamics-sales.md)  
[Настройка подключения к [!INCLUDE[crm_md](includes/crm_md.md)]](admin-how-to-set-up-a-dynamics-crm-connection.md)  
[Синхронизация Business Central и [!INCLUDE[crm_md](includes/crm_md.md)]](admin-synchronizing-business-central-and-sales.md)  
[Подготовка Dynamics 365 Sales к локальной интеграции](/dynamics365/business-central/dev-itpro/administration/prepare-dynamics-365-for-sales-for-integration)


[!INCLUDE[footer-include](includes/footer-banner.md)]
