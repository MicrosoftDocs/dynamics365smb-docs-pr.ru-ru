---
title: Перемещение товаров между складами | Документация Майкрософт
description: Описывается, как перемещать запасы из одного места или склада в другое место или склад с помощью журнала реклассификации или заказов на перемещение.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: move, warehouse
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 79dfe973780269480285bac6aca380461b1ab403
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3913300"
---
# <a name="transfer-inventory-between-locations"></a><span data-ttu-id="47138-103">Перемещение запасов между складами</span><span class="sxs-lookup"><span data-stu-id="47138-103">Transfer Inventory Between Locations</span></span>
<span data-ttu-id="47138-104">Вы можете перемещать складские товары между складами, создав заказы на перемещение.</span><span class="sxs-lookup"><span data-stu-id="47138-104">You can transfer inventory items between locations by creating transfer orders.</span></span> <span data-ttu-id="47138-105">В качестве альтернативы можно использовать журнал реклассификации товаров.</span><span class="sxs-lookup"><span data-stu-id="47138-105">Alternatively, you can use the item reclassification journal.</span></span>

<span data-ttu-id="47138-106">С помощью заказов на перемещение можно отгрузить исходящее перемещение с одного склада и получить входящее перемещение на другом складе.</span><span class="sxs-lookup"><span data-stu-id="47138-106">With transfer orders, you ship the outbound transfer from one location and receive the inbound transfer at the other location.</span></span> <span data-ttu-id="47138-107">Это позволяет управлять включенными складскими операциями и предоставляет большую определенность относительно того, что количества запасов обновлены правильно.</span><span class="sxs-lookup"><span data-stu-id="47138-107">This allows you to manage the involved warehouse activities and provides more certainty that inventory quantities are updated correctly.</span></span>

<span data-ttu-id="47138-108">С помощью журнала реклассификации достаточно заполнить поля **Код склада** и **Новый код склада**.</span><span class="sxs-lookup"><span data-stu-id="47138-108">With the reclassification journal, you simply fill in the **Location Code** and the **New Location Code** fields.</span></span> <span data-ttu-id="47138-109">При учете журнала операции книги товаров корректируются на соответствующих складах.</span><span class="sxs-lookup"><span data-stu-id="47138-109">When you post the journal, the item ledger entries are adjusted at the locations in question.</span></span> <span data-ttu-id="47138-110">С помощью этого метода невозможно управлять складскими операциями.</span><span class="sxs-lookup"><span data-stu-id="47138-110">With this method, warehouse activities are not managed.</span></span>

