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
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 977debf7386ad1113ef54147b20fd24c7c285a78
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-make-drop-shipments"></a><span data-ttu-id="eb8b4-103">Практическое руководство. Выполнение прямых поставок</span><span class="sxs-lookup"><span data-stu-id="eb8b4-103">How to: Make Drop Shipments</span></span>
<span data-ttu-id="eb8b4-104">Прямая поставка — это поставка товаров одним из ваших поставщиков непосредственно одному из ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-104">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="eb8b4-105">Когда заказ на продажу отмечен для прямой поставки и вы создаете заказ на покупку, указав клиента в поле **Код клиента (покупателя)**,</span><span class="sxs-lookup"><span data-stu-id="eb8b4-105">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Sell-to Customer No.**</span></span> <span data-ttu-id="eb8b4-106">можно связать эти два документа, дав таким образом поставщику инструкцию для поставки непосредственно в адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-106">field, you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="eb8b4-107">Создание заказа на продажу по прямой поставке</span><span class="sxs-lookup"><span data-stu-id="eb8b4-107">To create a sales order for drop shipment</span></span>
<span data-ttu-id="eb8b4-108">Для подготовки прямой поставки следует создать заказы на продажу для товара, как обычно, но необходимо указать в строке продажи, что продажа требует прямой поставки.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-108">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="eb8b4-109">Создайте заказ на продажу для товара.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-109">Create a sales order for an item.</span></span> <span data-ttu-id="eb8b4-110">Дополнительные сведения см. в разделе [Практическое руководство. Продажа продукции](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="eb8b4-110">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="eb8b4-111">В строке заказа на продажу для прямой поставки установите флажок **Прямая поставка**.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-111">On the sales order line for the drop shipment, select the **Drop Shipment** check box.</span></span> <span data-ttu-id="eb8b4-112">Используйте функцию **Выбрать столбцы**, если поле не отображается.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-112">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="eb8b4-113">Дополнительные сведения см. в разделе [Персонализация пользователя](ui-user-personalization.md).</span><span class="sxs-lookup"><span data-stu-id="eb8b4-113">For more information, see [User Personalization](ui-user-personalization.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="eb8b4-114">Эта функция требует, чтобы было задано значение **Пакет**.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-114">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="eb8b4-115">Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="eb8b4-115">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="eb8b4-116">Создание заказа на покупку для прямой поставки</span><span class="sxs-lookup"><span data-stu-id="eb8b4-116">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="eb8b4-117">Для подготовки прямой поставки для продаваемого товара следует создать обычный заказ на покупку, но необходимо указать в заказе на покупку, что он должен быть доставлен клиенту, а не вам.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-117">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="eb8b4-118">Создайте заказ покупки.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-118">Create a purchase order.</span></span> <span data-ttu-id="eb8b4-119">Не заполняйте никакие поля в строках.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-119">Do not fill any fields on the lines.</span></span> <span data-ttu-id="eb8b4-120">Дополнительные сведения см. в разделе [Практическое руководство. Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="eb8b4-120">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="eb8b4-121">В поле **Код клиента (покупателя)**</span><span class="sxs-lookup"><span data-stu-id="eb8b4-121">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="eb8b4-122">выберите клиента, которому осуществляется продажа.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-122">field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="eb8b4-123">Выберите действие **Прямые поставки**, затем выберите действие **Получить заказ на продажу**.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-123">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="eb8b4-124">В окне **Список продаж** выберите заказ на продажу, который был подготовлен в разделе "Создание заказа на продажу по прямой поставке".</span><span class="sxs-lookup"><span data-stu-id="eb8b4-124">In the **Sales List** window, select the sales order that you prepared in the "To create a sales order for drop shipment" section.</span></span>
5. <span data-ttu-id="eb8b4-125">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-125">Choose the **OK** button.</span></span>

<span data-ttu-id="eb8b4-126">Информация строки в заказе на продажу будет вставлена в строки заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-126">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="eb8b4-127">Теперь можно проинструктировать поставщика, чтобы он отгрузил товары клиенту, например, переслав заказ на покупку в виде файла PDF.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-127">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="eb8b4-128">Просмотр связанного заказа на покупку из заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="eb8b4-128">To view the linked purchase order from the sales order</span></span>
* <span data-ttu-id="eb8b4-129">Выберите строку заказа на продажу с прямой поставкой, выберите действие **Заказ**, выберите действие **Прямая поставка**, затем выберите действие **Заказ на покупку**.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-129">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="eb8b4-130">Учет прямой поставки</span><span class="sxs-lookup"><span data-stu-id="eb8b4-130">To post a drop shipment</span></span>
<span data-ttu-id="eb8b4-131">После отгрузки товаров поставщиком можно учесть заказ на продажу как отгруженный.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-131">After the vendor ships the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="eb8b4-132">Можно также учесть заказ на покупку, но только с параметром **Получить**, пока не будет выставлен счет по заказу на продажу.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-132">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>

1. <span data-ttu-id="eb8b4-133">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Заказы на продажу**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="eb8b4-134">Откройте заказ на продажу, созданный в разделе "Создание заказа на продажу по прямой поставке".</span><span class="sxs-lookup"><span data-stu-id="eb8b4-134">Open the sales order that you created in the "To create a sales order for a drop shipment" section.</span></span>
3. <span data-ttu-id="eb8b4-135">В поле **Кол-во для отгрузки** укажите, какое количество из заказа следует доставить, полное или частичное количество по заказу.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-135">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
4. <span data-ttu-id="eb8b4-136">Выберите действие **Учесть** или **Учесть и отправить**.</span><span class="sxs-lookup"><span data-stu-id="eb8b4-136">Choose the **Post** or **Post and Send** action.</span></span>
5. <span data-ttu-id="eb8b4-137">Выберите вариант **Отгрузить** (чтобы счет был выставлен позже) или вариант **Отгрузить и выставить счет** (чтобы счет был выставлен незамедлительно).</span><span class="sxs-lookup"><span data-stu-id="eb8b4-137">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="eb8b4-138">См. также</span><span class="sxs-lookup"><span data-stu-id="eb8b4-138">See Also</span></span>
[<span data-ttu-id="eb8b4-139">Практическое руководство. Продажа продукции</span><span class="sxs-lookup"><span data-stu-id="eb8b4-139">How to: Sell Products</span></span>](sales-how-sell-products.md)  
[<span data-ttu-id="eb8b4-140">Практическое руководство. Регистрация покупок</span><span class="sxs-lookup"><span data-stu-id="eb8b4-140">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="eb8b4-141">Продажи</span><span class="sxs-lookup"><span data-stu-id="eb8b4-141">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="eb8b4-142">Запасы</span><span class="sxs-lookup"><span data-stu-id="eb8b4-142">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="eb8b4-143">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="eb8b4-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

