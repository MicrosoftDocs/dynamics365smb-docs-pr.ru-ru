---
title: "Определение макета чека | Документы Майкрософт"
description: "Вы можете разрабатывать и печатать чеки в различных форматах, чтобы они соответствовали определенным стандартам."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 06/15/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: a2db2860846cd9b8010222faf580f0c9889e39a4
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017


---
# <a name="how-to-define-check-layouts"></a><span data-ttu-id="631ae-103">Практическое руководство. Определение макетов платежных документов</span><span class="sxs-lookup"><span data-stu-id="631ae-103">How to: Define Check Layouts</span></span>
<span data-ttu-id="631ae-104">Вы можете разработать платежные документы в соответствии со стандартами, установленными местными органами власти.</span><span class="sxs-lookup"><span data-stu-id="631ae-104">You can design your checks to conform with the standards set by the local authorities.</span></span> <span data-ttu-id="631ae-105">Изображения платежных документов можно печатать на английском, французском или испанском языке.</span><span class="sxs-lookup"><span data-stu-id="631ae-105">Check images can be printed in English, French, or Spanish.</span></span>

<span data-ttu-id="631ae-106">Платежные документы разрабатываются для печати в форматах изображений платежных документов США и Канады в формате "платежный документ-бланк-платежный документ" или "бланк-бланк-платежный документ".</span><span class="sxs-lookup"><span data-stu-id="631ae-106">Checks are designed to print in both the United States and Canadian check image formats in either a check-stub-check format or a stub-stub-check format.</span></span>

## <a name="to-define-check-layouts"></a><span data-ttu-id="631ae-107">Определение макетов платежных документов</span><span class="sxs-lookup"><span data-stu-id="631ae-107">To define check layouts</span></span>
1. <span data-ttu-id="631ae-108">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Выбор отчета - банковский счет**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="631ae-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Report Selections Bank Account**, and then choose the related link.</span></span>
2. <span data-ttu-id="631ae-109">В окне **Выбор отчета - банковский счет**</span><span class="sxs-lookup"><span data-stu-id="631ae-109">In the **Report Selection - Bank Acc.**</span></span> <span data-ttu-id="631ae-110">в поле **Использование** выберите **Платежный документ**.</span><span class="sxs-lookup"><span data-stu-id="631ae-110">window, in the **Usage** field, select **Check**.</span></span>
3. <span data-ttu-id="631ae-111">Выберите один из следующих кодов отчетов.</span><span class="sxs-lookup"><span data-stu-id="631ae-111">Select one of the following report IDs.</span></span>

| <span data-ttu-id="631ae-112">Код отчета</span><span class="sxs-lookup"><span data-stu-id="631ae-112">Report ID</span></span> | <span data-ttu-id="631ae-113">Название отчета</span><span class="sxs-lookup"><span data-stu-id="631ae-113">Report Name</span></span> | <span data-ttu-id="631ae-114">Описание</span><span class="sxs-lookup"><span data-stu-id="631ae-114">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="631ae-115">1401</span><span class="sxs-lookup"><span data-stu-id="631ae-115">1401</span></span> |<span data-ttu-id="631ae-116">Платежный документ</span><span class="sxs-lookup"><span data-stu-id="631ae-116">Check</span></span> |<span data-ttu-id="631ae-117">Это отчет по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="631ae-117">This is the default report.</span></span> |
| <span data-ttu-id="631ae-118">10401</span><span class="sxs-lookup"><span data-stu-id="631ae-118">10401</span></span> |<span data-ttu-id="631ae-119">Платежный документ (Бланк/Бланк/Платежный документ)</span><span class="sxs-lookup"><span data-stu-id="631ae-119">Check (Stub/Stub/Check)</span></span> |<span data-ttu-id="631ae-120">Этот отчет предназначен для печати платежных документов в формате "бланк/бланк/платежный документ".</span><span class="sxs-lookup"><span data-stu-id="631ae-120">This report is designed to print checks in a stub/stub/check format.</span></span> |
| <span data-ttu-id="631ae-121">10411</span><span class="sxs-lookup"><span data-stu-id="631ae-121">10411</span></span> |<span data-ttu-id="631ae-122">Платежный документ (Бланк/Платежный документ/Бланк)</span><span class="sxs-lookup"><span data-stu-id="631ae-122">Check (Stub/Check/Stub)</span></span> |<span data-ttu-id="631ae-123">Этот отчет предназначен для печати платежных документов в формате "платежный документ/бланк/платежный документ".</span><span class="sxs-lookup"><span data-stu-id="631ae-123">This report is designed to print checks in a check/stub/check format.</span></span> |

<span data-ttu-id="631ae-124">После настройки макетов платежных документов их можно распечатывать из окна **Журнал платежей**.</span><span class="sxs-lookup"><span data-stu-id="631ae-124">When you have set up check layouts, you can print checks from the **Payment Journal** window.</span></span> <span data-ttu-id="631ae-125">Дополнительные сведения см. в разделе [Практическое руководство. Работа с платежными документами](payables-how-work-checks.md).</span><span class="sxs-lookup"><span data-stu-id="631ae-125">For more information, see [How to: Work with Checks](payables-how-work-checks.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="631ae-126">См. также</span><span class="sxs-lookup"><span data-stu-id="631ae-126">See Also</span></span>
[<span data-ttu-id="631ae-127">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="631ae-127">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="631ae-128">[Управление банковскими счетами](bank-manage-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="631ae-128">[Managing Bank Accounts](bank-manage-bank-accounts.md) </span></span>  
[<span data-ttu-id="631ae-129">Выполнение процессов завершения периода</span><span class="sxs-lookup"><span data-stu-id="631ae-129">Completing Period-End Processes</span></span>](year-how-complete-period-end-processes.md)  
<span data-ttu-id="631ae-130">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="631ae-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="631ae-131">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="631ae-131">General Business Functionality</span></span>](ui-across-business-areas.md)

