---
title: "Создание счета покупки из счета продажи для покупки товаров для продажи | Документы Майкрософт"
description: "Из счета продажи для покупки продуктов вы можете создать счет покупки для поставщика."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supply planning, sales demand, replenish
ms.date: 05/16/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 2d7eb238395a0b1060668996fbbc3e13d9dd8a94
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-purchase-items-for-a-sale"></a><span data-ttu-id="6b0a4-103">Практическое руководство. Покупка товаров для продажи</span><span class="sxs-lookup"><span data-stu-id="6b0a4-103">How to: Purchase Items for a Sale</span></span>
<span data-ttu-id="6b0a4-104">Из заказов на продажу и счетов продажи можно быстро создавать документы покупки на недостающие количества товаров, требуемые для продажи.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-104">From sales orders and sales invoices, you can use functions to quickly create purchase documents for missing item quantities that are required by the sale.</span></span> <span data-ttu-id="6b0a4-105">Вы можете использовать две различные функции в зависимости от типа документа.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-105">You can use two different functions depending on the document type.</span></span>
|<span data-ttu-id="6b0a4-106">Функция</span><span class="sxs-lookup"><span data-stu-id="6b0a4-106">Function</span></span>|<span data-ttu-id="6b0a4-107">Описанием</span><span class="sxs-lookup"><span data-stu-id="6b0a4-107">Description</span></span>|
|--------|-----------|
|<span data-ttu-id="6b0a4-108">**Создать заказы на покупку**</span><span class="sxs-lookup"><span data-stu-id="6b0a4-108">**Create Purchase Orders**</span></span>|<span data-ttu-id="6b0a4-109">Из заказа на продажу эта функция позволяет создать заказ на покупку для каждого поставщика товаров в заказе на продажу.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-109">From a sales order, this function creates a purchase order for each vendor of items on the sales order.</span></span> <span data-ttu-id="6b0a4-110">Вы можете изменить количество покупки, прежде чем создать заказы на покупку.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-110">You can edit the purchase quantity before you create the purchase orders.</span></span> <span data-ttu-id="6b0a4-111">Предлагаются только недостающие количества.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-111">Only unavailable sales quantities are suggested.</span></span>
|<span data-ttu-id="6b0a4-112">**Создать счет покупки**</span><span class="sxs-lookup"><span data-stu-id="6b0a4-112">**Create Purchase Invoice**</span></span>|<span data-ttu-id="6b0a4-113">Из заказа на продажу и из счета продажи эта функция создает счет покупки для выбранного поставщика для всех строк или выбранных строк в документе продажи.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-113">From a sales order and from a sales invoice, this function creates a purchase invoice for a selected vendor for all lines or selected lines on the sales document.</span></span> <span data-ttu-id="6b0a4-114">Предлагается полное количество продажи.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-114">The full sales quantity is suggested.</span></span>|

## <a name="to-create-one-or-more-purchase-orders-from-a-sales-order"></a><span data-ttu-id="6b0a4-115">Создание одного или нескольких заказов на покупку из заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="6b0a4-115">To create one or more purchase orders from a sales order</span></span>
<span data-ttu-id="6b0a4-116">Чтобы создать заказ на покупку для каждого недостающего количества товаров в заказе на продажу, можно воспользоваться функцией **Создать заказы на покупку**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-116">To create a purchase order for each unavailable item quantity on the sales order, you use the **Create Purchase Orders** function.</span></span> 

> [!NOTE]  
>   <span data-ttu-id="6b0a4-117">Эта функция требует, чтобы было задано значение **Пакет**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-117">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="6b0a4-118">Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="6b0a4-118">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

1. <span data-ttu-id="6b0a4-119">На начальной странице выберите плитку **Текущие заказы на продажу**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-119">On the Home page, choose the **Ongoing Sales Orders** tile.</span></span>
2. <span data-ttu-id="6b0a4-120">Откройте заказ на продажу, для которого требуется купить товары.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-120">Open a sales order that you want to purchase items for.</span></span>
3. <span data-ttu-id="6b0a4-121">Выберите действие **Создать заказы на покупку**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-121">Choose the **Create Purchase Orders** action.</span></span>

    <span data-ttu-id="6b0a4-122">Откроется окно **Создать заказы на покупку**, содержащее строку для каждого отдельного товара в заказе на продажу.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-122">The **Create Purchase Orders** window opens showing a line for each different item on the sales order.</span></span> <span data-ttu-id="6b0a4-123">Строки для полностью доступных количеств продажи и недоступных количеств продажи (серые) отображаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-123">Lines for both fully available sales quantities and unavailable sales quantities (grayed) are shown by default.</span></span> <span data-ttu-id="6b0a4-124">Вы можете выбрать действие **Показать недоступные** для просмотра только строк для недоступных количеств продажи.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-124">You can choose the **Show Unavailable** action to only see lines for unavailable sales quantities.</span></span>

    <span data-ttu-id="6b0a4-125">Поле **Кол-во для покупки** по умолчанию содержит недоступное для продажи количество.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-125">The **Quantity to Purchase** field contains the unavailable sales quantity by default.</span></span>
