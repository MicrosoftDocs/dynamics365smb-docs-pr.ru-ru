---
title: Организация товаров по категориям | Документация Майкрософт
description: Чтобы находить товары, вы можете назначить им атрибуты и упорядочить их по категориям.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: category, search, attribute, facet
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: d75a24a065d87cee1b40149e1a30f2bc595eaa88
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3182280"
---
# <a name="categorize-items"></a>Категоризация товаров
Для общего представления о товарах и упрощения их сортировки и поиска целесообразно систематизировать товары по категориям товаров.

Чтобы искать товары по характеристикам, можно назначить товарам атрибуты, а также категории товаров. Дополнительные сведения см. в разделе [Работа с атрибутами продуктов](inventory-how-work-item-attributes.md).
<br><br>  

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4j4mo?rel=0]

## <a name="to-create-an-item-category"></a>Создание категории товара
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Категории товаров**, затем выберите соответствующую ссылку.
2. На странице **Категории товара** выберите действие **Создать**.
3. На странице **Карточка категории товаров** заполните требуемые поля на экспресс-вкладке **Общее**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. На экспресс-вкладке **Атрибуты** укажите все атрибуты товаров для категории товара. Дополнительные сведения см. в разделе [Назначение атрибутов товаров категориям товаров](inventory-how-work-item-attributes.md#to-assign-item-attributes-to-item-categories).

> [!NOTE]  
>   Если категория товаров имеет родительскую категорию товаров, как указано в поле **Родительская категория**, то все атрибуты товаров, назначенные этой родительской категории, будут уже заполнены на экспресс-вкладке **Атрибуты**.

> [!NOTE]  
>   Атрибуты товаров, назначенные категории товаров, автоматически применяются к товарам, которые назначены этой категории товаров.

## <a name="to-assign-an-item-category-to-an-item"></a>Назначение товару категории товаров
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.
2. Откройте карточку товара, которому нужно присвоить категорию товаров.
3. Нажмите кнопку выбора в поле **Код товарной категории** и выберите существующую категорию товаров. Можно также выбрать действие **Создать**, чтобы сначала создать новую категорию товаров, как объясняется в разделе [Создание категории товара](inventory-how-categorize-items.md#to-create-an-item-category).

## <a name="see-also"></a>См. также
[Работа с атрибутами товаров](inventory-how-work-item-attributes.md)  
[Регистрация новых товаров](inventory-how-register-new-items.md)  
[Запасы](inventory-manage-inventory.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
