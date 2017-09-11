---
title: "Обзор задач для управления продажами | Документы Майкрософт"
description: "Описывается порядок управления действиями продажи."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell
ms.date: 06/30/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: ebdcfc8c2be94398c1ebd7d5268a94b568e3b23b
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="sales"></a><span data-ttu-id="2295c-103">Продажи</span><span class="sxs-lookup"><span data-stu-id="2295c-103">Sales</span></span>
<span data-ttu-id="2295c-104">Счет продажи или заказы на продажу создаются для записи соглашения с клиентом о продаже определенных товаров на определенных условиях доставки и оплаты.</span><span class="sxs-lookup"><span data-stu-id="2295c-104">You create a sales invoice or sales order to record your agreement with a customer to sell certain products on certain delivery and payment terms.</span></span>

<span data-ttu-id="2295c-105">Заказы на продажу следует использовать, если процесс продажи требует, чтобы вы могли отгружать части количества в заказе, например потому, что полное количество недоступно в конкретный момент.</span><span class="sxs-lookup"><span data-stu-id="2295c-105">You must use sales orders if your sales process requires that you can ship parts of an order quantity, for example, because the full quantity is not available at once.</span></span> <span data-ttu-id="2295c-106">Если продажа товаров осуществляется путем непосредственной поставки от поставщика клиенту (прямая поставка), то также необходимо использовать заказы на продажу.</span><span class="sxs-lookup"><span data-stu-id="2295c-106">If you sell items by delivering directly from your vendor to your customer, as a drop shipment, then you must also use sales orders.</span></span> <span data-ttu-id="2295c-107">Во всех других аспектах заказы на продажу аналогичны счетам продажи.</span><span class="sxs-lookup"><span data-stu-id="2295c-107">In all other aspects, sales orders work the same way as sales invoices.</span></span>

<span data-ttu-id="2295c-108">Успешные методики продаж и маркетинга помогают принимать правильные решения в нужное время.</span><span class="sxs-lookup"><span data-stu-id="2295c-108">Good sales and marketing practices are all about how to make the best decisions at the right time.</span></span> <span data-ttu-id="2295c-109">Функции маркетинга в [!INCLUDE[d365fin](includes/d365fin_md.md)] предоставляют точный и своевременный обзор контактной информации для более эффективного обслуживания потенциальных клиентов и постоянного повышения качества этого обслуживания.</span><span class="sxs-lookup"><span data-stu-id="2295c-109">Marketing functionality in [!INCLUDE[d365fin](includes/d365fin_md.md)] provides precise and timely overview of your contact information so that you can serve your prospective customers more efficiently and increase customer satisfaction.</span></span> <span data-ttu-id="2295c-110">Дополнительные сведения см. разделе [Управление отношениями](marketing-relationship-management.md).</span><span class="sxs-lookup"><span data-stu-id="2295c-110">For more information, see [Relationship Management](marketing-relationship-management.md).</span></span>

<span data-ttu-id="2295c-111">Можно провести переговоры с клиентом, сначала создав предложение по продаже, которое можно преобразовать в счет продажи, когда вы договоритесь о продаже.</span><span class="sxs-lookup"><span data-stu-id="2295c-111">You can negotiate with the customer by first creating a sales quote, which you can convert to a sales invoice when you agree on the sale.</span></span> <span data-ttu-id="2295c-112">После подтверждения соглашения клиентом, например после процесса предложения, можно отправить подтверждение заказа, чтобы зафиксировать обязательства по доставке продуктов в соответствии с договоренностью.</span><span class="sxs-lookup"><span data-stu-id="2295c-112">After the customer has confirmed the agreement, for example after a quote process, you can send an order confirmation to record your obligation to deliver the products as agreed.</span></span>

<span data-ttu-id="2295c-113">При поставке продуктов, полностью или частично, вы учитываете счета продажи или заказы на продажу как отгруженные или как отгруженные и с выставленными счетами для создания соответствующих операций книг товаров и клиентов в своей системе.</span><span class="sxs-lookup"><span data-stu-id="2295c-113">When you deliver the products, either fully or partially, you post the sales invoice or sales order as shipped or as shipped and invoiced to create the related item and customer ledger entries in your system.</span></span>

