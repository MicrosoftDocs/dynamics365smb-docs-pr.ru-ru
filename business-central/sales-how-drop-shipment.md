---
title: Связывание заказа на продажу с заказом на покупку для прямой поставки | Документация Майкрософт
description: Рассматривается создание заказа на покупку, связанного с заказом на продажу, для обеспечения прямой поставки от поставщика клиенту.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 50198afaa8caae9a11a06a25357fa94ad26b0b8f
ms.sourcegitcommit: b570997f93d1f7141bc9539c93a67a91226660a8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2020
ms.locfileid: "2943189"
---
# <a name="make-drop-shipments"></a><span data-ttu-id="43d2d-103">Выполнение прямых поставок</span><span class="sxs-lookup"><span data-stu-id="43d2d-103">Make Drop Shipments</span></span>
<span data-ttu-id="43d2d-104">Прямая поставка — это поставка товаров одним из ваших поставщиков непосредственно одному из ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="43d2d-104">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="43d2d-105">Когда заказ на продажу помечен для прямой поставки, и вы создаете заказ на покупку, указывая клиента в поле **Получатель**, **Адрес клиента**, вы можете связать два документа и, тем самым, дать указание поставщику отправить товар непосредственно клиенту.</span><span class="sxs-lookup"><span data-stu-id="43d2d-105">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Ship-to** field, **Customer Address**, you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>
<br><br>  
  
> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4mOyM]

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="43d2d-106">Создание заказа на продажу по прямой поставке</span><span class="sxs-lookup"><span data-stu-id="43d2d-106">To create a sales order for drop shipment</span></span>
<span data-ttu-id="43d2d-107">Для подготовки прямой поставки следует создать заказы на продажу для товара, как обычно, но необходимо указать в строке продажи, что продажа требует прямой поставки.</span><span class="sxs-lookup"><span data-stu-id="43d2d-107">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="43d2d-108">Создайте заказ на продажу для товара.</span><span class="sxs-lookup"><span data-stu-id="43d2d-108">Create a sales order for an item.</span></span> <span data-ttu-id="43d2d-109">Дополнительные сведения см. в разделе [Продажа продукции](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="43d2d-109">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="43d2d-110">В строке заказа на продажу для прямой поставки установите флажок **Прямая поставка**.</span><span class="sxs-lookup"><span data-stu-id="43d2d-110">On the sales order line for the drop shipment, select the **Drop Shipment** check box.</span></span> <span data-ttu-id="43d2d-111">Используйте функцию **Выбрать столбцы**, если поле не отображается.</span><span class="sxs-lookup"><span data-stu-id="43d2d-111">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="43d2d-112">Дополнительные сведения см. в разделе [Персонализация рабочей области](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="43d2d-112">For more information, see [Personalize Your Workspace](ui-personalization-user.md).</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="43d2d-113">Создание заказа на покупку для прямой поставки</span><span class="sxs-lookup"><span data-stu-id="43d2d-113">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="43d2d-114">Для подготовки прямой поставки для продаваемого товара следует создать обычный заказ на покупку, но необходимо указать в заказе на покупку, что он должен быть доставлен клиенту, а не вам.</span><span class="sxs-lookup"><span data-stu-id="43d2d-114">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="43d2d-115">Создайте заказ покупки.</span><span class="sxs-lookup"><span data-stu-id="43d2d-115">Create a purchase order.</span></span> <span data-ttu-id="43d2d-116">Не заполняйте никакие поля в строках.</span><span class="sxs-lookup"><span data-stu-id="43d2d-116">Do not fill any fields on the lines.</span></span> <span data-ttu-id="43d2d-117">Дополнительные сведения см. в разделе [Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="43d2d-117">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="43d2d-118">В поле **Получатель** выберите **Адрес клиента**.</span><span class="sxs-lookup"><span data-stu-id="43d2d-118">In the **Ship-to** field, select **Customer Address**.</span></span>
3. <span data-ttu-id="43d2d-119">В поле **Клиент** выберите клиента, которому осуществляется продажа.</span><span class="sxs-lookup"><span data-stu-id="43d2d-119">In the **Customer** field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="43d2d-120">Выберите действие **Прямые поставки**, затем выберите действие **Получить заказ на продажу**.</span><span class="sxs-lookup"><span data-stu-id="43d2d-120">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="43d2d-121">На странице **Список продаж** выберите заказ на продажу, который был подготовлен в разделе [Создание заказа на продажу по прямой поставке](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment).</span><span class="sxs-lookup"><span data-stu-id="43d2d-121">On the **Sales List** page, select the sales order that you prepared in [To create a sales order for drop shipment](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment).</span></span>
5. <span data-ttu-id="43d2d-122">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="43d2d-122">Choose the **OK** button.</span></span>

<span data-ttu-id="43d2d-123">Информация строки в заказе на продажу будет вставлена в строки заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="43d2d-123">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="43d2d-124">Теперь можно проинструктировать поставщика, чтобы он отгрузил товары клиенту, например, переслав заказ на покупку в виде файла PDF.</span><span class="sxs-lookup"><span data-stu-id="43d2d-124">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="43d2d-125">Просмотр связанного заказа на покупку из заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="43d2d-125">To view the linked purchase order from the sales order</span></span>
* <span data-ttu-id="43d2d-126">Выберите строку заказа на продажу с прямой поставкой, выберите действие **Заказ**, выберите действие **Прямая поставка**, затем выберите действие **Заказ на покупку**.</span><span class="sxs-lookup"><span data-stu-id="43d2d-126">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="43d2d-127">Учет прямой поставки</span><span class="sxs-lookup"><span data-stu-id="43d2d-127">To post a drop shipment</span></span>
<span data-ttu-id="43d2d-128">После отгрузки товаров поставщиком можно учесть заказ на продажу как отгруженный.</span><span class="sxs-lookup"><span data-stu-id="43d2d-128">After the vendor ships the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="43d2d-129">Можно также учесть заказ на покупку, но только с параметром **Получить**, пока не будет выставлен счет по заказу на продажу.</span><span class="sxs-lookup"><span data-stu-id="43d2d-129">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>

1. <span data-ttu-id="43d2d-130">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="43d2d-130">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="43d2d-131">Откройте заказ на продажу, созданный в разделе [Создание заказа на продажу по прямой поставке]().</span><span class="sxs-lookup"><span data-stu-id="43d2d-131">Open the sales order that you created in [To create a sales order for drop shipment]().</span></span>
3. <span data-ttu-id="43d2d-132">В поле **Кол-во для отгрузки** укажите, какое количество из заказа следует доставить, полное или частичное количество по заказу.</span><span class="sxs-lookup"><span data-stu-id="43d2d-132">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
4. <span data-ttu-id="43d2d-133">Выберите действие **Учесть** или **Учесть и отправить**.</span><span class="sxs-lookup"><span data-stu-id="43d2d-133">Choose the **Post** or **Post and Send** action.</span></span>
5. <span data-ttu-id="43d2d-134">Выберите вариант **Отгрузить** (чтобы счет был выставлен позже) или вариант **Отгрузить и выставить счет** (чтобы счет был выставлен незамедлительно).</span><span class="sxs-lookup"><span data-stu-id="43d2d-134">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="43d2d-135">См. также</span><span class="sxs-lookup"><span data-stu-id="43d2d-135">See Also</span></span>
[<span data-ttu-id="43d2d-136">Создание специальных заказов</span><span class="sxs-lookup"><span data-stu-id="43d2d-136">Create Special Orders</span></span>](sales-how-to-create-special-orders.md)  
[<span data-ttu-id="43d2d-137">Покупка товаров для продажи</span><span class="sxs-lookup"><span data-stu-id="43d2d-137">Purchase Items for a Sale</span></span>](purchasing-how-purchase-products-sale.md)  
[<span data-ttu-id="43d2d-138">Продажа продуктов</span><span class="sxs-lookup"><span data-stu-id="43d2d-138">Sell Products</span></span>](sales-how-sell-products.md)  
[<span data-ttu-id="43d2d-139">Регистрация покупок</span><span class="sxs-lookup"><span data-stu-id="43d2d-139">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="43d2d-140">Продажи</span><span class="sxs-lookup"><span data-stu-id="43d2d-140">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="43d2d-141">Запасы</span><span class="sxs-lookup"><span data-stu-id="43d2d-141">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="43d2d-142">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="43d2d-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
