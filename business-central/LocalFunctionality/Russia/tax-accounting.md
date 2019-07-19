---
title: Налоговый учет в России
description: Российские улучшения включают налоговый учет.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: c6528f5a8cb496f6b62f58ca4f5733e16b519cfb
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738237"
---
# <a name="tax-accounting"></a><span data-ttu-id="b59d2-103">Налоговый учет</span><span class="sxs-lookup"><span data-stu-id="b59d2-103">Tax Accounting</span></span>

<span data-ttu-id="b59d2-104">В [!INCLUDE[prodshort](../../includes/prodshort.md)] можно настроить и вести налоговые регистры для отслеживания подлежащих налогообложению прибылей и убытков.</span><span class="sxs-lookup"><span data-stu-id="b59d2-104">In [!INCLUDE[prodshort](../../includes/prodshort.md)], you can set up and maintain tax registers to track taxable profits and losses.</span></span> <span data-ttu-id="b59d2-105">Это основано на следующих методах налогового учета:</span><span class="sxs-lookup"><span data-stu-id="b59d2-105">This is based on the following tax accounting principles:</span></span>

- <span data-ttu-id="b59d2-106">Финансовая база данных используется для налогового учета.</span><span class="sxs-lookup"><span data-stu-id="b59d2-106">The financial database is used for tax accounting.</span></span>
- <span data-ttu-id="b59d2-107">План счетов используется для отслеживания налогооблагаемых прибылей и убытков.</span><span class="sxs-lookup"><span data-stu-id="b59d2-107">The chart of accounts is used to track taxable profits and losses.</span></span>
- <span data-ttu-id="b59d2-108">Доходы и расходы записываются с использованием отдельных субсчетов и измерений.</span><span class="sxs-lookup"><span data-stu-id="b59d2-108">Income and expenses are recorded using separate subaccounts and dimensions.</span></span>
- <span data-ttu-id="b59d2-109">Транзакции и расходы основных средств для будущих периодов отслеживаются с использованием книги амортизации для налогового учета.</span><span class="sxs-lookup"><span data-stu-id="b59d2-109">Fixed asset transactions and expenses for future periods are tracked using the depreciation book for tax accounting.</span></span>
- <span data-ttu-id="b59d2-110">Налоговые регистры группируются и суммируются ежемесячно.</span><span class="sxs-lookup"><span data-stu-id="b59d2-110">Tax registers are grouped and totaled monthly.</span></span> <span data-ttu-id="b59d2-111">В каждом регистре содержится 12 значений для налогового периода в 12 месяцев.</span><span class="sxs-lookup"><span data-stu-id="b59d2-111">Each register has 12 values for a 12 month tax period.</span></span> 

<span data-ttu-id="b59d2-112">Поскольку [!INCLUDE[prodshort](../../includes/prodshort.md)] сохраняет историю всех транзакций, подробная информация из транзакций, которая изменяет налогооблагаемую прибыль, автоматически отслеживается.</span><span class="sxs-lookup"><span data-stu-id="b59d2-112">Because [!INCLUDE[prodshort](../../includes/prodshort.md)] keeps the history of all transactions, detailed information from a transaction that changes taxable profits is automatically tracked.</span></span> <span data-ttu-id="b59d2-113">Собранные сведения отображаются в налоговых регистрах в соответствии с принципами достоверности и законности налога.</span><span class="sxs-lookup"><span data-stu-id="b59d2-113">The information collected in tax registers meets the principles of tax reliability and tax validity.</span></span>

## <a name="tax-registers"></a><span data-ttu-id="b59d2-114">Налоговые регистры</span><span class="sxs-lookup"><span data-stu-id="b59d2-114">Tax Registers</span></span>

<span data-ttu-id="b59d2-115">Для отслеживания налогооблагаемых прибылей и убытков используются налоговые регистры двух типов.</span><span class="sxs-lookup"><span data-stu-id="b59d2-115">There are two types of tax registers that are used for tracking taxable profits and losses.</span></span> 

| <span data-ttu-id="b59d2-116">Тип налогового регистра</span><span class="sxs-lookup"><span data-stu-id="b59d2-116">Tax Register Type</span></span>      | <span data-ttu-id="b59d2-117">Описание</span><span class="sxs-lookup"><span data-stu-id="b59d2-117">Description</span></span>                                                  |
| :--------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="b59d2-118">Аналитический налоговый регистр</span><span class="sxs-lookup"><span data-stu-id="b59d2-118">Analytic Tax Register</span></span>  | <span data-ttu-id="b59d2-119">Аналитический регистр основан на операциях книги для налогооблагаемых транзакций.</span><span class="sxs-lookup"><span data-stu-id="b59d2-119">An analytic register is based on ledger entries for taxable transactions.</span></span> <span data-ttu-id="b59d2-120">Информация обеспечивает непрерывное отображение в хронологической последовательности бизнес-операций, что позволяет отслеживать налогооблагаемые прибыли и убытки на основе налоговых кодов.</span><span class="sxs-lookup"><span data-stu-id="b59d2-120">The information provides a continuous chronological reflection of business operations, which tracks taxable profits and losses based on tax codes.</span></span> |
| <span data-ttu-id="b59d2-121">Синтетический налоговый регистр</span><span class="sxs-lookup"><span data-stu-id="b59d2-121">Synthetic Tax Register</span></span> | <span data-ttu-id="b59d2-122">Синтетический регистр основан на суммарной и расчетной информации из аналитического регистра или другого синтетического регистра.</span><span class="sxs-lookup"><span data-stu-id="b59d2-122">A synthetic register is based on summarized and calculated information from an analytic register or another synthetic register.</span></span> |

