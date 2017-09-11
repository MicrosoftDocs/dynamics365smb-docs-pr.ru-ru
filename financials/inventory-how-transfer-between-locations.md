---
title: "Перемещение товаров между складами | Документы Майкрософт"
description: "Описывается, как перемещать запасы из одного места или склада в другое место или склад с помощью журнала реклассификации или заказов на перемещение."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: move, warehouse
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: d54b75240cb0a2dddcfabc488a18e0bf9635f82c
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017


---
# <a name="how-to-transfer-inventory-between-locations"></a><span data-ttu-id="3a775-103">Практическое руководство. Перемещение запасов между складами</span><span class="sxs-lookup"><span data-stu-id="3a775-103">How to: Transfer Inventory Between Locations</span></span>
<span data-ttu-id="3a775-104">Вы можете перемещать складские товары между складами, создав заказы на перемещение.</span><span class="sxs-lookup"><span data-stu-id="3a775-104">You can transfer inventory items between locations by creating transfer orders.</span></span> <span data-ttu-id="3a775-105">В качестве альтернативы можно использовать журнал реклассификации товаров.</span><span class="sxs-lookup"><span data-stu-id="3a775-105">Alternatively, you can use the item reclassification journal.</span></span>

<span data-ttu-id="3a775-106">С помощью заказов на перемещение можно отгрузить исходящее перемещение с одного склада и получить входящее перемещение на другом складе.</span><span class="sxs-lookup"><span data-stu-id="3a775-106">With transfer orders, you ship the outbound transfer from one location and receive the inbound transfer at the other location.</span></span> <span data-ttu-id="3a775-107">Это позволяет управлять включенными складскими операциями и предоставляет большую определенность относительно того, что количества запасов обновлены правильно.</span><span class="sxs-lookup"><span data-stu-id="3a775-107">This allows you to manage the involved warehouse activities and provides more certainty that inventory quantities are updated correctly.</span></span>

<span data-ttu-id="3a775-108">С помощью журнала реклассификации достаточно заполнить поля **Код склада** и **Новый код склада**.</span><span class="sxs-lookup"><span data-stu-id="3a775-108">With the reclassification journal, you simply fill in the **Location Code** and the **New Location Code** fields.</span></span> <span data-ttu-id="3a775-109">При учете журнала операции книги товаров корректируются на соответствующих складах.</span><span class="sxs-lookup"><span data-stu-id="3a775-109">When you post the journal, the item ledger entries are adjusted at the locations in question.</span></span> <span data-ttu-id="3a775-110">С помощью этого метода невозможно управлять складскими операциями.</span><span class="sxs-lookup"><span data-stu-id="3a775-110">With this method, warehouse activities are not managed.</span></span>

> [!NOTE]  
>   <span data-ttu-id="3a775-111">Если товары зарегистрированы в запасах без кода склада, например с тех времен, когда у вас был только один склад, вы не сможете переместить эти товары с помощью заказов на перемещение.</span><span class="sxs-lookup"><span data-stu-id="3a775-111">If you have items recorded in your inventory without a location code, for example from a time when you only had one warehouse, then you cannot transfer those items using transfer orders.</span></span> <span data-ttu-id="3a775-112">Вместо этого следует использовать журнал реклассификации для реклассификации товаров из пустого кода склада в фактический код склада.</span><span class="sxs-lookup"><span data-stu-id="3a775-112">Instead, you must use the reclassification journal to reclassify the items from a blank location code to an actual location code.</span></span>  <span data-ttu-id="3a775-113">Дополнительные сведения см. на шаге 3 в разделе "Перемещение товаров с помощью журнала реклассификации товаров".</span><span class="sxs-lookup"><span data-stu-id="3a775-113">For more information, see step 3 in the "To transfer items with the item reclassification journal" section.</span></span>

