---
title: Схема налогового агента поставщика в России
description: Российские усовершенствования включают схемы налоговых агентов поставщиков.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 787dc8a7a26472779d37858f152f288162404466
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3180982"
---
# <a name="vendor-tax-agent-scheme"></a><span data-ttu-id="4d6bd-103">Схема налогового агента поставщика</span><span class="sxs-lookup"><span data-stu-id="4d6bd-103">Vendor Tax Agent Scheme</span></span>

## <a name="vat-from-internal-funds"></a><span data-ttu-id="4d6bd-104">НДС из внутренних фондов</span><span class="sxs-lookup"><span data-stu-id="4d6bd-104">VAT from Internal Funds</span></span>

<span data-ttu-id="4d6bd-105">Заполните поля в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-105">Fill in the fields on the vendor card.</span></span>

1. <span data-ttu-id="4d6bd-106">Экспресс-вкладка **Договор**:</span><span class="sxs-lookup"><span data-stu-id="4d6bd-106">**Agreement** FastTab:</span></span>

    - <span data-ttu-id="4d6bd-107">Учет договоров - обязательно.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-107">Agreement posting - mandatory.</span></span>

    - <span data-ttu-id="4d6bd-108">Номера договоров обязательны.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-108">Agreement numbers required.</span></span>

2. <span data-ttu-id="4d6bd-109">На карточке договора:</span><span class="sxs-lookup"><span data-stu-id="4d6bd-109">On the agreement card:</span></span>

    - <span data-ttu-id="4d6bd-110">НДС бизнес-группа</span><span class="sxs-lookup"><span data-stu-id="4d6bd-110">VAT Bus. Posting Group</span></span>
    - <span data-ttu-id="4d6bd-111">НДС товарная группа налогового агента</span><span class="sxs-lookup"><span data-stu-id="4d6bd-111">VAT Agent Prod. Posting Group</span></span>
    - <span data-ttu-id="4d6bd-112">Тип источника оплаты НДС - Внутренние фонды</span><span class="sxs-lookup"><span data-stu-id="4d6bd-112">VAT Payment Source Type - Internal Funds</span></span>

## <a name="prepayment-and-payment-vat"></a><span data-ttu-id="4d6bd-113">Предоплата и оплата НДС</span><span class="sxs-lookup"><span data-stu-id="4d6bd-113">Prepayment and Payment VAT</span></span>

1. <span data-ttu-id="4d6bd-114">Создание и выпуск счета</span><span class="sxs-lookup"><span data-stu-id="4d6bd-114">Create and release an invoice</span></span>

<span data-ttu-id="4d6bd-115">Номер договора</span><span class="sxs-lookup"><span data-stu-id="4d6bd-115">Agreement No.</span></span> <span data-ttu-id="4d6bd-116">(с настройками для продавца с уплатой НДС из внутренних фондов) должен быть указан.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-116">(with settings for Vendor with VAT Payment from internal funds) should be specified.</span></span>

2. <span data-ttu-id="4d6bd-117">Создание строки в журнале платежей:</span><span class="sxs-lookup"><span data-stu-id="4d6bd-117">Create a line in Payment Journal:</span></span>

    - <span data-ttu-id="4d6bd-118">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="4d6bd-118">Document Type - Payment</span></span>
    - <span data-ttu-id="4d6bd-119">Предоплата - да</span><span class="sxs-lookup"><span data-stu-id="4d6bd-119">Prepayment - yes</span></span>
    - <span data-ttu-id="4d6bd-120">Номер документа предоплаты не требуется.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-120">Prepayment Document No is required.</span></span>

3. <span data-ttu-id="4d6bd-121">Выполните учет строк журнала.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-121">Post lines of Journal</span></span>

    <span data-ttu-id="4d6bd-122">Операции с НДС генерируются автоматически в рублях.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-122">Operations with VAT are automatically generated in rubles.</span></span>

4. <span data-ttu-id="4d6bd-123">Создайте и учтите в журнале платежей для налогового органа строку с суммой НДС для предоплаты.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-123">Create and post line in Payment Journal for Tax Authority with VAT Amount of prepayment.</span></span>

