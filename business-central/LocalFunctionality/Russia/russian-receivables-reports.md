---
title: Отчеты по расчетам с клиентами в России
description: Российские улучшения включают отчеты о расчетах с клиентами.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 07d7ab32d4a6d98a63bd4b9f68136598547ad707
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301126"
---
# <a name="russian-receivables-reports"></a><span data-ttu-id="054a0-103">Отчеты по расчетам с клиентами (Россия)</span><span class="sxs-lookup"><span data-stu-id="054a0-103">Russian Receivables Reports</span></span>

<span data-ttu-id="054a0-104">Функция отчетов о расчетах с клиентами позволяет создавать оборотную ведомость финансовых операций клиента для финансовых операций финансовых счетов с типом источника "Клиент".</span><span class="sxs-lookup"><span data-stu-id="054a0-104">The receivables report feature enables you to view the customer general ledger turnover for finance entries of general ledger accounts with the source type Customer.</span></span> <span data-ttu-id="054a0-105">Доступны также следующие отчеты:</span><span class="sxs-lookup"><span data-stu-id="054a0-105">The following reports are also provided:</span></span>

- <span data-ttu-id="054a0-106">Оборотная ведомость клиента по ГК (отчет 12450)</span><span class="sxs-lookup"><span data-stu-id="054a0-106">Customer General Ledger Turnover (report 12450)</span></span>
- <span data-ttu-id="054a0-107">Бухг. карточка клиента (отчет 12441)</span><span class="sxs-lookup"><span data-stu-id="054a0-107">Customer Accounting Card (report 12441)</span></span>
- <span data-ttu-id="054a0-108">Клиент - оборотная ведомость (отчет 12439)</span><span class="sxs-lookup"><span data-stu-id="054a0-108">Customer Turnover (report 12439)</span></span>
- <span data-ttu-id="054a0-109">Оборот по учетной группе клиентов (отчет 12440)</span><span class="sxs-lookup"><span data-stu-id="054a0-109">Customer Posting Group Turnover (report 12440)</span></span>
- <span data-ttu-id="054a0-110">Анализ операций клиента (отчет 12442)</span><span class="sxs-lookup"><span data-stu-id="054a0-110">Customer Entries Analysis (report 12442)</span></span>
- <span data-ttu-id="054a0-111">Клиент - акт выверки (отчет 14910)</span><span class="sxs-lookup"><span data-stu-id="054a0-111">Customer Reconciliation Act (report 14910)</span></span>

## <a name="customer-general-ledger-turnover-report-report-12450"></a><span data-ttu-id="054a0-112">Оборотная ведомость клиента по ГК (отчет 12450)</span><span class="sxs-lookup"><span data-stu-id="054a0-112">Customer General Ledger Turnover Report (Report 12450)</span></span>

<span data-ttu-id="054a0-113">Отчет **Оборотная ведомость клиента по ГК** используется для анализа оборотной ведомости, а также для анализа сальдо счета клиента.</span><span class="sxs-lookup"><span data-stu-id="054a0-113">The **Customer General Ledger Turnover** report is used to analyze the turnover and to analyze customer account balances.</span></span> <span data-ttu-id="054a0-114">Отчет обычно печатается ежемесячно, но может быть напечатан за любой выбранный период.</span><span class="sxs-lookup"><span data-stu-id="054a0-114">It is usually printed monthly, but it can be printed for any given period.</span></span>

<span data-ttu-id="054a0-115">Экспресс-вкладка **Параметры** содержит поля, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="054a0-115">The **Options** FastTab contains the fields listed in the following table.</span></span>

