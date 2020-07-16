---
title: Организация товаров по категориям | Документация Майкрософт
description: Чтобы находить товары, вы можете назначить им атрибуты и упорядочить их по категориям.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: category, search, attribute, facet
ms.date: 06/22/2020
ms.author: sgroespe
ms.openlocfilehash: 206a7bcfe9152102dffbb9b2653c273dc8a27cdd
ms.sourcegitcommit: 3e9c89f90db5eaed599630299353300621fe4007
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "3528567"
---
# <a name="categorize-items"></a><span data-ttu-id="43740-103">Категоризация товаров</span><span class="sxs-lookup"><span data-stu-id="43740-103">Categorize Items</span></span>

<span data-ttu-id="43740-104">Для общего представления о товарах и упрощения их сортировки и поиска целесообразно систематизировать товары по категориям товаров.</span><span class="sxs-lookup"><span data-stu-id="43740-104">To maintain an overview of your items and to help you sort and find items, it is useful to organize your items in item categories.</span></span>

<span data-ttu-id="43740-105">Чтобы искать товары по характеристикам, можно назначить товарам атрибуты, а также категории товаров.</span><span class="sxs-lookup"><span data-stu-id="43740-105">To find items by characteristics, you can assign item attributes to items and also to item categories.</span></span> <span data-ttu-id="43740-106">Дополнительные сведения см. в разделе [Работа с атрибутами продуктов](inventory-how-work-item-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="43740-106">For more information, see [Work with Item Attributes](inventory-how-work-item-attributes.md).</span></span>
<br><br>  

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4j4mo?rel=0]

## <a name="to-create-an-item-category"></a><span data-ttu-id="43740-107">Создание категории товара</span><span class="sxs-lookup"><span data-stu-id="43740-107">To create an item category</span></span>
1. <span data-ttu-id="43740-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Категории товаров**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="43740-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Categories**, and then choose the related link.</span></span>
2. <span data-ttu-id="43740-109">На странице **Категории товара** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="43740-109">On the **Item Categories** page, choose the **New** action.</span></span>
3. <span data-ttu-id="43740-110">На странице **Карточка категории товаров** заполните требуемые поля на экспресс-вкладке **Общее**.</span><span class="sxs-lookup"><span data-stu-id="43740-110">On the **Item Category Card** page, on the **General** FastTab, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="43740-111">На экспресс-вкладке **Атрибуты** укажите все атрибуты товаров для категории товара.</span><span class="sxs-lookup"><span data-stu-id="43740-111">On the **Attributes** FastTab, specify any item attributes for the item category.</span></span> <span data-ttu-id="43740-112">Дополнительные сведения см. в разделе [Назначение атрибутов товаров категориям товаров](inventory-how-work-item-attributes.md#to-assign-item-attributes-to-item-categories).</span><span class="sxs-lookup"><span data-stu-id="43740-112">For more information, see [To assign item attributes to item categories](inventory-how-work-item-attributes.md#to-assign-item-attributes-to-item-categories).</span></span>

> [!NOTE]  
> <span data-ttu-id="43740-113">Если категория товаров имеет родительскую категорию товаров, как указано в поле **Родительская категория**, то все атрибуты товаров, назначенные этой родительской категории, будут уже заполнены на экспресс-вкладке **Атрибуты**.</span><span class="sxs-lookup"><span data-stu-id="43740-113">If the item category has a parent item category, as indicated by the **Parent Category** field, then any item attributes that are assigned to that parent item category are prefilled on the **Attributes** FastTab.</span></span>

> [!NOTE]  
> <span data-ttu-id="43740-114">Атрибуты товаров, назначенные категории товаров, автоматически применяются к товарам, которые назначены этой категории товаров.</span><span class="sxs-lookup"><span data-stu-id="43740-114">Item attributes that you assign to an item category will automatically apply to the item that the item category is assigned to.</span></span>

## <a name="to-assign-an-item-category-to-an-item"></a><span data-ttu-id="43740-115">Назначение товару категории товаров</span><span class="sxs-lookup"><span data-stu-id="43740-115">To assign an item category to an item</span></span>

1. <span data-ttu-id="43740-116">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="43740-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="43740-117">Откройте карточку товара, которому нужно присвоить категорию товаров.</span><span class="sxs-lookup"><span data-stu-id="43740-117">Open the card for the item that you want to assign to an item category.</span></span>
3. <span data-ttu-id="43740-118">Нажмите кнопку выбора в поле **Код товарной категории** и выберите существующую категорию товаров.</span><span class="sxs-lookup"><span data-stu-id="43740-118">Choose the lookup button in the **Item Category Code** field and select an existing item category.</span></span> <span data-ttu-id="43740-119">Можно также выбрать действие **Создать**, чтобы сначала создать новую категорию товаров, как объясняется в разделе [Создание категории товара](inventory-how-categorize-items.md#to-create-an-item-category).</span><span class="sxs-lookup"><span data-stu-id="43740-119">Alternatively, choose the **New** action to first create a new item category as explained in [To create an item category](inventory-how-categorize-items.md#to-create-an-item-category).</span></span>

## <a name="categories-attributes-and-variants"></a><span data-ttu-id="43740-120">Категории, атрибуты и варианты</span><span class="sxs-lookup"><span data-stu-id="43740-120">Categories, attributes, and variants</span></span>

[!INCLUDE[inventory_variant](includes/inventory_variant.md)]

## <a name="see-also"></a><span data-ttu-id="43740-121">См. также</span><span class="sxs-lookup"><span data-stu-id="43740-121">See Also</span></span>

[<span data-ttu-id="43740-122">Работа с атрибутами товаров</span><span class="sxs-lookup"><span data-stu-id="43740-122">Work with Item Attributes</span></span>](inventory-how-work-item-attributes.md)  
[<span data-ttu-id="43740-123">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="43740-123">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="43740-124">Запасы</span><span class="sxs-lookup"><span data-stu-id="43740-124">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="43740-125">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="43740-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
