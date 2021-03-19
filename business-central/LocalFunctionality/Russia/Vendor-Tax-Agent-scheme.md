---
title: Схема налогового агента поставщика в России
description: Российские усовершенствования включают схемы налоговых агентов поставщиков.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: ee2a163b8b7cda17016ea500e4702303059a6680
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5382775"
---
# <a name="vendor-tax-agent-scheme"></a><span data-ttu-id="ee075-103">Схема налогового агента поставщика</span><span class="sxs-lookup"><span data-stu-id="ee075-103">Vendor Tax Agent Scheme</span></span>

## <a name="vat-from-internal-funds"></a><span data-ttu-id="ee075-104">НДС из внутренних фондов</span><span class="sxs-lookup"><span data-stu-id="ee075-104">VAT from Internal Funds</span></span>

<span data-ttu-id="ee075-105">Заполните поля в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="ee075-105">Fill in the fields on the vendor card.</span></span>

1. <span data-ttu-id="ee075-106">Экспресс-вкладка **Договор**:</span><span class="sxs-lookup"><span data-stu-id="ee075-106">**Agreement** FastTab:</span></span>

    - <span data-ttu-id="ee075-107">Учет договоров - обязательно.</span><span class="sxs-lookup"><span data-stu-id="ee075-107">Agreement posting - mandatory.</span></span>

    - <span data-ttu-id="ee075-108">Номера договоров обязательны.</span><span class="sxs-lookup"><span data-stu-id="ee075-108">Agreement numbers required.</span></span>

2. <span data-ttu-id="ee075-109">На карточке договора:</span><span class="sxs-lookup"><span data-stu-id="ee075-109">On the agreement card:</span></span>

    - <span data-ttu-id="ee075-110">НДС бизнес-группа</span><span class="sxs-lookup"><span data-stu-id="ee075-110">VAT Bus. Posting Group</span></span>
    - <span data-ttu-id="ee075-111">НДС товарная группа налогового агента</span><span class="sxs-lookup"><span data-stu-id="ee075-111">VAT Agent Prod. Posting Group</span></span>
    - <span data-ttu-id="ee075-112">Тип источника оплаты НДС - Внутренние фонды</span><span class="sxs-lookup"><span data-stu-id="ee075-112">VAT Payment Source Type - Internal Funds</span></span>

## <a name="prepayment-and-payment-vat"></a><span data-ttu-id="ee075-113">Предоплата и оплата НДС</span><span class="sxs-lookup"><span data-stu-id="ee075-113">Prepayment and Payment VAT</span></span>

1. <span data-ttu-id="ee075-114">Создание и выпуск счета</span><span class="sxs-lookup"><span data-stu-id="ee075-114">Create and release an invoice</span></span>

    <span data-ttu-id="ee075-115">Номер договора</span><span class="sxs-lookup"><span data-stu-id="ee075-115">Agreement No.</span></span> <span data-ttu-id="ee075-116">(с настройками для продавца с уплатой НДС из внутренних фондов) должен быть указан.</span><span class="sxs-lookup"><span data-stu-id="ee075-116">(with settings for Vendor with VAT Payment from internal funds) should be specified.</span></span>

2. <span data-ttu-id="ee075-117">Создание строки в журнале платежей:</span><span class="sxs-lookup"><span data-stu-id="ee075-117">Create a line in Payment Journal:</span></span>

    - <span data-ttu-id="ee075-118">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="ee075-118">Document Type - Payment</span></span>
    - <span data-ttu-id="ee075-119">Предоплата - да</span><span class="sxs-lookup"><span data-stu-id="ee075-119">Prepayment - yes</span></span>
    - <span data-ttu-id="ee075-120">Номер документа предоплаты не требуется.</span><span class="sxs-lookup"><span data-stu-id="ee075-120">Prepayment Document No is required.</span></span>

3. <span data-ttu-id="ee075-121">Выполните учет строк журнала.</span><span class="sxs-lookup"><span data-stu-id="ee075-121">Post lines of Journal</span></span>

    <span data-ttu-id="ee075-122">Операции с НДС генерируются автоматически в рублях.</span><span class="sxs-lookup"><span data-stu-id="ee075-122">Operations with VAT are automatically generated in rubles.</span></span>

4. <span data-ttu-id="ee075-123">Создайте и учтите в журнале платежей для налогового органа строку с суммой НДС для предоплаты.</span><span class="sxs-lookup"><span data-stu-id="ee075-123">Create and post line in Payment Journal for Tax Authority with VAT Amount of prepayment.</span></span>

5. <span data-ttu-id="ee075-124">Выполните отгрузку и учет счета.</span><span class="sxs-lookup"><span data-stu-id="ee075-124">Ship and post invoice.</span></span>

