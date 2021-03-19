---
title: Практическое руководство. Создание специальных заказов | Документация Майкрософт
description: Для отгрузки товара из каталога конкретному клиенту можно создать специальный заказ. Поставщик отгружает товар на склад организации, после чего этот товар отгружается в адрес клиента либо отдельно, либо вместе с другими товарами по другому заказу.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: fbd22ee25cb472a827468c578ccdb8a7427490bc
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5383029"
---
# <a name="create-special-orders"></a><span data-ttu-id="a71cc-104">Создание специальных заказов</span><span class="sxs-lookup"><span data-stu-id="a71cc-104">Create Special Orders</span></span>
<span data-ttu-id="a71cc-105">Для отгрузки товара из каталога конкретному клиенту можно создать специальный заказ.</span><span class="sxs-lookup"><span data-stu-id="a71cc-105">You can create a special order for a specific catalog item to be shipped to a specific customer.</span></span> <span data-ttu-id="a71cc-106">Поставщик отгружает товар на склад организации, после чего этот товар отгружается в адрес клиента либо отдельно, либо вместе с другими товарами по другому заказу.</span><span class="sxs-lookup"><span data-stu-id="a71cc-106">Your vendor ships the item to your warehouse and you can then ship the item on to your customer either independently or together with other items on another order.</span></span>  

<span data-ttu-id="a71cc-107">Специальные заказы предполагают наличие связи между заказом на покупку и заказом на продажу, позволяющей обеспечить подбор конкретного товара из каталога и его доставку клиенту.</span><span class="sxs-lookup"><span data-stu-id="a71cc-107">Special orders imply that the purchase and sales order are linked to ensure that the specific catalog item is picked and delivered to the customer.</span></span>  

<span data-ttu-id="a71cc-108">Перед использованием этой функции следует сначала настроить карточки клиента, поставщика и товара, которые необходимы для создания заказа.</span><span class="sxs-lookup"><span data-stu-id="a71cc-108">Before you can use this feature, you must first set up the customer, vendor, and item cards necessary for the order.</span></span>  

