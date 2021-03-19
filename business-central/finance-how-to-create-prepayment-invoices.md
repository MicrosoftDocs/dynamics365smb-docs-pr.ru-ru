---
title: Практическое руководство. Создание счетов на предоплату | Документация Майкрософт
description: Узнайте, как обрабатывать ситуации, в которых вы или ваш поставщик требует предоплату.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 3a1f79f089ef8633ca51be35930c5de5c2401b29
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5387403"
---
# <a name="create-prepayment-invoices"></a><span data-ttu-id="f6c0e-103">Создание счетов на предоплату</span><span class="sxs-lookup"><span data-stu-id="f6c0e-103">Create Prepayment Invoices</span></span>

<span data-ttu-id="f6c0e-104">Если вы требуете, чтобы ваши клиенты отправили платеж до того, как вы отправите им заказ, вы можете использовать функцию предоплаты.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-104">If you require your customers to submit payment before you ship an order to them, you can use the prepayment functionality.</span></span> <span data-ttu-id="f6c0e-105">То же самое применимо, если ваш поставщик требует, чтобы вы отправили платеж до того, как он отправит вам заказ.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-105">The same applies if your vendor requires you to submit payment before they ship an order to you.</span></span>  

<span data-ttu-id="f6c0e-106">При создании заказа продажи или покупки можно начать процесс предоплаты.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-106">You can start the prepayment process when you create a sales or purchase order.</span></span> <span data-ttu-id="f6c0e-107">Если у вас есть процент предоплаты по умолчанию для этого клиента или поставщика, он будет автоматически включен в итоговый счет предоплаты.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-107">If you have a default prepayment percentage for this customer or vendor, that will be included automatically in the resulting prepayment invoice.</span></span> <span data-ttu-id="f6c0e-108">Вы также можете указать процент предоплаты для всего документа.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-108">You can also specify a prepayment percentage to the entire document.</span></span>

<span data-ttu-id="f6c0e-109">После создания заказов продажи или покупки можно создать счет на предоплату.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-109">After you create a sales or purchase order, you can create a prepayment invoice.</span></span> <span data-ttu-id="f6c0e-110">Можно использовать процентные значения по умолчанию для каждой строки продажи или покупки, а также можно корректировать сумму по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-110">You can use the default percentages for each sales or purchase line, or you can adjust the amount as necessary.</span></span> <span data-ttu-id="f6c0e-111">Например, можно указать общую сумму для всего заказа.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-111">For example, you can specify a total amount for the entire order.</span></span>  

<span data-ttu-id="f6c0e-112">В следующей процедуре описывается, как выставлять счета на предоплату для заказов на продажу.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-112">The following procedure describes how to invoice a prepayment for a sales order.</span></span> <span data-ttu-id="f6c0e-113">Действия для заказов на покупку аналогичны.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-113">The steps are similar for purchase orders.</span></span>  

## <a name="to-create-a-prepayment-invoice"></a><span data-ttu-id="f6c0e-114">Процедура создания счета на предоплату</span><span class="sxs-lookup"><span data-stu-id="f6c0e-114">To create a prepayment invoice</span></span>