6. <span data-ttu-id="ee075-125">Создайте строку в журнале платежей</span><span class="sxs-lookup"><span data-stu-id="ee075-125">Create a line in Payment Journal</span></span>

    - <span data-ttu-id="ee075-126">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="ee075-126">Document Type - Payment</span></span>
    - <span data-ttu-id="ee075-127">Номер начального документа - Номер</span><span class="sxs-lookup"><span data-stu-id="ee075-127">Initial Document No. - No.</span></span> <span data-ttu-id="ee075-128">учтенного счета</span><span class="sxs-lookup"><span data-stu-id="ee075-128">of posted invoice</span></span>
    - <span data-ttu-id="ee075-129">Примен. к док. - номер - Номер</span><span class="sxs-lookup"><span data-stu-id="ee075-129">Applies-to Doc. No. - No.</span></span> <span data-ttu-id="ee075-130">учтенного счета</span><span class="sxs-lookup"><span data-stu-id="ee075-130">of posted invoice</span></span>

7. <span data-ttu-id="ee075-131">Создайте и выполните учет платежа в налоговый орган.</span><span class="sxs-lookup"><span data-stu-id="ee075-131">Create and post payment to the Tax Authority.</span></span>
8. <span data-ttu-id="ee075-132">Откройте журнал НДС.</span><span class="sxs-lookup"><span data-stu-id="ee075-132">Go to VAT Settlement Worksheet.</span></span> <span data-ttu-id="ee075-133">Выполните учет НДС (см. [Зачет НДС](Settlement-VAT.md)).</span><span class="sxs-lookup"><span data-stu-id="ee075-133">Post VAT (see [Settlement VAT](Settlement-VAT.md)).</span></span>

## <a name="vat-from-vendor-funds"></a><span data-ttu-id="ee075-134">НДС из фондов поставщика</span><span class="sxs-lookup"><span data-stu-id="ee075-134">VAT from Vendor Funds</span></span>

<span data-ttu-id="ee075-135">Заполните поля в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="ee075-135">Fill the fields in Vendor Card.</span></span>

1. <span data-ttu-id="ee075-136">На вкладке "Договор":</span><span class="sxs-lookup"><span data-stu-id="ee075-136">On Agreement tab:</span></span>

    - <span data-ttu-id="ee075-137">Учет договоров - обязательно.</span><span class="sxs-lookup"><span data-stu-id="ee075-137">Agreement posting - mandatory.</span></span>
    - <span data-ttu-id="ee075-138">Номера договоров обязательны.</span><span class="sxs-lookup"><span data-stu-id="ee075-138">Agreement Nos is required.</span></span>

2. <span data-ttu-id="ee075-139">В карточке договора:</span><span class="sxs-lookup"><span data-stu-id="ee075-139">In Agreement card:</span></span>

    - <span data-ttu-id="ee075-140">НДС бизнес-группа</span><span class="sxs-lookup"><span data-stu-id="ee075-140">VAT Bus. Posting Group</span></span>
    - <span data-ttu-id="ee075-141">НДС товарная группа налогового агента</span><span class="sxs-lookup"><span data-stu-id="ee075-141">VAT Agent Prod. Posting Group</span></span>
    - <span data-ttu-id="ee075-142">Тип источника оплаты НДС - Фонды поставщика</span><span class="sxs-lookup"><span data-stu-id="ee075-142">VAT Payment Source Type - Vendor Funds</span></span>

## <a name="post-prepayment-and-payment-vat"></a><span data-ttu-id="ee075-143">Учет предоплаты и оплаты НДС</span><span class="sxs-lookup"><span data-stu-id="ee075-143">Post Prepayment and Payment VAT</span></span>

1. <span data-ttu-id="ee075-144">Создайте и выпустите счет.</span><span class="sxs-lookup"><span data-stu-id="ee075-144">Create and release an invoice.</span></span>

