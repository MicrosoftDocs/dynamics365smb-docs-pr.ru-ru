---
title: "Создание счета покупки и запись покупок | Документы Майкрософт"
description: "Описывается, как приобрести товары типа \"Запасы\" или \"Услуга\" путем создания и учета счетов покупки или заказов на покупку."
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: procurement
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 60906dde627216903b5ef82e34ce4bc918f3c988
ms.contentlocale: ru-ru
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-record-purchases"></a><span data-ttu-id="5d876-103">Практическое руководство. Регистрация покупок</span><span class="sxs-lookup"><span data-stu-id="5d876-103">How to: Record Purchases</span></span>
<span data-ttu-id="5d876-104">Счет покупки или заказ на покупку создается для записи стоимости покупок и отслеживания кредиторской задолженности.</span><span class="sxs-lookup"><span data-stu-id="5d876-104">You create a purchase invoice or purchase order to record the cost of purchases and to track accounts payable.</span></span> <span data-ttu-id="5d876-105">Если требуется управлять запасами, счета покупки и заказы на покупку также используются для динамического обновления уровней запасов, чтобы уменьшить себестоимости запасов и обеспечить лучшее обслуживание клиентов.</span><span class="sxs-lookup"><span data-stu-id="5d876-105">If you need to control an inventory, purchase invoices and purchase orders are also used to dynamically update inventory levels so that you can minimize your inventory costs and provide better customer service.</span></span> <span data-ttu-id="5d876-106">Себестоимость покупок, включая затраты на обслуживание, и стоимость запасов, полученная из учета счетов покупки или заказы на покупку, влияют показатели прибыли и другие ключевые показатели эффективности финансовой деятельности, отображаемые на начальной странице.</span><span class="sxs-lookup"><span data-stu-id="5d876-106">The purchasing costs, including service expenses, and inventory values that result from posting purchase invoices or orders contribute to profit figures and other financial KPIs on your Home page.</span></span>

> [!NOTE]  
>   <span data-ttu-id="5d876-107">Заказы на покупку следует использовать, если процесс покупки требует, чтобы вы могли регистрировать частичную приемку количества в заказе, например потому, что полное количество недоступно у поставщика.</span><span class="sxs-lookup"><span data-stu-id="5d876-107">You must use purchase orders if your purchasing process requires that you record partial receipts of an order quantity, for example, because the full quantity was not available at the vendor.</span></span> <span data-ttu-id="5d876-108">Если продажа товаров осуществляется путем непосредственной поставки от поставщика клиенту (прямая поставка), то также необходимо использовать заказы на покупку.</span><span class="sxs-lookup"><span data-stu-id="5d876-108">If you sell items by delivering directly from your vendor to your customer, as a drop shipment, then you must also use purchase orders.</span></span> <span data-ttu-id="5d876-109">Дополнительные сведения см. в разделе [Практическое руководство. Выполнение прямых поставок](sales-how-drop-shipment.md).</span><span class="sxs-lookup"><span data-stu-id="5d876-109">For more information, see [How to: Make Drop Shipments](sales-how-drop-shipment.md).</span></span> <span data-ttu-id="5d876-110">Во всех других аспектах заказы на покупку аналогичны счетам покупки.</span><span class="sxs-lookup"><span data-stu-id="5d876-110">In all other aspects, purchase orders work the same way as purchase invoices.</span></span> <span data-ttu-id="5d876-111">Следующая процедура основана на счете покупки.</span><span class="sxs-lookup"><span data-stu-id="5d876-111">The following procedure is based on a purchase invoice.</span></span> <span data-ttu-id="5d876-112">Действия для заказа на покупку аналогичны.</span><span class="sxs-lookup"><span data-stu-id="5d876-112">The steps are similar for a purchase order.</span></span>

<span data-ttu-id="5d876-113">При получении складских товаров или выполнении приобретенной услуги счет покупки или заказ на покупку учитывается, чтобы обновить складские и финансовые записи и активировать платеж поставщику в соответствии с условиями оплаты.</span><span class="sxs-lookup"><span data-stu-id="5d876-113">When you receive the inventory items, or when the purchased service is completed, you post the purchase invoice or order to update inventory and financial records and to activate payment to the vendor according to the payment terms.</span></span> <span data-ttu-id="5d876-114">Дополнительные сведения см. в разделе [Осуществление платежей](payables-make-payments.md).</span><span class="sxs-lookup"><span data-stu-id="5d876-114">For more information, see [Make Payments](payables-make-payments.md).</span></span>

