---
title: Отчеты по расчетам с клиентами в России
description: Российские улучшения включают отчеты о расчетах с клиентами.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: e47ec952826fa8108585a683227e94c9aa3ab343
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3919761"
---
# <a name="russian-receivables-reports"></a><span data-ttu-id="da4b2-103">Отчеты по расчетам с клиентами (Россия)</span><span class="sxs-lookup"><span data-stu-id="da4b2-103">Russian Receivables Reports</span></span>

<span data-ttu-id="da4b2-104">Функция отчетов о расчетах с клиентами позволяет создавать оборотную ведомость финансовых операций клиента для финансовых операций финансовых счетов с типом источника "Клиент".</span><span class="sxs-lookup"><span data-stu-id="da4b2-104">The receivables report feature enables you to view the customer general ledger turnover for finance entries of general ledger accounts with the source type Customer.</span></span> <span data-ttu-id="da4b2-105">Доступны также следующие отчеты:</span><span class="sxs-lookup"><span data-stu-id="da4b2-105">The following reports are also provided:</span></span>

- <span data-ttu-id="da4b2-106">Оборотная ведомость клиента по ГК (отчет 12450)</span><span class="sxs-lookup"><span data-stu-id="da4b2-106">Customer General Ledger Turnover (report 12450)</span></span>
- <span data-ttu-id="da4b2-107">Бухг. карточка клиента (отчет 12441)</span><span class="sxs-lookup"><span data-stu-id="da4b2-107">Customer Accounting Card (report 12441)</span></span>
- <span data-ttu-id="da4b2-108">Клиент - оборотная ведомость (отчет 12439)</span><span class="sxs-lookup"><span data-stu-id="da4b2-108">Customer Turnover (report 12439)</span></span>
- <span data-ttu-id="da4b2-109">Оборот по учетной группе клиентов (отчет 12440)</span><span class="sxs-lookup"><span data-stu-id="da4b2-109">Customer Posting Group Turnover (report 12440)</span></span>
- <span data-ttu-id="da4b2-110">Анализ операций клиента (отчет 12442)</span><span class="sxs-lookup"><span data-stu-id="da4b2-110">Customer Entries Analysis (report 12442)</span></span>
- <span data-ttu-id="da4b2-111">Клиент - акт выверки (отчет 14910)</span><span class="sxs-lookup"><span data-stu-id="da4b2-111">Customer Reconciliation Act (report 14910)</span></span>

## <a name="customer-general-ledger-turnover-report-report-12450"></a><span data-ttu-id="da4b2-112">Оборотная ведомость клиента по ГК (отчет 12450)</span><span class="sxs-lookup"><span data-stu-id="da4b2-112">Customer General Ledger Turnover Report (Report 12450)</span></span>

<span data-ttu-id="da4b2-113">Отчет **Оборотная ведомость клиента по ГК** используется для анализа оборотной ведомости, а также для анализа сальдо счета клиента.</span><span class="sxs-lookup"><span data-stu-id="da4b2-113">The **Customer General Ledger Turnover** report is used to analyze the turnover and to analyze customer account balances.</span></span> <span data-ttu-id="da4b2-114">Отчет обычно печатается ежемесячно, но может быть напечатан за любой выбранный период.</span><span class="sxs-lookup"><span data-stu-id="da4b2-114">It is usually printed monthly, but it can be printed for any given period.</span></span>

<span data-ttu-id="da4b2-115">Экспресс-вкладка **Параметры** содержит поля, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="da4b2-115">The **Options** FastTab contains the fields listed in the following table.</span></span>