<span data-ttu-id="2295c-114">В бизнес-средах, в которых клиент должен осуществить платеж до доставки продуктов, например в розничной торговле, необходимо подождать получения платежа, прежде чем доставлять продукты.</span><span class="sxs-lookup"><span data-stu-id="2295c-114">In business environments where the customer must pay before products are delivered, such as in retail, you must wait for the receipt of payment before you deliver the products.</span></span> <span data-ttu-id="2295c-115">В большинстве случаев вы обрабатываете входящие платежи через несколько недель после отгрузки путем применения платежей к соответствующим учтенным неоплаченным счетам продажи.</span><span class="sxs-lookup"><span data-stu-id="2295c-115">In most cases, you process incoming payments some weeks after delivery by applying the payments to their related posted, unpaid sales invoices.</span></span> <span data-ttu-id="2295c-116">Дополнительные сведения см. в разделе [Практическое руководство. Выверка платежей с использованием автоматического применения](receivables-how-reconcile-payments-auto-application.md).</span><span class="sxs-lookup"><span data-stu-id="2295c-116">For more information, see [How to: Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).</span></span>

<span data-ttu-id="2295c-117">Можно легко скорректировать или отменить учтенный счет продажи до оплаты.</span><span class="sxs-lookup"><span data-stu-id="2295c-117">You can easily correct or cancel a posted sales invoice before it is paid.</span></span> <span data-ttu-id="2295c-118">Это используется, если нужно исправить опечатку или клиент запрашивает изменение на раннем этапе обработки заказа.</span><span class="sxs-lookup"><span data-stu-id="2295c-118">This is useful if you want to correct a typing mistake or if the customer requests a change early in the order process.</span></span> <span data-ttu-id="2295c-119">Если учтенный счет продажи оплачен, необходимо создать кредит-ноту продажи для сторнирования продажи.</span><span class="sxs-lookup"><span data-stu-id="2295c-119">If the posted sales invoice is paid, then you must create a sales credit memo to reverse the sale.</span></span>

<span data-ttu-id="2295c-120">Документы продажи могут быть отправлены в виде файлов PDF, вложенных в сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2295c-120">Sales documents can be sent as PDF files attached to email.</span></span> <span data-ttu-id="2295c-121">Текст сообщения электронной почты будет содержать выдержку из документа продажи, например информацию о продукте, общей сумме и ссылку на сайт PayPal.</span><span class="sxs-lookup"><span data-stu-id="2295c-121">The email body will contain an extract of the sales document, such as products, total amount, and a link to the PayPal site.</span></span> <span data-ttu-id="2295c-122">Дополнительные сведения см. в разделе [Практическое руководство. Отправка документов по электронной почте](ui-how-send-documents-email.md).</span><span class="sxs-lookup"><span data-stu-id="2295c-122">For more information, see [How to: Send Documents by Email](ui-how-send-documents-email.md).</span></span>

