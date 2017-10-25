---
title: "Создание заказа на продажу, связанного с заказом на покупку для прямой поставки | Документы Майкрософт"
description: "Рассматривается создание заказа на покупку, связанного с заказом на продажу, для обеспечения прямой поставки от поставщика клиенту."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 990867cb428f860b1001177738d1a027f72485bc
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-make-drop-shipments"></a><span data-ttu-id="77ec2-103">Практическое руководство. Выполнение прямых поставок</span><span class="sxs-lookup"><span data-stu-id="77ec2-103">How to: Make Drop Shipments</span></span>
<span data-ttu-id="77ec2-104">Прямая поставка — это поставка товаров одним из ваших поставщиков непосредственно одному из ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="77ec2-104">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="77ec2-105">Когда заказ на продажу отмечен для прямой поставки и вы создаете заказ на покупку, указав клиента в поле **Код клиента (покупателя)**,</span><span class="sxs-lookup"><span data-stu-id="77ec2-105">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Sell-to Customer No.**</span></span> <span data-ttu-id="77ec2-106">можно связать эти два документа, дав таким образом поставщику инструкцию для поставки непосредственно в адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="77ec2-106">field, you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="77ec2-107">Создание заказа на продажу по прямой поставке</span><span class="sxs-lookup"><span data-stu-id="77ec2-107">To create a sales order for drop shipment</span></span>
<span data-ttu-id="77ec2-108">Для подготовки прямой поставки следует создать заказы на продажу для товара, как обычно, но необходимо указать в строке продажи, что продажа требует прямой поставки.</span><span class="sxs-lookup"><span data-stu-id="77ec2-108">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="77ec2-109">Создайте заказ на продажу для товара.</span><span class="sxs-lookup"><span data-stu-id="77ec2-109">Create a sales order for an item.</span></span> <span data-ttu-id="77ec2-110">Дополнительные сведения см. в разделе [Практическое руководство. Продажа продукции](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="77ec2-110">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="77ec2-111">В строке заказа на продажу для прямой поставки установите флажок **Прямая поставка**.</span><span class="sxs-lookup"><span data-stu-id="77ec2-111">On the sales order line for the drop shipment, select the **Drop Shipment** check box.</span></span> <span data-ttu-id="77ec2-112">Используйте функцию **Выбрать столбцы**, если поле не отображается.</span><span class="sxs-lookup"><span data-stu-id="77ec2-112">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="77ec2-113">Дополнительные сведения см. в разделе [Персонализация пользователя](ui-user-personalization.md).</span><span class="sxs-lookup"><span data-stu-id="77ec2-113">For more information, see [User Personalization](ui-user-personalization.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="77ec2-114">Эта функция требует, чтобы было задано значение **Suite**.</span><span class="sxs-lookup"><span data-stu-id="77ec2-114">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="77ec2-115">Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="77ec2-115">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="77ec2-116">Создание заказа на покупку для прямой поставки</span><span class="sxs-lookup"><span data-stu-id="77ec2-116">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="77ec2-117">Для подготовки прямой поставки для продаваемого товара следует создать обычный заказ на покупку, но необходимо указать в заказе на покупку, что он должен быть доставлен клиенту, а не вам.</span><span class="sxs-lookup"><span data-stu-id="77ec2-117">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="77ec2-118">Создайте заказ покупки.</span><span class="sxs-lookup"><span data-stu-id="77ec2-118">Create a purchase order.</span></span> <span data-ttu-id="77ec2-119">Не заполняйте никакие поля в строках.</span><span class="sxs-lookup"><span data-stu-id="77ec2-119">Do not fill any fields on the lines.</span></span> <span data-ttu-id="77ec2-120">Дополнительные сведения см. в разделе [Практическое руководство. Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="77ec2-120">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="77ec2-121">В поле **Код клиента (покупателя)**</span><span class="sxs-lookup"><span data-stu-id="77ec2-121">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="77ec2-122">выберите клиента, которому осуществляется продажа.</span><span class="sxs-lookup"><span data-stu-id="77ec2-122">field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="77ec2-123">Выберите действие **Прямые поставки**, затем выберите действие **Получить заказ на продажу**.</span><span class="sxs-lookup"><span data-stu-id="77ec2-123">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="77ec2-124">В окне **Список продаж** выберите заказ на продажу, который был подготовлен в разделе "Создание заказа на продажу по прямой поставке".</span><span class="sxs-lookup"><span data-stu-id="77ec2-124">In the **Sales List** window, select the sales order that you prepared in the "To create a sales order for drop shipment" section.</span></span>
5. <span data-ttu-id="77ec2-125">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="77ec2-125">Choose the **OK** button.</span></span>

<span data-ttu-id="77ec2-126">Информация строки в заказе на продажу будет вставлена в строки заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="77ec2-126">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="77ec2-127">Теперь можно проинструктировать поставщика, чтобы он отгрузил товары клиенту, например, переслав заказ на покупку в виде файла PDF.</span><span class="sxs-lookup"><span data-stu-id="77ec2-127">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="77ec2-128">Просмотр связанного заказа на покупку из заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="77ec2-128">To view the linked purchase order from the sales order</span></span>
* <span data-ttu-id="77ec2-129">Выберите строку заказа на продажу с прямой поставкой, выберите действие **Заказ**, выберите действие **Прямая поставка**, затем выберите действие **Заказ на покупку**.</span><span class="sxs-lookup"><span data-stu-id="77ec2-129">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="77ec2-130">Учет прямой поставки</span><span class="sxs-lookup"><span data-stu-id="77ec2-130">To post a drop shipment</span></span>
<span data-ttu-id="77ec2-131">После отгрузки товаров поставщиком можно учесть заказ на продажу как отгруженный.</span><span class="sxs-lookup"><span data-stu-id="77ec2-131">After the vendor ships the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="77ec2-132">Можно также учесть заказ на покупку, но только с параметром **Получить**, пока не будет выставлен счет по заказу на продажу.</span><span class="sxs-lookup"><span data-stu-id="77ec2-132">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>

1. <span data-ttu-id="77ec2-133">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Заказы на продажу**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="77ec2-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="77ec2-134">Откройте заказ на продажу, созданный в разделе "Создание заказа на продажу по прямой поставке".</span><span class="sxs-lookup"><span data-stu-id="77ec2-134">Open the sales order that you created in the "To create a sales order for a drop shipment" section.</span></span>
3. <span data-ttu-id="77ec2-135">В поле **Кол-во для отгрузки** укажите, какое количество из заказа следует доставить, полное или частичное количество по заказу.</span><span class="sxs-lookup"><span data-stu-id="77ec2-135">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
4. <span data-ttu-id="77ec2-136">Выберите действие **Учесть** или **Учесть и отправить**.</span><span class="sxs-lookup"><span data-stu-id="77ec2-136">Choose the **Post** or **Post and Send** action.</span></span>
5. <span data-ttu-id="77ec2-137">Выберите вариант **Отгрузить** (чтобы счет был выставлен позже) или вариант **Отгрузить и выставить счет** (чтобы счет был выставлен незамедлительно).</span><span class="sxs-lookup"><span data-stu-id="77ec2-137">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="77ec2-138">См. также</span><span class="sxs-lookup"><span data-stu-id="77ec2-138">See Also</span></span>
<span data-ttu-id="77ec2-139">[Практическое руководство. Создание специальных заказов](sales-how-to-create-special-orders.md)|</span><span class="sxs-lookup"><span data-stu-id="77ec2-139">[How to: Create Special Orders](sales-how-to-create-special-orders.md)|</span></span>  
[<span data-ttu-id="77ec2-140">Практическое руководство. Продажа продукции</span><span class="sxs-lookup"><span data-stu-id="77ec2-140">How to: Sell Products</span></span>](sales-how-sell-products.md)  
[<span data-ttu-id="77ec2-141">Практическое руководство. Регистрация покупок</span><span class="sxs-lookup"><span data-stu-id="77ec2-141">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="77ec2-142">Продажи</span><span class="sxs-lookup"><span data-stu-id="77ec2-142">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="77ec2-143">Наличие</span><span class="sxs-lookup"><span data-stu-id="77ec2-143">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="77ec2-144">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="77ec2-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