| <span data-ttu-id="054a0-116">Поле</span><span class="sxs-lookup"><span data-stu-id="054a0-116">Field</span></span>                             | <span data-ttu-id="054a0-117">Описание</span><span class="sxs-lookup"><span data-stu-id="054a0-117">Description</span></span>                                                  |
| --------------------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="054a0-118">**Точность округления**</span><span class="sxs-lookup"><span data-stu-id="054a0-118">**Rounding Precision**</span></span>            | <span data-ttu-id="054a0-119">Выберите это поле, чтобы выбрать нужную точность округления, например: 0,001; 0,01; 1 или 1000.</span><span class="sxs-lookup"><span data-stu-id="054a0-119">Select this field to choose the required rounding precision: 0.001, 0.01, 1, or 1000.</span></span> |
| <span data-ttu-id="054a0-120">**Заменять нулевые значения на пропуски**</span><span class="sxs-lookup"><span data-stu-id="054a0-120">**Replace zero values by blanks**</span></span> | <span data-ttu-id="054a0-121">Выберите это поле, чтобы заменять нулевые значения пробелами при печати.</span><span class="sxs-lookup"><span data-stu-id="054a0-121">Select this field to replace zero values with blanks during printing.</span></span> |
| <span data-ttu-id="054a0-122">**Пропускать нулевые строки**</span><span class="sxs-lookup"><span data-stu-id="054a0-122">**Skip zero lines**</span></span>               | <span data-ttu-id="054a0-123">Выберите это поле, чтобы исключить строки с нулевыми значениями.</span><span class="sxs-lookup"><span data-stu-id="054a0-123">Select this field to exclude lines with zero values.</span></span>         |
| <span data-ttu-id="054a0-124">**Печать договоров**</span><span class="sxs-lookup"><span data-stu-id="054a0-124">**Print Agreements**</span></span>              | <span data-ttu-id="054a0-125">Если выбрано, все суммы в отчетах будут рассчитываться и показываться в разделе договоров.</span><span class="sxs-lookup"><span data-stu-id="054a0-125">if it is selected, all amounts in reports will be calculated and shown in the section of agreements.</span></span> |

## <a name="customer-accounting-card-report-report-12441"></a><span data-ttu-id="054a0-126">Бухг. карточка клиента (отчет 12441)</span><span class="sxs-lookup"><span data-stu-id="054a0-126">Customer Accounting Card Report (Report 12441)</span></span>

<span data-ttu-id="054a0-127">В отчете **Бухг. карточка клиента** предоставляются следующие сведения обо всех операциях клиента за определенный период:</span><span class="sxs-lookup"><span data-stu-id="054a0-127">The **Customer Accounting Card** report provides the following information for all of a customer's entries for a specific period:</span></span>

- <span data-ttu-id="054a0-128">Начальное сальдо</span><span class="sxs-lookup"><span data-stu-id="054a0-128">Starting balance</span></span>
- <span data-ttu-id="054a0-129">Дата учета</span><span class="sxs-lookup"><span data-stu-id="054a0-129">Posting date</span></span>
- <span data-ttu-id="054a0-130">Документ Но.</span><span class="sxs-lookup"><span data-stu-id="054a0-130">Document number</span></span>
- <span data-ttu-id="054a0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="054a0-131">Description</span></span>
- <span data-ttu-id="054a0-132">Оборот по дебету</span><span class="sxs-lookup"><span data-stu-id="054a0-132">Net change debit</span></span>
- <span data-ttu-id="054a0-133">Оборот по кредиту</span><span class="sxs-lookup"><span data-stu-id="054a0-133">Net change credit</span></span>
- <span data-ttu-id="054a0-134">Тип документа</span><span class="sxs-lookup"><span data-stu-id="054a0-134">Document type</span></span>
- <span data-ttu-id="054a0-135">Конечное сальдо</span><span class="sxs-lookup"><span data-stu-id="054a0-135">Ending balance</span></span>

<span data-ttu-id="054a0-136">Отчет обычно печатается ежемесячно и на дату инвентаризации, но может быть напечатан за любой выбранный период.</span><span class="sxs-lookup"><span data-stu-id="054a0-136">It is printed monthly and on the date of inventory, but can be printed for any given period.</span></span>

<span data-ttu-id="054a0-137">Следующая процедура показывает, как получить доступ к отчету **Бухг. карточка клиента**.</span><span class="sxs-lookup"><span data-stu-id="054a0-137">The following procedure shows how to access the **Customer Accounting Card** report.</span></span>

