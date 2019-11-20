---
title: Настройка предоплат клиентов в России
description: Российские улучшения включают предоплату клиентов.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: a6764e37c30d31ef8d98cf9e915f045cf1c65a69
ms.sourcegitcommit: 319023e53627dbe8e68643908aacc6fd594a4957
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/04/2019
ms.locfileid: "2554499"
---
# <a name="set-up-customer-prepayments"></a><span data-ttu-id="14542-103">Настройка предоплат клиентов</span><span class="sxs-lookup"><span data-stu-id="14542-103">Set Up Customer Prepayments</span></span>

<span data-ttu-id="14542-104">Предоплаты — это авансовые платежи по заказам на продажу, которые получены, для которых создан счет и которые учтены, но до окончательного выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="14542-104">Prepayments are advance payments on sales orders that are received, invoiced, and posted before the final invoice is issued.</span></span> <span data-ttu-id="14542-105">Например, вам может потребоваться задаток, чтобы произвести товар и отгрузить его клиенту.</span><span class="sxs-lookup"><span data-stu-id="14542-105">For example, you may require a deposit before you manufacture and ship an item to a customer.</span></span> <span data-ttu-id="14542-106">Предоплаты позволяют создавать счета и собирать авансовые платежи от клиентов и учитывать платежи для правильных счетов.</span><span class="sxs-lookup"><span data-stu-id="14542-106">Prepayments let you invoice and collect advance payments from customers and post the payments against the correct invoices and accounts.</span></span>

## <a name="to-set-up-customer-prepayments"></a><span data-ttu-id="14542-107">Настройка предоплат клиентов</span><span class="sxs-lookup"><span data-stu-id="14542-107">To set up customer prepayments</span></span>

1. <span data-ttu-id="14542-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Продажи"**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="14542-108">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>

2. <span data-ttu-id="14542-109">На экспресс-вкладке **Нумерация** убедитесь, что серия номеров **Серия номеров учт. счетов предопл.** совпадает с **Серия номеров учт. счетов**.</span><span class="sxs-lookup"><span data-stu-id="14542-109">On the **Numbering** FastTab, verify that the number series for the **Posted Prepmt. Inv. Nos.** is the same as the **Posted Invoice Nos.**.</span></span> <span data-ttu-id="14542-110">Убедитесь также, что серия номеров для **Серия номеров учт. кр.-нот предопл.** совпадает с серией для **Серия номеров учт. кредит-нот**.</span><span class="sxs-lookup"><span data-stu-id="14542-110">Also verify that the number series for the **Posted Prepmt. Cr. Memo Nos.** is the same as the **Posted Credit Memo Nos.**.</span></span>