| <span data-ttu-id="da4b2-116">Поле</span><span class="sxs-lookup"><span data-stu-id="da4b2-116">Field</span></span>                             | <span data-ttu-id="da4b2-117">Описание</span><span class="sxs-lookup"><span data-stu-id="da4b2-117">Description</span></span>                                                  |
| --------------------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="da4b2-118">**Точность округления**</span><span class="sxs-lookup"><span data-stu-id="da4b2-118">**Rounding Precision**</span></span>            | <span data-ttu-id="da4b2-119">Выберите это поле, чтобы выбрать нужную точность округления, например: 0,001; 0,01; 1 или 1000.</span><span class="sxs-lookup"><span data-stu-id="da4b2-119">Select this field to choose the required rounding precision: 0.001, 0.01, 1, or 1000.</span></span> |
| <span data-ttu-id="da4b2-120">**Заменять нулевые значения на пропуски**</span><span class="sxs-lookup"><span data-stu-id="da4b2-120">**Replace zero values by blanks**</span></span> | <span data-ttu-id="da4b2-121">Выберите это поле, чтобы заменять нулевые значения пробелами при печати.</span><span class="sxs-lookup"><span data-stu-id="da4b2-121">Select this field to replace zero values with blanks during printing.</span></span> |
| <span data-ttu-id="da4b2-122">**Пропускать нулевые строки**</span><span class="sxs-lookup"><span data-stu-id="da4b2-122">**Skip zero lines**</span></span>               | <span data-ttu-id="da4b2-123">Выберите это поле, чтобы исключить строки с нулевыми значениями.</span><span class="sxs-lookup"><span data-stu-id="da4b2-123">Select this field to exclude lines with zero values.</span></span>         |
| <span data-ttu-id="da4b2-124">**Печать договоров**</span><span class="sxs-lookup"><span data-stu-id="da4b2-124">**Print Agreements**</span></span>              | <span data-ttu-id="da4b2-125">Если выбрано, все суммы в отчетах будут рассчитываться и показываться в разделе договоров.</span><span class="sxs-lookup"><span data-stu-id="da4b2-125">if it is selected, all amounts in reports will be calculated and shown in the section of agreements.</span></span> |

## <a name="customer-accounting-card-report-report-12441"></a><span data-ttu-id="da4b2-126">Бухг. карточка клиента (отчет 12441)</span><span class="sxs-lookup"><span data-stu-id="da4b2-126">Customer Accounting Card Report (Report 12441)</span></span>

<span data-ttu-id="da4b2-127">В отчете **Бухг. карточка клиента** предоставляются следующие сведения обо всех операциях клиента за определенный период:</span><span class="sxs-lookup"><span data-stu-id="da4b2-127">The **Customer Accounting Card** report provides the following information for all of a customer's entries for a specific period:</span></span>

- <span data-ttu-id="da4b2-128">Начальное сальдо</span><span class="sxs-lookup"><span data-stu-id="da4b2-128">Starting balance</span></span>
- <span data-ttu-id="da4b2-129">Дата учета</span><span class="sxs-lookup"><span data-stu-id="da4b2-129">Posting date</span></span>
- <span data-ttu-id="da4b2-130">Документ Но.</span><span class="sxs-lookup"><span data-stu-id="da4b2-130">Document number</span></span>
- <span data-ttu-id="da4b2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="da4b2-131">Description</span></span>
- <span data-ttu-id="da4b2-132">Оборот по дебету</span><span class="sxs-lookup"><span data-stu-id="da4b2-132">Net change debit</span></span>
- <span data-ttu-id="da4b2-133">Оборот по кредиту</span><span class="sxs-lookup"><span data-stu-id="da4b2-133">Net change credit</span></span>
- <span data-ttu-id="da4b2-134">Тип документа</span><span class="sxs-lookup"><span data-stu-id="da4b2-134">Document type</span></span>
- <span data-ttu-id="da4b2-135">Конечное сальдо</span><span class="sxs-lookup"><span data-stu-id="da4b2-135">Ending balance</span></span>

<span data-ttu-id="da4b2-136">Отчет обычно печатается ежемесячно и на дату инвентаризации, но может быть напечатан за любой выбранный период.</span><span class="sxs-lookup"><span data-stu-id="da4b2-136">It is printed monthly and on the date of inventory, but can be printed for any given period.</span></span>

<span data-ttu-id="da4b2-137">Следующая процедура показывает, как получить доступ к отчету **Бухг. карточка клиента**.</span><span class="sxs-lookup"><span data-stu-id="da4b2-137">The following procedure shows how to access the **Customer Accounting Card** report.</span></span>