<span data-ttu-id="2295c-123">Для всех процессов продажи можно реализовать рабочий процесс утверждения, например, чтобы крупные продажи определенным клиентам утверждались главным бухгалтером.</span><span class="sxs-lookup"><span data-stu-id="2295c-123">For all sales processes, you can incorporate an approval workflow, for example, to require that large sales to certain customers are approved by the accounting manager.</span></span> <span data-ttu-id="2295c-124">Дополнительные сведения см. в разделе [Использование рабочих процессов утверждения](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="2295c-124">For more information, see [Using Approval Workflows](across-how-use-approval-workflows.md).</span></span>

<span data-ttu-id="2295c-125">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="2295c-125">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="2295c-126">Действие</span><span class="sxs-lookup"><span data-stu-id="2295c-126">To</span></span> | <span data-ttu-id="2295c-127">Ссылка</span><span class="sxs-lookup"><span data-stu-id="2295c-127">See</span></span> |
| --- | --- |
| <span data-ttu-id="2295c-128">Создайте предложение по продаже, в котором будут предлагаться продукты на согласуемых условиях, прежде чем преобразовать предложение в счет продажи.</span><span class="sxs-lookup"><span data-stu-id="2295c-128">Create a sales quote where you offer products on negotiable terms before converting the quote to a sales invoice.</span></span> |[<span data-ttu-id="2295c-129">Практическое руководство. Создание предложений</span><span class="sxs-lookup"><span data-stu-id="2295c-129">How to: Make Offers</span></span>](sales-how-make-offers.md) |
| <span data-ttu-id="2295c-130">Создайте счет продажи для записи соглашения с клиентом о продаже продуктов с определенными условиями доставки и оплаты.</span><span class="sxs-lookup"><span data-stu-id="2295c-130">Create a sales invoice to record your agreement with a customer to sell products on certain delivery and payment terms.</span></span> |[<span data-ttu-id="2295c-131">Практическое руководство. Выставление счетов продажи</span><span class="sxs-lookup"><span data-stu-id="2295c-131">How to: Invoice Sales</span></span>](sales-how-invoice-sales.md) |
| <span data-ttu-id="2295c-132">Обработка заказов на продажу, в которых используется частичная отгрузка или прямая поставка.</span><span class="sxs-lookup"><span data-stu-id="2295c-132">Process a sales order that involves partial shipping or drop shipment.</span></span> |[<span data-ttu-id="2295c-133">Практическое руководство. Продажа продукции</span><span class="sxs-lookup"><span data-stu-id="2295c-133">How to: Sell Products</span></span>](sales-how-sell-products.md) |
|<span data-ttu-id="2295c-134">Настройка стандартных строк продажи или покупки. которые можно быстро вставить в документы, например для типовых заказов на пополнение.</span><span class="sxs-lookup"><span data-stu-id="2295c-134">Set up standard sales or purchase lines that you can quickly insert on documents, for example, for recurring replenishment orders.</span></span>|[<span data-ttu-id="2295c-135">Практическое руководство. Создание типовых строк продажи и покупки</span><span class="sxs-lookup"><span data-stu-id="2295c-135">How to: Create Recurring Sales and Purchase Lines</span></span>](sales-how-work-standard-lines.md)|  
| <span data-ttu-id="2295c-136">Связывание заказов на продажу с заказом на покупку для продажи товаров с прямой поставкой, которые будут доставляться непосредственно от поставщика клиенту.</span><span class="sxs-lookup"><span data-stu-id="2295c-136">Link a sales order to a purchase order to sell a drop-shipment item that will be delivered directly from your vendor to your customer.</span></span> |[<span data-ttu-id="2295c-137">Практическое руководство. Выполнение прямых поставок</span><span class="sxs-lookup"><span data-stu-id="2295c-137">How to: Make Drop Shipments</span></span>](sales-how-drop-shipment.md) |
| <span data-ttu-id="2295c-138">Выполните действие в учтенном счете неоплаченной продажи, чтобы автоматически создать кредит-ноту и либо отменить счет продажи, либо воссоздать его для внесения изменений.</span><span class="sxs-lookup"><span data-stu-id="2295c-138">Perform an action on an unpaid posted sales invoice to automatically create a credit memo and either cancel the sales invoice or recreate it so you can make corrections.</span></span> |[<span data-ttu-id="2295c-139">Практическое руководство. Исправление или отмена неоплаченных счетов продажи</span><span class="sxs-lookup"><span data-stu-id="2295c-139">How to: Correct or Cancel Unpaid Sales Invoices</span></span>](sales-how-correct-cancel-sales-invoice.md) |
| <span data-ttu-id="2295c-140">Создайте кредит-ноту продажи, чтобы отменить определенный учтенный счет продажи для отражения продуктов, возвращаемых клиентом, и возмещаемой суммы платежа.</span><span class="sxs-lookup"><span data-stu-id="2295c-140">Create a sales credit memo to revert a specific posted sales invoice to reflect which products the customer returns and which payment amount you will refund.</span></span> |[<span data-ttu-id="2295c-141">Практическое руководство. Обработка возвратов продажи или отмен</span><span class="sxs-lookup"><span data-stu-id="2295c-141">How to: Process Sales Returns or Cancellations</span></span>](sales-how-process-sales-returns-cancellations.md) |
| <span data-ttu-id="2295c-142">Создание карточки клиента для каждого клиента, которому осуществляется продажа.</span><span class="sxs-lookup"><span data-stu-id="2295c-142">Create a customer card for each customer that you sell to.</span></span> |[<span data-ttu-id="2295c-143">Практическое руководство. Регистрация новых клиентов</span><span class="sxs-lookup"><span data-stu-id="2295c-143">How to: Register New Customers</span></span>](sales-how-register-new-customers.md) |

## <a name="see-also"></a><span data-ttu-id="2295c-144">См. также</span><span class="sxs-lookup"><span data-stu-id="2295c-144">See Also</span></span>
[<span data-ttu-id="2295c-145">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="2295c-145">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="2295c-146">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="2295c-146">Managing Receivables</span></span>](receivables-manage-receivables.md)  
[<span data-ttu-id="2295c-147">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="2295c-147">Managing Payables</span></span>](payables-manage-payables.MD)  
<span data-ttu-id="2295c-148">[Управление проектами](projects-manage-projects.md)  </span><span class="sxs-lookup"><span data-stu-id="2295c-148">[Project Management](projects-manage-projects.md)  </span></span>  
<span data-ttu-id="2295c-149">[Цепочка поставок](madeira-supply-chain.md)    </span><span class="sxs-lookup"><span data-stu-id="2295c-149">[Supply Chain](madeira-supply-chain.md)    </span></span>  
<span data-ttu-id="2295c-150">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2295c-150">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="2295c-151">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="2295c-151">General Business Functionality</span></span>](ui-across-business-areas.md)

## [!INCLUDE[d365fin](includes/free_trial_md.md)]