1. <span data-ttu-id="054a0-138">Выберите действие **Финансовый менеджмент**, выберите действие **Расчеты с клиентами**, затем выберите действие **Оборотная ведомость**.</span><span class="sxs-lookup"><span data-stu-id="054a0-138">Choose the **Financial Management** action, choose the **Receivables** action, and then choose the **Turnover** action.</span></span>
2. <span data-ttu-id="054a0-139">Выберите действие **Оборотная ведомость клиента по ГК**, выберите действие **Печать**, затем выберите действие **Бухг. карточка клиента**.</span><span class="sxs-lookup"><span data-stu-id="054a0-139">Choose the **Customer G/L Turnover** action, choose the **Print** action, and then choose the **Customer Accounting Card** action.</span></span>

<span data-ttu-id="054a0-140">На экспресс-вкладке **Клиент** страницы запроса содержатся те же поля, что и на экспресс-вкладке **Клиент** отчета "Оборотная ведомость клиента по ГК".</span><span class="sxs-lookup"><span data-stu-id="054a0-140">The **Customer** FastTab of the request page contains the same fields as the **Customer** FastTab of the Customer General Ledger Turnover report.</span></span> <span data-ttu-id="054a0-141">На экспресс-вкладке **Параметры** можно установить флажок **Новая страница для клиента**, чтобы информация по каждому клиенту была напечатана на отдельном листе.</span><span class="sxs-lookup"><span data-stu-id="054a0-141">On the **Options** FastTab, you can select the **New page per Customer** field to print the information for each customer on a separate sheet.</span></span>

## <a name="customer-turnover-report-report-12439"></a><span data-ttu-id="054a0-142">Клиент - оборотная ведомость (отчет 12439)</span><span class="sxs-lookup"><span data-stu-id="054a0-142">Customer Turnover Report (Report 12439)</span></span>

<span data-ttu-id="054a0-143">Отчет **Клиент - оборотная ведомость** используется для печати данных об операциях клиента за определенный период.</span><span class="sxs-lookup"><span data-stu-id="054a0-143">The **Customer Turnover** report is used to print the data about a customer's entries for a specific period.</span></span> <span data-ttu-id="054a0-144">Он также может быть создан для клиентов по отдельным договорам.</span><span class="sxs-lookup"><span data-stu-id="054a0-144">It can also be created for customers separately for agreements.</span></span> <span data-ttu-id="054a0-145">Печатаемые данные включают:</span><span class="sxs-lookup"><span data-stu-id="054a0-145">The printed data contains the following information:</span></span>

- <span data-ttu-id="054a0-146">Номер</span><span class="sxs-lookup"><span data-stu-id="054a0-146">Number</span></span>
- <span data-ttu-id="054a0-147">Name</span><span class="sxs-lookup"><span data-stu-id="054a0-147">Name</span></span>
- <span data-ttu-id="054a0-148">Начальное сальдо (дебет или кредит на начало периода)</span><span class="sxs-lookup"><span data-stu-id="054a0-148">Starting balance (debit or credit at beginning of the period)</span></span>
- <span data-ttu-id="054a0-149">Оборот (дебет или кредит)</span><span class="sxs-lookup"><span data-stu-id="054a0-149">Net change (debit or credit)</span></span>
- <span data-ttu-id="054a0-150">Конечное сальдо (дебет или кредит на конец периода)</span><span class="sxs-lookup"><span data-stu-id="054a0-150">Ending balance (debit or credit at end of the period)</span></span>

<span data-ttu-id="054a0-151">Для доступа к отчету **Клиент - оборотная ведомость**</span><span class="sxs-lookup"><span data-stu-id="054a0-151">To access the **Customer Turnover** report</span></span>

- <span data-ttu-id="054a0-152">Выберите действие **Финансовый менеджмент**, выберите действие **Расчеты с клиентами**, выберите действие **Отчеты**, затем выберите действие **Клиент - оборотная ведомость**.</span><span class="sxs-lookup"><span data-stu-id="054a0-152">Choose the **Financial Management** action, choose the **Receivables** action, choose the **Reports** action, and then choose the **Customer Turnover** action.</span></span>

<span data-ttu-id="054a0-153">На экспресс-вкладке **Клиент** страницы запроса содержатся те же поля, что и на экспресс-вкладке **Клиент** отчета **Оборотная ведомость клиента по ГК**.</span><span class="sxs-lookup"><span data-stu-id="054a0-153">The **Customer** FastTab of the request page contains the same fields as the **Customer** FastTab of the **Customer General Ledger Turnover** report.</span></span> 