1. <span data-ttu-id="da4b2-138">Выберите действие **Финансовый менеджмент**, выберите действие **Расчеты с клиентами**, затем выберите действие **Оборотная ведомость**.</span><span class="sxs-lookup"><span data-stu-id="da4b2-138">Choose the **Financial Management** action, choose the **Receivables** action, and then choose the **Turnover** action.</span></span>
2. <span data-ttu-id="da4b2-139">Выберите действие **Оборотная ведомость клиента по ГК**, выберите действие **Печать**, затем выберите действие **Бухг. карточка клиента**.</span><span class="sxs-lookup"><span data-stu-id="da4b2-139">Choose the **Customer G/L Turnover** action, choose the **Print** action, and then choose the **Customer Accounting Card** action.</span></span>

<span data-ttu-id="da4b2-140">На экспресс-вкладке **Клиент** страницы запроса содержатся те же поля, что и на экспресс-вкладке **Клиент** отчета "Оборотная ведомость клиента по ГК".</span><span class="sxs-lookup"><span data-stu-id="da4b2-140">The **Customer** FastTab of the request page contains the same fields as the **Customer** FastTab of the Customer General Ledger Turnover report.</span></span> <span data-ttu-id="da4b2-141">На экспресс-вкладке **Параметры** можно установить флажок **Новая страница для клиента**, чтобы информация по каждому клиенту была напечатана на отдельном листе.</span><span class="sxs-lookup"><span data-stu-id="da4b2-141">On the **Options** FastTab, you can select the **New page per Customer** field to print the information for each customer on a separate sheet.</span></span>

## <a name="customer-turnover-report-report-12439"></a><span data-ttu-id="da4b2-142">Клиент - оборотная ведомость (отчет 12439)</span><span class="sxs-lookup"><span data-stu-id="da4b2-142">Customer Turnover Report (Report 12439)</span></span>

<span data-ttu-id="da4b2-143">Отчет **Клиент - оборотная ведомость** используется для печати данных об операциях клиента за определенный период.</span><span class="sxs-lookup"><span data-stu-id="da4b2-143">The **Customer Turnover** report is used to print the data about a customer's entries for a specific period.</span></span> <span data-ttu-id="da4b2-144">Он также может быть создан для клиентов по отдельным договорам.</span><span class="sxs-lookup"><span data-stu-id="da4b2-144">It can also be created for customers separately for agreements.</span></span> <span data-ttu-id="da4b2-145">Печатаемые данные включают:</span><span class="sxs-lookup"><span data-stu-id="da4b2-145">The printed data contains the following information:</span></span>

- <span data-ttu-id="da4b2-146">Номер</span><span class="sxs-lookup"><span data-stu-id="da4b2-146">Number</span></span>
- <span data-ttu-id="da4b2-147">Name</span><span class="sxs-lookup"><span data-stu-id="da4b2-147">Name</span></span>
- <span data-ttu-id="da4b2-148">Начальное сальдо (дебет или кредит на начало периода)</span><span class="sxs-lookup"><span data-stu-id="da4b2-148">Starting balance (debit or credit at beginning of the period)</span></span>
- <span data-ttu-id="da4b2-149">Оборот (дебет или кредит)</span><span class="sxs-lookup"><span data-stu-id="da4b2-149">Net change (debit or credit)</span></span>
- <span data-ttu-id="da4b2-150">Конечное сальдо (дебет или кредит на конец периода)</span><span class="sxs-lookup"><span data-stu-id="da4b2-150">Ending balance (debit or credit at end of the period)</span></span>

<span data-ttu-id="da4b2-151">Для доступа к отчету **Клиент - оборотная ведомость**</span><span class="sxs-lookup"><span data-stu-id="da4b2-151">To access the **Customer Turnover** report</span></span>

- <span data-ttu-id="da4b2-152">Выберите действие **Финансовый менеджмент**, выберите действие **Расчеты с клиентами**, выберите действие **Отчеты**, затем выберите действие **Клиент - оборотная ведомость**.</span><span class="sxs-lookup"><span data-stu-id="da4b2-152">Choose the **Financial Management** action, choose the **Receivables** action, choose the **Reports** action, and then choose the **Customer Turnover** action.</span></span>

<span data-ttu-id="da4b2-153">На экспресс-вкладке **Клиент** страницы запроса содержатся те же поля, что и на экспресс-вкладке **Клиент** отчета **Оборотная ведомость клиента по ГК**.</span><span class="sxs-lookup"><span data-stu-id="da4b2-153">The **Customer** FastTab of the request page contains the same fields as the **Customer** FastTab of the **Customer General Ledger Turnover** report.</span></span> 

