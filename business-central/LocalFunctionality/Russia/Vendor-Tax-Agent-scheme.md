---
title: Схема налогового агента поставщика в России
description: Российские усовершенствования включают схемы налоговых агентов поставщиков.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: f92e284150926fcd24530777c13722e7a72228aa
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5773458"
---
# <a name="vendor-tax-agent-scheme"></a><span data-ttu-id="959fc-103">Схема налогового агента поставщика</span><span class="sxs-lookup"><span data-stu-id="959fc-103">Vendor Tax Agent Scheme</span></span>

## <a name="vat-from-internal-funds"></a><span data-ttu-id="959fc-104">НДС из внутренних фондов</span><span class="sxs-lookup"><span data-stu-id="959fc-104">VAT from Internal Funds</span></span>

<span data-ttu-id="959fc-105">Заполните поля в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="959fc-105">Fill in the fields on the vendor card.</span></span>

1. <span data-ttu-id="959fc-106">Экспресс-вкладка **Договор**:</span><span class="sxs-lookup"><span data-stu-id="959fc-106">**Agreement** FastTab:</span></span>

    - <span data-ttu-id="959fc-107">Учет договоров - обязательно.</span><span class="sxs-lookup"><span data-stu-id="959fc-107">Agreement posting - mandatory.</span></span>

    - <span data-ttu-id="959fc-108">Номера договоров обязательны.</span><span class="sxs-lookup"><span data-stu-id="959fc-108">Agreement numbers required.</span></span>

2. <span data-ttu-id="959fc-109">На карточке договора:</span><span class="sxs-lookup"><span data-stu-id="959fc-109">On the agreement card:</span></span>

    - <span data-ttu-id="959fc-110">НДС бизнес-группа</span><span class="sxs-lookup"><span data-stu-id="959fc-110">VAT Bus. Posting Group</span></span>
    - <span data-ttu-id="959fc-111">НДС товарная группа налогового агента</span><span class="sxs-lookup"><span data-stu-id="959fc-111">VAT Agent Prod. Posting Group</span></span>
    - <span data-ttu-id="959fc-112">Тип источника оплаты НДС - Внутренние фонды</span><span class="sxs-lookup"><span data-stu-id="959fc-112">VAT Payment Source Type - Internal Funds</span></span>

## <a name="prepayment-and-payment-vat"></a><span data-ttu-id="959fc-113">Предоплата и оплата НДС</span><span class="sxs-lookup"><span data-stu-id="959fc-113">Prepayment and Payment VAT</span></span>

1. <span data-ttu-id="959fc-114">Создание и выпуск счета</span><span class="sxs-lookup"><span data-stu-id="959fc-114">Create and release an invoice</span></span>

    <span data-ttu-id="959fc-115">Номер договора</span><span class="sxs-lookup"><span data-stu-id="959fc-115">Agreement No.</span></span> <span data-ttu-id="959fc-116">(с настройками для продавца с уплатой НДС из внутренних фондов) должен быть указан.</span><span class="sxs-lookup"><span data-stu-id="959fc-116">(with settings for Vendor with VAT Payment from internal funds) should be specified.</span></span>

2. <span data-ttu-id="959fc-117">Создание строки в журнале платежей:</span><span class="sxs-lookup"><span data-stu-id="959fc-117">Create a line in Payment Journal:</span></span>

    - <span data-ttu-id="959fc-118">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="959fc-118">Document Type - Payment</span></span>
    - <span data-ttu-id="959fc-119">Предоплата - да</span><span class="sxs-lookup"><span data-stu-id="959fc-119">Prepayment - yes</span></span>
    - <span data-ttu-id="959fc-120">Номер документа предоплаты не требуется.</span><span class="sxs-lookup"><span data-stu-id="959fc-120">Prepayment Document No is required.</span></span>

3. <span data-ttu-id="959fc-121">Выполните учет строк журнала.</span><span class="sxs-lookup"><span data-stu-id="959fc-121">Post lines of Journal</span></span>

    <span data-ttu-id="959fc-122">Операции с НДС генерируются автоматически в рублях.</span><span class="sxs-lookup"><span data-stu-id="959fc-122">Operations with VAT are automatically generated in rubles.</span></span>

4. <span data-ttu-id="959fc-123">Создайте и учтите в журнале платежей для налогового органа строку с суммой НДС для предоплаты.</span><span class="sxs-lookup"><span data-stu-id="959fc-123">Create and post line in Payment Journal for Tax Authority with VAT Amount of prepayment.</span></span>

5. <span data-ttu-id="959fc-124">Выполните отгрузку и учет счета.</span><span class="sxs-lookup"><span data-stu-id="959fc-124">Ship and post invoice.</span></span>

