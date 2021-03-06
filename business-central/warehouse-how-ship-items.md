---
title: Как отгружать товары | Документация Майкрософт
description: В зависимости от конфигурации склада, можно либо напрямую зарегистрировать отправку в соответствующем исходящем бизнес-документе, таком как заказ на продажу, либо использовать складские документы отгрузки, соответствующие рабочему процессу и интегрированные в различные складские операции.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 22404e97c578f6bcaaa5f74ec40408beca7fe3c8
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5782763"
---
# <a name="ship-items"></a>Отгрузка товаров

Когда товары отгружаются со склада, который не был настроен для обработки складской отгрузки, вы просто регистрируете отгрузку в соответствующем бизнес-документе, таком как заказ на продажу, сервисный заказ, заказ на возврат покупки или исходящий заказ на перемещение.

При отгрузке товаров со склада, который настроен для обработки складской отгрузки, товары можно отгружать только на основании документов-источников, выпущенных другими подразделениями организации на склад для выполнения действия.

> [!NOTE]
> Если на складе используются переброска и ячейки для каждой строки, можно просмотреть количество товаров, помещенных в ячейки переброски. Эти количества вычисляются приложением автоматически при обновлении полей отгрузки. Если товары в ячейке являются товарами для готовящейся отгрузки, подбор можно создать для всех строк, и затем завершить отгрузку. Дополнительные сведения см. в разделе [Переброска товаров](warehouse-how-to-cross-dock-items.md).

## <a name="to-ship-items-with-a-sales-order"></a>Отгрузка товаров с помощью заказа на продажу

Ниже описано, как отгружать товары из заказа на продажу. Шаги аналогичны для заказов на возврат покупки, сервисных заказов и исходящих заказов на перемещение.  

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.
2. Откройте существующий заказ на продажу или создайте новый заказ. Дополнительные сведения см. в разделе [Продажа продукции](sales-how-sell-products.md).
3. В поле **Кол-во для отгрузки** введите отгруженное количество.

    Значение в поле **Отгруж. кол-во** обновляется соответствующим образом. Если это частичная отгрузка, то это значение меньше значения в поле **Количество**.
4. Выберите действие **Учет**.

> [!NOTE]
> Если ваша организация не использует заказы на продажу, то, когда вы публикуете счет продажи, [!INCLUDE [prod_short](includes/prod_short.md)] предполагает, что вы отгрузили полное количество. Если это противоречит принципам работы вашей организации, мы рекомендуем использовать заказы на продажу и регистрировать отгрузки, как описано в этой статье.

## <a name="to-ship-items-with-a-warehouse-shipment"></a>Отгрузка товаров с помощью складской отгрузки

Сначала создается отгрузочный документ из исходного бизнес-документа. Затем следует скомплектовать товары для отгрузки.

### <a name="to-create-a-warehouse-shipment"></a>Создание складской отгрузки

Обычно сотрудник, ответственный за отгрузку, создает складскую отгрузку. Следующая процедура описывает, как создать отгрузку вручную в версии по умолчанию [!INCLUDE[prod_short](includes/prod_short.md)], но ваша организация может автоматизировать часть процесса, например, с использованием ручных или смонтированных сканеров, которые поддерживаются внешними поставщиками.  

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Складские отгрузки**, затем выберите соответствующую ссылку.  
2. Выберите действие **Создать**.  

    Заполните поля на экспресс-вкладке **Общее**. При получении строк документа-источника некоторая информация копируется в каждую строку.  

    Для конфигурации склада с расширенным подбором и размещением: если на складе имеются стандартные зоны и ячейки для отгрузки, то поля **Код зоны** и **Код ячейки** заполняются автоматически, но в них можно вносить необходимые изменения.  

    > [!NOTE]  
    > Если требуется отгрузить товары с кодами класса склада, отличающимися от кода класса ячейки из поля **Код ячейки** заголовка документа, то перед получением строк документа-источника для этих товаров необходимо удалить содержимое поля **Код ячейки** в заголовке документа.  
