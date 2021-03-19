---
title: Связывание заказа на продажу с заказом на покупку для прямой поставки | Документация Майкрософт
description: Рассматривается создание заказа на покупку, связанного с заказом на продажу, для обеспечения прямой поставки от поставщика клиенту.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 938b0cc9f35e980ca9121cb037665b8699ca336f
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5393377"
---
# <a name="make-drop-shipments"></a><span data-ttu-id="21077-103">Выполнение прямых поставок</span><span class="sxs-lookup"><span data-stu-id="21077-103">Make Drop Shipments</span></span>

<span data-ttu-id="21077-104">Прямая поставка — это поставка товаров одним из ваших поставщиков непосредственно одному из ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="21077-104">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="21077-105">Когда заказ на продажу помечен для прямой поставки, и вы создаете заказ на покупку, указывая клиента в поле **Получатель**, **Адрес клиента**, вы можете связать два документа, чтобы дать указание поставщику отправить товар непосредственно клиенту.</span><span class="sxs-lookup"><span data-stu-id="21077-105">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Ship-to** field, **Customer Address**, you can link the two documents to instruct the vendor to ship directly to the customer.</span></span>
<br><br>  
  
> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4mOyM?rel=0]

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="21077-106">Создание заказа на продажу по прямой поставке</span><span class="sxs-lookup"><span data-stu-id="21077-106">To create a sales order for drop shipment</span></span>