<span data-ttu-id="da4b2-154">Экспресс-вкладка **Параметры** содержит поля, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="da4b2-154">The **Options** FastTab contains the fields listed in the following table.</span></span>

| <span data-ttu-id="da4b2-155">Поле</span><span class="sxs-lookup"><span data-stu-id="da4b2-155">Field</span></span>                                      | <span data-ttu-id="da4b2-156">Описание</span><span class="sxs-lookup"><span data-stu-id="da4b2-156">Description</span></span>                                                  |
| ------------------------------------------ | ------------------------------------------------------------ |
| <span data-ttu-id="da4b2-157">**Точность округления**</span><span class="sxs-lookup"><span data-stu-id="da4b2-157">**Rounding Precision**</span></span>                     | <span data-ttu-id="da4b2-158">Выберите это поле, чтобы выбрать нужную точность округления, например: 0,001; 0,01; 1 или 1000.</span><span class="sxs-lookup"><span data-stu-id="da4b2-158">Select this field to choose the required rounding precision: 0.001, 0.01, 1, or 1000.</span></span> |
| <span data-ttu-id="da4b2-159">**Заменять нулевые значения на пропуски**</span><span class="sxs-lookup"><span data-stu-id="da4b2-159">**Replace zero values by blanks**</span></span>          | <span data-ttu-id="da4b2-160">Выберите это поле, чтобы заменять нулевые значения пробелами при печати.</span><span class="sxs-lookup"><span data-stu-id="da4b2-160">Select this field to replace zero values with blanks during printing.</span></span> |
| <span data-ttu-id="da4b2-161">**Пропускать счета без оборотов**</span><span class="sxs-lookup"><span data-stu-id="da4b2-161">**Skip accounts without net changes**</span></span>      | <span data-ttu-id="da4b2-162">Выберите это поле, чтобы исключить строки, не имеющие оборота за указанный период.</span><span class="sxs-lookup"><span data-stu-id="da4b2-162">Select this field to exclude lines without net changes within the period.</span></span> |
| <span data-ttu-id="da4b2-163">**Пропускать счета с нулевым конечным сальдо**</span><span class="sxs-lookup"><span data-stu-id="da4b2-163">**Skip accounts with zero ending balance**</span></span> | <span data-ttu-id="da4b2-164">Выберите это поле, чтобы исключить строки с нулевым конечным сальдо на конец периода.</span><span class="sxs-lookup"><span data-stu-id="da4b2-164">Select this field to exclude lines with zero ending balances at the end of the period.</span></span> |
| <span data-ttu-id="da4b2-165">**Пропускать нулевые строки**</span><span class="sxs-lookup"><span data-stu-id="da4b2-165">**Skip zero lines**</span></span>                        | <span data-ttu-id="da4b2-166">Выберите это поле, чтобы исключить строки с нулевыми значениями.</span><span class="sxs-lookup"><span data-stu-id="da4b2-166">Select this field to exclude lines with zero values.</span></span>         |

## <a name="customer-posting-group-turnover-report-report-12440"></a><span data-ttu-id="da4b2-167">Оборот по учетной группе клиентов (отчет 12440)</span><span class="sxs-lookup"><span data-stu-id="da4b2-167">Customer Posting Group Turnover Report (Report 12440)</span></span>

<span data-ttu-id="da4b2-168">Отчет **Оборот по учетной группе клиентов** используется для печати сведений об операциях клиентов, которые собираются для учетных групп клиентов.</span><span class="sxs-lookup"><span data-stu-id="da4b2-168">The **Customer Posting Group Turnover** report is used to print information on the customer's entries that are accumulated in the customer posting groups.</span></span> <span data-ttu-id="da4b2-169">Печатаемые данные включают:</span><span class="sxs-lookup"><span data-stu-id="da4b2-169">The printed data contains the following information:</span></span>