4. <span data-ttu-id="6b0a4-126">Чтобы купить количество, отличное от недоступного для продажи, измените значение поля **Кол-во для покупки**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-126">To purchase another quantity than the unavailable sales quantity, edit the value in the **Quantity to Purchase** field.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="6b0a4-127">Также можно изменить поле **Кол-во для покупки** в серых строках, даже если они представляют полностью доступное количество для продажи.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-127">You can also change the **Quantity to Purchase** field on grayed lines even though they represent fully available sales quantities.</span></span>
5. <span data-ttu-id="6b0a4-128">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-128">Choose the **OK** button.</span></span> 
    
    <span data-ttu-id="6b0a4-129">Заказ на покупку создается для каждого поставщика товаров в заказа на продажу и включает все изменения количества, которые вы сделали в окне **Создать заказы на покупку**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-129">A purchase order is created for each vendor of items on the sales order, including any quantity changes that you made in the **Create Purchase Orders** window.</span></span>
7. <span data-ttu-id="6b0a4-130">Продолжите обработку заказов на покупку, например изменив или добавив строки заказов на покупку.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-130">Proceed to process the purchase order or orders, for example, by editing or adding purchase order lines.</span></span> <span data-ttu-id="6b0a4-131">Дополнительные сведения см. в разделе [Практическое руководство. Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="6b0a4-131">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>


## <a name="to-create-a-purchase-invoice-from-a-sales-order-or-sales-invoice"></a><span data-ttu-id="6b0a4-132">Создание счета покупки из заказа на продажу или счета продажи</span><span class="sxs-lookup"><span data-stu-id="6b0a4-132">To create a purchase invoice from a sales order or sales invoice</span></span>
<span data-ttu-id="6b0a4-133">Чтобы создать отдельный счет покупки для одно или нескольких строк в документе продажи, выбрав поставщика, у которого будет совершена покупка, воспользуйтесь функцией **Создать счет покупки**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-133">To create a single purchase invoice for one or more lines on a sales document by first selecting which vendor to buy from, you use the **Create Purchase Invoice** function.</span></span> 

> [!NOTE]  
>   <span data-ttu-id="6b0a4-134">Эта функция создает счет покупки на точное количество товара в выбранном документе продажи.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-134">This function creates a purchase invoice for the exact item quantity on the selected sales document.</span></span> <span data-ttu-id="6b0a4-135">Чтобы изменить количество для покупки, необходимо изменить счет покупки после его создания.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-135">To change the purchase quantity, you must edit the purchase invoice after it is created.</span></span>  

1. <span data-ttu-id="6b0a4-136">На начальной странице выберите плитку **Текущие счета продажи**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-136">On the Home page, choose the **Ongoing Sales Invoices** tile.</span></span>
2. <span data-ttu-id="6b0a4-137">Откройте счет продажи, для которого требуется купить товары.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-137">Open a sales invoice that you want to purchase items for.</span></span>
3. <span data-ttu-id="6b0a4-138">Выберите одну или несколько строк счета продажи, которые требуется использовать в счете покупки.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-138">Select one or more sales invoice lines that you want to use on the purchase invoice.</span></span> <span data-ttu-id="6b0a4-139">Для использования всех строк счета продажи выберите их все или не выбирайте ни одной.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-139">To use all the sales invoice lines, select either all of them or do not select any lines.</span></span>
4. <span data-ttu-id="6b0a4-140">Выберите действие **Создать счет покупки**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-140">Choose the **Create Purchase Invoice** action.</span></span>
5. <span data-ttu-id="6b0a4-141">Выберите **Все строки** или **Выбранные строки**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-141">Select either **All Lines** or **Selected Lines**, and then choose the **OK** button.</span></span>  
6. <span data-ttu-id="6b0a4-142">В открывшемся списке поставщиков выберите поставщика, у которого требуется купить все товары, и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-142">In the list of vendors that appears, select the vendor that you want to buy all the items from, and then choose the **OK** button.</span></span>

    <span data-ttu-id="6b0a4-143">Создается счет покупки с одной, несколькими или всеми строками из счета продажи.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-143">A purchase invoice is created that contains one, more, or all the lines on the sales invoice.</span></span>
7. <span data-ttu-id="6b0a4-144">Продолжите обработку счета покупки, например изменив или добавив строки счета покупки.</span><span class="sxs-lookup"><span data-stu-id="6b0a4-144">Proceed to process the purchase invoice, for example, by editing or adding purchase invoice lines.</span></span> <span data-ttu-id="6b0a4-145">Дополнительные сведения см. в разделе [Практическое руководство. Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="6b0a4-145">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="6b0a4-146">См. также</span><span class="sxs-lookup"><span data-stu-id="6b0a4-146">See Also</span></span>
[<span data-ttu-id="6b0a4-147">Покупки</span><span class="sxs-lookup"><span data-stu-id="6b0a4-147">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="6b0a4-148">Практическое руководство. Регистрация покупок</span><span class="sxs-lookup"><span data-stu-id="6b0a4-148">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="6b0a4-149">Практическое руководство. Выставление счетов продажи</span><span class="sxs-lookup"><span data-stu-id="6b0a4-149">How to: Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="6b0a4-150">Практическое руководство. Регистрация новых поставщиков</span><span class="sxs-lookup"><span data-stu-id="6b0a4-150">How to: Register New Vendors</span></span>](purchasing-how-register-new-vendors.md)  
<span data-ttu-id="6b0a4-151">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6b0a4-151">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