<span data-ttu-id="3a775-114">Для перемещения товаров, следует настроить склады и маршруты перемещения.</span><span class="sxs-lookup"><span data-stu-id="3a775-114">To transfer items, locations and transfer routes must be set up.</span></span> <span data-ttu-id="3a775-115">Дополнительные сведения см. в разделе [Практическое руководство. Настройка складов](inventory-how-setup-locations.md).</span><span class="sxs-lookup"><span data-stu-id="3a775-115">For more information, see [How to: Set Up Locations](inventory-how-setup-locations.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="3a775-116">Эта функция требует, чтобы было задано значение **Пакет**.</span><span class="sxs-lookup"><span data-stu-id="3a775-116">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="3a775-117">Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="3a775-117">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-transfer-items-with-a-transfer-order"></a><span data-ttu-id="3a775-118">Перемещение товаров с помощью заказа на перемещение</span><span class="sxs-lookup"><span data-stu-id="3a775-118">To transfer items with a transfer order</span></span>
1. <span data-ttu-id="3a775-119">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Заказы на перемещение**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3a775-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="3a775-120">В окне **Заказ на перемещение** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="3a775-120">In the **Transfer Order** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
>   <span data-ttu-id="3a775-121">Если заполнены поля **Код транзитного склада**, **Код экспедитора** и **Услуги экспедитора** в окне **Спец. транс. маршрута**</span><span class="sxs-lookup"><span data-stu-id="3a775-121">If you have filled in the **In-Transit Code**, **Shipping Agent Code**, and **Shipping Agent Service** fields in the **Trans. Route Spec.**</span></span> <span data-ttu-id="3a775-122">при настройке маршрута перемещения, то соответствующие поля в заказе на перемещение заполняется автоматически.</span><span class="sxs-lookup"><span data-stu-id="3a775-122">window when you set up the transfer route, then the corresponding fields on the transfer order are filled in automatically.</span></span>

    <span data-ttu-id="3a775-123">После заполнения поля **Услуги экспедитора** дата приемки на складе-получателе рассчитывается путем добавления времени услуг экспедитора к дате отгрузки.</span><span class="sxs-lookup"><span data-stu-id="3a775-123">When you fill in the **Shipping Agent Service** field, the receipt date at the transfer-to location is calculated by adding the shipping time of the shipping agent service to the shipment date.</span></span>

    <span data-ttu-id="3a775-124">Как работник склада на складе отправки продолжите отгрузку товаров.</span><span class="sxs-lookup"><span data-stu-id="3a775-124">As a warehouse worker at the transfer-from location, proceed to ship the items.</span></span>
3. <span data-ttu-id="3a775-125">Выберите действие **Учет**, выберите параметр **Отгрузить** и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="3a775-125">Choose the **Post** action, choose the **Ship** option, and then choose the **OK** button.</span></span>

    <span data-ttu-id="3a775-126">Товары будут перемещены в транзит между указанными складами в соответствии с указанным маршрутом перемещения.</span><span class="sxs-lookup"><span data-stu-id="3a775-126">The items are now in transit between the specified locations, according to the specifies transfer route.</span></span>

    <span data-ttu-id="3a775-127">Как работник склада на складе отправки продолжите получение товаров.</span><span class="sxs-lookup"><span data-stu-id="3a775-127">As a warehouse worker at the transfer-from location, proceed to receive the items.</span></span>
4. <span data-ttu-id="3a775-128">Выберите действие **Учет**, выберите параметр **Получить** и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="3a775-128">Choose the **Post** action, choose the **Receive** option, and then choose the **OK** button.</span></span>

## <a name="to-transfer-items-with-the-item-reclassification-journal"></a><span data-ttu-id="3a775-129">Перемещение товаров с помощью журнала реклассификации товаров</span><span class="sxs-lookup"><span data-stu-id="3a775-129">To transfer items with the item reclassification journal</span></span>
1. <span data-ttu-id="3a775-130">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы реклассификации товаров**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3a775-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Reclass. Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="3a775-131">В окне **Журнал реклассификации товаров** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="3a775-131">In the **Item Reclass. Journal** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="3a775-132">В поле **Код склада** введите склад, на котором хранятся товары в данный момент.</span><span class="sxs-lookup"><span data-stu-id="3a775-132">In the **Location Code** field, enter the location where the items are currently stored.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="3a775-133">Для перемещения товаров без кода склада оставьте поле **Код склада** пустым.</span><span class="sxs-lookup"><span data-stu-id="3a775-133">To transfer items that have no location code, leave the **Location Code** field blank.</span></span>
4. <span data-ttu-id="3a775-134">В поле **Новый код склада** введите склад, на который требуется переместить товары.</span><span class="sxs-lookup"><span data-stu-id="3a775-134">In the **New Location Code** field, enter the location that you want to transfer the items to.</span></span>
5. <span data-ttu-id="3a775-135">Выберите действие **Учесть**.</span><span class="sxs-lookup"><span data-stu-id="3a775-135">Choose the **Post** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="3a775-136">См. также</span><span class="sxs-lookup"><span data-stu-id="3a775-136">See Also</span></span>
[<span data-ttu-id="3a775-137">Управление запасами</span><span class="sxs-lookup"><span data-stu-id="3a775-137">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="3a775-138">Практическое руководство. Настройка складов</span><span class="sxs-lookup"><span data-stu-id="3a775-138">How to: Set Up Locations</span></span>](inventory-how-setup-locations.md)  
[<span data-ttu-id="3a775-139">Цепочка поставок</span><span class="sxs-lookup"><span data-stu-id="3a775-139">Supply Chain</span></span>](madeira-supply-chain.md)  
<span data-ttu-id="3a775-140">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3a775-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="3a775-141">[Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="3a775-141">[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)</span></span>  
[<span data-ttu-id="3a775-142">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="3a775-142">General Business Functionality</span></span>](ui-across-business-areas.md)

## [!INCLUDE[d365fin](includes/free_trial_md.md)]