<span data-ttu-id="21077-107">Для подготовки прямой поставки следует создать заказы на продажу для товара и указать в строке продажи, что продажа требует прямой поставки.</span><span class="sxs-lookup"><span data-stu-id="21077-107">To prepare a drop shipment, you create a sales order for an item and indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="21077-108">Создайте заказ на продажу для товара.</span><span class="sxs-lookup"><span data-stu-id="21077-108">Create a sales order for an item.</span></span> <span data-ttu-id="21077-109">Дополнительные сведения см. в разделе [Продажа продукции](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="21077-109">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="21077-110">В строке заказа на продажу для прямой поставки установите флажок **Прямая поставка**.</span><span class="sxs-lookup"><span data-stu-id="21077-110">On the sales order line for the drop shipment, select the **Drop Shipment** check box.</span></span> <span data-ttu-id="21077-111">Используйте функцию **Выбрать столбцы**, если поле не отображается.</span><span class="sxs-lookup"><span data-stu-id="21077-111">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="21077-112">Дополнительные сведения см. в разделе [Персонализация рабочей области](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="21077-112">For more information, see [Personalize Your Workspace](ui-personalization-user.md).</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="21077-113">Создание заказа на покупку для прямой поставки</span><span class="sxs-lookup"><span data-stu-id="21077-113">To create the purchase order for drop shipment</span></span>

<span data-ttu-id="21077-114">Чтобы подготовить прямую поставку, вы указываете в заказе на покупку, что он должен быть доставлен вашему клиенту, а не вам.</span><span class="sxs-lookup"><span data-stu-id="21077-114">To prepare a drop shipment, you indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="21077-115">Создайте заказ покупки.</span><span class="sxs-lookup"><span data-stu-id="21077-115">Create a purchase order.</span></span> <span data-ttu-id="21077-116">Не заполняйте никакие поля в строках.</span><span class="sxs-lookup"><span data-stu-id="21077-116">Do not fill any fields on the lines.</span></span> <span data-ttu-id="21077-117">Дополнительные сведения см. в разделе [Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="21077-117">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="21077-118">В поле **Получатель** выберите **Адрес клиента**.</span><span class="sxs-lookup"><span data-stu-id="21077-118">In the **Ship-to** field, select **Customer Address**.</span></span>
3. <span data-ttu-id="21077-119">В поле **Клиент** выберите клиента, которому осуществляется продажа.</span><span class="sxs-lookup"><span data-stu-id="21077-119">In the **Customer** field, select the customer that you are selling to.</span></span>
4. <span data-ttu-id="21077-120">Выберите действие **Прямые поставки**, затем выберите действие **Получить заказ на продажу**.</span><span class="sxs-lookup"><span data-stu-id="21077-120">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
5. <span data-ttu-id="21077-121">На странице **Список продаж** выберите заказ на продажу, который был подготовлен в разделе [Создание заказа на продажу по прямой поставке](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment).</span><span class="sxs-lookup"><span data-stu-id="21077-121">On the **Sales List** page, select the sales order that you prepared in [To create a sales order for drop shipment](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment).</span></span>
6. <span data-ttu-id="21077-122">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="21077-122">Choose the **OK** button.</span></span>

<span data-ttu-id="21077-123">Информация строки в заказе на продажу будет вставлена в строки заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="21077-123">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="21077-124">Теперь можно проинструктировать поставщика, чтобы он отгрузил товары клиенту, например, переслав заказ на покупку в виде файла PDF.</span><span class="sxs-lookup"><span data-stu-id="21077-124">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-create-multiple-purchase-orders-for-drop-shipments"></a><span data-ttu-id="21077-125">Для создания нескольких заказов на покупку для прямых поставок</span><span class="sxs-lookup"><span data-stu-id="21077-125">To create multiple purchase orders for drop shipments</span></span>

<span data-ttu-id="21077-126">Вы также можете использовать лист заявки, чтобы создать заказ на покупку для поставщика.</span><span class="sxs-lookup"><span data-stu-id="21077-126">You can also use the requisition worksheet to create the purchase order for the vendor.</span></span> <span data-ttu-id="21077-127">Преимущество использования листа заявок заключается в том, что с его помощью можно создавать заказы на закупку для всех незавершенных прямых поставок, поэтому вам не нужно создавать каждый из них отдельно.</span><span class="sxs-lookup"><span data-stu-id="21077-127">The advantage of using the requisition worksheet is that it can create purchase orders for all outstanding drop shipments, so you don't have to create each one individually.</span></span>

1. <span data-ttu-id="21077-128">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы заявок**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="21077-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Requistion Worksheets**, and then choose the related link.</span></span>
2. <span data-ttu-id="21077-129">Выберите действие **Прямые поставки**, затем выберите действие **Получить заказ на продажу**.</span><span class="sxs-lookup"><span data-stu-id="21077-129">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
3. <span data-ttu-id="21077-130">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="21077-130">Choose the **OK** button.</span></span>
4. <span data-ttu-id="21077-131">Просмотрите строки заказа на покупку и в поле **Номер производителя** выберите поставщика, поставляющего необходимые товары.</span><span class="sxs-lookup"><span data-stu-id="21077-131">Review the purchase order lines, and in the **Vendor No.** field, select vendor that supplies required goods.</span></span> 
5. <span data-ttu-id="21077-132">Выберите действие **Выполнить указание** для преобразования проверенных строк в заказ на покупку.</span><span class="sxs-lookup"><span data-stu-id="21077-132">Choose the **Carry Out Action Message** action to convert reviewed lines to a purchase order.</span></span>

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="21077-133">Просмотр связанного заказа на покупку из заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="21077-133">To view the linked purchase order from the sales order</span></span>

* <span data-ttu-id="21077-134">Выберите строку заказа на продажу с прямой поставкой, выберите действие **Заказ**, выберите действие **Прямая поставка**, затем выберите действие **Заказ на покупку**.</span><span class="sxs-lookup"><span data-stu-id="21077-134">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="21077-135">Учет прямой поставки</span><span class="sxs-lookup"><span data-stu-id="21077-135">To post a drop shipment</span></span>

<span data-ttu-id="21077-136">После отгрузки товаров поставщиком можно учесть заказ на продажу как отгруженный.</span><span class="sxs-lookup"><span data-stu-id="21077-136">After the vendor ships the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="21077-137">Можно также учесть заказ на покупку, но только с параметром **Получить**, пока не будет выставлен счет по заказу на продажу.</span><span class="sxs-lookup"><span data-stu-id="21077-137">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>

1. <span data-ttu-id="21077-138">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="21077-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="21077-139">Откройте заказ на продажу, созданный в разделе [Создание заказа на продажу по прямой поставке](#to-create-a-sales-order-for-drop-shipment).</span><span class="sxs-lookup"><span data-stu-id="21077-139">Open the sales order that you created in [To create a sales order for drop shipment](#to-create-a-sales-order-for-drop-shipment).</span></span>
3. <span data-ttu-id="21077-140">В поле **Кол-во для отгрузки** укажите, какое количество из заказа следует доставить, полное или частичное количество по заказу.</span><span class="sxs-lookup"><span data-stu-id="21077-140">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
4. <span data-ttu-id="21077-141">Выберите действие **Учесть** или **Учесть и отправить**.</span><span class="sxs-lookup"><span data-stu-id="21077-141">Choose the **Post** or **Post and Send** action.</span></span>
5. <span data-ttu-id="21077-142">Выберите вариант **Отгрузить** (чтобы счет был выставлен позже) или вариант **Отгрузить и выставить счет** (чтобы счет был выставлен незамедлительно).</span><span class="sxs-lookup"><span data-stu-id="21077-142">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="21077-143">См. также</span><span class="sxs-lookup"><span data-stu-id="21077-143">See Also</span></span>

[<span data-ttu-id="21077-144">Создание специальных заказов</span><span class="sxs-lookup"><span data-stu-id="21077-144">Create Special Orders</span></span>](sales-how-to-create-special-orders.md)  
[<span data-ttu-id="21077-145">Покупка товаров для продажи</span><span class="sxs-lookup"><span data-stu-id="21077-145">Purchase Items for a Sale</span></span>](purchasing-how-purchase-products-sale.md)  
[<span data-ttu-id="21077-146">Продажа продуктов</span><span class="sxs-lookup"><span data-stu-id="21077-146">Sell Products</span></span>](sales-how-sell-products.md)  
[<span data-ttu-id="21077-147">Регистрация покупок</span><span class="sxs-lookup"><span data-stu-id="21077-147">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="21077-148">Продажи</span><span class="sxs-lookup"><span data-stu-id="21077-148">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="21077-149">Запасы</span><span class="sxs-lookup"><span data-stu-id="21077-149">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="21077-150">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="21077-150">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]