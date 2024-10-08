---
title: Создание новых записей значений для элементов в инвентаре| Microsoft Docs
description: 'Описывается, как повысить или понизить операции стоимости одного или нескольких товаров в запасах путем учета текущей вычисленной стоимости.'
documentationcenter: ''
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'costing, inventory cost, value entries'
ms.search.forms: '5803,'
ms.date: 07/29/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# <a name="revalue-inventory"></a>Переоценка запасов
Чтобы повысить или понизить стоимость изделия или конкретной учтенной товарной операции, нужно воспользоваться журналом переоценки.

## <a name="to-revalue-inventory"></a>Переоценка запасов
1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Журнал переоценки**, а затем выберите связанную ссылку.
2. Выберите действие **Расчет стоимости запасов**.
3. На странице **Расчет стоимости запасов** заполните требуемые поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Нажмите кнопку **ОК**.
5. В каждой строке на странице **Журналы переоценки позиций** в поле **Стоимость единицы (переоцененная)** введите новую стоимость единицы. Можно также ввести новую общую сумму в поле **Стоимость запасов (переоценка)**.

    Соответствующие поля обновляются автоматически. Поле **Сумма**  показывает фактическое изменение стоимости инвентаря для выбранной записи книги учета товаров. Там подсчитывается разница между полями **Стоимость запасов (расчетная)** и **Стоимость запасов (переоценка)**.
6. После того как будут заполнены все строки в журнале переоценки, выберите действие **Учет**.

Создаются новые операции стоимости, которые отражают учтенную переоценку. Новые значения можно просмотреть в соответствующей карточке товара.

## <a name="see-also"></a>См. также
[Детали проекта: Переоценка](design-details-revaluation.md)    
[Наличие](inventory-manage-inventory.md)    
[Продажи](sales-manage-sales.md)    
[Покупки](purchasing-manage-purchasing.md)    
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