- <span data-ttu-id="da4b2-170">Код учетной группы клиента</span><span class="sxs-lookup"><span data-stu-id="da4b2-170">Customer posting group code</span></span>
- <span data-ttu-id="da4b2-171">Название учетной группы клиента</span><span class="sxs-lookup"><span data-stu-id="da4b2-171">Customer posting group name</span></span>
- <span data-ttu-id="da4b2-172">Начальное сальдо (дебет или кредит)</span><span class="sxs-lookup"><span data-stu-id="da4b2-172">Starting balance (debit or credit)</span></span>
- <span data-ttu-id="da4b2-173">Оборот (дебет или кредит)</span><span class="sxs-lookup"><span data-stu-id="da4b2-173">Net change (debit or credit)</span></span>
- <span data-ttu-id="da4b2-174">Конечное сальдо (дебет или кредит)</span><span class="sxs-lookup"><span data-stu-id="da4b2-174">Ending balance (debit or credit)</span></span>

<span data-ttu-id="da4b2-175">Для доступа к отчету **Оборот по учетной группе клиентов**</span><span class="sxs-lookup"><span data-stu-id="da4b2-175">To access the **Customer Posting Group Turnover** report</span></span>

- <span data-ttu-id="da4b2-176">Выберите действие **Финансовый менеджмент**, выберите действие **Расчеты с клиентами**, выберите действие **Отчеты**, затем выберите действие **Оборот по учетной группе клиентов**.</span><span class="sxs-lookup"><span data-stu-id="da4b2-176">Choose the **Financial Management** action, choose the **Receivables** action, choose the **Reports** action, and then choose the **Customer Posting Group Turnover** action.</span></span>

<span data-ttu-id="da4b2-177">На экспресс-вкладке **Параметры** имеется возможность указать те же параметры форматирования, что и на экспресс-вкладке **Параметры** отчета **Оборотная ведомость клиента по ГК**.</span><span class="sxs-lookup"><span data-stu-id="da4b2-177">On the **Options** FastTab, you can specify the same format options as on the **Options** FastTab of the **Customer General Ledger Turnover** report.</span></span>

## <a name="customer-entries-analysis-report-12442"></a><span data-ttu-id="da4b2-178">Анализ операций клиента (отчет 12442)</span><span class="sxs-lookup"><span data-stu-id="da4b2-178">Customer Entries Analysis (Report 12442)</span></span>

<span data-ttu-id="da4b2-179">В отчете **Анализ операций клиента** указываются обязательства клиента на начало и конец периода, анализ операции и информация об оплате счетов.</span><span class="sxs-lookup"><span data-stu-id="da4b2-179">The **Customer Entries Analysis** report shows the customer's liabilities at the beginning and at the end of the period, entry analysis, and invoice discharging.</span></span> <span data-ttu-id="da4b2-180">Печатаемые данные включают:</span><span class="sxs-lookup"><span data-stu-id="da4b2-180">The printed data contains the following information</span></span>

- <span data-ttu-id="da4b2-181">Дата учета</span><span class="sxs-lookup"><span data-stu-id="da4b2-181">Posting date</span></span>
- <span data-ttu-id="da4b2-182">Документ Но.</span><span class="sxs-lookup"><span data-stu-id="da4b2-182">Document number</span></span>
- <span data-ttu-id="da4b2-183">Название документа</span><span class="sxs-lookup"><span data-stu-id="da4b2-183">Document name</span></span>
- <span data-ttu-id="da4b2-184">Тип (платеж, счет)</span><span class="sxs-lookup"><span data-stu-id="da4b2-184">Type (payment, invoice)</span></span>
- <span data-ttu-id="da4b2-185">Сумма</span><span class="sxs-lookup"><span data-stu-id="da4b2-185">Amount</span></span>
- <span data-ttu-id="da4b2-186">Сумма закрытия</span><span class="sxs-lookup"><span data-stu-id="da4b2-186">Amount closed</span></span>
- <span data-ttu-id="da4b2-187">Дата оплаты</span><span class="sxs-lookup"><span data-stu-id="da4b2-187">Payment date</span></span>

<span data-ttu-id="da4b2-188">В этом отчете отображаются все операции клиента за определенный период.</span><span class="sxs-lookup"><span data-stu-id="da4b2-188">This report shows all the entries of the customer for a certain period.</span></span> <span data-ttu-id="da4b2-189">Анализ данного отчета позволяет определить взаимозависимость счетов и оплаты, а также показывает закрытые операции, счета к оплате, частично оплаченные счета и суммы предоплаты клиентов.</span><span class="sxs-lookup"><span data-stu-id="da4b2-189">The analysis of the report enables you to determine the invoice and payment interdependence, shows closed entries, due invoices, partially discharged invoices, and customer prepayment amounts.</span></span>

