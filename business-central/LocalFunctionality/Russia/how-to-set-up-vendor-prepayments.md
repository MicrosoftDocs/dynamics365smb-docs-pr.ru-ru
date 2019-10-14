---
title: Настройка предоплат поставщиков в России
description: Российские улучшения включают предоплату поставщикам.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 1c4bf3306d9b2e9701327539a28992890c25b817
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301140"
---
# <a name="how-to-set-up-vendor-prepayments"></a><span data-ttu-id="feda2-103">Практическое руководство. Настройка предоплат поставщикам</span><span class="sxs-lookup"><span data-stu-id="feda2-103">How to: Set Up Vendor Prepayments</span></span>

<span data-ttu-id="feda2-104">Предоплаты — это авансовые платежи для заказов на покупку, которые оплачиваются до формирования окончательного счета.</span><span class="sxs-lookup"><span data-stu-id="feda2-104">Prepayments are advance payments on purchase orders that are paid before the final invoice is issued.</span></span> <span data-ttu-id="feda2-105">Например, может потребоваться оплатить поставщику 20 процентов суммы счета за производимый товар.</span><span class="sxs-lookup"><span data-stu-id="feda2-105">For example, you may be required by a vendor to prepay 20 percent of the invoice amount on a manufactured item.</span></span> <span data-ttu-id="feda2-106">Предоплаты позволяют отслеживать и регистрировать авансовые платежи по счетам покупки.</span><span class="sxs-lookup"><span data-stu-id="feda2-106">Prepayments allow you track and record advance payments on purchase invoices.</span></span>

## <a name="to-set-up-vendor-prepayments"></a><span data-ttu-id="feda2-107">Настройка предоплат поставщикам</span><span class="sxs-lookup"><span data-stu-id="feda2-107">To set up vendor prepayments</span></span>

1. <span data-ttu-id="feda2-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Покупки"**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="feda2-108">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>

2. <span data-ttu-id="feda2-109">На экспресс-вкладке **Нумерация** убедитесь, что серия номеров **Серия номеров учт. счетов предопл.** совпадает с **Серия номеров учт. счетов**.</span><span class="sxs-lookup"><span data-stu-id="feda2-109">On the **Numbering** FastTab, verify that the number series for the **Posted Prepmt. Inv. Nos.** is the same as the **Posted Invoice Nos.**.</span></span> <span data-ttu-id="feda2-110">Убедитесь также, что серия номеров для **Серия номеров учт. кр.-нот предопл.** совпадает с серией для **Серия номеров учт. кредит-нот**.</span><span class="sxs-lookup"><span data-stu-id="feda2-110">Also verify that the number series for **Posted Prepmt. Cr. Memo Nos.** is the same as the **Posted Credit Memo Nos.**.</span></span>