1. <span data-ttu-id="f6c0e-115">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f6c0e-116">Создать новый заказ на продажу для соответствующего клиента.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-116">Create a new sales order for the relevant customer.</span></span> <span data-ttu-id="f6c0e-117">Дополнительные сведения см. в разделе [Продажа продукции](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="f6c0e-117">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>  

    <span data-ttu-id="f6c0e-118">На Экспресс-вкладка **Предоплата**, в поле **Предоплата (%)** указывается процент, используемый для расчета суммы предоплаты.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-118">On the **Prepayment** FastTab, the **Prepayment %** field specifies the percentage to use to calculate the prepayment amount.</span></span> <span data-ttu-id="f6c0e-119">Поле заполняется автоматически, если в карточке клиента указан процент предоплаты по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-119">If there is a default prepayment percentage on the customer card, the field is filled in automatically.</span></span> <span data-ttu-id="f6c0e-120">Процент может быть изменено.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-120">You can change the percentage.</span></span> <!--This percentage is applied to lines where the item on that line does not already specify a prepayment percentage. The prepayment percentage is only copied from the header to lines that do not copy the default prepayment percentage from the item.-->  

    <span data-ttu-id="f6c0e-121">Выбрать поле **Сжать предоплату**, если вы хотите создать в счете на предоплату строки, объединяющие строки из заказа на продажу, если:</span><span class="sxs-lookup"><span data-stu-id="f6c0e-121">Choose the **Compress Prepayment** field if you want to create lines on the prepayment invoice that combine lines from the sales order if:</span></span>  

    - <span data-ttu-id="f6c0e-122">Они имеют один и тот же счет главной книги для учета предоплаты, что определяется общей настройкой учета.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-122">They have the same general ledger account for prepayments as determined by the general posting setup.</span></span>  
    - <span data-ttu-id="f6c0e-123">Они имеют одинаковые измерения.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-123">They have the same dimensions.</span></span>  

    <span data-ttu-id="f6c0e-124">Не выбирайте поле **Сжать предоплату**, если требуется определить счет на предоплату с отдельным строками для каждой строки заказа продажи, которая имеет процент предоплаты.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-124">If you want to specify a prepayment invoice with one line for each sales order line that has a prepayment percentage, then do not choose the **Compress Prepayment** field.</span></span>  

    <span data-ttu-id="f6c0e-125">Срок оплаты предоплаты рассчитывается автоматически на основе значения **Код условий предоплаты**.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-125">The due date for the prepayment is calculated automatically based on the value of the **Prepmt. Payment Terms Code**.</span></span>

3. <span data-ttu-id="f6c0e-126">Заполните строки продажи.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-126">Fill in the sales lines.</span></span>  

    <span data-ttu-id="f6c0e-127">Если вы указали процент предоплаты по умолчанию для клиента или на экспресс-вкладке **Предоплата** для этого документа, это значение копируется в каждую строку.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-127">If you have specified a default prepayment percentage either for the customer or on the **Prepayment** FastTab on this document, this value is copied to each line.</span></span> <span data-ttu-id="f6c0e-128">Можно изменить содержимое поля **Предоплата (%)** в строке.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-128">You can change the contents of the **Prepayment %** field on the line.</span></span>  

4. <span data-ttu-id="f6c0e-129">Для просмотра общей суммы предоплаты выберите действие **Статистика**.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-129">To view the total prepayment amount, choose the **Statistics** action.</span></span>

    <span data-ttu-id="f6c0e-130">Если необходимо скорректировать сумму предоплаты для данного заказа, можно изменить содержимое поля **Сумма предоплаты** на странице **Статистика заказов на продажу**.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-130">If you want to adjust the total prepayment amount for the order, you can change the contents of the **Prepayment Amount** field on the **Sales Order Statistics** page.</span></span>  

    <span data-ttu-id="f6c0e-131">Если выбрано поле **Цены с учетом НДС**, а поле **Сумма предоплаты включая НДС** доступно для редактирования.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-131">If the **Prices Including VAT** field is selected, the **Prepayment Amount Incl. VAT** field is editable.</span></span>  

    <span data-ttu-id="f6c0e-132">При изменении значения поля **Сумма предоплаты** данная сумма будет пропорционально распределяться между всеми строками, за исключением тех строк, у которых значение поля **Предоплата (%)** равно **0**.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-132">If you change the contents of the **Prepayment Amount** field, the amount will be distributed proportionately between all lines, except those that have **0** in the **Prepayment %** field.</span></span>  

5. <span data-ttu-id="f6c0e-133">Чтобы напечатать тестовый отчет перед учетом счета на предоплату, выберите действие **Предоплата**, затем выберите действие **Тестовый отчет о предоплате**.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-133">To print a test report before posting the prepayment invoice, choose the **Prepayment** action, and then choose the **Prepayment Test Report** action.</span></span>  
6. <span data-ttu-id="f6c0e-134">Чтобы учесть счет на предоплату, выберите действие **Предоплата**, затем выберите действие **Учет счета на предоплату**.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-134">To post the prepayment invoice, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action.</span></span>  

    <span data-ttu-id="f6c0e-135">Чтобы учесть и распечатать счет на предоплату, выберите действие **Учет и печать счета на предоплату**.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-135">To post and print the prepayment invoice, choose the **Post and Print Prepmt. Invoice** action.</span></span>  

<span data-ttu-id="f6c0e-136">Для данного заказа можно создать дополнительные счета на предоплату.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-136">You can issue additional prepayment invoices for the order.</span></span> <span data-ttu-id="f6c0e-137">Для этого необходимо увеличить сумму предоплаты в одной или нескольких строках, скорректировать дату в случае необходимости и учесть счет на предоплату.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-137">To do this, increase the prepayment amount on one or more lines, adjust the document date if necessary, and post the prepayment invoice.</span></span> <span data-ttu-id="f6c0e-138">Новый счет будет создан на сумму разницы между суммами предоплаты, уже включенными в счет, и новой суммой предоплаты.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-138">A new invoice will be created for the difference between the prepayment amounts invoiced so far and the new prepayment amount.</span></span>  

> [!NOTE]  
> <span data-ttu-id="f6c0e-139">Если вы расположены в Северной Америке, вы не можете изменить процент предоплаты после учета счета на предоплату.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-139">If you are located in North America, you cannot change the prepayment percentage after the prepayment invoice has been posted.</span></span> <span data-ttu-id="f6c0e-140">Это запрещено в североамериканской версии [!INCLUDE[prod_short](includes/prod_short.md)], поскольку в противном случае расчет налога будет неверным.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-140">This is prevented in the North American version of [!INCLUDE[prod_short](includes/prod_short.md)] because the calculation of sales tax will otherwise be incorrect.</span></span>  

 <span data-ttu-id="f6c0e-141">Когда все готово для учета остатка по счету, его учет выполняется так же, как и учет любого счета, а сумма предоплаты автоматически вычитается из причитающейся суммы.</span><span class="sxs-lookup"><span data-stu-id="f6c0e-141">When you are ready to post the rest of the invoice, post it as you would post any invoice, and the prepayment amount will automatically be deducted from the amount due.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f6c0e-142">См. также</span><span class="sxs-lookup"><span data-stu-id="f6c0e-142">See Also</span></span>

[<span data-ttu-id="f6c0e-143">Выставление счетов на предоплату</span><span class="sxs-lookup"><span data-stu-id="f6c0e-143">Invoicing Prepayments</span></span>](finance-invoice-prepayments.md)  
[<span data-ttu-id="f6c0e-144">Пошаговое руководство. Настройка и выставление счетов на продажу</span><span class="sxs-lookup"><span data-stu-id="f6c0e-144">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[<span data-ttu-id="f6c0e-145">Финансы</span><span class="sxs-lookup"><span data-stu-id="f6c0e-145">Finance</span></span>](finance.md)  
<span data-ttu-id="f6c0e-146">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f6c0e-146">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]