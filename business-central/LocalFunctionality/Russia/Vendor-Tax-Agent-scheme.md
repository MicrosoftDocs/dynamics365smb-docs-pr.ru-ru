---
title: Схема налогового агента поставщика в России
description: Российские усовершенствования включают схемы налоговых агентов поставщиков.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: f638de2d02331d4ec1c0faba4784f7d665b4ec5c
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3921280"
---
# <a name="vendor-tax-agent-scheme"></a><span data-ttu-id="52819-103">Схема налогового агента поставщика</span><span class="sxs-lookup"><span data-stu-id="52819-103">Vendor Tax Agent Scheme</span></span>

## <a name="vat-from-internal-funds"></a><span data-ttu-id="52819-104">НДС из внутренних фондов</span><span class="sxs-lookup"><span data-stu-id="52819-104">VAT from Internal Funds</span></span>

<span data-ttu-id="52819-105">Заполните поля в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="52819-105">Fill in the fields on the vendor card.</span></span>

1. <span data-ttu-id="52819-106">Экспресс-вкладка **Договор**:</span><span class="sxs-lookup"><span data-stu-id="52819-106">**Agreement** FastTab:</span></span>

    - <span data-ttu-id="52819-107">Учет договоров - обязательно.</span><span class="sxs-lookup"><span data-stu-id="52819-107">Agreement posting - mandatory.</span></span>

    - <span data-ttu-id="52819-108">Номера договоров обязательны.</span><span class="sxs-lookup"><span data-stu-id="52819-108">Agreement numbers required.</span></span>

2. <span data-ttu-id="52819-109">На карточке договора:</span><span class="sxs-lookup"><span data-stu-id="52819-109">On the agreement card:</span></span>

    - <span data-ttu-id="52819-110">НДС бизнес-группа</span><span class="sxs-lookup"><span data-stu-id="52819-110">VAT Bus. Posting Group</span></span>
    - <span data-ttu-id="52819-111">НДС товарная группа налогового агента</span><span class="sxs-lookup"><span data-stu-id="52819-111">VAT Agent Prod. Posting Group</span></span>
    - <span data-ttu-id="52819-112">Тип источника оплаты НДС - Внутренние фонды</span><span class="sxs-lookup"><span data-stu-id="52819-112">VAT Payment Source Type - Internal Funds</span></span>

## <a name="prepayment-and-payment-vat"></a><span data-ttu-id="52819-113">Предоплата и оплата НДС</span><span class="sxs-lookup"><span data-stu-id="52819-113">Prepayment and Payment VAT</span></span>

1. <span data-ttu-id="52819-114">Создание и выпуск счета</span><span class="sxs-lookup"><span data-stu-id="52819-114">Create and release an invoice</span></span>

    <span data-ttu-id="52819-115">Номер договора</span><span class="sxs-lookup"><span data-stu-id="52819-115">Agreement No.</span></span> <span data-ttu-id="52819-116">(с настройками для продавца с уплатой НДС из внутренних фондов) должен быть указан.</span><span class="sxs-lookup"><span data-stu-id="52819-116">(with settings for Vendor with VAT Payment from internal funds) should be specified.</span></span>

2. <span data-ttu-id="52819-117">Создание строки в журнале платежей:</span><span class="sxs-lookup"><span data-stu-id="52819-117">Create a line in Payment Journal:</span></span>

    - <span data-ttu-id="52819-118">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="52819-118">Document Type - Payment</span></span>
    - <span data-ttu-id="52819-119">Предоплата - да</span><span class="sxs-lookup"><span data-stu-id="52819-119">Prepayment - yes</span></span>
    - <span data-ttu-id="52819-120">Номер документа предоплаты не требуется.</span><span class="sxs-lookup"><span data-stu-id="52819-120">Prepayment Document No is required.</span></span>

3. <span data-ttu-id="52819-121">Выполните учет строк журнала.</span><span class="sxs-lookup"><span data-stu-id="52819-121">Post lines of Journal</span></span>

    <span data-ttu-id="52819-122">Операции с НДС генерируются автоматически в рублях.</span><span class="sxs-lookup"><span data-stu-id="52819-122">Operations with VAT are automatically generated in rubles.</span></span>

4. <span data-ttu-id="52819-123">Создайте и учтите в журнале платежей для налогового органа строку с суммой НДС для предоплаты.</span><span class="sxs-lookup"><span data-stu-id="52819-123">Create and post line in Payment Journal for Tax Authority with VAT Amount of prepayment.</span></span>