6. <span data-ttu-id="959fc-125">Создайте строку в журнале платежей</span><span class="sxs-lookup"><span data-stu-id="959fc-125">Create a line in Payment Journal</span></span>

    - <span data-ttu-id="959fc-126">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="959fc-126">Document Type - Payment</span></span>
    - <span data-ttu-id="959fc-127">Номер начального документа - Номер</span><span class="sxs-lookup"><span data-stu-id="959fc-127">Initial Document No. - No.</span></span> <span data-ttu-id="959fc-128">учтенного счета</span><span class="sxs-lookup"><span data-stu-id="959fc-128">of posted invoice</span></span>
    - <span data-ttu-id="959fc-129">Примен. к док. - номер - Номер</span><span class="sxs-lookup"><span data-stu-id="959fc-129">Applies-to Doc. No. - No.</span></span> <span data-ttu-id="959fc-130">учтенного счета</span><span class="sxs-lookup"><span data-stu-id="959fc-130">of posted invoice</span></span>

7. <span data-ttu-id="959fc-131">Создайте и выполните учет платежа в налоговый орган.</span><span class="sxs-lookup"><span data-stu-id="959fc-131">Create and post payment to the Tax Authority.</span></span>
8. <span data-ttu-id="959fc-132">Откройте журнал НДС.</span><span class="sxs-lookup"><span data-stu-id="959fc-132">Go to VAT Settlement Worksheet.</span></span> <span data-ttu-id="959fc-133">Выполните учет НДС (см. [Зачет НДС](Settlement-VAT.md)).</span><span class="sxs-lookup"><span data-stu-id="959fc-133">Post VAT (see [Settlement VAT](Settlement-VAT.md)).</span></span>

## <a name="vat-from-vendor-funds"></a><span data-ttu-id="959fc-134">НДС из фондов поставщика</span><span class="sxs-lookup"><span data-stu-id="959fc-134">VAT from Vendor Funds</span></span>

<span data-ttu-id="959fc-135">Заполните поля в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="959fc-135">Fill the fields in Vendor Card.</span></span>

1. <span data-ttu-id="959fc-136">На вкладке "Договор":</span><span class="sxs-lookup"><span data-stu-id="959fc-136">On Agreement tab:</span></span>

    - <span data-ttu-id="959fc-137">Учет договоров - обязательно.</span><span class="sxs-lookup"><span data-stu-id="959fc-137">Agreement posting - mandatory.</span></span>
    - <span data-ttu-id="959fc-138">Номера договоров обязательны.</span><span class="sxs-lookup"><span data-stu-id="959fc-138">Agreement Nos is required.</span></span>

2. <span data-ttu-id="959fc-139">В карточке договора:</span><span class="sxs-lookup"><span data-stu-id="959fc-139">In Agreement card:</span></span>

    - <span data-ttu-id="959fc-140">НДС бизнес-группа</span><span class="sxs-lookup"><span data-stu-id="959fc-140">VAT Bus. Posting Group</span></span>
    - <span data-ttu-id="959fc-141">НДС товарная группа налогового агента</span><span class="sxs-lookup"><span data-stu-id="959fc-141">VAT Agent Prod. Posting Group</span></span>
    - <span data-ttu-id="959fc-142">Тип источника оплаты НДС - Фонды поставщика</span><span class="sxs-lookup"><span data-stu-id="959fc-142">VAT Payment Source Type - Vendor Funds</span></span>

## <a name="post-prepayment-and-payment-vat"></a><span data-ttu-id="959fc-143">Учет предоплаты и оплаты НДС</span><span class="sxs-lookup"><span data-stu-id="959fc-143">Post Prepayment and Payment VAT</span></span>

1. <span data-ttu-id="959fc-144">Создайте и выпустите счет.</span><span class="sxs-lookup"><span data-stu-id="959fc-144">Create and release an invoice.</span></span>