> [!CAUTION]  
>   <span data-ttu-id="5d876-115">Не выполняйте учет счета покупки, пока не будут получены товары и не будет известна конечная стоимость покупки, включая все дополнительные издержки.</span><span class="sxs-lookup"><span data-stu-id="5d876-115">Do not post a purchase invoice until you receive the items and know the final cost of the purchase, including any additional charges.</span></span> <span data-ttu-id="5d876-116">В противном случае значения стоимости запасов и прибыли могут быть неверными.</span><span class="sxs-lookup"><span data-stu-id="5d876-116">Otherwise, your inventory value and profit figures may be skewed.</span></span>

<span data-ttu-id="5d876-117">Можно легко скорректировать или отменить учтенный счет покупки до оплаты поставщику.</span><span class="sxs-lookup"><span data-stu-id="5d876-117">You can easily correct or cancel a posted purchase invoice before you pay the vendor.</span></span> <span data-ttu-id="5d876-118">Это используется, если нужно исправить опечатку или внести изменение в покупку на раннем этапе обработки заказа.</span><span class="sxs-lookup"><span data-stu-id="5d876-118">This is useful if you want to correct a typing mistake or if you want to change the purchase early in the order process.</span></span> <span data-ttu-id="5d876-119">Дополнительные сведения см. в разделе [Практическое руководство. Исправление или отмена неоплаченных счетов покупки](purchasing-how-correct-cancel-unpaid-purchase-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="5d876-119">For more information, see [How to: Correct or Cancel Unpaid Purchase Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md).</span></span> <span data-ttu-id="5d876-120">Если товары в учтенном счете покупки уже оплачены, необходимо создать кредит-ноту покупки для сторнирования покупки.</span><span class="sxs-lookup"><span data-stu-id="5d876-120">If you have already paid for items on the posted purchase invoice, then you must create a purchase credit memo to reverse the purchase.</span></span> <span data-ttu-id="5d876-121">Дополнительные сведения см. в разделе [Практическое руководство. Обработка возвратов покупки или отмен](purchasing-how-process-purchase-returns-cancellations.md)</span><span class="sxs-lookup"><span data-stu-id="5d876-121">For more information, see [How to: Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).</span></span>

<span data-ttu-id="5d876-122">Товар может иметь тип **Запасы** или **Услуга**.</span><span class="sxs-lookup"><span data-stu-id="5d876-122">Items can be type **Inventory** or **Service**.</span></span> <span data-ttu-id="5d876-123">Дополнительные сведения см. в разделе [Практическое руководство. Регистрация новых товаров](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="5d876-123">For more information, see [How to: Register New Items](inventory-how-register-new-items.md).</span></span> <span data-ttu-id="5d876-124">Процедура обработки счетов покупки такая же для обоих типов товаров.</span><span class="sxs-lookup"><span data-stu-id="5d876-124">The purchase invoice process is the same for both item types.</span></span>

> [!NOTE]  
>   <span data-ttu-id="5d876-125">Функция заказа на покупку требует, чтобы было задано значение **Пакет**.</span><span class="sxs-lookup"><span data-stu-id="5d876-125">Purchase order functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="5d876-126">Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="5d876-126">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

<span data-ttu-id="5d876-127">Можно заполнить поля поставщика в счете покупки двумя способами в зависимости от того, зарегистрирован ли уже поставщик.</span><span class="sxs-lookup"><span data-stu-id="5d876-127">You can fill vendor fields on the purchase invoice in two ways depending on whether the vendor is already registered.</span></span>

## <a name="to-create-a-purchase-invoice"></a><span data-ttu-id="5d876-128">Создание счета покупки</span><span class="sxs-lookup"><span data-stu-id="5d876-128">To create a purchase invoice</span></span>
1. <span data-ttu-id="5d876-129">На начальной странице выберите действие **Счет покупки**.</span><span class="sxs-lookup"><span data-stu-id="5d876-129">On the Home page, choose the **Purchase Invoice** action.</span></span>  
2. <span data-ttu-id="5d876-130">В поле **Поставщик** введите название существующего поставщика.</span><span class="sxs-lookup"><span data-stu-id="5d876-130">In the **Vendor** field, enter the name of an existing vendor.</span></span>

    <span data-ttu-id="5d876-131">Остальные поля в окне **Счет покупки** заполнятся стандартными сведениями о выбранном поставщике.</span><span class="sxs-lookup"><span data-stu-id="5d876-131">Other fields in the **Purchase Invoice** window are now filled with the standard information of the selected vendor.</span></span> <span data-ttu-id="5d876-132">Если поставщик не зарегистрирован, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="5d876-132">If the vendor is not registered, then follow these steps:</span></span>
3. <span data-ttu-id="5d876-133">В поле **Поставщик** введите название нового поставщика.</span><span class="sxs-lookup"><span data-stu-id="5d876-133">In the **Vendor** field, enter the name of the new vendor.</span></span>
4. <span data-ttu-id="5d876-134">В диалоговом окне регистрации нового поставщика нажмите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="5d876-134">In the dialog box about registering the new vendor, choose the **Yes** button.</span></span>
5. <span data-ttu-id="5d876-135">В окне **Выбор шаблона для нового поставщика** выберите шаблон для создания новой карточки поставщика и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="5d876-135">In the **Select a template for a new vendor** window, choose a template to base the new vendor card on, and then choose the **OK** button.</span></span>
6. <span data-ttu-id="5d876-136">Откроется новая карточка поставщика, предварительно заполненная сведениями из выбранного шаблона поставщика.</span><span class="sxs-lookup"><span data-stu-id="5d876-136">A new vendor card opens, prefilled with the information on the selected vendor template.</span></span> <span data-ttu-id="5d876-137">Поле **Название** предварительно заполняется названием нового поставщика, введенным в счете покупки.</span><span class="sxs-lookup"><span data-stu-id="5d876-137">The **Name** field is prefilled with the new vendor’s name that you entered on the purchase invoice.</span></span>
7. <span data-ttu-id="5d876-138">Перейдите к заполнению остальных полей в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="5d876-138">Proceed to fill in the remaining fields on the vendor card.</span></span> <span data-ttu-id="5d876-139">Дополнительные сведения см. в разделе [Практическое руководство. Регистрация новых поставщиков](purchasing-how-register-new-vendors.md).</span><span class="sxs-lookup"><span data-stu-id="5d876-139">For more information, see [How to: Register New Vendors](purchasing-how-register-new-vendors.md).</span></span>  
8. <span data-ttu-id="5d876-140">Заполнив карточку поставщика, нажмите кнопку **ОК**, чтобы вернуться в окно **Счет покупки**.</span><span class="sxs-lookup"><span data-stu-id="5d876-140">When you have completed the vendor card, choose the **OK** button to return to the **Purchase Invoice** window.</span></span>

    <span data-ttu-id="5d876-141">Несколько полей в окне **Счет покупки** заполняются сведениями, указанными в новой карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="5d876-141">Several fields in the **Purchase Invoice** window are filled with information that you specified on the new vendor card.</span></span>
9. <span data-ttu-id="5d876-142">Заполните остальные поля в окне **Счет покупки**, как требуется.</span><span class="sxs-lookup"><span data-stu-id="5d876-142">Fill in the remaining fields in the **Purchase Invoice** window as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    <span data-ttu-id="5d876-143">Теперь вы готовы к заполнению строк счета покупки сведениями о товарах в запасах или услугах, приобретенных у поставщика.</span><span class="sxs-lookup"><span data-stu-id="5d876-143">You are now ready to fill in the purchase invoice lines with inventory items or services that you have purchased from the vendor.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="5d876-144">Если заданы строки типовых покупок для поставщика, например ежемесячный заказ пополнения заказов, можно вставить строки в счет, выбрав действие **Получить строки типовых покупок**.</span><span class="sxs-lookup"><span data-stu-id="5d876-144">If you have set up recurring purchase lines for the vendor, such as a monthly replenishment order, then you can insert these lines on the invoice by choosing the **Get Recurring Purchase Lines** action.</span></span>
10. <span data-ttu-id="5d876-145">На экспресс-вкладке **Строки** в поле **Номенклатурный номер**</span><span class="sxs-lookup"><span data-stu-id="5d876-145">On the **Lines** FastTab, in the **Item No.**</span></span> <span data-ttu-id="5d876-146">введите номер товара в запасах или услуги.</span><span class="sxs-lookup"><span data-stu-id="5d876-146">field, enter the number of an inventory item or service.</span></span>
11. <span data-ttu-id="5d876-147">В поле **Кол-во** введите количество покупаемых товаров.</span><span class="sxs-lookup"><span data-stu-id="5d876-147">In the **Quantity** field, enter the number of items to be purchased.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="5d876-148">Количество товаров типа **Услуга** измеряется в единицах времени, например часах, как указано в поле **Код единицы измерения** строки.</span><span class="sxs-lookup"><span data-stu-id="5d876-148">For items of type **Service**, the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.</span></span>

    <span data-ttu-id="5d876-149">Поле **Сумма строки** обновляется и отображает значение в поле **Прямая себестоимость единицы**, умноженное на значение в поле **Кол-во**.</span><span class="sxs-lookup"><span data-stu-id="5d876-149">The **Line Amount** field is updated to show the value in the **Direct Unit Cost** field multiplied by the value in the **Quantity** field.</span></span>

    <span data-ttu-id="5d876-150">Значения цены и суммы строки отображаются с налогом или без него в зависимости от выбранного параметра в поле **Цены с учетом налога** на карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="5d876-150">The price and line amount are shown with or without sales tax depending on what you selected in the **Prices Including Tax** field on the vendor card.</span></span>
12. <span data-ttu-id="5d876-151">В поле **Сумма скидки по счету** введите сумму, которую нужно вычесть из значения, отображенного в поле **Всего с учетом налога** в нижней части счета.</span><span class="sxs-lookup"><span data-stu-id="5d876-151">In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. Tax** field at the bottom of the invoice.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="5d876-152">Если установлены скидки по счету для поставщика, то указанное значение процента автоматически вводится в поле **Скидка по счету поставщика, %**, если соблюдены условия, а связанная сумма вводится в поле **Сумма скидки по счету**.</span><span class="sxs-lookup"><span data-stu-id="5d876-152">If you have set up invoice discounts for the vendor, then the specified percentage value is automatically inserted in the **Vendor Invoice Discount %** field if the criteria are met, and the related amount is inserted in the **Invoice Discount Amount** field.</span></span>
13. <span data-ttu-id="5d876-153">При получении приобретенных товаров или услуг выберите **Учесть**.</span><span class="sxs-lookup"><span data-stu-id="5d876-153">When you receive the purchased items or services, choose **Post**.</span></span>

<span data-ttu-id="5d876-154">Покупка теперь отражается в запасах и финансовых записях, а платеж поставщику активирован.</span><span class="sxs-lookup"><span data-stu-id="5d876-154">The purchase is now reflected in inventory and financial records, and the vendor payment is activated.</span></span> <span data-ttu-id="5d876-155">Счет покупки удаляется из списка счетов покупки и заменяется новым документом в списке учтенных счетов покупки.</span><span class="sxs-lookup"><span data-stu-id="5d876-155">The purchase invoice is removed from the list of purchase invoices and replaced with a new document in the list of posted purchase invoices.</span></span>

## <a name="see-also"></a><span data-ttu-id="5d876-156">См. также</span><span class="sxs-lookup"><span data-stu-id="5d876-156">See Also</span></span>
[<span data-ttu-id="5d876-157">Покупки</span><span class="sxs-lookup"><span data-stu-id="5d876-157">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="5d876-158">Настройка покупки</span><span class="sxs-lookup"><span data-stu-id="5d876-158">Setting Up Purchasing</span></span>](purchasing-setup-purchasing.md)  
[<span data-ttu-id="5d876-159">Практическое руководство. Покупка товаров для продажи</span><span class="sxs-lookup"><span data-stu-id="5d876-159">How to: Purchase Items for a Sale</span></span>](purchasing-how-purchase-products-sale.md)  
[<span data-ttu-id="5d876-160">Практическое руководство. Регистрация новых поставщиков</span><span class="sxs-lookup"><span data-stu-id="5d876-160">How to: Register New Vendors</span></span>](purchasing-how-register-new-vendors.md)  
[<span data-ttu-id="5d876-161">Практическое руководство. Подготовка прямых поставок</span><span class="sxs-lookup"><span data-stu-id="5d876-161">How to: Prepare Drop Shipments</span></span>](sales-how-drop-shipment.md)  
<span data-ttu-id="5d876-162">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5d876-162">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