5. <span data-ttu-id="52819-124">Выполните отгрузку и учет счета.</span><span class="sxs-lookup"><span data-stu-id="52819-124">Ship and post invoice.</span></span>

6. <span data-ttu-id="52819-125">Создайте строку в журнале платежей</span><span class="sxs-lookup"><span data-stu-id="52819-125">Create a line in Payment Journal</span></span>

    - <span data-ttu-id="52819-126">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="52819-126">Document Type - Payment</span></span>
    - <span data-ttu-id="52819-127">Номер начального документа - Номер</span><span class="sxs-lookup"><span data-stu-id="52819-127">Initial Document No. - No.</span></span> <span data-ttu-id="52819-128">учтенного счета</span><span class="sxs-lookup"><span data-stu-id="52819-128">of posted invoice</span></span>
    - <span data-ttu-id="52819-129">Примен. к док. - номер - Номер</span><span class="sxs-lookup"><span data-stu-id="52819-129">Applies-to Doc. No. - No.</span></span> <span data-ttu-id="52819-130">учтенного счета</span><span class="sxs-lookup"><span data-stu-id="52819-130">of posted invoice</span></span>

7. <span data-ttu-id="52819-131">Создайте и выполните учет платежа в налоговый орган.</span><span class="sxs-lookup"><span data-stu-id="52819-131">Create and post payment to the Tax Authority.</span></span>
8. <span data-ttu-id="52819-132">Откройте журнал НДС.</span><span class="sxs-lookup"><span data-stu-id="52819-132">Go to VAT Settlement Worksheet.</span></span> <span data-ttu-id="52819-133">Выполните учет НДС (см. [Зачет НДС](Settlement-VAT.md)).</span><span class="sxs-lookup"><span data-stu-id="52819-133">Post VAT (see [Settlement VAT](Settlement-VAT.md)).</span></span>

## <a name="vat-from-vendor-funds"></a><span data-ttu-id="52819-134">НДС из фондов поставщика</span><span class="sxs-lookup"><span data-stu-id="52819-134">VAT from Vendor Funds</span></span>

<span data-ttu-id="52819-135">Заполните поля в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="52819-135">Fill the fields in Vendor Card.</span></span>

1. <span data-ttu-id="52819-136">На вкладке "Договор":</span><span class="sxs-lookup"><span data-stu-id="52819-136">On Agreement tab:</span></span>

    - <span data-ttu-id="52819-137">Учет договоров - обязательно.</span><span class="sxs-lookup"><span data-stu-id="52819-137">Agreement posting - mandatory.</span></span>
    - <span data-ttu-id="52819-138">Номера договоров обязательны.</span><span class="sxs-lookup"><span data-stu-id="52819-138">Agreement Nos is required.</span></span>

2. <span data-ttu-id="52819-139">В карточке договора:</span><span class="sxs-lookup"><span data-stu-id="52819-139">In Agreement card:</span></span>

    - <span data-ttu-id="52819-140">НДС бизнес-группа</span><span class="sxs-lookup"><span data-stu-id="52819-140">VAT Bus. Posting Group</span></span>
    - <span data-ttu-id="52819-141">НДС товарная группа налогового агента</span><span class="sxs-lookup"><span data-stu-id="52819-141">VAT Agent Prod. Posting Group</span></span>
    - <span data-ttu-id="52819-142">Тип источника оплаты НДС - Фонды поставщика</span><span class="sxs-lookup"><span data-stu-id="52819-142">VAT Payment Source Type - Vendor Funds</span></span>

## <a name="post-prepayment-and-payment-vat"></a><span data-ttu-id="52819-143">Учет предоплаты и оплаты НДС</span><span class="sxs-lookup"><span data-stu-id="52819-143">Post Prepayment and Payment VAT</span></span>

1. <span data-ttu-id="52819-144">Создайте и выпустите счет.</span><span class="sxs-lookup"><span data-stu-id="52819-144">Create and release an invoice.</span></span>