5. <span data-ttu-id="4d6bd-124">Выполните отгрузку и учет счета.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-124">Ship and post invoice.</span></span>

6. <span data-ttu-id="4d6bd-125">Создайте строку в журнале платежей</span><span class="sxs-lookup"><span data-stu-id="4d6bd-125">Create a line in Payment Journal</span></span>

    - <span data-ttu-id="4d6bd-126">Тип документа - Платеж</span><span class="sxs-lookup"><span data-stu-id="4d6bd-126">Document Type - Payment</span></span>
    - <span data-ttu-id="4d6bd-127">Номер начального документа - Номер</span><span class="sxs-lookup"><span data-stu-id="4d6bd-127">Initial Document No. - No.</span></span> <span data-ttu-id="4d6bd-128">учтенного счета</span><span class="sxs-lookup"><span data-stu-id="4d6bd-128">of posted invoice</span></span>
    - <span data-ttu-id="4d6bd-129">Примен. к док. - номер - Номер</span><span class="sxs-lookup"><span data-stu-id="4d6bd-129">Applies-to Doc. No. - No.</span></span> <span data-ttu-id="4d6bd-130">учтенного счета</span><span class="sxs-lookup"><span data-stu-id="4d6bd-130">of posted invoice</span></span>

7. <span data-ttu-id="4d6bd-131">Создайте и выполните учет платежа в налоговый орган.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-131">Create and post payment to the Tax Authority.</span></span>
8. <span data-ttu-id="4d6bd-132">Откройте журнал НДС.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-132">Go to VAT Settlement Worksheet.</span></span> <span data-ttu-id="4d6bd-133">Выполните учет НДС (см. [Зачет НДС](Settlement-VAT.md)).</span><span class="sxs-lookup"><span data-stu-id="4d6bd-133">Post VAT (see [Settlement VAT](Settlement-VAT.md)).</span></span>

## <a name="vat-from-vendor-funds"></a><span data-ttu-id="4d6bd-134">НДС из фондов поставщика</span><span class="sxs-lookup"><span data-stu-id="4d6bd-134">VAT from Vendor Funds</span></span>

<span data-ttu-id="4d6bd-135">Заполните поля в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-135">Fill the fields in Vendor Card.</span></span>

1. <span data-ttu-id="4d6bd-136">На вкладке "Договор":</span><span class="sxs-lookup"><span data-stu-id="4d6bd-136">On Agreement tab:</span></span>

    - <span data-ttu-id="4d6bd-137">Учет договоров - обязательно.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-137">Agreement posting - mandatory.</span></span>
    - <span data-ttu-id="4d6bd-138">Номера договоров обязательны.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-138">Agreement Nos is required.</span></span>

2. <span data-ttu-id="4d6bd-139">В карточке договора:</span><span class="sxs-lookup"><span data-stu-id="4d6bd-139">In Agreement card:</span></span>

    - <span data-ttu-id="4d6bd-140">НДС бизнес-группа</span><span class="sxs-lookup"><span data-stu-id="4d6bd-140">VAT Bus. Posting Group</span></span>
    - <span data-ttu-id="4d6bd-141">НДС товарная группа налогового агента</span><span class="sxs-lookup"><span data-stu-id="4d6bd-141">VAT Agent Prod. Posting Group</span></span>
    - <span data-ttu-id="4d6bd-142">Тип источника оплаты НДС - Фонды поставщика</span><span class="sxs-lookup"><span data-stu-id="4d6bd-142">VAT Payment Source Type - Vendor Funds</span></span>

## <a name="prepayment-and-payment-vat"></a><span data-ttu-id="4d6bd-143">Предоплата и оплата НДС</span><span class="sxs-lookup"><span data-stu-id="4d6bd-143">Prepayment and Payment VAT</span></span>

1. <span data-ttu-id="4d6bd-144">Создайте и выпустите счет.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-144">Create and release an invoice.</span></span>