<span data-ttu-id="054a0-154">Экспресс-вкладка **Параметры** содержит поля, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="054a0-154">The **Options** FastTab contains the fields listed in the following table.</span></span>

| <span data-ttu-id="054a0-155">Поле</span><span class="sxs-lookup"><span data-stu-id="054a0-155">Field</span></span>                                      | <span data-ttu-id="054a0-156">Описание</span><span class="sxs-lookup"><span data-stu-id="054a0-156">Description</span></span>                                                  |
| ------------------------------------------ | ------------------------------------------------------------ |
| <span data-ttu-id="054a0-157">**Точность округления**</span><span class="sxs-lookup"><span data-stu-id="054a0-157">**Rounding Precision**</span></span>                     | <span data-ttu-id="054a0-158">Выберите это поле, чтобы выбрать нужную точность округления, например: 0,001; 0,01; 1 или 1000.</span><span class="sxs-lookup"><span data-stu-id="054a0-158">Select this field to choose the required rounding precision: 0.001, 0.01, 1, or 1000.</span></span> |
| <span data-ttu-id="054a0-159">**Заменять нулевые значения на пропуски**</span><span class="sxs-lookup"><span data-stu-id="054a0-159">**Replace zero values by blanks**</span></span>          | <span data-ttu-id="054a0-160">Выберите это поле, чтобы заменять нулевые значения пробелами при печати.</span><span class="sxs-lookup"><span data-stu-id="054a0-160">Select this field to replace zero values with blanks during printing.</span></span> |
| <span data-ttu-id="054a0-161">**Пропускать счета без оборотов**</span><span class="sxs-lookup"><span data-stu-id="054a0-161">**Skip accounts without net changes**</span></span>      | <span data-ttu-id="054a0-162">Выберите это поле, чтобы исключить строки, не имеющие оборота за указанный период.</span><span class="sxs-lookup"><span data-stu-id="054a0-162">Select this field to exclude lines without net changes within the period.</span></span> |
| <span data-ttu-id="054a0-163">**Пропускать счета с нулевым конечным сальдо**</span><span class="sxs-lookup"><span data-stu-id="054a0-163">**Skip accounts with zero ending balance**</span></span> | <span data-ttu-id="054a0-164">Выберите это поле, чтобы исключить строки с нулевым конечным сальдо на конец периода.</span><span class="sxs-lookup"><span data-stu-id="054a0-164">Select this field to exclude lines with zero ending balances at the end of the period.</span></span> |
| <span data-ttu-id="054a0-165">**Пропускать нулевые строки**</span><span class="sxs-lookup"><span data-stu-id="054a0-165">**Skip zero lines**</span></span>                        | <span data-ttu-id="054a0-166">Выберите это поле, чтобы исключить строки с нулевыми значениями.</span><span class="sxs-lookup"><span data-stu-id="054a0-166">Select this field to exclude lines with zero values.</span></span>         |

## <a name="customer-posting-group-turnover-report-report-12440"></a><span data-ttu-id="054a0-167">Оборот по учетной группе клиентов (отчет 12440)</span><span class="sxs-lookup"><span data-stu-id="054a0-167">Customer Posting Group Turnover Report (Report 12440)</span></span>

<span data-ttu-id="054a0-168">Отчет **Оборот по учетной группе клиентов** используется для печати сведений об операциях клиентов, которые собираются для учетных групп клиентов.</span><span class="sxs-lookup"><span data-stu-id="054a0-168">The **Customer Posting Group Turnover** report is used to print information on the customer's entries that are accumulated in the customer posting groups.</span></span> <span data-ttu-id="054a0-169">Печатаемые данные включают:</span><span class="sxs-lookup"><span data-stu-id="054a0-169">The printed data contains the following information:</span></span>