2. <span data-ttu-id="52819-145">Для оплаты в валюте для банка и в рублях для поставщика необходимо создать две строки в **журнале платежей**.</span><span class="sxs-lookup"><span data-stu-id="52819-145">For the payment in the currency for the bank and in rubles for the vendor it is necessary to create two lines in the **payment journal**.</span></span>

    - <span data-ttu-id="52819-146">**Для поставщика:**</span><span class="sxs-lookup"><span data-stu-id="52819-146">**For vendor:**</span></span>

        - <span data-ttu-id="52819-147">Дата учета,</span><span class="sxs-lookup"><span data-stu-id="52819-147">Posting Date,</span></span>
        - <span data-ttu-id="52819-148">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="52819-148">Document Type - Payment</span></span>
        - <span data-ttu-id="52819-149">Предоплата - да</span><span class="sxs-lookup"><span data-stu-id="52819-149">Prepayment - yes</span></span>
        - <span data-ttu-id="52819-150">Тип счета — поставщик</span><span class="sxs-lookup"><span data-stu-id="52819-150">Account Type - Vendor</span></span>
        - <span data-ttu-id="52819-151">Номер счета</span><span class="sxs-lookup"><span data-stu-id="52819-151">Account No.</span></span>
        - <span data-ttu-id="52819-152">Номер договора</span><span class="sxs-lookup"><span data-stu-id="52819-152">Agreement No.</span></span>
        - <span data-ttu-id="52819-153">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="52819-153">Bal. Account Type - G/L Account</span></span>
        - <span data-ttu-id="52819-154">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="52819-154">Bal. Account - " "</span></span>
        - <span data-ttu-id="52819-155">Код валюты — " "</span><span class="sxs-lookup"><span data-stu-id="52819-155">Currency Code - " "</span></span>
        - <span data-ttu-id="52819-156">Номер документа предоплаты требуется</span><span class="sxs-lookup"><span data-stu-id="52819-156">Prepayment Document No. is required</span></span>
        - <span data-ttu-id="52819-157">Сумма — в рублях</span><span class="sxs-lookup"><span data-stu-id="52819-157">Amount - in rubles</span></span>

    - <span data-ttu-id="52819-158">**Для банка:**</span><span class="sxs-lookup"><span data-stu-id="52819-158">**For Bank:**</span></span>

        - <span data-ttu-id="52819-159">Дата учета,</span><span class="sxs-lookup"><span data-stu-id="52819-159">Posting Date,</span></span>
        - <span data-ttu-id="52819-160">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="52819-160">Document Type - Payment</span></span>
        - <span data-ttu-id="52819-161">Предоплата - да</span><span class="sxs-lookup"><span data-stu-id="52819-161">Prepayment - yes</span></span>
        - <span data-ttu-id="52819-162">Тип счета — банковский счет</span><span class="sxs-lookup"><span data-stu-id="52819-162">Account Type - Bank Account</span></span>
        - <span data-ttu-id="52819-163">Номер счета</span><span class="sxs-lookup"><span data-stu-id="52819-163">Account No.</span></span>
        - <span data-ttu-id="52819-164">Номер договора</span><span class="sxs-lookup"><span data-stu-id="52819-164">Agreement No.</span></span>
        - <span data-ttu-id="52819-165">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="52819-165">Bal. Account Type -  G/L Account</span></span>
        - <span data-ttu-id="52819-166">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="52819-166">Bal. Account - " "</span></span>
        - <span data-ttu-id="52819-167">код валюты;</span><span class="sxs-lookup"><span data-stu-id="52819-167">Currency Code</span></span>
        - <span data-ttu-id="52819-168">Сумма — в долларах США/Евро</span><span class="sxs-lookup"><span data-stu-id="52819-168">Amount - in USD/EUR</span></span>

3. <span data-ttu-id="52819-169">Выполните учет строк журнала.</span><span class="sxs-lookup"><span data-stu-id="52819-169">Post the lines of Journal.</span></span>
4. <span data-ttu-id="52819-170">Выполните отгрузку.</span><span class="sxs-lookup"><span data-stu-id="52819-170">Ship.</span></span>

    <span data-ttu-id="52819-171">Вы можете изменить код валюты и сумму в счете.</span><span class="sxs-lookup"><span data-stu-id="52819-171">You can change the Currency Code and Amount in the Invoice.</span></span>

5. <span data-ttu-id="52819-172">Учет счета.</span><span class="sxs-lookup"><span data-stu-id="52819-172">Post the invoice.</span></span>

6. <span data-ttu-id="52819-173">Примените операцию.</span><span class="sxs-lookup"><span data-stu-id="52819-173">Apply Entry.</span></span>

7. <span data-ttu-id="52819-174">Откройте журнал НДС.</span><span class="sxs-lookup"><span data-stu-id="52819-174">Go to VAT Settlement Worksheet.</span></span> <span data-ttu-id="52819-175">Выполните учет НДС (см. [Зачет НДС](Settlement-VAT.md)).</span><span class="sxs-lookup"><span data-stu-id="52819-175">Post VAT (see [Settlement VAT](Settlement-VAT.md)).</span></span>

    <span data-ttu-id="52819-176">В конце периода будут формироваться операции в результате переоценки задолженности.</span><span class="sxs-lookup"><span data-stu-id="52819-176">At the end of the period will be formed entries as a result of revaluation of debt.</span></span>

