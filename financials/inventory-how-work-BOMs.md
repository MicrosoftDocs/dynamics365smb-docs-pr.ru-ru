---
title: "Работа со спецификациями для управления компонентами | Документы Майкрософт"
description: "Сборочные спецификации служат для определения компонентов или ресурсов, которые нужно собрать вместе, чтобы получить соответствующий товар, и вы можете просматривать компоненты сборочного элемента."
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 05/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: e6aef60ee5b206b0ae978f72b92e6f8778290509
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-work-with-bills-of-material"></a><span data-ttu-id="868cf-103">Практическое руководство. Работа со спецификациями</span><span class="sxs-lookup"><span data-stu-id="868cf-103">How to: Work with Bills of Material</span></span>
> [!NOTE]  
>   <span data-ttu-id="868cf-104">Текущая версия [!INCLUDE[d365fin](includes/d365fin_md.md)] содержит только первую часть функции управления сборкой.</span><span class="sxs-lookup"><span data-stu-id="868cf-104">The current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] only contains the first part of the Assembly Management feature.</span></span> <span data-ttu-id="868cf-105">На данный момент можно только создавать сборочные спецификации, а затем обрабатывать связанные родительские товары как обычные складские товары.</span><span class="sxs-lookup"><span data-stu-id="868cf-105">For now, you can only create assembly BOMs and then handle the related parent items as normal inventory items.</span></span> <span data-ttu-id="868cf-106">В будущем обновлении можно будет управлять фактической сборкой товаров из компонентов в потоках сборки на склад или сборки на заказ и продавать компоненты как наборы.</span><span class="sxs-lookup"><span data-stu-id="868cf-106">In a future update, you can manage the actual assembly of items from components, either in assemble-to-stock or assemble-to-order flows, and you can sell components as kits.</span></span>

<span data-ttu-id="868cf-107">Спецификация используется для структурирования родительских товаров, которые вы продаете как наборы, состоящие из компонентов родительского товара, или которые вы собираете для заказа или складирования.</span><span class="sxs-lookup"><span data-stu-id="868cf-107">You use bills of materials (BOMs) to structure parent items that you sell as kits consisting of the parent's components or that you assemble to order or to stock.</span></span>

<span data-ttu-id="868cf-108">В [!INCLUDE[d365fin](includes/d365fin_md.md)] спецификация называется сборочной спецификацией.</span><span class="sxs-lookup"><span data-stu-id="868cf-108">In [!INCLUDE[d365fin](includes/d365fin_md.md)], a bill of materials is referred to as an "assembly BOM".</span></span> <span data-ttu-id="868cf-109">Сборочная спецификации указывает, какие компоненты содержатся в родительских товарах.</span><span class="sxs-lookup"><span data-stu-id="868cf-109">Assembly BOMs specify which components are contained in parent items.</span></span> <span data-ttu-id="868cf-110">В этой документации родительский товар называется "сборочным элементом".</span><span class="sxs-lookup"><span data-stu-id="868cf-110">In this documentation, a parent item is referred to as an "assembly item".</span></span>

<span data-ttu-id="868cf-111">Сборочные спецификации обычно содержат товары, но могут также содержать один или несколько ресурсов, которые необходимы для создания сборочного элемента.</span><span class="sxs-lookup"><span data-stu-id="868cf-111">Assembly BOMs usually contain items but can also contain one or more resources that are required to put the assembly item together.</span></span>

<span data-ttu-id="868cf-112">Сборочные спецификации могут быть многоуровневыми, что означает, что компонент сборочной спецификации может сам быть сборочным элементом.</span><span class="sxs-lookup"><span data-stu-id="868cf-112">Assembly BOMs can have multiple levels, which means that a component on the assembly BOM can be an assembly item itself.</span></span> <span data-ttu-id="868cf-113">В этом случае поле **Сборочная спецификация** в строке сборочной спецификации содержит значение **Да**.</span><span class="sxs-lookup"><span data-stu-id="868cf-113">In that case, the **Assembly BOM** field on the assembly BOM line contains **Yes**.</span></span>