2. <span data-ttu-id="ee075-145">Для оплаты в валюте для банка и в рублях для поставщика необходимо создать две строки в **журнале платежей**.</span><span class="sxs-lookup"><span data-stu-id="ee075-145">For the payment in the currency for the bank and in rubles for the vendor it is necessary to create two lines in the **payment journal**.</span></span>

    - <span data-ttu-id="ee075-146">**Для поставщика:**</span><span class="sxs-lookup"><span data-stu-id="ee075-146">**For vendor:**</span></span>

        - <span data-ttu-id="ee075-147">Дата учета,</span><span class="sxs-lookup"><span data-stu-id="ee075-147">Posting Date,</span></span>
        - <span data-ttu-id="ee075-148">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="ee075-148">Document Type - Payment</span></span>
        - <span data-ttu-id="ee075-149">Предоплата - да</span><span class="sxs-lookup"><span data-stu-id="ee075-149">Prepayment - yes</span></span>
        - <span data-ttu-id="ee075-150">Тип счета — поставщик</span><span class="sxs-lookup"><span data-stu-id="ee075-150">Account Type - Vendor</span></span>
        - <span data-ttu-id="ee075-151">Номер счета</span><span class="sxs-lookup"><span data-stu-id="ee075-151">Account No.</span></span>
        - <span data-ttu-id="ee075-152">Номер договора</span><span class="sxs-lookup"><span data-stu-id="ee075-152">Agreement No.</span></span>
        - <span data-ttu-id="ee075-153">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="ee075-153">Bal. Account Type - G/L Account</span></span>
        - <span data-ttu-id="ee075-154">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="ee075-154">Bal. Account - " "</span></span>
        - <span data-ttu-id="ee075-155">Код валюты — " "</span><span class="sxs-lookup"><span data-stu-id="ee075-155">Currency Code - " "</span></span>
        - <span data-ttu-id="ee075-156">Номер документа предоплаты требуется</span><span class="sxs-lookup"><span data-stu-id="ee075-156">Prepayment Document No. is required</span></span>
        - <span data-ttu-id="ee075-157">Сумма — в рублях</span><span class="sxs-lookup"><span data-stu-id="ee075-157">Amount - in rubles</span></span>

    - <span data-ttu-id="ee075-158">**Для банка:**</span><span class="sxs-lookup"><span data-stu-id="ee075-158">**For Bank:**</span></span>

        - <span data-ttu-id="ee075-159">Дата учета,</span><span class="sxs-lookup"><span data-stu-id="ee075-159">Posting Date,</span></span>
        - <span data-ttu-id="ee075-160">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="ee075-160">Document Type - Payment</span></span>
        - <span data-ttu-id="ee075-161">Предоплата - да</span><span class="sxs-lookup"><span data-stu-id="ee075-161">Prepayment - yes</span></span>
        - <span data-ttu-id="ee075-162">Тип счета — банковский счет</span><span class="sxs-lookup"><span data-stu-id="ee075-162">Account Type - Bank Account</span></span>
        - <span data-ttu-id="ee075-163">Номер счета</span><span class="sxs-lookup"><span data-stu-id="ee075-163">Account No.</span></span>
        - <span data-ttu-id="ee075-164">Номер договора</span><span class="sxs-lookup"><span data-stu-id="ee075-164">Agreement No.</span></span>
        - <span data-ttu-id="ee075-165">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="ee075-165">Bal. Account Type -  G/L Account</span></span>
        - <span data-ttu-id="ee075-166">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="ee075-166">Bal. Account - " "</span></span>
        - <span data-ttu-id="ee075-167">код валюты;</span><span class="sxs-lookup"><span data-stu-id="ee075-167">Currency Code</span></span>
        - <span data-ttu-id="ee075-168">Сумма — в долларах США/Евро</span><span class="sxs-lookup"><span data-stu-id="ee075-168">Amount - in USD/EUR</span></span>

3. <span data-ttu-id="ee075-169">Выполните учет строк журнала.</span><span class="sxs-lookup"><span data-stu-id="ee075-169">Post the lines of Journal.</span></span>
4. <span data-ttu-id="ee075-170">Выполните отгрузку.</span><span class="sxs-lookup"><span data-stu-id="ee075-170">Ship.</span></span>

    <span data-ttu-id="ee075-171">Вы можете изменить код валюты и сумму в счете.</span><span class="sxs-lookup"><span data-stu-id="ee075-171">You can change the Currency Code and Amount in the Invoice.</span></span>

5. <span data-ttu-id="ee075-172">Учет счета.</span><span class="sxs-lookup"><span data-stu-id="ee075-172">Post the invoice.</span></span>

6. <span data-ttu-id="ee075-173">Примените операцию.</span><span class="sxs-lookup"><span data-stu-id="ee075-173">Apply Entry.</span></span>

7. <span data-ttu-id="ee075-174">Откройте журнал НДС.</span><span class="sxs-lookup"><span data-stu-id="ee075-174">Go to VAT Settlement Worksheet.</span></span> <span data-ttu-id="ee075-175">Выполните учет НДС (см. [Зачет НДС](Settlement-VAT.md)).</span><span class="sxs-lookup"><span data-stu-id="ee075-175">Post VAT (see [Settlement VAT](Settlement-VAT.md)).</span></span>

    <span data-ttu-id="ee075-176">В конце периода будут формироваться операции в результате переоценки задолженности.</span><span class="sxs-lookup"><span data-stu-id="ee075-176">At the end of the period will be formed entries as a result of revaluation of debt.</span></span>

