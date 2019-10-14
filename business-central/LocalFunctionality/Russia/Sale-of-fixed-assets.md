---
title: Продажа основных средств в России
description: Российские усовершенствования включают управление продажей или перемещением основных средств.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: a928eed21d3a5df80f86c7ea8e798fb539f1929e
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301188"
---
# <a name="selling-fixed-assets"></a><span data-ttu-id="89980-103">Продажа основных средств</span><span class="sxs-lookup"><span data-stu-id="89980-103">Selling fixed assets</span></span>

<span data-ttu-id="89980-104">Продажа или перемещение основного средства состоит из двух этапов.</span><span class="sxs-lookup"><span data-stu-id="89980-104">A sale or transfer of a fixed asset consists of two stages.</span></span>

## <a name="stage-1-depreciation-of-fixed-assets"></a><span data-ttu-id="89980-105">Этап 1: Аморт. основных средств</span><span class="sxs-lookup"><span data-stu-id="89980-105">Stage 1: Depreciation of fixed assets</span></span>

1. <span data-ttu-id="89980-106">Выберите **Подразделения > Финансовый менеджмент > Основные средства > Журналы ГК для ОС**.</span><span class="sxs-lookup"><span data-stu-id="89980-106">Go to **Departments > Financial management > Fixed Assets > FA G/L Journals**.</span></span>
2. <span data-ttu-id="89980-107">Заполните строки журнала.</span><span class="sxs-lookup"><span data-stu-id="89980-107">Fill the journal lines:</span></span>

| <span data-ttu-id="89980-108">Поле</span><span class="sxs-lookup"><span data-stu-id="89980-108">Field</span></span>                       | <span data-ttu-id="89980-109">Описание</span><span class="sxs-lookup"><span data-stu-id="89980-109">Description</span></span>                                                  |
| --------------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="89980-110">Дата учета</span><span class="sxs-lookup"><span data-stu-id="89980-110">Posting Date</span></span>                | <span data-ttu-id="89980-111">Определяет дату, совпадающую со значением в поле "Дата учета ОС", при учете строки.</span><span class="sxs-lookup"><span data-stu-id="89980-111">Specifies the same date as the FA Posting Date field when the line is posted.</span></span> |
| <span data-ttu-id="89980-112">Тип счета</span><span class="sxs-lookup"><span data-stu-id="89980-112">Account Type</span></span>                | <span data-ttu-id="89980-113">Основное средство</span><span class="sxs-lookup"><span data-stu-id="89980-113">Fixed Asset</span></span>                                                  |
| <span data-ttu-id="89980-114">Номер счета</span><span class="sxs-lookup"><span data-stu-id="89980-114">Account No.</span></span>                 | <span data-ttu-id="89980-115">Код основного средства для амортизации</span><span class="sxs-lookup"><span data-stu-id="89980-115">Fixed asset code to be depreciate</span></span>                            |
| <span data-ttu-id="89980-116">Код книги амортизации</span><span class="sxs-lookup"><span data-stu-id="89980-116">Depreciation Book Code</span></span>      | <span data-ttu-id="89980-117">Определяет код книги амортизации, в которой будет учтена строка.</span><span class="sxs-lookup"><span data-stu-id="89980-117">Specifies the code for the depreciation book to which the line will be posted</span></span> |
| <span data-ttu-id="89980-118">Тип учета ОС</span><span class="sxs-lookup"><span data-stu-id="89980-118">FA Posting Type</span></span>             | <span data-ttu-id="89980-119">Амортизация</span><span class="sxs-lookup"><span data-stu-id="89980-119">Depriciation</span></span>                                                 |
| <span data-ttu-id="89980-120">Сумма</span><span class="sxs-lookup"><span data-stu-id="89980-120">Amount</span></span>                      | <span data-ttu-id="89980-121">Не заполнять</span><span class="sxs-lookup"><span data-stu-id="89980-121">not fill</span></span>                                                     |
| <span data-ttu-id="89980-122">Тип баланс. счета</span><span class="sxs-lookup"><span data-stu-id="89980-122">Bal. Account Type</span></span>           | <span data-ttu-id="89980-123">Счет ГК</span><span class="sxs-lookup"><span data-stu-id="89980-123">G/L Account</span></span>                                                  |
| <span data-ttu-id="89980-124">Номер баланс. счета</span><span class="sxs-lookup"><span data-stu-id="89980-124">Bal.Account No.</span></span>             | <span data-ttu-id="89980-125">Счет ГК для расходов, связанных с продажей основных средств</span><span class="sxs-lookup"><span data-stu-id="89980-125">G/L Account for expenses related to the sale of fixed assets</span></span> |
| <span data-ttu-id="89980-126">Амортизация до даты учета ОС</span><span class="sxs-lookup"><span data-stu-id="89980-126">Depr. until FA Posting Date</span></span> | <span data-ttu-id="89980-127">Выбрано</span><span class="sxs-lookup"><span data-stu-id="89980-127">Selected</span></span>                                                     |