3. <span data-ttu-id="feda2-111">На экспресс-вкладке **Предоплата** введите следующие сведения.</span><span class="sxs-lookup"><span data-stu-id="feda2-111">On the **Prepayment** FastTab, enter the following information.</span></span>

   | <span data-ttu-id="feda2-112">Поле</span><span class="sxs-lookup"><span data-stu-id="feda2-112">Field</span></span>                             | <span data-ttu-id="feda2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="feda2-113">Description</span></span>                                                  |
   | :-------------------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="feda2-114">**Использовать счет ГК предоплаты**</span><span class="sxs-lookup"><span data-stu-id="feda2-114">**Use Prepayment Account**</span></span>        | <span data-ttu-id="feda2-115">Выберите это поле, чтобы учесть предоплаты поставщикам, используя специальный субсчет, указанный в поле **Счет ГК предоплаты** в окне **Учетные группы поставщика**.</span><span class="sxs-lookup"><span data-stu-id="feda2-115">Select to post prepayments using the special subaccount specified in the **Prepayment Account** field in the **Vendor Posting Groups** window.</span></span> |
   | <span data-ttu-id="feda2-116">**Учт. разн. по предопл. - серия ном. док.**</span><span class="sxs-lookup"><span data-stu-id="feda2-116">**Posted PD Doc. Nos.**</span></span>           | <span data-ttu-id="feda2-117">Введите код серии номеров, который требуется использовать для документов предоплаты.</span><span class="sxs-lookup"><span data-stu-id="feda2-117">Enter the code of the number series that you want to use for prepayment documents.</span></span> |
   | <span data-ttu-id="feda2-118">**Разн. по предопл. - тип серии номеров док.**</span><span class="sxs-lookup"><span data-stu-id="feda2-118">**PD Doc. Nos. Type**</span></span>             | <span data-ttu-id="feda2-119">Укажите, требуется ли использовать серию номеров или символ для идентификации документов предоплаты.</span><span class="sxs-lookup"><span data-stu-id="feda2-119">Select if you want to use a number series or symbol to identify prepayment documents.</span></span> |
   | <span data-ttu-id="feda2-120">**Символ для док. разн. по предопл.**</span><span class="sxs-lookup"><span data-stu-id="feda2-120">**Symbol for PD Doc.**</span></span>            | <span data-ttu-id="feda2-121">Введите символ, который будет печататься на документах предоплаты.</span><span class="sxs-lookup"><span data-stu-id="feda2-121">Enter a symbol to be printed on prepayment documents.</span></span>        |
   | <span data-ttu-id="feda2-122">**Разн. по предопл.: прибыль - знач. изм. условия**</span><span class="sxs-lookup"><span data-stu-id="feda2-122">**PD Gains Condition Dim Value**</span></span>  | <span data-ttu-id="feda2-123">Введите код для измерения, которое используется для создания условной прибыли от предоплаты.</span><span class="sxs-lookup"><span data-stu-id="feda2-123">Enter the code for the dimension that is used to generate conditional prepayment gains.</span></span> |
   | <span data-ttu-id="feda2-124">**Разн. по предопл.: убытки - знач. изм. условия**</span><span class="sxs-lookup"><span data-stu-id="feda2-124">**PD Losses Condition Dim Value**</span></span> | <span data-ttu-id="feda2-125">Введите код для измерения, которое используется для создания условного убытка от предоплаты.</span><span class="sxs-lookup"><span data-stu-id="feda2-125">Enter the code for the dimension that is used to generate conditional prepayment losses.</span></span> |
   | <span data-ttu-id="feda2-126">**Разн. по предопл.: прибыль - знач. изм. вида**</span><span class="sxs-lookup"><span data-stu-id="feda2-126">**PD Gains Kind Dim Value**</span></span>       | <span data-ttu-id="feda2-127">Введите код для измерения, которое используется для создания платежа с точки зрения прибыли от предоплаты.</span><span class="sxs-lookup"><span data-stu-id="feda2-127">Enter the code for the dimension that is used to generate payment in kind prepayment gains.</span></span> |
   | <span data-ttu-id="feda2-128">**Разн. по предопл.: убытки - знач. изм. вида**</span><span class="sxs-lookup"><span data-stu-id="feda2-128">**PD Losses Kind Dim Value**</span></span>      | <span data-ttu-id="feda2-129">Введите код для измерения, которое используется для создания платежа с точки зрения убытка от предоплаты.</span><span class="sxs-lookup"><span data-stu-id="feda2-129">Enter the code for the dimension that is used to generate payment in kind prepayment losses.</span></span> |

4. <span data-ttu-id="feda2-130">Откройте окно **Учетные группы поставщика**.</span><span class="sxs-lookup"><span data-stu-id="feda2-130">Open the **Vendor Posting Groups** window.</span></span>

5. <span data-ttu-id="feda2-131">В поле **Счет предоплаты** укажите счет главной книги, который должен использоваться для учета предоплаты поставщикам.</span><span class="sxs-lookup"><span data-stu-id="feda2-131">In the **Prepayment Account** field, specify the general ledger accounts that you want to use for posting vendor prepayments.</span></span>

6. <span data-ttu-id="feda2-132">Нажмите **Закрыть**, чтобы закрыть окно и сохранить введенные данные.</span><span class="sxs-lookup"><span data-stu-id="feda2-132">Choose **Close** to close the window and save your entries.</span></span>

<span data-ttu-id="feda2-133">Теперь вы можете отслеживать и регистрировать предоплаты по счетам покупки.</span><span class="sxs-lookup"><span data-stu-id="feda2-133">You can now track and record advance payments on purchase invoices.</span></span>

## <a name="see-also"></a><span data-ttu-id="feda2-134">См. также</span><span class="sxs-lookup"><span data-stu-id="feda2-134">See Also</span></span>

[<span data-ttu-id="feda2-135">Выставление счетов на предоплату</span><span class="sxs-lookup"><span data-stu-id="feda2-135">Invoicing Prepayments</span></span>](../../finance-invoice-prepayments.md)  
[<span data-ttu-id="feda2-136">Пошаговое руководство. Настройка и выставление счетов на продажу</span><span class="sxs-lookup"><span data-stu-id="feda2-136">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](../../walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