<span data-ttu-id="da4b2-190">Для доступа к отчету **Анализ операций клиента**</span><span class="sxs-lookup"><span data-stu-id="da4b2-190">To access the **Customer Entries Analysis** report</span></span>

- <span data-ttu-id="da4b2-191">Выберите действие **Финансовый менеджмент**, выберите действие **Расчеты с клиентами**, выберите действие **Отчеты**, затем выберите действие **Анализ операций клиента**.</span><span class="sxs-lookup"><span data-stu-id="da4b2-191">Choose the **Financial Management** action, choose the **Receivables** action, choose the **Reports** action, and then choose the **Customer Entries Analysis** action.</span></span>

<span data-ttu-id="da4b2-192">На экспресс-вкладке **Клиент** страницы запроса определите номер или диапазон номеров клиентов, в зависимости от того, нужно ли печатать отчет для одного или для диапазона клиентов.</span><span class="sxs-lookup"><span data-stu-id="da4b2-192">On the **Customer** FastTab of the request page, define the customer number or a range of numbers, depending on whether you want to print the report for one customer or for a range of customers.</span></span> <span data-ttu-id="da4b2-193">На экспресс-вкладке **Операция книги клиентов** имеется возможность ввести значение фильтра для одного документа или для диапазона документов.</span><span class="sxs-lookup"><span data-stu-id="da4b2-193">On the **Customer Ledger Entry** FastTab, you can enter a filter value for one document or for a range of documents.</span></span>

<span data-ttu-id="da4b2-194">На экспресс-вкладке **Параметры** имеется возможность указать параметры форматирования, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="da4b2-194">On the **Options** FastTab, you can specify the format options listed in the following table.</span></span>

| <span data-ttu-id="da4b2-195">Параметр</span><span class="sxs-lookup"><span data-stu-id="da4b2-195">Parameter</span></span>                 | <span data-ttu-id="da4b2-196">Описание</span><span class="sxs-lookup"><span data-stu-id="da4b2-196">Description</span></span>                                                  |
| ------------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="da4b2-197">**Дата начала**</span><span class="sxs-lookup"><span data-stu-id="da4b2-197">**Starting Date**</span></span>         | <span data-ttu-id="da4b2-198">Введите дату начала периода.</span><span class="sxs-lookup"><span data-stu-id="da4b2-198">Enter the start date of the period.</span></span>                          |
| <span data-ttu-id="da4b2-199">**Окончание периода**</span><span class="sxs-lookup"><span data-stu-id="da4b2-199">**Ending of period**</span></span>      | <span data-ttu-id="da4b2-200">Введите дату окончания периода.</span><span class="sxs-lookup"><span data-stu-id="da4b2-200">Enter the end date of the period</span></span>                             |
| <span data-ttu-id="da4b2-201">**Валюта отчета**</span><span class="sxs-lookup"><span data-stu-id="da4b2-201">**Report Currency**</span></span>       | <span data-ttu-id="da4b2-202">Введите валюту для использования в отчете.</span><span class="sxs-lookup"><span data-stu-id="da4b2-202">Enter currency that you want to use in the report.</span></span> <span data-ttu-id="da4b2-203">Вы можете выбрать варианты:   -   Местная валюта -   Валюта транзакции</span><span class="sxs-lookup"><span data-stu-id="da4b2-203">You can choose:   -   Local currency -   Transaction currency</span></span> |
| <span data-ttu-id="da4b2-204">**Новая страница для клиента**</span><span class="sxs-lookup"><span data-stu-id="da4b2-204">**New Page For Customer**</span></span> | <span data-ttu-id="da4b2-205">Выберите это поле, чтобы напечатать данные для каждого клиента на отдельной странице.</span><span class="sxs-lookup"><span data-stu-id="da4b2-205">Select this field to print the data for each customer on a separate page.</span></span> |

## <a name="customer---reconciliation-act-report-14910"></a><span data-ttu-id="da4b2-206">Клиент - Акт выверки (отчет 14910)</span><span class="sxs-lookup"><span data-stu-id="da4b2-206">Customer - Reconciliation Act (Report 14910)</span></span>