## <a name="stage-2-sale-of-fixed-assets-by-the-sales-account"></a><span data-ttu-id="89980-128">Этап 2: Продажа основных средств по счету продаж</span><span class="sxs-lookup"><span data-stu-id="89980-128">Stage 2: Sale of fixed assets by the sales account</span></span>

1. <span data-ttu-id="89980-129">Выберите **Финансовый менеджмент > Расчеты с клиентами > Счета**</span><span class="sxs-lookup"><span data-stu-id="89980-129">Go to **Financial management > Receivables > Invoices**</span></span>
2. <span data-ttu-id="89980-130">Поля в заголовке документа заполняются так же, как поля заказа на продажу.</span><span class="sxs-lookup"><span data-stu-id="89980-130">The fields in the document header are filled in the same way as the sales order fields.</span></span>
3. <span data-ttu-id="89980-131">Заполните строки:</span><span class="sxs-lookup"><span data-stu-id="89980-131">Fill the lines:</span></span>

| <span data-ttu-id="89980-132">Поле</span><span class="sxs-lookup"><span data-stu-id="89980-132">Field</span></span>      | <span data-ttu-id="89980-133">Описание</span><span class="sxs-lookup"><span data-stu-id="89980-133">Description</span></span>          |
| ---------- | -------------------- |
| <span data-ttu-id="89980-134">Тип</span><span class="sxs-lookup"><span data-stu-id="89980-134">Type</span></span>       | <span data-ttu-id="89980-135">Основное средство</span><span class="sxs-lookup"><span data-stu-id="89980-135">Fixed Asset</span></span>          |
| <span data-ttu-id="89980-136">Номер</span><span class="sxs-lookup"><span data-stu-id="89980-136">No.</span></span>        | <span data-ttu-id="89980-137">Код основного средства</span><span class="sxs-lookup"><span data-stu-id="89980-137">Fixed Asset Code</span></span>     |
| <span data-ttu-id="89980-138">Количество</span><span class="sxs-lookup"><span data-stu-id="89980-138">Quantity</span></span>   | <span data-ttu-id="89980-139">1</span><span class="sxs-lookup"><span data-stu-id="89980-139">1</span></span>                    |
| <span data-ttu-id="89980-140">Цена единицы</span><span class="sxs-lookup"><span data-stu-id="89980-140">Unit Price</span></span> | <span data-ttu-id="89980-141">Цена основного средства</span><span class="sxs-lookup"><span data-stu-id="89980-141">Price of Fixed Asset</span></span> |

4. <span data-ttu-id="89980-142">Учет счета.</span><span class="sxs-lookup"><span data-stu-id="89980-142">Post the invoice.</span></span>

## <a name="see-also"></a><span data-ttu-id="89980-143">См. также</span><span class="sxs-lookup"><span data-stu-id="89980-143">See Also</span></span>

[<span data-ttu-id="89980-144">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="89980-144">Fixed Assets</span></span>](fixed-assets.md)  