## <a name="to-create-a-special-order"></a><span data-ttu-id="a71cc-109">Создание специального заказа</span><span class="sxs-lookup"><span data-stu-id="a71cc-109">To create a special order</span></span>  
1.  <span data-ttu-id="a71cc-110">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказ на продажу**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="a71cc-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Order**, and then choose the related link.</span></span>  
2. <span data-ttu-id="a71cc-111">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="a71cc-111">Choose the **New** action.</span></span> <span data-ttu-id="a71cc-112">Создайте и заполните заказ на продажу товара.</span><span class="sxs-lookup"><span data-stu-id="a71cc-112">Create and fill in a  sales order for the item.</span></span> <span data-ttu-id="a71cc-113">Дополнительные сведения см. в разделе [Продажа продукции](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="a71cc-113">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>
3.  <span data-ttu-id="a71cc-114">На экспресс-вкладке **Строки** заполните строку продажи.</span><span class="sxs-lookup"><span data-stu-id="a71cc-114">On the **Lines** FastTab, fill in the sales line.</span></span> <span data-ttu-id="a71cc-115">В поле **Код закупки** выберите код покупки, для которого выбрано поле **Специальный заказ**.</span><span class="sxs-lookup"><span data-stu-id="a71cc-115">In the **Purchasing Code** field, select a purchasing code that has the **Special Order** field selected.</span></span>

    <span data-ttu-id="a71cc-116">Теперь необходимо создать заказ на покупку на основе журнала заявок.</span><span class="sxs-lookup"><span data-stu-id="a71cc-116">You must now create a purchase order from a requisition worksheet.</span></span>  
4. <span data-ttu-id="a71cc-117">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал заявок**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="a71cc-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Requisition Worksheet**, and then choose the related link.</span></span>  
5. <span data-ttu-id="a71cc-118">Выберите действие **Специальный заказ**, затем выберите действие **Получить заказы на продажу**.</span><span class="sxs-lookup"><span data-stu-id="a71cc-118">Choose the **Special Order** action, and then choose the **Get Sales Orders** action.</span></span>  
6.  <span data-ttu-id="a71cc-119">На странице **Получить заказы на продажу** отображаются результаты, в которых **Номер документа** является номером заказа на продажу.</span><span class="sxs-lookup"><span data-stu-id="a71cc-119">On the **Get Sales Orders** page, show results where the **Document No.** is the sales order number.</span></span> <span data-ttu-id="a71cc-120">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="a71cc-120">Choose the **OK** button.</span></span> <span data-ttu-id="a71cc-121">Для товара создается строка журнала заявок.</span><span class="sxs-lookup"><span data-stu-id="a71cc-121">A requisition worksheet line is created for the item.</span></span>  
7.  <span data-ttu-id="a71cc-122">В строке заявки выберите в поле **Указание** выберите **Новое**.</span><span class="sxs-lookup"><span data-stu-id="a71cc-122">On the requisition worksheet line, in the **Action Message** field, select **New**.</span></span>  
8.  <span data-ttu-id="a71cc-123">На странице **Журнал заявок** выберите действие **Выполнить указание**.</span><span class="sxs-lookup"><span data-stu-id="a71cc-123">On the **Req. Worksheet** page, choose the **Carry Out Action Message** action.</span></span> <span data-ttu-id="a71cc-124">Открывается страница **Выполнение указаний - заявка**.</span><span class="sxs-lookup"><span data-stu-id="a71cc-124">The **Carry Out Action Msg. - Req.** page opens.</span></span> <span data-ttu-id="a71cc-125">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="a71cc-125">Choose the **OK** button.</span></span>  

    <span data-ttu-id="a71cc-126">Отобразится сообщение о том, что созданы заказы на покупку.</span><span class="sxs-lookup"><span data-stu-id="a71cc-126">A message appears telling you that the purchase orders have been created.</span></span> <span data-ttu-id="a71cc-127">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="a71cc-127">Choost the **OK** button.</span></span>  

<span data-ttu-id="a71cc-128">Заказ на покупку, созданный как специальный заказ для заказа на продажу, учитывается системой планирования, поскольку балансирует спрос и предложение.</span><span class="sxs-lookup"><span data-stu-id="a71cc-128">A purchase order created as a special order for a sales order is respected by the planning system as it balances demand and supply.</span></span> <span data-ttu-id="a71cc-129">Это означает, что заказ на покупку (предложение) остается связанным с заказом на продажу (требованием), даже если заказ на покупку мог бы быть использован для поставки по более раннему требованию.</span><span class="sxs-lookup"><span data-stu-id="a71cc-129">That is, the purchase order (supply) remains linked to the sales order (demand), even if that purchase order could supply another earlier demand.</span></span> <span data-ttu-id="a71cc-130">Дополнительные сведения см. в разделе [Сведения о проектировании. Политики дозаказа](design-details-reservation-order-tracking-and-action-messaging.md).</span><span class="sxs-lookup"><span data-stu-id="a71cc-130">For more information, see [Design Details: Reordering Policies](design-details-reservation-order-tracking-and-action-messaging.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="a71cc-131">Нельзя использовать функцию специального заказа, если товар уже зарезервирован.</span><span class="sxs-lookup"><span data-stu-id="a71cc-131">You cannot use the special order functionality if the item is already reserved.</span></span> <span data-ttu-id="a71cc-132">Поэтому для товаров, которые продаются по специальным заказам, убедитесь, что значение в поле **Резервировать** в карточке товара не равно **Всегда**.</span><span class="sxs-lookup"><span data-stu-id="a71cc-132">Therefore, for items that are sold on special orders, make sure the **Reserve** field on the item card is not set to **Always**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a71cc-133">См. также</span><span class="sxs-lookup"><span data-stu-id="a71cc-133">See Also</span></span>  
[<span data-ttu-id="a71cc-134">Работа с товарами из каталога</span><span class="sxs-lookup"><span data-stu-id="a71cc-134">Work with Catalog Items</span></span>](inventory-how-work-nonstock-items.md)  
[<span data-ttu-id="a71cc-135">Продажи</span><span class="sxs-lookup"><span data-stu-id="a71cc-135">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="a71cc-136">[Выполнение прямых поставок](sales-how-drop-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="a71cc-136">[Make Drop Shipments](sales-how-drop-shipment.md) </span></span>  
[<span data-ttu-id="a71cc-137">Сведения о проектировании: политики дозаказа</span><span class="sxs-lookup"><span data-stu-id="a71cc-137">Design Details: Reordering Policies</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
<span data-ttu-id="a71cc-138">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a71cc-138">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]