---
title: "Перемещение товаров между складами | Документы Майкрософт"
description: "Описывается, как перемещать запасы из одного места или склада в другое место или склад с помощью журнала реклассификации или заказов на перемещение."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: move, warehouse
ms.date: 10/01/2018
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 0e21299ab25f05f465b8a33d3a12bc35d9037d0b
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="transfer-inventory-between-locations"></a><span data-ttu-id="1fba8-103">Перемещение запасов между складами</span><span class="sxs-lookup"><span data-stu-id="1fba8-103">Transfer Inventory Between Locations</span></span>
<span data-ttu-id="1fba8-104">Вы можете перемещать складские товары между складами, создав заказы на перемещение.</span><span class="sxs-lookup"><span data-stu-id="1fba8-104">You can transfer inventory items between locations by creating transfer orders.</span></span> <span data-ttu-id="1fba8-105">В качестве альтернативы можно использовать журнал реклассификации товаров.</span><span class="sxs-lookup"><span data-stu-id="1fba8-105">Alternatively, you can use the item reclassification journal.</span></span>

<span data-ttu-id="1fba8-106">С помощью заказов на перемещение можно отгрузить исходящее перемещение с одного склада и получить входящее перемещение на другом складе.</span><span class="sxs-lookup"><span data-stu-id="1fba8-106">With transfer orders, you ship the outbound transfer from one location and receive the inbound transfer at the other location.</span></span> <span data-ttu-id="1fba8-107">Это позволяет управлять включенными складскими операциями и предоставляет большую определенность относительно того, что количества запасов обновлены правильно.</span><span class="sxs-lookup"><span data-stu-id="1fba8-107">This allows you to manage the involved warehouse activities and provides more certainty that inventory quantities are updated correctly.</span></span>

<span data-ttu-id="1fba8-108">С помощью журнала реклассификации достаточно заполнить поля **Код склада** и **Новый код склада**.</span><span class="sxs-lookup"><span data-stu-id="1fba8-108">With the reclassification journal, you simply fill in the **Location Code** and the **New Location Code** fields.</span></span> <span data-ttu-id="1fba8-109">При учете журнала операции книги товаров корректируются на соответствующих складах.</span><span class="sxs-lookup"><span data-stu-id="1fba8-109">When you post the journal, the item ledger entries are adjusted at the locations in question.</span></span> <span data-ttu-id="1fba8-110">С помощью этого метода невозможно управлять складскими операциями.</span><span class="sxs-lookup"><span data-stu-id="1fba8-110">With this method, warehouse activities are not managed.</span></span>

> [!NOTE]  
>   <span data-ttu-id="1fba8-111">Если товары зарегистрированы в запасах без кода склада, например с тех времен, когда у вас был только один склад, вы не сможете переместить эти товары с помощью заказов на перемещение.</span><span class="sxs-lookup"><span data-stu-id="1fba8-111">If you have items recorded in your inventory without a location code, for example from a time when you only had one warehouse, then you cannot transfer those items using transfer orders.</span></span> <span data-ttu-id="1fba8-112">Вместо этого следует использовать журнал реклассификации для реклассификации товаров из пустого кода склада в фактический код склада.</span><span class="sxs-lookup"><span data-stu-id="1fba8-112">Instead, you must use the reclassification journal to reclassify the items from a blank location code to an actual location code.</span></span>  <span data-ttu-id="1fba8-113">Дополнительные сведения см. на шаге 3 в разделе "Перемещение товаров с помощью журнала реклассификации товаров".</span><span class="sxs-lookup"><span data-stu-id="1fba8-113">For more information, see step 3 in the "To transfer items with the item reclassification journal" section.</span></span>

<span data-ttu-id="1fba8-114">Для перемещения товаров, следует настроить склады и маршруты перемещения.</span><span class="sxs-lookup"><span data-stu-id="1fba8-114">To transfer items, locations and transfer routes must be set up.</span></span> <span data-ttu-id="1fba8-115">Дополнительные сведения см. в разделе [Настройка складов](inventory-how-setup-locations.md).</span><span class="sxs-lookup"><span data-stu-id="1fba8-115">For more information, see [Set Up Locations](inventory-how-setup-locations.md).</span></span>