- <span data-ttu-id="054a0-170">Код учетной группы клиента</span><span class="sxs-lookup"><span data-stu-id="054a0-170">Customer posting group code</span></span>
- <span data-ttu-id="054a0-171">Название учетной группы клиента</span><span class="sxs-lookup"><span data-stu-id="054a0-171">Customer posting group name</span></span>
- <span data-ttu-id="054a0-172">Начальное сальдо (дебет или кредит)</span><span class="sxs-lookup"><span data-stu-id="054a0-172">Starting balance (debit or credit)</span></span>
- <span data-ttu-id="054a0-173">Оборот (дебет или кредит)</span><span class="sxs-lookup"><span data-stu-id="054a0-173">Net change (debit or credit)</span></span>
- <span data-ttu-id="054a0-174">Конечное сальдо (дебет или кредит)</span><span class="sxs-lookup"><span data-stu-id="054a0-174">Ending balance (debit or credit)</span></span>

<span data-ttu-id="054a0-175">Для доступа к отчету **Оборот по учетной группе клиентов**</span><span class="sxs-lookup"><span data-stu-id="054a0-175">To access the **Customer Posting Group Turnover** report</span></span>

- <span data-ttu-id="054a0-176">Выберите действие **Финансовый менеджмент**, выберите действие **Расчеты с клиентами**, выберите действие **Отчеты**, затем выберите действие **Оборот по учетной группе клиентов**.</span><span class="sxs-lookup"><span data-stu-id="054a0-176">Choose the **Financial Management** action, choose the **Receivables** action, choose the **Reports** action, and then choose the **Customer Posting Group Turnover** action.</span></span>

<span data-ttu-id="054a0-177">На экспресс-вкладке **Параметры** имеется возможность указать те же параметры форматирования, что и на экспресс-вкладке **Параметры** отчета **Оборотная ведомость клиента по ГК**.</span><span class="sxs-lookup"><span data-stu-id="054a0-177">On the **Options** FastTab, you can specify the same format options as on the **Options** FastTab of the **Customer General Ledger Turnover** report.</span></span>

## <a name="customer-entries-analysis-report-12442"></a><span data-ttu-id="054a0-178">Анализ операций клиента (отчет 12442)</span><span class="sxs-lookup"><span data-stu-id="054a0-178">Customer Entries Analysis (Report 12442)</span></span>

<span data-ttu-id="054a0-179">В отчете **Анализ операций клиента** указываются обязательства клиента на начало и конец периода, анализ операции и информация об оплате счетов.</span><span class="sxs-lookup"><span data-stu-id="054a0-179">The **Customer Entries Analysis** report shows the customer's liabilities at the beginning and at the end of the period, entry analysis, and invoice discharging.</span></span> <span data-ttu-id="054a0-180">Печатаемые данные включают:</span><span class="sxs-lookup"><span data-stu-id="054a0-180">The printed data contains the following information</span></span>

- <span data-ttu-id="054a0-181">Дата учета</span><span class="sxs-lookup"><span data-stu-id="054a0-181">Posting date</span></span>
- <span data-ttu-id="054a0-182">Документ Но.</span><span class="sxs-lookup"><span data-stu-id="054a0-182">Document number</span></span>
- <span data-ttu-id="054a0-183">Название документа</span><span class="sxs-lookup"><span data-stu-id="054a0-183">Document name</span></span>
- <span data-ttu-id="054a0-184">Тип (платеж, счет)</span><span class="sxs-lookup"><span data-stu-id="054a0-184">Type (payment, invoice)</span></span>
- <span data-ttu-id="054a0-185">Сумма</span><span class="sxs-lookup"><span data-stu-id="054a0-185">Amount</span></span>
- <span data-ttu-id="054a0-186">Сумма закрытия</span><span class="sxs-lookup"><span data-stu-id="054a0-186">Amount closed</span></span>
- <span data-ttu-id="054a0-187">Дата оплаты</span><span class="sxs-lookup"><span data-stu-id="054a0-187">Payment date</span></span>

<span data-ttu-id="054a0-188">В этом отчете отображаются все операции клиента за определенный период.</span><span class="sxs-lookup"><span data-stu-id="054a0-188">This report shows all the entries of the customer for a certain period.</span></span> <span data-ttu-id="054a0-189">Анализ данного отчета позволяет определить взаимозависимость счетов и оплаты, а также показывает закрытые операции, счета к оплате, частично оплаченные счета и суммы предоплаты клиентов.</span><span class="sxs-lookup"><span data-stu-id="054a0-189">The analysis of the report enables you to determine the invoice and payment interdependence, shows closed entries, due invoices, partially discharged invoices, and customer prepayment amounts.</span></span>

