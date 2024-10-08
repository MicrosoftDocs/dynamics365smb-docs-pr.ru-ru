---
title: Упорядочение товаров по категориям
description: 'Чтобы находить товары, вы можете назначить им атрибуты и упорядочить их по категориям.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'category, search, attribute, facet'
ms.search.form: '5730, 5733, 5401'
ms.date: 06/10/2024
ms.service: dynamics-365-business-central
---

# <a name="categorize-items"></a>Категоризация товаров

Для общего представления о товарах и упрощения их сортировки и поиска полезно систематизировать товары по категориям товаров.

Чтобы искать товары по характеристикам, можно назначить товарам атрибуты, а также категории товаров. Дополнительные сведения см. в разделе [Работа с атрибутами продуктов](inventory-how-work-item-attributes.md).
<br><br>  

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4j4mo?rel=0]

## <a name="to-create-an-item-category"></a>Создание категории товара
1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Категории товаров**, а затем выберите связанную ссылку.
2. На странице **Категории товара** выберите действие **Создать**.
3. На странице **Карточка категории товаров** заполните требуемые поля на экспресс-вкладке **Общее**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. На экспресс-вкладке **Атрибуты** укажите все атрибуты товаров для категории товара. Дополнительные сведения см. в разделе [Назначение атрибутов товаров категориям товаров](inventory-how-work-item-attributes.md#assign-item-attributes-to-item-categories).

> [!NOTE]  
> Если категория товаров имеет родительскую категорию товаров, как указано в поле **Родительская категория**, то все атрибуты товаров, назначенные этой родительской категории, будут уже заполнены на экспресс-вкладке **Атрибуты**.

> [!NOTE]  
> Атрибуты товаров, назначенные категории товаров, автоматически применяются к товарам, которые назначены этой категории товаров.

Если вы передумали относительно категории предметов, вы можете удалить ее. Однако если категория назначена товару, необходимо сначала удалить это назначение.

## <a name="to-assign-an-item-category-to-an-item"></a>Назначение товару категории товаров

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок введите **Товары**, а затем выберите связанную ссылку.
2. Откройте карточку товара, которому нужно присвоить категорию товаров.
3. Нажмите кнопку выбора в поле **Код товарной категории** и выберите существующую категорию товаров. Можно также выбрать действие **Создать**, чтобы сначала создать новую категорию товаров, как объясняется в разделе [Создание категории товара](inventory-how-categorize-items.md#to-create-an-item-category).

## <a name="categories-attributes-and-variants"></a>Категории, атрибуты и варианты

[!INCLUDE[inventory_variant](includes/inventory_variant.md)]

## <a name="see-also"></a>См. также

[Работа с атрибутами элемента](inventory-how-work-item-attributes.md)    
[Управление вариантами продукта](inventory-item-variants.md)    
[Регистрация новых товаров](inventory-how-register-new-items.md)    
[Наличие](inventory-manage-inventory.md)    
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