8. <span data-ttu-id="ee075-177">Создайте строки в журнале платежей и учтите их.</span><span class="sxs-lookup"><span data-stu-id="ee075-177">Create and post lines in Payment Journal.</span></span>

    <span data-ttu-id="ee075-178">Для оплаты в валюте для банка и в рублях для поставщика необходимо создать две строки в журнале платежей.</span><span class="sxs-lookup"><span data-stu-id="ee075-178">For the payment in the currency for the bank and in rubles for the vendor it is necessary to create two lines in the payment journal.</span></span>

    - <span data-ttu-id="ee075-179">**Для поставщика:**</span><span class="sxs-lookup"><span data-stu-id="ee075-179">**For vendor:**</span></span>

        - <span data-ttu-id="ee075-180">Дата учета</span><span class="sxs-lookup"><span data-stu-id="ee075-180">Posting Date</span></span>
        - <span data-ttu-id="ee075-181">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="ee075-181">Document Type - Payment</span></span>
        - <span data-ttu-id="ee075-182">Тип счета — поставщик</span><span class="sxs-lookup"><span data-stu-id="ee075-182">Account Type - Vendor</span></span>
        - <span data-ttu-id="ee075-183">Номер счета</span><span class="sxs-lookup"><span data-stu-id="ee075-183">Account No.</span></span>
        - <span data-ttu-id="ee075-184">Номер внешнего документа</span><span class="sxs-lookup"><span data-stu-id="ee075-184">External Document No.</span></span>
        - <span data-ttu-id="ee075-185">Номер внутреннего документа</span><span class="sxs-lookup"><span data-stu-id="ee075-185">Internal Document No.</span></span>
        - <span data-ttu-id="ee075-186">Номер договора</span><span class="sxs-lookup"><span data-stu-id="ee075-186">Agreement No.</span></span>
        - <span data-ttu-id="ee075-187">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="ee075-187">Bal. Account Type - G/L Account</span></span>
        - <span data-ttu-id="ee075-188">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="ee075-188">Bal. Account - " "</span></span>
        - <span data-ttu-id="ee075-189">Код валюты — " "</span><span class="sxs-lookup"><span data-stu-id="ee075-189">Currency Code - " "</span></span>
        - <span data-ttu-id="ee075-190">Номер документа предоплаты требуется</span><span class="sxs-lookup"><span data-stu-id="ee075-190">Prepayment Document No. is required</span></span>
        - <span data-ttu-id="ee075-191">Сумма — в рублях</span><span class="sxs-lookup"><span data-stu-id="ee075-191">Amount - in rubles</span></span>

    - <span data-ttu-id="ee075-192">**Для банка:**</span><span class="sxs-lookup"><span data-stu-id="ee075-192">**For Bank:**</span></span>

        - <span data-ttu-id="ee075-193">Дата учета,</span><span class="sxs-lookup"><span data-stu-id="ee075-193">Posting Date,</span></span>
        - <span data-ttu-id="ee075-194">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="ee075-194">Document Type - Payment</span></span>
        - <span data-ttu-id="ee075-195">Тип счета — банковский счет</span><span class="sxs-lookup"><span data-stu-id="ee075-195">Account Type - Bank Account</span></span>
        - <span data-ttu-id="ee075-196">Номер счета</span><span class="sxs-lookup"><span data-stu-id="ee075-196">Account No.</span></span>
        - <span data-ttu-id="ee075-197">Номер договора</span><span class="sxs-lookup"><span data-stu-id="ee075-197">Agreement No.</span></span>
        - <span data-ttu-id="ee075-198">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="ee075-198">Bal. Account Type -  G/L Account</span></span>
        - <span data-ttu-id="ee075-199">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="ee075-199">Bal. Account - " "</span></span>
        - <span data-ttu-id="ee075-200">код валюты;</span><span class="sxs-lookup"><span data-stu-id="ee075-200">Currency Code</span></span>
        - <span data-ttu-id="ee075-201">Сумма — в долларах США/Евро</span><span class="sxs-lookup"><span data-stu-id="ee075-201">Amount - in USD/EUR</span></span>

## <a name="see-also"></a><span data-ttu-id="ee075-202">См. также</span><span class="sxs-lookup"><span data-stu-id="ee075-202">See Also</span></span>

[<span data-ttu-id="ee075-203">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="ee075-203">Russia Local Functionality</span></span>](russia-local-functionality.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]