<span data-ttu-id="da4b2-207">В отчете **Клиент - акт выверки** указываются платежи и обязательства клиента.</span><span class="sxs-lookup"><span data-stu-id="da4b2-207">The **Customer – Reconciliation Act** report shows the payments or liabilities of the customer.</span></span> <span data-ttu-id="da4b2-208">Он используется для взаимной выверки платежей между контрагентами.</span><span class="sxs-lookup"><span data-stu-id="da4b2-208">It is used for the reconciliation of mutual payments of contractors.</span></span>

<span data-ttu-id="da4b2-209">Для доступа к отчету **Клиент - акт выверки** выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="da4b2-209">To access the **Customer – Reconciliation Act** report</span></span>

- <span data-ttu-id="da4b2-210">Выберите действие **Финансовый менеджмент**, выберите действие **Расчеты с клиентами**, выберите действие **Отчеты**, затем выберите действие **Клиент - акт выверки**.</span><span class="sxs-lookup"><span data-stu-id="da4b2-210">Choose the **Financial Management** action, choose the **Receivables** action, choose the **Reports** action, and then choose the **Customer - Reconciliation Act** action.</span></span>

<span data-ttu-id="da4b2-211">Возможные уровни подробностей:</span><span class="sxs-lookup"><span data-stu-id="da4b2-211">The following levels of detail are possible:</span></span>

- <span data-ttu-id="da4b2-212">Полностью</span><span class="sxs-lookup"><span data-stu-id="da4b2-212">Full</span></span>
- <span data-ttu-id="da4b2-213">Частично</span><span class="sxs-lookup"><span data-stu-id="da4b2-213">Partial</span></span>
- <span data-ttu-id="da4b2-214">Нет</span><span class="sxs-lookup"><span data-stu-id="da4b2-214">None</span></span>

### <a name="full-detail"></a><span data-ttu-id="da4b2-215">Все подробности</span><span class="sxs-lookup"><span data-stu-id="da4b2-215">Full Detail</span></span>

<span data-ttu-id="da4b2-216">Если выбран уровень "Полностью", отчет печатает следующие данные для каждого документа за текущий и предыдущий периоды:</span><span class="sxs-lookup"><span data-stu-id="da4b2-216">If Full is selected as the detail level, the report prints the following data for each document for the current and previous periods:</span></span>

- <span data-ttu-id="da4b2-217">Номер документа и номера связанных с ним документов.</span><span class="sxs-lookup"><span data-stu-id="da4b2-217">Document number and numbers of documents connected with it</span></span>
- <span data-ttu-id="da4b2-218">Сальдо для каждого документа (дебет или кредит)</span><span class="sxs-lookup"><span data-stu-id="da4b2-218">The balance on each document (debit or credit)</span></span>
- <span data-ttu-id="da4b2-219">Дата документа</span><span class="sxs-lookup"><span data-stu-id="da4b2-219">Document date</span></span>
- <span data-ttu-id="da4b2-220">Описание</span><span class="sxs-lookup"><span data-stu-id="da4b2-220">Description</span></span>