3. Выберите действие **Получить исходные документы**. Откроется страница **Документы-источники**.

    В новой или открытой складской отгрузке можно использовать страницу **Фильтры для получения первичных документов**, чтобы получить строки выпущенных исходных документов, определяющих товары, которые должно быть отгружены.

    1. Выберите действие **Исп. фильтры для получ. исх. документов**.  
    2. Для настройки нового фильтра введите описательный код в поле **Код**, затем выберите действие **Изменить**.  
    3. Определите тип строк документа-источника, которые следует извлечь, заполнив соответствующие поля фильтра.  
    4. Выберите действие **Выполнить**.  

    Все выпущенные строки документа-источника, которые удовлетворяют критериям фильтрации, теперь вставляются на страницу **Складская отгрузка**, из которого вы активировали функцию фильтра.  

    Определяемые пользователем комбинации фильтров сохраняются на странице **Фильтры для получения первичных документов** для последующего использования. Количество комбинаций фильтров не ограничено. Можно в любой момент изменить критерии, выбрав действие **Изменить**.

4. Выберите исходный документ, на основании которого будет проводиться отгрузка товаров, затем выберите кнопку **ОК**.  

Строки документа-источника отображаются на странице **Складская отгрузка**. Поле **Кол-во для отгрузки** заполняется информацией о недопоставленном количестве для каждой строки, но при необходимости количество можно изменить. Если содержимое поля **Код ячейки** на экспресс-вкладке **Общее** удалено до получения строк, необходимо ввести соответствующий код ячейки в каждой строке расходной накладной.  

> [!NOTE]  
> Невозможно отгрузить товаров больше, чем указано в поле **Недопоставленное кол-во** строки документа-источника. Чтобы отгрузить дополнительные товары, нужно, воспользовавшись функцией фильтрации для документов, содержащих определенный товар, вызвать другой документ-источник со строкой для данного товара.  

При наличии строк, подлежащих отгрузке, нужно запустить процесс отсылки строк работникам склада для подбора.

### <a name="to-pick-and-ship"></a>Подбор и отгрузка

Как правило, ответственный за комплектацию работник склада создается документ подбора либо открывает уже созданный документ подбора.  

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Складские отгрузки**, затем выберите соответствующую ссылку.
2. Выберите складскую отгрузочную накладную, которую требуется скомплектовать, затем выберите действие **Создать подбор**.
3. Заполните поля на странице запроса, после чего выберите кнопку **ОК**. Создается указанный документ складского подбора.

    Можно также открыть существующий складской подбор.
4. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Подборы**, затем выберите соответствующую ссылку. Выберите необходимый складской подбор.

    Если на складе используются ячейки, строки подбора будут преобразованы в строки действий "Взять" и "Поместить".

    Можно сортировать строки, назначать работника для осуществления подбора, устанавливать фильтр разбивки, если применяется расширенный подбор и размещение, и распечатывать инструкции по подбору.

5. Выполните подбор товаров и поместите их в заданную ячейку отгрузки (или в область отгрузки, если ячеек нет).
6. Выберите действие **Зарегистрировать подбор**.

    Поля **Кол-во для отгрузки** и **Статус документа** в заголовке документа отгрузки обновляются. Товары, подбор которых осуществлен, уже не доступны для подбора для других отгрузок или внутренних операций.
7. Распечатайте отгрузочные документы, подготовьте отгружаемые упаковки, затем учтите отгрузку.

Дополнительные сведения о подборе для складской отгрузки см. в разделе [Подбор товаров для складской отгрузки](warehouse-how-to-pick-items-for-warehouse-shipment.md).

Журнал подбора можно использовать также для сведения нескольких инструкций по подбору в одну инструкцию (для нескольких отгрузок), что делает процедуру подбора на складе более эффективной. Дополнительные сведения см. в разделе [Планирование подборов в журналах](warehouse-how-to-plan-picks-in-worksheets.md).

> [!NOTE]
> Если на складе ожидается прибытие конкретных товаров и используется функция переброски, то в каждой строке журнала отгрузки или подбора [!INCLUDE[prod_short](includes/prod_short.md)] вычисляет количество товара, находящегося в ячейке переброски. Это поле обновляется при каждом закрытии и открытии документа отгрузки или журнала. Дополнительные сведения см. в разделе [Переброска товаров](warehouse-how-to-cross-dock-items.md).

## <a name="see-also"></a>См. также

[Управление складом](warehouse-manage-warehouse.md)  
[Наличие](inventory-manage-inventory.md)  
[Настройка управления складом](warehouse-setup-warehouse.md)  
[Управление сборкой](assembly-assemble-items.md)  
[Сведения о проектировании: управление складом](design-details-warehouse-management.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]