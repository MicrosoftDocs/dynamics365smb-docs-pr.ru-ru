---
title: "Организация товаров по категориям | Документы Майкрософт"
description: "Чтобы находить товары, вы можете назначить им атрибуты и упорядочить их по категориям."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: category, search, attribute, facet
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f7f40054c511b5f3bf1d61dc40d6107cc717dcd8
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="categorize-items"></a><span data-ttu-id="d649f-103">Категоризация товаров</span><span class="sxs-lookup"><span data-stu-id="d649f-103">Categorize Items</span></span>
<span data-ttu-id="d649f-104">Для общего представления о товарах и упрощения их сортировки и поиска целесообразно систематизировать товары по категориям товаров.</span><span class="sxs-lookup"><span data-stu-id="d649f-104">To maintain an overview of your items and to help you sort and find items, it is useful to organize your items in item categories.</span></span>

<span data-ttu-id="d649f-105">Чтобы искать товары по характеристикам, можно назначить товарам атрибуты, а также категории товаров.</span><span class="sxs-lookup"><span data-stu-id="d649f-105">To find items by characteristics, you can assign item attributes to items and also to item categories.</span></span> <span data-ttu-id="d649f-106">Дополнительные сведения см. в разделе [Работа с атрибутами продуктов](inventory-how-work-item-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="d649f-106">For more information, see [Work with Item Attributes](inventory-how-work-item-attributes.md).</span></span>

## <a name="to-create-an-item-category"></a><span data-ttu-id="d649f-107">Создание категории товара</span><span class="sxs-lookup"><span data-stu-id="d649f-107">To create an item category</span></span>
1. <span data-ttu-id="d649f-108">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Категории товаров**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d649f-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Categories**, and then choose the related link.</span></span>
2. <span data-ttu-id="d649f-109">В окне **Категории товара** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="d649f-109">In the **Item Categories** window, choose the **New** action.</span></span>
3. <span data-ttu-id="d649f-110">В окне **Карточка категории товаров** заполните требуемые поля на экспресс-вкладке **Общее**.</span><span class="sxs-lookup"><span data-stu-id="d649f-110">In the **Item Category Card** window, on the **General** FastTab, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="d649f-111">На экспресс-вкладке **Атрибуты** укажите все атрибуты товаров для категории товара.</span><span class="sxs-lookup"><span data-stu-id="d649f-111">On the **Attributes** FastTab, specify any item attributes for the item category.</span></span> <span data-ttu-id="d649f-112">Дополнительные сведения см. в пункте "Назначение атрибутов товара категории товаров" раздела [Работа с атрибутами продуктов](inventory-how-work-item-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="d649f-112">For more information, see the "To assign item attributes to an item category" section in [Work with Item Attributes](inventory-how-work-item-attributes.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="d649f-113">Если категория товаров имеет родительскую категорию товаров, как указано в поле **Родительская категория**, то все атрибуты товаров, назначенные этой родительской категории, будут уже заполнены на экспресс-вкладке **Атрибуты**.</span><span class="sxs-lookup"><span data-stu-id="d649f-113">If the item category has a parent item category, as indicated by the **Parent Category** field, then any item attributes that are assigned to that parent item category are prefilled on the **Attributes** FastTab.</span></span>

> [!NOTE]  
>   <span data-ttu-id="d649f-114">Атрибуты товаров, назначенные категории товаров, автоматически применяются к товарам, которые назначены этой категории товаров.</span><span class="sxs-lookup"><span data-stu-id="d649f-114">Item attributes that you assign to an item category will automatically apply to the item that the item category is assigned to.</span></span>

## <a name="to-assign-an-item-category-to-an-item"></a><span data-ttu-id="d649f-115">Назначение товару категории товаров</span><span class="sxs-lookup"><span data-stu-id="d649f-115">To assign an item category to an item</span></span>
1. <span data-ttu-id="d649f-116">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Товары**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d649f-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="d649f-117">Откройте карточку товара, которому нужно присвоить категорию товаров.</span><span class="sxs-lookup"><span data-stu-id="d649f-117">Open the card for the item that you want to assign to an item category.</span></span>
3. <span data-ttu-id="d649f-118">Нажмите кнопку выбора в поле **Код товарной категории** и выберите существующую категорию товаров.</span><span class="sxs-lookup"><span data-stu-id="d649f-118">Choose the lookup button in the **Item Category Code** field and select an existing item category.</span></span> <span data-ttu-id="d649f-119">Можно также выбрать действие **Создать**, чтобы сначала создать новую категорию товаров, как объясняется в разделе "Создание категории товара".</span><span class="sxs-lookup"><span data-stu-id="d649f-119">Alternatively, choose the **New** action to first create a new item category as explained in the "To create an item category" section.</span></span>

## <a name="see-also"></a><span data-ttu-id="d649f-120">См. также</span><span class="sxs-lookup"><span data-stu-id="d649f-120">See Also</span></span>
[<span data-ttu-id="d649f-121">Работа с атрибутами товаров</span><span class="sxs-lookup"><span data-stu-id="d649f-121">Work with Item Attributes</span></span>](inventory-how-work-item-attributes.md)  
[<span data-ttu-id="d649f-122">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="d649f-122">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="d649f-123">Наличие</span><span class="sxs-lookup"><span data-stu-id="d649f-123">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="d649f-124">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d649f-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