8. <span data-ttu-id="52819-177">Создайте строки в журнале платежей и учтите их.</span><span class="sxs-lookup"><span data-stu-id="52819-177">Create and post lines in Payment Journal.</span></span>

    <span data-ttu-id="52819-178">Для оплаты в валюте для банка и в рублях для поставщика необходимо создать две строки в журнале платежей.</span><span class="sxs-lookup"><span data-stu-id="52819-178">For the payment in the currency for the bank and in rubles for the vendor it is necessary to create two lines in the payment journal.</span></span>

    - <span data-ttu-id="52819-179">**Для поставщика:**</span><span class="sxs-lookup"><span data-stu-id="52819-179">**For vendor:**</span></span>

        - <span data-ttu-id="52819-180">Дата учета</span><span class="sxs-lookup"><span data-stu-id="52819-180">Posting Date</span></span>
        - <span data-ttu-id="52819-181">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="52819-181">Document Type - Payment</span></span>
        - <span data-ttu-id="52819-182">Тип счета — поставщик</span><span class="sxs-lookup"><span data-stu-id="52819-182">Account Type - Vendor</span></span>
        - <span data-ttu-id="52819-183">Номер счета</span><span class="sxs-lookup"><span data-stu-id="52819-183">Account No.</span></span>
        - <span data-ttu-id="52819-184">Номер внешнего документа</span><span class="sxs-lookup"><span data-stu-id="52819-184">External Document No.</span></span>
        - <span data-ttu-id="52819-185">Номер внутреннего документа</span><span class="sxs-lookup"><span data-stu-id="52819-185">Internal Document No.</span></span>
        - <span data-ttu-id="52819-186">Номер договора</span><span class="sxs-lookup"><span data-stu-id="52819-186">Agreement No.</span></span>
        - <span data-ttu-id="52819-187">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="52819-187">Bal. Account Type - G/L Account</span></span>
        - <span data-ttu-id="52819-188">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="52819-188">Bal. Account - " "</span></span>
        - <span data-ttu-id="52819-189">Код валюты — " "</span><span class="sxs-lookup"><span data-stu-id="52819-189">Currency Code - " "</span></span>
        - <span data-ttu-id="52819-190">Номер документа предоплаты требуется</span><span class="sxs-lookup"><span data-stu-id="52819-190">Prepayment Document No. is required</span></span>
        - <span data-ttu-id="52819-191">Сумма — в рублях</span><span class="sxs-lookup"><span data-stu-id="52819-191">Amount - in rubles</span></span>

    - <span data-ttu-id="52819-192">**Для банка:**</span><span class="sxs-lookup"><span data-stu-id="52819-192">**For Bank:**</span></span>

        - <span data-ttu-id="52819-193">Дата учета,</span><span class="sxs-lookup"><span data-stu-id="52819-193">Posting Date,</span></span>
        - <span data-ttu-id="52819-194">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="52819-194">Document Type - Payment</span></span>
        - <span data-ttu-id="52819-195">Тип счета — банковский счет</span><span class="sxs-lookup"><span data-stu-id="52819-195">Account Type - Bank Account</span></span>
        - <span data-ttu-id="52819-196">Номер счета</span><span class="sxs-lookup"><span data-stu-id="52819-196">Account No.</span></span>
        - <span data-ttu-id="52819-197">Номер договора</span><span class="sxs-lookup"><span data-stu-id="52819-197">Agreement No.</span></span>
        - <span data-ttu-id="52819-198">Тип балансового счета — счет ГК</span><span class="sxs-lookup"><span data-stu-id="52819-198">Bal. Account Type -  G/L Account</span></span>
        - <span data-ttu-id="52819-199">Баланс. счет — " "</span><span class="sxs-lookup"><span data-stu-id="52819-199">Bal. Account - " "</span></span>
        - <span data-ttu-id="52819-200">код валюты;</span><span class="sxs-lookup"><span data-stu-id="52819-200">Currency Code</span></span>
        - <span data-ttu-id="52819-201">Сумма — в долларах США/Евро</span><span class="sxs-lookup"><span data-stu-id="52819-201">Amount - in USD/EUR</span></span>

## <a name="see-also"></a><span data-ttu-id="52819-202">См. также</span><span class="sxs-lookup"><span data-stu-id="52819-202">See Also</span></span>

[<span data-ttu-id="52819-203">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="52819-203">Russia Local Functionality</span></span>](russia-local-functionality.md)  