2. <span data-ttu-id="959fc-145">Для оплаты в валюте для банка и в рублях для поставщика необходимо создать две строки в **журнале платежей**.</span><span class="sxs-lookup"><span data-stu-id="959fc-145">For the payment in the currency for the bank and in rubles for the vendor it is necessary to create two lines in the **payment journal**.</span></span>

    - <span data-ttu-id="959fc-146">**Для поставщика:**</span><span class="sxs-lookup"><span data-stu-id="959fc-146">**For vendor:**</span></span>

        - <span data-ttu-id="959fc-147">Дата учета,</span><span class="sxs-lookup"><span data-stu-id="959fc-147">Posting Date,</span></span>
        - <span data-ttu-id="959fc-148">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="959fc-148">Document Type - Payment</span></span>
        - <span data-ttu-id="959fc-149">Предоплата - да</span><span class="sxs-lookup"><span data-stu-id="959fc-149">Prepayment - yes</span></span>
        - <span data-ttu-id="959fc-150">Тип счета — поставщик</span><span class="sxs-lookup"><span data-stu-id="959fc-150">Account Type - Vendor</span></span>
        - <span data-ttu-id="959fc-151">Номер счета</span><span class="sxs-lookup"><span data-stu-id="959fc-151">Account No.</span></span>
        - <span data-ttu-id="959fc-152">Номер договора</span><span class="sxs-lookup"><span data-stu-id="959fc-152">Agreement No.</span></span>
        - <span data-ttu-id="959fc-153">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="959fc-153">Bal. Account Type - G/L Account</span></span>
        - <span data-ttu-id="959fc-154">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="959fc-154">Bal. Account - " "</span></span>
        - <span data-ttu-id="959fc-155">Код валюты — " "</span><span class="sxs-lookup"><span data-stu-id="959fc-155">Currency Code - " "</span></span>
        - <span data-ttu-id="959fc-156">Номер документа предоплаты требуется</span><span class="sxs-lookup"><span data-stu-id="959fc-156">Prepayment Document No. is required</span></span>
        - <span data-ttu-id="959fc-157">Сумма — в рублях</span><span class="sxs-lookup"><span data-stu-id="959fc-157">Amount - in rubles</span></span>

    - <span data-ttu-id="959fc-158">**Для банка:**</span><span class="sxs-lookup"><span data-stu-id="959fc-158">**For Bank:**</span></span>

        - <span data-ttu-id="959fc-159">Дата учета,</span><span class="sxs-lookup"><span data-stu-id="959fc-159">Posting Date,</span></span>
        - <span data-ttu-id="959fc-160">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="959fc-160">Document Type - Payment</span></span>
        - <span data-ttu-id="959fc-161">Предоплата - да</span><span class="sxs-lookup"><span data-stu-id="959fc-161">Prepayment - yes</span></span>
        - <span data-ttu-id="959fc-162">Тип счета — банковский счет</span><span class="sxs-lookup"><span data-stu-id="959fc-162">Account Type - Bank Account</span></span>
        - <span data-ttu-id="959fc-163">Номер счета</span><span class="sxs-lookup"><span data-stu-id="959fc-163">Account No.</span></span>
        - <span data-ttu-id="959fc-164">Номер договора</span><span class="sxs-lookup"><span data-stu-id="959fc-164">Agreement No.</span></span>
        - <span data-ttu-id="959fc-165">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="959fc-165">Bal. Account Type -  G/L Account</span></span>
        - <span data-ttu-id="959fc-166">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="959fc-166">Bal. Account - " "</span></span>
        - <span data-ttu-id="959fc-167">код валюты;</span><span class="sxs-lookup"><span data-stu-id="959fc-167">Currency Code</span></span>
        - <span data-ttu-id="959fc-168">Сумма — в долларах США/Евро</span><span class="sxs-lookup"><span data-stu-id="959fc-168">Amount - in USD/EUR</span></span>

3. <span data-ttu-id="959fc-169">Выполните учет строк журнала.</span><span class="sxs-lookup"><span data-stu-id="959fc-169">Post the lines of Journal.</span></span>
4. <span data-ttu-id="959fc-170">Выполните отгрузку.</span><span class="sxs-lookup"><span data-stu-id="959fc-170">Ship.</span></span>

    <span data-ttu-id="959fc-171">Вы можете изменить код валюты и сумму в счете.</span><span class="sxs-lookup"><span data-stu-id="959fc-171">You can change the Currency Code and Amount in the Invoice.</span></span>

5. <span data-ttu-id="959fc-172">Учет счета.</span><span class="sxs-lookup"><span data-stu-id="959fc-172">Post the invoice.</span></span>

6. <span data-ttu-id="959fc-173">Примените операцию.</span><span class="sxs-lookup"><span data-stu-id="959fc-173">Apply Entry.</span></span>

7. <span data-ttu-id="959fc-174">Откройте журнал НДС.</span><span class="sxs-lookup"><span data-stu-id="959fc-174">Go to VAT Settlement Worksheet.</span></span> <span data-ttu-id="959fc-175">Выполните учет НДС (см. [Зачет НДС](Settlement-VAT.md)).</span><span class="sxs-lookup"><span data-stu-id="959fc-175">Post VAT (see [Settlement VAT](Settlement-VAT.md)).</span></span>

    <span data-ttu-id="959fc-176">В конце периода будут формироваться операции в результате переоценки задолженности.</span><span class="sxs-lookup"><span data-stu-id="959fc-176">At the end of the period will be formed entries as a result of revaluation of debt.</span></span>