<span data-ttu-id="054a0-190">Для доступа к отчету **Анализ операций клиента**</span><span class="sxs-lookup"><span data-stu-id="054a0-190">To access the **Customer Entries Analysis** report</span></span>

- <span data-ttu-id="054a0-191">Выберите действие **Финансовый менеджмент**, выберите действие **Расчеты с клиентами**, выберите действие **Отчеты**, затем выберите действие **Анализ операций клиента**.</span><span class="sxs-lookup"><span data-stu-id="054a0-191">Choose the **Financial Management** action, choose the **Receivables** action, choose the **Reports** action, and then choose the **Customer Entries Analysis** action.</span></span>

<span data-ttu-id="054a0-192">На экспресс-вкладке **Клиент** страницы запроса определите номер или диапазон номеров клиентов, в зависимости от того, нужно ли печатать отчет для одного или для диапазона клиентов.</span><span class="sxs-lookup"><span data-stu-id="054a0-192">On the **Customer** FastTab of the request page, define the customer number or a range of numbers, depending on whether you want to print the report for one customer or for a range of customers.</span></span> <span data-ttu-id="054a0-193">На экспресс-вкладке **Операция книги клиентов** имеется возможность ввести значение фильтра для одного документа или для диапазона документов.</span><span class="sxs-lookup"><span data-stu-id="054a0-193">On the **Customer Ledger Entry** FastTab, you can enter a filter value for one document or for a range of documents.</span></span>

<span data-ttu-id="054a0-194">На экспресс-вкладке **Параметры** имеется возможность указать параметры форматирования, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="054a0-194">On the **Options** FastTab, you can specify the format options listed in the following table.</span></span>

| <span data-ttu-id="054a0-195">Параметр</span><span class="sxs-lookup"><span data-stu-id="054a0-195">Parameter</span></span>                 | <span data-ttu-id="054a0-196">Описание</span><span class="sxs-lookup"><span data-stu-id="054a0-196">Description</span></span>                                                  |
| ------------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="054a0-197">**Дата начала**</span><span class="sxs-lookup"><span data-stu-id="054a0-197">**Starting Date**</span></span>         | <span data-ttu-id="054a0-198">Введите дату начала периода.</span><span class="sxs-lookup"><span data-stu-id="054a0-198">Enter the start date of the period.</span></span>                          |
| <span data-ttu-id="054a0-199">**Окончание периода**</span><span class="sxs-lookup"><span data-stu-id="054a0-199">**Ending of period**</span></span>      | <span data-ttu-id="054a0-200">Введите дату окончания периода.</span><span class="sxs-lookup"><span data-stu-id="054a0-200">Enter the end date of the period</span></span>                             |
| <span data-ttu-id="054a0-201">**Валюта отчета**</span><span class="sxs-lookup"><span data-stu-id="054a0-201">**Report Currency**</span></span>       | <span data-ttu-id="054a0-202">Введите валюту для использования в отчете.</span><span class="sxs-lookup"><span data-stu-id="054a0-202">Enter currency that you want to use in the report.</span></span> <span data-ttu-id="054a0-203">Можно выбрать следующие варианты:   -   Местная валюта -   Валюта транзакции</span><span class="sxs-lookup"><span data-stu-id="054a0-203">You can choose:   -   Local currency -   Transaction currency</span></span> |
| <span data-ttu-id="054a0-204">**Новая страница для клиента**</span><span class="sxs-lookup"><span data-stu-id="054a0-204">**New Page For Customer**</span></span> | <span data-ttu-id="054a0-205">Выберите это поле, чтобы напечатать данные для каждого клиента на отдельной странице.</span><span class="sxs-lookup"><span data-stu-id="054a0-205">Select this field to print the data for each customer on a separate page.</span></span> |

## <a name="customer---reconciliation-act-report-14910"></a><span data-ttu-id="054a0-206">Клиент - Акт выверки (отчет 14910)</span><span class="sxs-lookup"><span data-stu-id="054a0-206">Customer - Reconciliation Act (Report 14910)</span></span>