<span data-ttu-id="868cf-114">Особенные требования применяются к товарам в сборочных спецификациях в отношении доступности.</span><span class="sxs-lookup"><span data-stu-id="868cf-114">Special requirements apply to items on assembly BOMs with regards to availability.</span></span> <span data-ttu-id="868cf-115">Дополнительные сведения см. в подразделе "Просмотр доступности товара по использованию в сборочных спецификациях" раздела [Практическое руководство. Просмотр наличия товара](inventory-how-availability-overview.md).</span><span class="sxs-lookup"><span data-stu-id="868cf-115">For more information, see the "To see the availability of an item by its use in assembly BOMs" section in [How to: View the Availability of Items](inventory-how-availability-overview.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="868cf-116">Эта функция требует, чтобы было задано значение **Пакет**.</span><span class="sxs-lookup"><span data-stu-id="868cf-116">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="868cf-117">Дополнительные сведения см. в разделе [Настройка взаимодействия Financials](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="868cf-117">For more information, see [Customizing Your Financials Experience](ui-experiences.md).</span></span>

## <a name="to-create-an-assembly-bom"></a><span data-ttu-id="868cf-118">Создание сборочной спецификации</span><span class="sxs-lookup"><span data-stu-id="868cf-118">To create an assembly BOM</span></span>
<span data-ttu-id="868cf-119">Для определения родительского товара, который состоит из других товаров и, возможно, ресурсов, необходимых для создания родительского элемента, следует создать сборочную спецификацию.</span><span class="sxs-lookup"><span data-stu-id="868cf-119">To define a parent item that consists of other items, and potentially of resources required to put the parent together, you must create an assembly BOM.</span></span>  

<span data-ttu-id="868cf-120">Создание новой сборочной спецификации выполняется в два этапа:</span><span class="sxs-lookup"><span data-stu-id="868cf-120">There are two parts to creating an assembly BOM:</span></span>
- <span data-ttu-id="868cf-121">Настройка нового товара</span><span class="sxs-lookup"><span data-stu-id="868cf-121">Setting up a new item</span></span>
- <span data-ttu-id="868cf-122">Определение структуры спецификации сборочного элемента.</span><span class="sxs-lookup"><span data-stu-id="868cf-122">Defining the BOM structure of the assembly item.</span></span>

1. <span data-ttu-id="868cf-123">Настройте новый товар.</span><span class="sxs-lookup"><span data-stu-id="868cf-123">Set up a new item.</span></span> <span data-ttu-id="868cf-124">Дополнительные сведения см. в разделе [Практическое руководство. Регистрация новых товаров](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="868cf-124">For more information, see [How to: Register New Items](inventory-how-register-new-items.md).</span></span>

    <span data-ttu-id="868cf-125">Введите компоненты или ресурсы в сборочной спецификации.</span><span class="sxs-lookup"><span data-stu-id="868cf-125">Proceed to enter components or resources on the assembly BOM.</span></span>  
2. <span data-ttu-id="868cf-126">В окне **Карточка товара** для сборочного элемента выберите действие **Сборка**, а затем выберите действие **Сборочная спецификация**.</span><span class="sxs-lookup"><span data-stu-id="868cf-126">In the **Item Card** window for an assembly item, choose the **Assembly** action, and then choose the **Assembly BOM** action.</span></span>
3. <span data-ttu-id="868cf-127">В окне **Сборочная спецификация** заполните поля по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="868cf-127">In the **Assembly BOM** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-view-the-components-of-an-assembly-item-indented-according-to-the-bom-structure"></a><span data-ttu-id="868cf-128">Просмотр компонентов сборочного элемента с отступом согласно структуре спецификации</span><span class="sxs-lookup"><span data-stu-id="868cf-128">To view the components of an assembly item indented according to the BOM structure</span></span>
<span data-ttu-id="868cf-129">В окне **Сборочная спецификация** можно открыть отдельное окно, в котором отображаются компоненты и все ресурсы с отступом согласно позиции спецификации в сборочном элементе.</span><span class="sxs-lookup"><span data-stu-id="868cf-129">From the **Assembly BOM** window, you can open a separate window that shows the components and any resources indented according to their BOM position under the assembly item.</span></span>

1. <span data-ttu-id="868cf-130">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Товары**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="868cf-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="868cf-131">Откройте карточку сборочного элемента.</span><span class="sxs-lookup"><span data-stu-id="868cf-131">Open the card for an assembly item.</span></span> <span data-ttu-id="868cf-132">(Поле **Сборочная спецификация** в окне **Товары** содержит значение **Да**).</span><span class="sxs-lookup"><span data-stu-id="868cf-132">(The **Assembly BOM** field in the **Items** window contains **Yes**.)</span></span>
3. <span data-ttu-id="868cf-133">В окне **Карточка товара** выберите действие **Сборка**, а затем выберите действие **Сборочная спецификация**.</span><span class="sxs-lookup"><span data-stu-id="868cf-133">In the **Item Card** window, choose the **Assembly** action, and then choose the **Assembly BOM** action.</span></span>
4. <span data-ttu-id="868cf-134">В окне **Сборочная спецификация** выберите действие **Показать спецификацию**.</span><span class="sxs-lookup"><span data-stu-id="868cf-134">In the **Assembly BOM** window, choose the **Show BOM** action.</span></span>

## <a name="to-buy-sell-or-transfer-assembly-items"></a><span data-ttu-id="868cf-135">Покупка, продажа или перемещение сборочных элементов</span><span class="sxs-lookup"><span data-stu-id="868cf-135">To buy, sell, or transfer assembly items</span></span>
<span data-ttu-id="868cf-136">Поскольку текущая версия [!INCLUDE[d365fin](includes/d365fin_md.md)] предоставляет возможность только определить и назначить сборочные спецификации товарам, можно обрабатывать сборочные элементы в строках документа только как обычные товары.</span><span class="sxs-lookup"><span data-stu-id="868cf-136">Because the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] only contains the ability to define and assign assembly BOMs to items, you can handle assembly items on document lines as normal items only.</span></span>

<span data-ttu-id="868cf-137">**Внимание**! При этом количество запасов компонента спецификации не будет корректироваться.</span><span class="sxs-lookup"><span data-stu-id="868cf-137">**Caution**: The inventory quantity of BOM components will not be adjusted if you do so.</span></span>

## <a name="see-also"></a><span data-ttu-id="868cf-138">См. также</span><span class="sxs-lookup"><span data-stu-id="868cf-138">See Also</span></span>
[<span data-ttu-id="868cf-139">Практическое руководство. Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="868cf-139">How to: Register New Items</span></span>](inventory-how-register-new-items.md)  
<span data-ttu-id="868cf-140">[Практическое руководство. Просмотр наличия товара](inventory-how-availability-overview.md)   </span><span class="sxs-lookup"><span data-stu-id="868cf-140">[How to: View the Availability of Items](inventory-how-availability-overview.md)   </span></span>  
[<span data-ttu-id="868cf-141">Запасы</span><span class="sxs-lookup"><span data-stu-id="868cf-141">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="868cf-142">[Работа с [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="868cf-142">[Working with [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>