## <a name="to-transfer-items-with-a-transfer-order"></a><span data-ttu-id="1fba8-116">Перемещение товаров с помощью заказа на перемещение</span><span class="sxs-lookup"><span data-stu-id="1fba8-116">To transfer items with a transfer order</span></span>
1. <span data-ttu-id="1fba8-117">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на перемещение**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="1fba8-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="1fba8-118">В окне **Заказ на перемещение** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="1fba8-118">In the **Transfer Order** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    >   <span data-ttu-id="1fba8-119">После заполнения полей **Код транзитного склада**, **Код экспедитора** и **Услуги экспедитора** в окне **Спец. транс. маршрута** при настройке маршрута перемещения соответствующие поля в заказе на перемещение заполняются автоматически.</span><span class="sxs-lookup"><span data-stu-id="1fba8-119">If you have filled in the **In-Transit Code**, **Shipping Agent Code**, and **Shipping Agent Service** fields in the **Trans. Route Spec.** window when you set up the transfer route, then the corresponding fields on the transfer order are filled in automatically.</span></span>

    <span data-ttu-id="1fba8-120">После заполнения поля **Услуги экспедитора** дата приемки на складе-получателе рассчитывается путем добавления времени услуг экспедитора к дате отгрузки.</span><span class="sxs-lookup"><span data-stu-id="1fba8-120">When you fill in the **Shipping Agent Service** field, the receipt date at the transfer-to location is calculated by adding the shipping time of the shipping agent service to the shipment date.</span></span>

    <span data-ttu-id="1fba8-121">Как работник склада на складе отправки продолжите отгрузку товаров.</span><span class="sxs-lookup"><span data-stu-id="1fba8-121">As a warehouse worker at the transfer-from location, proceed to ship the items.</span></span>
3. <span data-ttu-id="1fba8-122">Выберите действие **Учет**, выберите параметр **Отгрузить** и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="1fba8-122">Choose the **Post** action, choose the **Ship** option, and then choose the **OK** button.</span></span>

    <span data-ttu-id="1fba8-123">Товары будут перемещены в транзит между указанными складами в соответствии с указанным маршрутом перемещения.</span><span class="sxs-lookup"><span data-stu-id="1fba8-123">The items are now in transit between the specified locations, according to the specifies transfer route.</span></span>

    <span data-ttu-id="1fba8-124">Как работник склада на складе отправки продолжите получение товаров.</span><span class="sxs-lookup"><span data-stu-id="1fba8-124">As a warehouse worker at the transfer-from location, proceed to receive the items.</span></span>
4. <span data-ttu-id="1fba8-125">Выберите действие **Учет**, выберите параметр **Получить** и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="1fba8-125">Choose the **Post** action, choose the **Receive** option, and then choose the **OK** button.</span></span>

## <a name="to-transfer-items-with-the-item-reclassification-journal"></a><span data-ttu-id="1fba8-126">Перемещение товаров с помощью журнала реклассификации товаров</span><span class="sxs-lookup"><span data-stu-id="1fba8-126">To transfer items with the item reclassification journal</span></span>
1. <span data-ttu-id="1fba8-127">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы рекласс. товаров**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="1fba8-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Reclass. Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="1fba8-128">В окне **Журнал реклассификации товаров** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="1fba8-128">In the **Item Reclass. Journal** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="1fba8-129">В поле **Код склада** введите склад, на котором хранятся товары в данный момент.</span><span class="sxs-lookup"><span data-stu-id="1fba8-129">In the **Location Code** field, enter the location where the items are currently stored.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="1fba8-130">Для перемещения товаров без кода склада оставьте поле **Код склада** пустым.</span><span class="sxs-lookup"><span data-stu-id="1fba8-130">To transfer items that have no location code, leave the **Location Code** field blank.</span></span>
4. <span data-ttu-id="1fba8-131">В поле **Новый код склада** введите склад, на который требуется переместить товары.</span><span class="sxs-lookup"><span data-stu-id="1fba8-131">In the **New Location Code** field, enter the location that you want to transfer the items to.</span></span>
5. <span data-ttu-id="1fba8-132">Выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="1fba8-132">Choose the **Post** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="1fba8-133">См. также</span><span class="sxs-lookup"><span data-stu-id="1fba8-133">See Also</span></span>
[<span data-ttu-id="1fba8-134">Управление запасами</span><span class="sxs-lookup"><span data-stu-id="1fba8-134">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="1fba8-135">Настройка складов</span><span class="sxs-lookup"><span data-stu-id="1fba8-135">Set Up Locations</span></span>](inventory-how-setup-locations.md)  
<span data-ttu-id="1fba8-136">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1fba8-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="1fba8-137">Изменение набора отображаемых функций</span><span class="sxs-lookup"><span data-stu-id="1fba8-137">Changing Which Features are Displayed</span></span>](ui-experiences.md)  
[<span data-ttu-id="1fba8-138">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="1fba8-138">General Business Functionality</span></span>](ui-across-business-areas.md)