8. <span data-ttu-id="959fc-177">Создайте строки в журнале платежей и учтите их.</span><span class="sxs-lookup"><span data-stu-id="959fc-177">Create and post lines in Payment Journal.</span></span>

    <span data-ttu-id="959fc-178">Для оплаты в валюте для банка и в рублях для поставщика необходимо создать две строки в журнале платежей.</span><span class="sxs-lookup"><span data-stu-id="959fc-178">For the payment in the currency for the bank and in rubles for the vendor it is necessary to create two lines in the payment journal.</span></span>

    - <span data-ttu-id="959fc-179">**Для поставщика:**</span><span class="sxs-lookup"><span data-stu-id="959fc-179">**For vendor:**</span></span>

        - <span data-ttu-id="959fc-180">Дата учета</span><span class="sxs-lookup"><span data-stu-id="959fc-180">Posting Date</span></span>
        - <span data-ttu-id="959fc-181">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="959fc-181">Document Type - Payment</span></span>
        - <span data-ttu-id="959fc-182">Тип счета — поставщик</span><span class="sxs-lookup"><span data-stu-id="959fc-182">Account Type - Vendor</span></span>
        - <span data-ttu-id="959fc-183">Номер счета</span><span class="sxs-lookup"><span data-stu-id="959fc-183">Account No.</span></span>
        - <span data-ttu-id="959fc-184">Номер внешнего документа</span><span class="sxs-lookup"><span data-stu-id="959fc-184">External Document No.</span></span>
        - <span data-ttu-id="959fc-185">Номер внутреннего документа</span><span class="sxs-lookup"><span data-stu-id="959fc-185">Internal Document No.</span></span>
        - <span data-ttu-id="959fc-186">Номер договора</span><span class="sxs-lookup"><span data-stu-id="959fc-186">Agreement No.</span></span>
        - <span data-ttu-id="959fc-187">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="959fc-187">Bal. Account Type - G/L Account</span></span>
        - <span data-ttu-id="959fc-188">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="959fc-188">Bal. Account - " "</span></span>
        - <span data-ttu-id="959fc-189">Код валюты — " "</span><span class="sxs-lookup"><span data-stu-id="959fc-189">Currency Code - " "</span></span>
        - <span data-ttu-id="959fc-190">Номер документа предоплаты требуется</span><span class="sxs-lookup"><span data-stu-id="959fc-190">Prepayment Document No. is required</span></span>
        - <span data-ttu-id="959fc-191">Сумма — в рублях</span><span class="sxs-lookup"><span data-stu-id="959fc-191">Amount - in rubles</span></span>

    - <span data-ttu-id="959fc-192">**Для банка:**</span><span class="sxs-lookup"><span data-stu-id="959fc-192">**For Bank:**</span></span>

        - <span data-ttu-id="959fc-193">Дата учета,</span><span class="sxs-lookup"><span data-stu-id="959fc-193">Posting Date,</span></span>
        - <span data-ttu-id="959fc-194">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="959fc-194">Document Type - Payment</span></span>
        - <span data-ttu-id="959fc-195">Тип счета — банковский счет</span><span class="sxs-lookup"><span data-stu-id="959fc-195">Account Type - Bank Account</span></span>
        - <span data-ttu-id="959fc-196">Номер счета</span><span class="sxs-lookup"><span data-stu-id="959fc-196">Account No.</span></span>
        - <span data-ttu-id="959fc-197">Номер договора</span><span class="sxs-lookup"><span data-stu-id="959fc-197">Agreement No.</span></span>
        - <span data-ttu-id="959fc-198">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="959fc-198">Bal. Account Type -  G/L Account</span></span>
        - <span data-ttu-id="959fc-199">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="959fc-199">Bal. Account - " "</span></span>
        - <span data-ttu-id="959fc-200">код валюты;</span><span class="sxs-lookup"><span data-stu-id="959fc-200">Currency Code</span></span>
        - <span data-ttu-id="959fc-201">Сумма — в долларах США/Евро</span><span class="sxs-lookup"><span data-stu-id="959fc-201">Amount - in USD/EUR</span></span>

## <a name="see-also"></a><span data-ttu-id="959fc-202">См. также</span><span class="sxs-lookup"><span data-stu-id="959fc-202">See Also</span></span>

[<span data-ttu-id="959fc-203">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="959fc-203">Russia Local Functionality</span></span>](russia-local-functionality.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]