<span data-ttu-id="054a0-207">В отчете **Клиент - акт выверки** указываются платежи и обязательства клиента.</span><span class="sxs-lookup"><span data-stu-id="054a0-207">The **Customer – Reconciliation Act** report shows the payments or liabilities of the customer.</span></span> <span data-ttu-id="054a0-208">Он используется для взаимной выверки платежей между контрагентами.</span><span class="sxs-lookup"><span data-stu-id="054a0-208">It is used for the reconciliation of mutual payments of contractors.</span></span>

<span data-ttu-id="054a0-209">Для доступа к отчету **Клиент - акт выверки** выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="054a0-209">To access the **Customer – Reconciliation Act** report</span></span>

- <span data-ttu-id="054a0-210">Выберите действие **Финансовый менеджмент**, выберите действие **Расчеты с клиентами**, выберите действие **Отчеты**, затем выберите действие **Клиент - акт выверки**.</span><span class="sxs-lookup"><span data-stu-id="054a0-210">Choose the **Financial Management** action, choose the **Receivables** action, choose the **Reports** action, and then choose the **Customer - Reconciliation Act** action.</span></span>

<span data-ttu-id="054a0-211">Возможные уровни подробностей:</span><span class="sxs-lookup"><span data-stu-id="054a0-211">The following levels of detail are possible:</span></span>

- <span data-ttu-id="054a0-212">Полностью</span><span class="sxs-lookup"><span data-stu-id="054a0-212">Full</span></span>
- <span data-ttu-id="054a0-213">Частично</span><span class="sxs-lookup"><span data-stu-id="054a0-213">Partial</span></span>
- <span data-ttu-id="054a0-214">Нет</span><span class="sxs-lookup"><span data-stu-id="054a0-214">None</span></span>

### <a name="full-detail"></a><span data-ttu-id="054a0-215">Все подробности</span><span class="sxs-lookup"><span data-stu-id="054a0-215">Full Detail</span></span>

<span data-ttu-id="054a0-216">Если выбран уровень "Полностью", отчет печатает следующие данные для каждого документа за текущий и предыдущий периоды:</span><span class="sxs-lookup"><span data-stu-id="054a0-216">If Full is selected as the detail level, the report prints the following data for each document for the current and previous periods:</span></span>

- <span data-ttu-id="054a0-217">Номер документа и номера связанных с ним документов.</span><span class="sxs-lookup"><span data-stu-id="054a0-217">Document number and numbers of documents connected with it</span></span>
- <span data-ttu-id="054a0-218">Сальдо для каждого документа (дебет или кредит)</span><span class="sxs-lookup"><span data-stu-id="054a0-218">The balance on each document (debit or credit)</span></span>
- <span data-ttu-id="054a0-219">Дата документа</span><span class="sxs-lookup"><span data-stu-id="054a0-219">Document date</span></span>
- <span data-ttu-id="054a0-220">Описание</span><span class="sxs-lookup"><span data-stu-id="054a0-220">Description</span></span>