> [!NOTE]  
>   <span data-ttu-id="47138-111">Если товары зарегистрированы в запасах без кода склада, например с тех времен, когда у вас был только один склад, вы не сможете переместить эти товары с помощью заказов на перемещение.</span><span class="sxs-lookup"><span data-stu-id="47138-111">If you have items recorded in your inventory without a location code, for example from a time when you only had one warehouse, then you cannot transfer those items using transfer orders.</span></span> <span data-ttu-id="47138-112">Вместо этого следует использовать журнал реклассификации для реклассификации товаров из пустого кода склада в фактический код склада.</span><span class="sxs-lookup"><span data-stu-id="47138-112">Instead, you must use the reclassification journal to reclassify the items from a blank location code to an actual location code.</span></span>  <span data-ttu-id="47138-113">Дополнительные сведения см. на шаге 3 в разделе [Перемещение товаров с помощью журнала реклассификации товаров](inventory-how-transfer-between-locations.md#to-transfer-items-with-the-item-reclassification-journal).</span><span class="sxs-lookup"><span data-stu-id="47138-113">For more information, see step 3 in [To transfer items with the item reclassification journal](inventory-how-transfer-between-locations.md#to-transfer-items-with-the-item-reclassification-journal).</span></span>

<span data-ttu-id="47138-114">Для перемещения товаров, следует настроить склады и маршруты перемещения.</span><span class="sxs-lookup"><span data-stu-id="47138-114">To transfer items, locations and transfer routes must be set up.</span></span> <span data-ttu-id="47138-115">Дополнительные сведения см. в разделе [Настройка складов](inventory-how-setup-locations.md).</span><span class="sxs-lookup"><span data-stu-id="47138-115">For more information, see [Set Up Locations](inventory-how-setup-locations.md).</span></span>

## <a name="to-transfer-items-with-a-transfer-order"></a><span data-ttu-id="47138-116">Перемещение товаров с помощью заказа на перемещение</span><span class="sxs-lookup"><span data-stu-id="47138-116">To transfer items with a transfer order</span></span>
1. <span data-ttu-id="47138-117">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на перемещение**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="47138-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="47138-118">В заголовке страницы **Заказ на перемещение** заполните поля требуемым образом.</span><span class="sxs-lookup"><span data-stu-id="47138-118">On the header of the **Transfer Order** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    >   <span data-ttu-id="47138-119">После заполнения полей **Код транзитного склада**, **Код экспедитора** и **Услуги экспедитора** на странице **Спец. транс. маршрута** при настройке маршрута перемещения соответствующие поля в заказе на перемещение заполняются автоматически.</span><span class="sxs-lookup"><span data-stu-id="47138-119">If you have filled in the **In-Transit Code**, **Shipping Agent Code**, and **Shipping Agent Service** fields on the **Trans. Route Spec.** page when you set up the transfer route, then the corresponding fields on the transfer order are filled in automatically.</span></span>

    <span data-ttu-id="47138-120">После заполнения поля **Услуги экспедитора** дата приемки на складе-получателе рассчитывается путем добавления времени услуг экспедитора к дате отгрузки.</span><span class="sxs-lookup"><span data-stu-id="47138-120">When you fill in the **Shipping Agent Service** field, the receipt date at the transfer-to location is calculated by adding the shipping time of the shipping agent service to the shipment date.</span></span>

3. <span data-ttu-id="47138-121">Чтобы заполнить строки, введите их вручную или выберите один из следующих вариантов под действием **Функция**:</span><span class="sxs-lookup"><span data-stu-id="47138-121">To fill in the lines, either enter them manually or choose one of the following options on the under the **Functions** action:</span></span>
    - <span data-ttu-id="47138-122">Выберите действие **Получить содержимое ячейки**, чтобы выбрать существующие товары из конкретной ячейки на складе.</span><span class="sxs-lookup"><span data-stu-id="47138-122">Choose the **Get Bin Content** action to select existing items from a specific bin at the location.</span></span>
    - <span data-ttu-id="47138-123">Выберите **Получить строки прих. накладной**, чтобы выбрать товары, которые только что прибыли на склад отправки.</span><span class="sxs-lookup"><span data-stu-id="47138-123">Choose the **Get Receipt Lines** to select items that have just arrived at the transfer-from location.</span></span>   

    <span data-ttu-id="47138-124">Как работник склада на складе отправки продолжите отгрузку товаров.</span><span class="sxs-lookup"><span data-stu-id="47138-124">As a warehouse worker at the transfer-from location, proceed to ship the items.</span></span>
4. <span data-ttu-id="47138-125">Выберите действие **Учет**, выберите параметр **Отгрузить** и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="47138-125">Choose the **Post** action, choose the **Ship** option, and then choose the **OK** button.</span></span>

    <span data-ttu-id="47138-126">Товары будут перемещены в транзит между указанными складами в соответствии с указанным маршрутом перемещения.</span><span class="sxs-lookup"><span data-stu-id="47138-126">The items are now in transit between the specified locations, according to the specifies transfer route.</span></span>

    <span data-ttu-id="47138-127">Как работник склада на складе отправки продолжите получение товаров.</span><span class="sxs-lookup"><span data-stu-id="47138-127">As a warehouse worker at the transfer-from location, proceed to receive the items.</span></span> <span data-ttu-id="47138-128">Строки заказа на перемещение — такие же, как при отправке, и редактировать их невозможно.</span><span class="sxs-lookup"><span data-stu-id="47138-128">The transfer order lines are the same as when shipped and cannot be edited.</span></span>
5. <span data-ttu-id="47138-129">Выберите действие **Учет**, выберите параметр **Получить** и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="47138-129">Choose the **Post** action, choose the **Receive** option, and then choose the **OK** button.</span></span>

## <a name="to-transfer-items-with-the-item-reclassification-journal"></a><span data-ttu-id="47138-130">Перемещение товаров с помощью журнала реклассификации товаров</span><span class="sxs-lookup"><span data-stu-id="47138-130">To transfer items with the item reclassification journal</span></span>
1. <span data-ttu-id="47138-131">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы рекласс. товаров**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="47138-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Reclass. Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="47138-132">На странице **Журнал реклассификации товаров** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="47138-132">On the **Item Reclass. Journal** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="47138-133">В поле **Код склада** введите склад, на котором хранятся товары в данный момент.</span><span class="sxs-lookup"><span data-stu-id="47138-133">In the **Location Code** field, enter the location where the items are currently stored.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="47138-134">Для перемещения товаров без кода склада оставьте поле **Код склада** пустым.</span><span class="sxs-lookup"><span data-stu-id="47138-134">To transfer items that have no location code, leave the **Location Code** field blank.</span></span>
4. <span data-ttu-id="47138-135">В поле **Новый код склада** введите склад, на который требуется переместить товары.</span><span class="sxs-lookup"><span data-stu-id="47138-135">In the **New Location Code** field, enter the location that you want to transfer the items to.</span></span>
5. <span data-ttu-id="47138-136">Выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="47138-136">Choose the **Post** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="47138-137">См. также</span><span class="sxs-lookup"><span data-stu-id="47138-137">See Also</span></span>
[<span data-ttu-id="47138-138">Управление запасами</span><span class="sxs-lookup"><span data-stu-id="47138-138">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="47138-139">Настройка складов</span><span class="sxs-lookup"><span data-stu-id="47138-139">Set Up Locations</span></span>](inventory-how-setup-locations.md)  
<span data-ttu-id="47138-140">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="47138-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="47138-141">Изменение набора отображаемых функций</span><span class="sxs-lookup"><span data-stu-id="47138-141">Change Which Features are Displayed</span></span>](ui-experiences.md)  
[<span data-ttu-id="47138-142">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="47138-142">General Business Functionality</span></span>](ui-across-business-areas.md)
