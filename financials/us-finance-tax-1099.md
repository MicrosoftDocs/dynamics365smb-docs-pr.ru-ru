---
title: "Отчетность по зарплате по форме 1099 в США | Документы Майкрософт"
description: "Налоговое ведомств IRS требует налоговую форму 1099 для платежей поставщикам, и вы можете указать, что документ продажи подлежит учету по форме 1099, и задать код 1099 для поставщика."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: local
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: c20c52927aa979e56aeef7975fbcee1564ca4dd7
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="reporting-transactions-as-1099-liable-in-the-us"></a><span data-ttu-id="29d2c-103">Отчетность по транзакциям, подлежащим учету по форме 1099 в США</span><span class="sxs-lookup"><span data-stu-id="29d2c-103">Reporting Transactions as 1099 Liable in the US</span></span>

<span data-ttu-id="29d2c-104">Налоговое ведомство Internal Revenue Service (IRS) требует одну или несколько версий налоговой формы 1099 для платежей поставщикам.</span><span class="sxs-lookup"><span data-stu-id="29d2c-104">The Internal Revenue Service (IRS) requires one or more versions of the 1099 tax form for payments to vendors.</span></span> <span data-ttu-id="29d2c-105">Копии этих форм необходимо отправлять поставщикам ежегодно в последний день января или ранее.</span><span class="sxs-lookup"><span data-stu-id="29d2c-105">Copies of these forms must be sent to vendors annually on or before the last day of January.</span></span> <span data-ttu-id="29d2c-106">В документах покупки можно указать, что он подходит для формы 1099, а также указать код 1099 для поставщика.</span><span class="sxs-lookup"><span data-stu-id="29d2c-106">On your purchase documents, you can specify that the document is 1099 liable, and you can specify the 1099 code for the vendor.</span></span>  

## <a name="1099-codes"></a><span data-ttu-id="29d2c-107">Коды 1099</span><span class="sxs-lookup"><span data-stu-id="29d2c-107">1099 codes</span></span>
<span data-ttu-id="29d2c-108">В [!INCLUDE[d365fin](includes/d365fin_md.md)] самые распространенные коды 1099 уже настроены, чтобы вам было проще создавать обязательные отчеты.</span><span class="sxs-lookup"><span data-stu-id="29d2c-108">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the most common 1099 codes are already set up for you so you are ready to generate the required reports.</span></span> <span data-ttu-id="29d2c-109">Коды определены в окне **Форма IRS 1099**, в котором также можно добавить новые коды 1099.</span><span class="sxs-lookup"><span data-stu-id="29d2c-109">The codes are defined in the **IRS 1099 Form Box** window where you can also add new 1099 codes.</span></span> <span data-ttu-id="29d2c-110">Для каждого подлежащего налогообложению поставщика можно указать соответствующий код 1099 на экспресс-вкладке **Платежи** в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="29d2c-110">For each tax liable vendor, you can then specify the relevant 1099 code on the **Payments** FastTab on the Vendor card.</span></span>  

<span data-ttu-id="29d2c-111">В отчете **Сведения поставщика по форме 1099** можно просмотреть транзакции по форме 1099, оплаченные в течение указанного периода.</span><span class="sxs-lookup"><span data-stu-id="29d2c-111">With the **Vendor 1099 Information** report, you can review 1099 transactions paid during a specified period.</span></span> <span data-ttu-id="29d2c-112">В конце года можно напечатать транзакции по форме 1099 на бланках.</span><span class="sxs-lookup"><span data-stu-id="29d2c-112">At the end of the year, you can print 1099 transactions on preprinted forms.</span></span>  

## <a name="printing-1099-tax-forms"></a><span data-ttu-id="29d2c-113">Печать налоговых форм 1099</span><span class="sxs-lookup"><span data-stu-id="29d2c-113">Printing 1099 tax forms</span></span>
<span data-ttu-id="29d2c-114">В окне **Форма IRS 1099** можно получить доступ к следующим налоговым формам:</span><span class="sxs-lookup"><span data-stu-id="29d2c-114">From the **IRS 1099 Form Box** window, you can access the following tax forms:</span></span>  

* <span data-ttu-id="29d2c-115">Поставщик Div 1099</span><span class="sxs-lookup"><span data-stu-id="29d2c-115">Vendor 1099 Div</span></span>  

  <span data-ttu-id="29d2c-116">Печатается федеральная форма 1099-DIV для дивидендов и распределения.</span><span class="sxs-lookup"><span data-stu-id="29d2c-116">Prints the federal form 1099-DIV for dividends and distribution.</span></span> <span data-ttu-id="29d2c-117">Можно напечатать все или конкретные формы 1099-DIV.</span><span class="sxs-lookup"><span data-stu-id="29d2c-117">You can print all or specific 1099-DIV forms.</span></span> <span data-ttu-id="29d2c-118">В отчете используются коды, которые применяются к полям сумм формы DIV в окне **Форма IRS 1099**.</span><span class="sxs-lookup"><span data-stu-id="29d2c-118">The report uses the codes that apply to the DIV form amount boxes from the **IRS 1099 Form-Box** window.</span></span>  
* <span data-ttu-id="29d2c-119">Поставщик 1099 Int</span><span class="sxs-lookup"><span data-stu-id="29d2c-119">Vendor 1099 Int</span></span>  

  <span data-ttu-id="29d2c-120">Печатается федеральная форма 1099-INT для процентного дохода.</span><span class="sxs-lookup"><span data-stu-id="29d2c-120">Prints the federal form 1099-INT for interest income.</span></span> <span data-ttu-id="29d2c-121">Можно напечатать все или конкретные формы 1099-INT.</span><span class="sxs-lookup"><span data-stu-id="29d2c-121">You can print all or specific 1099-INT forms.</span></span> <span data-ttu-id="29d2c-122">В отчете используются коды, которые применяются к полям сумм формы INT в окне **Форма IRS 1099**.</span><span class="sxs-lookup"><span data-stu-id="29d2c-122">The report uses the codes that apply to the INT form amount boxes from the **IRS 1099 Form-Box** window.</span></span>  