<span data-ttu-id="054a0-221">Если флажок **Печать данных контрагента** выбран на экспресс-вкладке **Параметры** страницы запроса, с правой стороны окна (данные клиента) отчета будут напечатаны следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="054a0-221">The report prints the following information on the right side of the window (customer's data) in case the **Print Contactor Data** check box is selected on the **Options** FastTab of the request page:</span></span>

- <span data-ttu-id="054a0-222">Сумма документа</span><span class="sxs-lookup"><span data-stu-id="054a0-222">Document amount</span></span>
- <span data-ttu-id="054a0-223">Дебет</span><span class="sxs-lookup"><span data-stu-id="054a0-223">Debit</span></span>
- <span data-ttu-id="054a0-224">Кредит</span><span class="sxs-lookup"><span data-stu-id="054a0-224">Credit</span></span>

### <a name="partial-detail"></a><span data-ttu-id="054a0-225">Частичные подробности</span><span class="sxs-lookup"><span data-stu-id="054a0-225">Partial Detail</span></span>

<span data-ttu-id="054a0-226">Если выбран уровень подробностей "Частично", отчет отображает сальдо для каждого документа за текущий и предыдущий периоды, но не отображает связи со счетами, кредит-нотами и оплатами.</span><span class="sxs-lookup"><span data-stu-id="054a0-226">If Partial Detail is selected as the detail level, the report shows the balance on each document for the current and previous periods, but no connections to the invoices, credit notes, and payments.</span></span>

### <a name="none"></a><span data-ttu-id="054a0-227">Нет</span><span class="sxs-lookup"><span data-stu-id="054a0-227">None</span></span>

<span data-ttu-id="054a0-228">Если выбрано значение "Нет", отчет отображает для каждого клиента начальное сальдо, оборот за период, а также сальдо на конец периода.</span><span class="sxs-lookup"><span data-stu-id="054a0-228">If None is selected as the detail level, the report shows, for each customer, the balance at the beginning of the period, net changes for the period, and the balance at the end of the period.</span></span> <span data-ttu-id="054a0-229">Он показывает также сумму обязательств клиента.</span><span class="sxs-lookup"><span data-stu-id="054a0-229">It also shows the amount of the customer liabilities.</span></span>

<span data-ttu-id="054a0-230">На экспресс-вкладке **Параметры** имеется возможность указать параметры форматирования, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="054a0-230">On the **Options** FastTab, you can specify the format options listed in the following table.</span></span>

| <span data-ttu-id="054a0-231">Параметр</span><span class="sxs-lookup"><span data-stu-id="054a0-231">Parameter</span></span>                     | <span data-ttu-id="054a0-232">Описание</span><span class="sxs-lookup"><span data-stu-id="054a0-232">Description</span></span>                                                  |
| ----------------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="054a0-233">**Дата начала**</span><span class="sxs-lookup"><span data-stu-id="054a0-233">**Starting Date**</span></span>             | <span data-ttu-id="054a0-234">Введите дату начала периода.</span><span class="sxs-lookup"><span data-stu-id="054a0-234">Enter the start date of the period.</span></span>                          |
| <span data-ttu-id="054a0-235">**Дата окончания периода**</span><span class="sxs-lookup"><span data-stu-id="054a0-235">**Ending Date of the Period**</span></span> | <span data-ttu-id="054a0-236">Введите дату окончания периода.</span><span class="sxs-lookup"><span data-stu-id="054a0-236">Enter the end date of the period.</span></span>                            |
| <span data-ttu-id="054a0-237">**Валюта отчета**</span><span class="sxs-lookup"><span data-stu-id="054a0-237">**Report Currency**</span></span>           | <span data-ttu-id="054a0-238">Введите валюту для использования в отчете.</span><span class="sxs-lookup"><span data-stu-id="054a0-238">Enter the currency that you want to use in the report.</span></span> <span data-ttu-id="054a0-239">Имеется возможность выбрать любую валюту из списка валют.</span><span class="sxs-lookup"><span data-stu-id="054a0-239">You can choose any currency from the glossary of currencies.</span></span> |
| <span data-ttu-id="054a0-240">**Подробно**</span><span class="sxs-lookup"><span data-stu-id="054a0-240">**Detailed**</span></span>                  | <span data-ttu-id="054a0-241">Выберите один из следующих вариантов:   -   **Все** -   **Частично** -   **Нет**</span><span class="sxs-lookup"><span data-stu-id="054a0-241">Select one of these values:   -   **Full** -   **Partial** -   **None**</span></span> |

## <a name="see-also"></a><span data-ttu-id="054a0-242">См. также</span><span class="sxs-lookup"><span data-stu-id="054a0-242">See Also</span></span>

[<span data-ttu-id="054a0-243">Отчеты о платежах (Россия)</span><span class="sxs-lookup"><span data-stu-id="054a0-243">Russian Payables Reports</span></span>](Russian-Payables-Reports.md)  
[<span data-ttu-id="054a0-244">Практическое руководство. Настройка договоров с клиентами и поставщиками</span><span class="sxs-lookup"><span data-stu-id="054a0-244">How to: Set Up Customer and Vendor Agreements</span></span>](How-to-Set-Up-Customer-and-Vendor-Agreements.md)  