3. <span data-ttu-id="14542-111">На экспресс-вкладке **Предоплата** введите следующие сведения.</span><span class="sxs-lookup"><span data-stu-id="14542-111">On the **Prepayment** FastTab, enter the following information.</span></span>

   | <span data-ttu-id="14542-112">Поле</span><span class="sxs-lookup"><span data-stu-id="14542-112">Field</span></span>                             | <span data-ttu-id="14542-113">Описание</span><span class="sxs-lookup"><span data-stu-id="14542-113">Description</span></span>                                                  |
   | :-------------------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="14542-114">**Использовать счет ГК предоплаты**</span><span class="sxs-lookup"><span data-stu-id="14542-114">**Use Prepayment Account**</span></span>        | <span data-ttu-id="14542-115">Выберите это поле, чтобы учесть предоплаты поставщикам, используя субсчет, указанный в поле **Счет предоплаты** в окне **Учетные группы клиента**.</span><span class="sxs-lookup"><span data-stu-id="14542-115">Select to post prepayments using the subaccount specified in the **Prepayment Account** field in the **Customer Posting Groups** window.</span></span> |
   | <span data-ttu-id="14542-116">**Создание счета на предоплату**</span><span class="sxs-lookup"><span data-stu-id="14542-116">**Create Prepayment Invoice**</span></span>     | <span data-ttu-id="14542-117">Выберите, чтобы создать счет на предоплату.</span><span class="sxs-lookup"><span data-stu-id="14542-117">Select to create an invoice for the prepayment.</span></span> <span data-ttu-id="14542-118">Если это поле не выбрано, счет на предоплату создан не будет.</span><span class="sxs-lookup"><span data-stu-id="14542-118">If this field is not selected, an invoice for the prepayment will not be created.</span></span> |
   | <span data-ttu-id="14542-119">**Серия номеров учт. предоплат**</span><span class="sxs-lookup"><span data-stu-id="14542-119">**Posted Prepayment Nos.**</span></span>        | <span data-ttu-id="14542-120">Введите код серии номеров, который требуется использовать для счетов на предоплату.</span><span class="sxs-lookup"><span data-stu-id="14542-120">Enter the code of the number series that you want to use for prepayment invoices.</span></span> |
   | <span data-ttu-id="14542-121">**Учт. разн. по предопл. - серия ном. док.**</span><span class="sxs-lookup"><span data-stu-id="14542-121">**Posted PD Doc. Nos.**</span></span>           | <span data-ttu-id="14542-122">Введите код серии номеров, который требуется использовать для документов предоплаты.</span><span class="sxs-lookup"><span data-stu-id="14542-122">Enter the code of the number series that you want to use for prepayment documents.</span></span> |
   | <span data-ttu-id="14542-123">**Разн. по предопл. - тип серии номеров док.**</span><span class="sxs-lookup"><span data-stu-id="14542-123">**PD Doc. Nos. Type**</span></span>             | <span data-ttu-id="14542-124">Укажите, требуется ли использовать серию номеров или символ для идентификации документов предоплаты.</span><span class="sxs-lookup"><span data-stu-id="14542-124">Select if you want to use a number series or symbol to identify prepayment documents.</span></span> |
   | <span data-ttu-id="14542-125">**Символ для док. разн. по предопл.**</span><span class="sxs-lookup"><span data-stu-id="14542-125">**Symbol for PD Doc.**</span></span>            | <span data-ttu-id="14542-126">Введите символ, который будет печататься на документах предоплаты.</span><span class="sxs-lookup"><span data-stu-id="14542-126">Enter a symbol to be printed on prepayment documents.</span></span>        |
   | <span data-ttu-id="14542-127">**Разн. по предопл.: прибыль - знач. изм. условия**</span><span class="sxs-lookup"><span data-stu-id="14542-127">**PD Gains Condition Dim Value**</span></span>  | <span data-ttu-id="14542-128">Введите код для измерения, которое используется для создания условной прибыли от предоплаты.</span><span class="sxs-lookup"><span data-stu-id="14542-128">Enter the code for the dimension that is used to generate conditional prepayment gains.</span></span> |
   | <span data-ttu-id="14542-129">**Разн. по предопл.: убытки - знач. изм. условия**</span><span class="sxs-lookup"><span data-stu-id="14542-129">**PD Losses Condition Dim Value**</span></span> | <span data-ttu-id="14542-130">Введите код для измерения, которое используется для создания условного убытка от предоплаты.</span><span class="sxs-lookup"><span data-stu-id="14542-130">Enter the code for the dimension that is used to generate conditional prepayment losses.</span></span> |
   | <span data-ttu-id="14542-131">**Разн. по предопл.: прибыль - знач. изм. вида**</span><span class="sxs-lookup"><span data-stu-id="14542-131">**PD Gains Kind Dim Value**</span></span>       | <span data-ttu-id="14542-132">Введите код для измерения, которое используется для создания платежа с точки зрения прибыли от предоплаты.</span><span class="sxs-lookup"><span data-stu-id="14542-132">Enter the code for the dimension that is used to generate payment in kind prepayment gains.</span></span> |
   | <span data-ttu-id="14542-133">**Разн. по предопл.: убытки - знач. изм. вида**</span><span class="sxs-lookup"><span data-stu-id="14542-133">**PD Losses Kind Dim Value**</span></span>      | <span data-ttu-id="14542-134">Введите код для измерения, которое используется для создания платежа с точки зрения прибыли от предоплаты.</span><span class="sxs-lookup"><span data-stu-id="14542-134">Enter the code for the dimension that is used to generate payment in kind prepayment gains.</span></span> |

4. <span data-ttu-id="14542-135">Откройте окно **Учетные группы клиента**.</span><span class="sxs-lookup"><span data-stu-id="14542-135">Open the **Customer Posting Groups** window.</span></span>

5. <span data-ttu-id="14542-136">В поле **Счет предоплаты** укажите счет главной книги, который должен использоваться для учета предоплаты клиентов.</span><span class="sxs-lookup"><span data-stu-id="14542-136">In the **Prepayment Account** field, specify the general ledger accounts that you want to use for posting customer prepayments.</span></span>

6. <span data-ttu-id="14542-137">Нажмите кнопку **Закрыть**, чтобы закрыть окно и сохранить введенные данные.</span><span class="sxs-lookup"><span data-stu-id="14542-137">Choose the **Close** button to close the window and save your entries.</span></span>

<span data-ttu-id="14542-138">Теперь вы можете создавать счета и собирать авансовые платежи от клиентов и учитывать платежи для правильных счетов.</span><span class="sxs-lookup"><span data-stu-id="14542-138">You can now invoice and collect advance payments from customers and post the payments to the correct invoices and accounts.</span></span>

## <a name="see-also"></a><span data-ttu-id="14542-139">См. также</span><span class="sxs-lookup"><span data-stu-id="14542-139">See Also</span></span>

[<span data-ttu-id="14542-140">Выставление счетов на предоплату</span><span class="sxs-lookup"><span data-stu-id="14542-140">Invoicing Prepayments</span></span>](../../finance-invoice-prepayments.md)  
[<span data-ttu-id="14542-141">Пошаговое руководство. Настройка и выставление счетов на продажу</span><span class="sxs-lookup"><span data-stu-id="14542-141">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](../../walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