<span data-ttu-id="b59d2-123">Транзакции обрабатываются с помощью определенных методов налогового учета, которые применяются к следующим типам налоговых регистров.</span><span class="sxs-lookup"><span data-stu-id="b59d2-123">Transactions are processed using specific tax accounting principles that are applied to the following types of tax registers.</span></span> 

| <span data-ttu-id="b59d2-124">Налоговый регистр</span><span class="sxs-lookup"><span data-stu-id="b59d2-124">Tax Register</span></span>         | <span data-ttu-id="b59d2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b59d2-125">Description</span></span>                                                  |
| :------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="b59d2-126">Операция главной книги</span><span class="sxs-lookup"><span data-stu-id="b59d2-126">General Ledger Entry</span></span> | <span data-ttu-id="b59d2-127">Аналитический регистр основан на операциях транзакций главной книги.</span><span class="sxs-lookup"><span data-stu-id="b59d2-127">An analytic register based on general ledger transaction entries.</span></span> |
| <span data-ttu-id="b59d2-128">Операция по КП</span><span class="sxs-lookup"><span data-stu-id="b59d2-128">CV Entry</span></span>             | <span data-ttu-id="b59d2-129">Группа аналитических регистров основана на информации, связанной с обязательствами дебиторов и кредиторов.</span><span class="sxs-lookup"><span data-stu-id="b59d2-129">A group of analytic registers based on information associated with debtor or creditor liabilities.</span></span> |
| <span data-ttu-id="b59d2-130">Операция ОС</span><span class="sxs-lookup"><span data-stu-id="b59d2-130">Fixed Asset Entry</span></span>    | <span data-ttu-id="b59d2-131">Группа аналитических регистров основана на налоговых данных для основных средств.</span><span class="sxs-lookup"><span data-stu-id="b59d2-131">A group of analytic registers based on tax data for fixed assets.</span></span> <span data-ttu-id="b59d2-132">Эта группа создается с использованием книги ОС и книги амортизации для налогового учета, которая не интегрирована с книгой финансового учета.</span><span class="sxs-lookup"><span data-stu-id="b59d2-132">This group is created by using a fixed asset ledger and a tax depreciation book that is not integrated with the financial accounting ledger.</span></span> |
| <span data-ttu-id="b59d2-133">Операция товара</span><span class="sxs-lookup"><span data-stu-id="b59d2-133">Item Entry</span></span>           | <span data-ttu-id="b59d2-134">Аналитический регистр основан на учтенных товарных операциях.</span><span class="sxs-lookup"><span data-stu-id="b59d2-134">An analytic register based on posted item transactions.</span></span>      |
| <span data-ttu-id="b59d2-135">Операция РБП</span><span class="sxs-lookup"><span data-stu-id="b59d2-135">Future Expense Entry</span></span> | <span data-ttu-id="b59d2-136">Группа аналитических регистров основана на налоговых данных для расходов будущих периодов.</span><span class="sxs-lookup"><span data-stu-id="b59d2-136">A group of analytic registers based on tax data for future expenses.</span></span> <span data-ttu-id="b59d2-137">Эта группа создается с использованием книги ОС и книги амортизации для налогового учета, которая не интегрирована с книгой финансового учета.</span><span class="sxs-lookup"><span data-stu-id="b59d2-137">This group is created by using a fixed asset ledger and a tax depreciation book that is not integrated with the financial accounting ledger.</span></span> |
| <span data-ttu-id="b59d2-138">Накопление</span><span class="sxs-lookup"><span data-stu-id="b59d2-138">Accumulation</span></span>         | <span data-ttu-id="b59d2-139">Синтетический регистр основан на расчетных алгоритмах, определенных при настройке налогового регистра.</span><span class="sxs-lookup"><span data-stu-id="b59d2-139">A synthetic register based on calculated algorithms defined during tax register set up.</span></span> |


## <a name="see-also"></a><span data-ttu-id="b59d2-140">См. также</span><span class="sxs-lookup"><span data-stu-id="b59d2-140">See Also</span></span>

[<span data-ttu-id="b59d2-141">Практическое руководство. Настройка налогового учета</span><span class="sxs-lookup"><span data-stu-id="b59d2-141">How to: Set Up Tax Accounting</span></span>](How-to-Set-Up-Tax-Accounting.md)  
[<span data-ttu-id="b59d2-142">Налоговые регистры</span><span class="sxs-lookup"><span data-stu-id="b59d2-142">Tax Registers</span></span>](Tax-Registers.md)  
[<span data-ttu-id="b59d2-143">Практическое руководство. Создание налоговых регистров</span><span class="sxs-lookup"><span data-stu-id="b59d2-143">How to: Create Tax Registers</span></span>](How-to-Create-Tax-Registers.md)  
[<span data-ttu-id="b59d2-144">Практическое руководство. Настройка секций налогового регистра</span><span class="sxs-lookup"><span data-stu-id="b59d2-144">How to: Set Up Tax Register Sections</span></span>](How-to-Set-Up-Tax-Register-Sections.md)  
[<span data-ttu-id="b59d2-145">Налоговые разницы</span><span class="sxs-lookup"><span data-stu-id="b59d2-145">Tax Differences</span></span>](Tax-Differences.md)  
[<span data-ttu-id="b59d2-146">Учет платежей подоходного налога</span><span class="sxs-lookup"><span data-stu-id="b59d2-146">Accounting for personal income tax payments</span></span>](Accounting-for-personal-income-tax-payments.md)  
[<span data-ttu-id="b59d2-147">Загрузка КЛАДР</span><span class="sxs-lookup"><span data-stu-id="b59d2-147">Upload KLADR</span></span>](Upload-KLADR.md)  