<span data-ttu-id="da4b2-221">Если флажок **Печать данных контрагента** выбран на экспресс-вкладке **Параметры** страницы запроса, с правой стороны окна (данные клиента) отчета будут напечатаны следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="da4b2-221">The report prints the following information on the right side of the window (customer's data) in case the **Print Contactor Data** check box is selected on the **Options** FastTab of the request page:</span></span>

- <span data-ttu-id="da4b2-222">Сумма документа</span><span class="sxs-lookup"><span data-stu-id="da4b2-222">Document amount</span></span>
- <span data-ttu-id="da4b2-223">Дебет</span><span class="sxs-lookup"><span data-stu-id="da4b2-223">Debit</span></span>
- <span data-ttu-id="da4b2-224">Кредит</span><span class="sxs-lookup"><span data-stu-id="da4b2-224">Credit</span></span>

### <a name="partial-detail"></a><span data-ttu-id="da4b2-225">Частичные подробности</span><span class="sxs-lookup"><span data-stu-id="da4b2-225">Partial Detail</span></span>

<span data-ttu-id="da4b2-226">Если выбран уровень подробностей "Частично", отчет отображает сальдо для каждого документа за текущий и предыдущий периоды, но не отображает связи со счетами, кредит-нотами и оплатами.</span><span class="sxs-lookup"><span data-stu-id="da4b2-226">If Partial Detail is selected as the detail level, the report shows the balance on each document for the current and previous periods, but no connections to the invoices, credit notes, and payments.</span></span>

### <a name="none"></a><span data-ttu-id="da4b2-227">Нет</span><span class="sxs-lookup"><span data-stu-id="da4b2-227">None</span></span>

<span data-ttu-id="da4b2-228">Если выбрано значение "Нет", отчет отображает для каждого клиента начальное сальдо, оборот за период, а также сальдо на конец периода.</span><span class="sxs-lookup"><span data-stu-id="da4b2-228">If None is selected as the detail level, the report shows, for each customer, the balance at the beginning of the period, net changes for the period, and the balance at the end of the period.</span></span> <span data-ttu-id="da4b2-229">Он показывает также сумму обязательств клиента.</span><span class="sxs-lookup"><span data-stu-id="da4b2-229">It also shows the amount of the customer liabilities.</span></span>

<span data-ttu-id="da4b2-230">На экспресс-вкладке **Параметры** имеется возможность указать параметры форматирования, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="da4b2-230">On the **Options** FastTab, you can specify the format options listed in the following table.</span></span>

| <span data-ttu-id="da4b2-231">Параметр</span><span class="sxs-lookup"><span data-stu-id="da4b2-231">Parameter</span></span>                     | <span data-ttu-id="da4b2-232">Описание</span><span class="sxs-lookup"><span data-stu-id="da4b2-232">Description</span></span>                                                  |
| ----------------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="da4b2-233">**Дата начала**</span><span class="sxs-lookup"><span data-stu-id="da4b2-233">**Starting Date**</span></span>             | <span data-ttu-id="da4b2-234">Введите дату начала периода.</span><span class="sxs-lookup"><span data-stu-id="da4b2-234">Enter the start date of the period.</span></span>                          |
| <span data-ttu-id="da4b2-235">**Дата окончания периода**</span><span class="sxs-lookup"><span data-stu-id="da4b2-235">**Ending Date of the Period**</span></span> | <span data-ttu-id="da4b2-236">Введите дату окончания периода.</span><span class="sxs-lookup"><span data-stu-id="da4b2-236">Enter the end date of the period.</span></span>                            |
| <span data-ttu-id="da4b2-237">**Валюта отчета**</span><span class="sxs-lookup"><span data-stu-id="da4b2-237">**Report Currency**</span></span>           | <span data-ttu-id="da4b2-238">Введите валюту для использования в отчете.</span><span class="sxs-lookup"><span data-stu-id="da4b2-238">Enter the currency that you want to use in the report.</span></span> <span data-ttu-id="da4b2-239">Имеется возможность выбрать любую валюту из списка валют.</span><span class="sxs-lookup"><span data-stu-id="da4b2-239">You can choose any currency from the glossary of currencies.</span></span> |
| <span data-ttu-id="da4b2-240">**Подробно**</span><span class="sxs-lookup"><span data-stu-id="da4b2-240">**Detailed**</span></span>                  | <span data-ttu-id="da4b2-241">Выберите один из следующих вариантов:   -   **Полностью** -   **Частично** -   **Нет**</span><span class="sxs-lookup"><span data-stu-id="da4b2-241">Select one of these values:   -   **Full** -   **Partial** -   **None**</span></span> |

## <a name="see-also"></a><span data-ttu-id="da4b2-242">См. также</span><span class="sxs-lookup"><span data-stu-id="da4b2-242">See Also</span></span>

[<span data-ttu-id="da4b2-243">Отчеты о платежах (Россия)</span><span class="sxs-lookup"><span data-stu-id="da4b2-243">Russian Payables Reports</span></span>](Russian-Payables-Reports.md)  
[<span data-ttu-id="da4b2-244">Настройка договоров с клиентами и поставщиками</span><span class="sxs-lookup"><span data-stu-id="da4b2-244">Set Up Customer and Vendor Agreements</span></span>](How-to-Set-Up-Customer-and-Vendor-Agreements.md)  