2. <span data-ttu-id="4d6bd-145">Для оплаты в валюте для банка и в рублях для поставщика необходимо создать две строки в **журнале платежей**.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-145">For the payment in the currency for the bank and in rubles for the vendor it is necessary to create two lines in the **payment journal**.</span></span>

    <span data-ttu-id="4d6bd-146">**Для поставщика:**</span><span class="sxs-lookup"><span data-stu-id="4d6bd-146">**For vendor:**</span></span>

        - Posting Date,
        - Document Type - Payment
        - Prepayment - yes
        - Account Type - Vendor
        - Account No.
        - Agreement No.
        - Bal. Account Type - G/L Account
        - Bal. Account - “ ”
        - Currency Code - “ “
        - Prepayment Document No. is required
        - Amount - in rubles

    <span data-ttu-id="4d6bd-147">**Для банка:**</span><span class="sxs-lookup"><span data-stu-id="4d6bd-147">**For Bank:**</span></span>

        - Posting Date,
        - Document Type - Payment
        - Prepayment - yes
        - Account Type - Bank Account
        - Account No.
        - Agreement No.
        - Bal. Account Type -  G/L Account
        - Bal. Account - “ ”
        - Currency Code
        - Amount - in USD/EUR

3. <span data-ttu-id="4d6bd-148">Выполните учет строк журнала.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-148">Post the lines of Journal.</span></span>
4. <span data-ttu-id="4d6bd-149">Выполните отгрузку.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-149">Ship.</span></span>

    <span data-ttu-id="4d6bd-150">Вы можете изменить код валюты и сумму в счете.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-150">You can change the Currency Code and Amount in the Invoice.</span></span>

5. <span data-ttu-id="4d6bd-151">Учет счета.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-151">Post the invoice.</span></span>

6. <span data-ttu-id="4d6bd-152">Примените операцию.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-152">Apply Entry.</span></span>

7. <span data-ttu-id="4d6bd-153">Откройте журнал НДС.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-153">Go to VAT Settlement Worksheet.</span></span> <span data-ttu-id="4d6bd-154">Выполните учет НДС (см. [Зачет НДС](Settlement-VAT.md)).</span><span class="sxs-lookup"><span data-stu-id="4d6bd-154">Post VAT (see [Settlement VAT](Settlement-VAT.md)).</span></span>

    <span data-ttu-id="4d6bd-155">В конце периода будут формироваться операции в результате переоценки задолженности.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-155">At the end of the period will be formed entries as a result of revaluation of debt.</span></span>

8. <span data-ttu-id="4d6bd-156">Создайте строки в журнале платежей и учтите их.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-156">Create and post lines in Payment Journal.</span></span>

    <span data-ttu-id="4d6bd-157">Для оплаты в валюте для банка и в рублях для поставщика необходимо создать две строки в журнале платежей.</span><span class="sxs-lookup"><span data-stu-id="4d6bd-157">For the payment in the currency for the bank and in rubles for the vendor it is necessary to create two lines in the payment journal.</span></span>

    <span data-ttu-id="4d6bd-158">**Для поставщика:**</span><span class="sxs-lookup"><span data-stu-id="4d6bd-158">**For vendor:**</span></span>

        - Posting Date
        - Document Type - Payment
        - Account Type - Vendor
        - Account No.
        - External Document No.
        - Internal Document No.
        - Agreement No.
        - Bal. Account Type - G/L Account
        - Bal. Account - “ ”
        - Currency Code - “ “
        - Prepayment Document No. is required
        - Amount - in rubles

    <span data-ttu-id="4d6bd-159">**Для банка:**</span><span class="sxs-lookup"><span data-stu-id="4d6bd-159">**For Bank:**</span></span>

        - Posting Date,
        - Document Type - Payment
        - Account Type - Bank Account
        - Account No.
        - Agreement No.
        - Bal. Account Type -  G/L Account
        - Bal. Account - “ ”
        - Currency Code
        - Amount - in USD/EUR

## <a name="see-also"></a><span data-ttu-id="4d6bd-160">См. также</span><span class="sxs-lookup"><span data-stu-id="4d6bd-160">See Also</span></span>

[<span data-ttu-id="4d6bd-161">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="4d6bd-161">Russia Local Functionality</span></span>](russia-local-functionality.md)  
