---
title: Налоговый учет в России
description: Российские улучшения включают налоговый учет.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 7422630ca27315c60405b315b55d7046a0cea5bb
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4753217"
---
# <a name="tax-accounting"></a><span data-ttu-id="f3194-103">Налоговый учет</span><span class="sxs-lookup"><span data-stu-id="f3194-103">Tax Accounting</span></span>

<span data-ttu-id="f3194-104">В [!INCLUDE[prod_short](../../includes/prod_short.md)] можно настроить и вести налоговые регистры для отслеживания подлежащих налогообложению прибылей и убытков.</span><span class="sxs-lookup"><span data-stu-id="f3194-104">In [!INCLUDE[prod_short](../../includes/prod_short.md)], you can set up and maintain tax registers to track taxable profits and losses.</span></span> <span data-ttu-id="f3194-105">Это основано на следующих методах налогового учета:</span><span class="sxs-lookup"><span data-stu-id="f3194-105">This is based on the following tax accounting principles:</span></span>

- <span data-ttu-id="f3194-106">Финансовая база данных используется для налогового учета.</span><span class="sxs-lookup"><span data-stu-id="f3194-106">The financial database is used for tax accounting.</span></span>
- <span data-ttu-id="f3194-107">План счетов используется для отслеживания налогооблагаемых прибылей и убытков.</span><span class="sxs-lookup"><span data-stu-id="f3194-107">The chart of accounts is used to track taxable profits and losses.</span></span>
- <span data-ttu-id="f3194-108">Доходы и расходы записываются с использованием отдельных субсчетов и измерений.</span><span class="sxs-lookup"><span data-stu-id="f3194-108">Income and expenses are recorded using separate subaccounts and dimensions.</span></span>
- <span data-ttu-id="f3194-109">Транзакции и расходы основных средств для будущих периодов отслеживаются с использованием книги амортизации для налогового учета.</span><span class="sxs-lookup"><span data-stu-id="f3194-109">Fixed asset transactions and expenses for future periods are tracked using the depreciation book for tax accounting.</span></span>
- <span data-ttu-id="f3194-110">Налоговые регистры группируются и суммируются ежемесячно.</span><span class="sxs-lookup"><span data-stu-id="f3194-110">Tax registers are grouped and totaled monthly.</span></span> <span data-ttu-id="f3194-111">В каждом регистре содержится 12 значений для налогового периода в 12 месяцев.</span><span class="sxs-lookup"><span data-stu-id="f3194-111">Each register has 12 values for a 12 month tax period.</span></span> 

<span data-ttu-id="f3194-112">Поскольку [!INCLUDE[prod_short](../../includes/prod_short.md)] сохраняет историю всех транзакций, подробная информация из транзакций, которая изменяет налогооблагаемую прибыль, автоматически отслеживается.</span><span class="sxs-lookup"><span data-stu-id="f3194-112">Because [!INCLUDE[prod_short](../../includes/prod_short.md)] keeps the history of all transactions, detailed information from a transaction that changes taxable profits is automatically tracked.</span></span> <span data-ttu-id="f3194-113">Собранные сведения отображаются в налоговых регистрах в соответствии с принципами достоверности и законности налога.</span><span class="sxs-lookup"><span data-stu-id="f3194-113">The information collected in tax registers meets the principles of tax reliability and tax validity.</span></span>

## <a name="tax-registers"></a><span data-ttu-id="f3194-114">Налоговые регистры</span><span class="sxs-lookup"><span data-stu-id="f3194-114">Tax Registers</span></span>

<span data-ttu-id="f3194-115">Для отслеживания налогооблагаемых прибылей и убытков используются налоговые регистры двух типов.</span><span class="sxs-lookup"><span data-stu-id="f3194-115">There are two types of tax registers that are used for tracking taxable profits and losses.</span></span> 

| <span data-ttu-id="f3194-116">Тип налогового регистра</span><span class="sxs-lookup"><span data-stu-id="f3194-116">Tax Register Type</span></span>      | <span data-ttu-id="f3194-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f3194-117">Description</span></span>                                                  |
| :--------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="f3194-118">Аналитический налоговый регистр</span><span class="sxs-lookup"><span data-stu-id="f3194-118">Analytic Tax Register</span></span>  | <span data-ttu-id="f3194-119">Аналитический регистр основан на операциях книги для налогооблагаемых транзакций.</span><span class="sxs-lookup"><span data-stu-id="f3194-119">An analytic register is based on ledger entries for taxable transactions.</span></span> <span data-ttu-id="f3194-120">Информация обеспечивает непрерывное отображение в хронологической последовательности бизнес-операций, что позволяет отслеживать налогооблагаемые прибыли и убытки на основе налоговых кодов.</span><span class="sxs-lookup"><span data-stu-id="f3194-120">The information provides a continuous chronological reflection of business operations, which tracks taxable profits and losses based on tax codes.</span></span> |
| <span data-ttu-id="f3194-121">Синтетический налоговый регистр</span><span class="sxs-lookup"><span data-stu-id="f3194-121">Synthetic Tax Register</span></span> | <span data-ttu-id="f3194-122">Синтетический регистр основан на суммарной и расчетной информации из аналитического регистра или другого синтетического регистра.</span><span class="sxs-lookup"><span data-stu-id="f3194-122">A synthetic register is based on summarized and calculated information from an analytic register or another synthetic register.</span></span> |