* <span data-ttu-id="29d2c-123">Поставщик 1099 Misc — Прочие доходы</span><span class="sxs-lookup"><span data-stu-id="29d2c-123">Vendor 1099 Misc - Miscellaneous income</span></span>  

  <span data-ttu-id="29d2c-124">Печатается федеральная форма 1099-MISC для прочих доходов.</span><span class="sxs-lookup"><span data-stu-id="29d2c-124">Prints the federal form 1099-MISC for miscellaneous income.</span></span> <span data-ttu-id="29d2c-125">Можно напечатать все или конкретные формы 1099-MISC.</span><span class="sxs-lookup"><span data-stu-id="29d2c-125">You can print all or specific 1099-MISC forms.</span></span> <span data-ttu-id="29d2c-126">В отчете используются коды, которые применяются к полям сумм формы MISC в окне **Форма IRS 1099**.</span><span class="sxs-lookup"><span data-stu-id="29d2c-126">The report uses the codes that apply to the MISC form amount boxes from the **IRS 1099 Form-Box** window.</span></span>  

<span data-ttu-id="29d2c-127">Изменения в законодательстве, влияющие на этот отчет, и данные таблицы обычно обрабатываются обновлениях в конце года.</span><span class="sxs-lookup"><span data-stu-id="29d2c-127">Regulatory changes affecting this report and the table data are generally handled in end-of-year updates.</span></span>
<span data-ttu-id="29d2c-128">Можно выполнить отчет **Сведения поставщика по форме 1099** для просмотра данных перед печатью форм.</span><span class="sxs-lookup"><span data-stu-id="29d2c-128">It may be helpful to run the **Vendor 1099 Information** report to review the data before printing the forms.</span></span>

## <a name="submitting-1099-tax-forms-electronically"></a><span data-ttu-id="29d2c-129">Представление налоговых форм 1099 в электронном виде</span><span class="sxs-lookup"><span data-stu-id="29d2c-129">Submitting 1099 tax forms electronically</span></span>
<span data-ttu-id="29d2c-130">Чтобы предоставить налоговые формы 1099 в электронном виде, используйте отчет **Магнитный носитель поставщика по форме 1099**.</span><span class="sxs-lookup"><span data-stu-id="29d2c-130">To submit the 1099 tax forms electronically, use the **Vendor 1099 Magnetic Media** report.</span></span> <span data-ttu-id="29d2c-131">Определяются формы 1099, которые можно экспортировать.</span><span class="sxs-lookup"><span data-stu-id="29d2c-131">Specifies the 1099 forms that can be exported.</span></span> <span data-ttu-id="29d2c-132">Сведения формы, экспортированные в этом отчете, аналогичны отчетам, по которым печатаются формы 1099, описанные в предыдущем разделе.</span><span class="sxs-lookup"><span data-stu-id="29d2c-132">The form information exported by this report is the same as the reports that print 1099 forms that are described in the previous section.</span></span>  

<span data-ttu-id="29d2c-133">В отчете используются коды, которые применяются к полям сумм формы в окне **Форма IRS 1099**.</span><span class="sxs-lookup"><span data-stu-id="29d2c-133">The report uses the codes that apply to the form amount boxes from the **IRS 1099 Form-Box** window.</span></span> <span data-ttu-id="29d2c-134">Коды сопоставляются с полями формы a макетах файла этого отчета, и поэтому данные таблицы и версия отчета по определенному налоговому году должны быть согласованы.</span><span class="sxs-lookup"><span data-stu-id="29d2c-134">The codes are mapped to the form boxes in the file layouts of this report, therefore the table data and report version for a particular tax year must be in agreement.</span></span> <span data-ttu-id="29d2c-135">Если добавляются пользовательские коды в таблицу, их необходимо сопоставить с полями форм внутри этого объекта.</span><span class="sxs-lookup"><span data-stu-id="29d2c-135">If any custom codes are added to the table these must be mapped to the form boxes inside this object.</span></span>  

<span data-ttu-id="29d2c-136">Изменения в законодательстве, влияющие на этот отчет, и данные таблицы обычно обрабатываются обновлениях в конце года.</span><span class="sxs-lookup"><span data-stu-id="29d2c-136">Regulatory changes affecting this report and the table data are generally handled in end-of-year updates.</span></span>
<span data-ttu-id="29d2c-137">Можно выполнить отчет **Сведения поставщика по форме 1099** для просмотра данных перед созданием электронного файла.</span><span class="sxs-lookup"><span data-stu-id="29d2c-137">It may be helpful to run the **Vendor 1099 Information** report to review the data before generating the electronic file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="29d2c-138">См. также</span><span class="sxs-lookup"><span data-stu-id="29d2c-138">See Also</span></span>
[<span data-ttu-id="29d2c-139">Практическое руководство. Регистрация новых поставщиков</span><span class="sxs-lookup"><span data-stu-id="29d2c-139">How to: Register New Vendors</span></span>](purchasing-how-register-new-vendors.md)  
[<span data-ttu-id="29d2c-140">Практическое руководство. Регистрация покупки</span><span class="sxs-lookup"><span data-stu-id="29d2c-140">How to: Record Purchase</span></span>](purchasing-how-record-purchases.md)  
<span data-ttu-id="29d2c-141">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="29d2c-141">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