<span data-ttu-id="f3194-123">Транзакции обрабатываются с помощью определенных методов налогового учета, которые применяются к следующим типам налоговых регистров.</span><span class="sxs-lookup"><span data-stu-id="f3194-123">Transactions are processed using specific tax accounting principles that are applied to the following types of tax registers.</span></span> 

| <span data-ttu-id="f3194-124">Налоговый регистр</span><span class="sxs-lookup"><span data-stu-id="f3194-124">Tax Register</span></span>         | <span data-ttu-id="f3194-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f3194-125">Description</span></span>                                                  |
| :------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="f3194-126">Операция главной книги</span><span class="sxs-lookup"><span data-stu-id="f3194-126">General Ledger Entry</span></span> | <span data-ttu-id="f3194-127">Аналитический регистр основан на операциях транзакций главной книги.</span><span class="sxs-lookup"><span data-stu-id="f3194-127">An analytic register based on general ledger transaction entries.</span></span> |
| <span data-ttu-id="f3194-128">Операция по КП</span><span class="sxs-lookup"><span data-stu-id="f3194-128">CV Entry</span></span>             | <span data-ttu-id="f3194-129">Группа аналитических регистров основана на информации, связанной с обязательствами дебиторов и кредиторов.</span><span class="sxs-lookup"><span data-stu-id="f3194-129">A group of analytic registers based on information associated with debtor or creditor liabilities.</span></span> |
| <span data-ttu-id="f3194-130">Операция ОС</span><span class="sxs-lookup"><span data-stu-id="f3194-130">Fixed Asset Entry</span></span>    | <span data-ttu-id="f3194-131">Группа аналитических регистров основана на налоговых данных для основных средств.</span><span class="sxs-lookup"><span data-stu-id="f3194-131">A group of analytic registers based on tax data for fixed assets.</span></span> <span data-ttu-id="f3194-132">Эта группа создается с использованием книги ОС и книги амортизации для налогового учета, которая не интегрирована с книгой финансового учета.</span><span class="sxs-lookup"><span data-stu-id="f3194-132">This group is created by using a fixed asset ledger and a tax depreciation book that is not integrated with the financial accounting ledger.</span></span> |
| <span data-ttu-id="f3194-133">Операция товара</span><span class="sxs-lookup"><span data-stu-id="f3194-133">Item Entry</span></span>           | <span data-ttu-id="f3194-134">Аналитический регистр основан на учтенных товарных операциях.</span><span class="sxs-lookup"><span data-stu-id="f3194-134">An analytic register based on posted item transactions.</span></span>      |
| <span data-ttu-id="f3194-135">Операция РБП</span><span class="sxs-lookup"><span data-stu-id="f3194-135">Future Expense Entry</span></span> | <span data-ttu-id="f3194-136">Группа аналитических регистров основана на налоговых данных для расходов будущих периодов.</span><span class="sxs-lookup"><span data-stu-id="f3194-136">A group of analytic registers based on tax data for future expenses.</span></span> <span data-ttu-id="f3194-137">Эта группа создается с использованием книги ОС и книги амортизации для налогового учета, которая не интегрирована с книгой финансового учета.</span><span class="sxs-lookup"><span data-stu-id="f3194-137">This group is created by using a fixed asset ledger and a tax depreciation book that is not integrated with the financial accounting ledger.</span></span> |
| <span data-ttu-id="f3194-138">Накопление</span><span class="sxs-lookup"><span data-stu-id="f3194-138">Accumulation</span></span>         | <span data-ttu-id="f3194-139">Синтетический регистр основан на расчетных алгоритмах, определенных при настройке налогового регистра.</span><span class="sxs-lookup"><span data-stu-id="f3194-139">A synthetic register based on calculated algorithms defined during tax register set up.</span></span> |


## <a name="see-also"></a><span data-ttu-id="f3194-140">См. также</span><span class="sxs-lookup"><span data-stu-id="f3194-140">See Also</span></span>

[<span data-ttu-id="f3194-141">Настройка налогового учета</span><span class="sxs-lookup"><span data-stu-id="f3194-141">Set Up Tax Accounting</span></span>](How-to-Set-Up-Tax-Accounting.md)  
[<span data-ttu-id="f3194-142">Налоговые регистры</span><span class="sxs-lookup"><span data-stu-id="f3194-142">Tax Registers</span></span>](Tax-Registers.md)  
[<span data-ttu-id="f3194-143">Расчет налоговых регистров</span><span class="sxs-lookup"><span data-stu-id="f3194-143">Create Tax Registers</span></span>](How-to-Create-Tax-Registers.md)  
[<span data-ttu-id="f3194-144">Настройка секций налогового регистра</span><span class="sxs-lookup"><span data-stu-id="f3194-144">Set Up Tax Register Sections</span></span>](How-to-Set-Up-Tax-Register-Sections.md)  
[<span data-ttu-id="f3194-145">Налоговые разницы</span><span class="sxs-lookup"><span data-stu-id="f3194-145">Tax Differences</span></span>](Tax-Differences.md)  
[<span data-ttu-id="f3194-146">Учет платежей подоходного налога</span><span class="sxs-lookup"><span data-stu-id="f3194-146">Accounting for personal income tax payments</span></span>](Accounting-for-personal-income-tax-payments.md)  
[<span data-ttu-id="f3194-147">Загрузка КЛАДР</span><span class="sxs-lookup"><span data-stu-id="f3194-147">Upload KLADR</span></span>](Upload-KLADR.md)  
