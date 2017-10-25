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
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: a2db2860846cd9b8010222faf580f0c9889e39a4
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-define-check-layouts"></a><span data-ttu-id="1f42a-103">Практическое руководство. Определение макетов платежных документов</span><span class="sxs-lookup"><span data-stu-id="1f42a-103">How to: Define Check Layouts</span></span>
<span data-ttu-id="1f42a-104">Вы можете разработать платежные документы в соответствии со стандартами, установленными местными органами власти.</span><span class="sxs-lookup"><span data-stu-id="1f42a-104">You can design your checks to conform with the standards set by the local authorities.</span></span> <span data-ttu-id="1f42a-105">Изображения платежных документов можно печатать на английском, французском или испанском языке.</span><span class="sxs-lookup"><span data-stu-id="1f42a-105">Check images can be printed in English, French, or Spanish.</span></span>

<span data-ttu-id="1f42a-106">Платежные документы разрабатываются для печати в форматах изображений платежных документов США и Канады в формате "платежный документ-бланк-платежный документ" или "бланк-бланк-платежный документ".</span><span class="sxs-lookup"><span data-stu-id="1f42a-106">Checks are designed to print in both the United States and Canadian check image formats in either a check-stub-check format or a stub-stub-check format.</span></span>

## <a name="to-define-check-layouts"></a><span data-ttu-id="1f42a-107">Определение макетов платежных документов</span><span class="sxs-lookup"><span data-stu-id="1f42a-107">To define check layouts</span></span>
1. <span data-ttu-id="1f42a-108">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Выбор отчета - банковский счет**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="1f42a-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Report Selections Bank Account**, and then choose the related link.</span></span>
2. <span data-ttu-id="1f42a-109">В окне **Выбор отчета - банковский счет** в поле **Использование** выберите **Платежный документ**.</span><span class="sxs-lookup"><span data-stu-id="1f42a-109">In the **Report Selection - Bank Acc.** window, in the **Usage** field, select **Check**.</span></span>
3. <span data-ttu-id="1f42a-110">Выберите один из следующих кодов отчетов.</span><span class="sxs-lookup"><span data-stu-id="1f42a-110">Select one of the following report IDs.</span></span>

| <span data-ttu-id="1f42a-111">Код отчета</span><span class="sxs-lookup"><span data-stu-id="1f42a-111">Report ID</span></span> | <span data-ttu-id="1f42a-112">Название отчета</span><span class="sxs-lookup"><span data-stu-id="1f42a-112">Report Name</span></span> | <span data-ttu-id="1f42a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1f42a-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1f42a-114">1401</span><span class="sxs-lookup"><span data-stu-id="1f42a-114">1401</span></span> |<span data-ttu-id="1f42a-115">Платежный документ</span><span class="sxs-lookup"><span data-stu-id="1f42a-115">Check</span></span> |<span data-ttu-id="1f42a-116">Это отчет по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1f42a-116">This is the default report.</span></span> |
| <span data-ttu-id="1f42a-117">10401</span><span class="sxs-lookup"><span data-stu-id="1f42a-117">10401</span></span> |<span data-ttu-id="1f42a-118">Платежный документ (Бланк/Бланк/Платежный документ)</span><span class="sxs-lookup"><span data-stu-id="1f42a-118">Check (Stub/Stub/Check)</span></span> |<span data-ttu-id="1f42a-119">Этот отчет предназначен для печати платежных документов в формате "бланк/бланк/платежный документ".</span><span class="sxs-lookup"><span data-stu-id="1f42a-119">This report is designed to print checks in a stub/stub/check format.</span></span> |
| <span data-ttu-id="1f42a-120">10411</span><span class="sxs-lookup"><span data-stu-id="1f42a-120">10411</span></span> |<span data-ttu-id="1f42a-121">Платежный документ (Бланк/Платежный документ/Бланк)</span><span class="sxs-lookup"><span data-stu-id="1f42a-121">Check (Stub/Check/Stub)</span></span> |<span data-ttu-id="1f42a-122">Этот отчет предназначен для печати платежных документов в формате "платежный документ/бланк/платежный документ".</span><span class="sxs-lookup"><span data-stu-id="1f42a-122">This report is designed to print checks in a check/stub/check format.</span></span> |

<span data-ttu-id="1f42a-123">После настройки макетов платежных документов их можно распечатывать из окна **Журнал платежей**.</span><span class="sxs-lookup"><span data-stu-id="1f42a-123">When you have set up check layouts, you can print checks from the **Payment Journal** window.</span></span> <span data-ttu-id="1f42a-124">Дополнительные сведения см. в разделе [Практическое руководство. Работа с платежными документами](payables-how-work-checks.md).</span><span class="sxs-lookup"><span data-stu-id="1f42a-124">For more information, see [How to: Work with Checks](payables-how-work-checks.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="1f42a-125">См. также</span><span class="sxs-lookup"><span data-stu-id="1f42a-125">See Also</span></span>
[<span data-ttu-id="1f42a-126">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="1f42a-126">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="1f42a-127">[Управление банковскими счетами](bank-manage-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="1f42a-127">[Managing Bank Accounts](bank-manage-bank-accounts.md) </span></span>  
[<span data-ttu-id="1f42a-128">Выполнение процессов завершения периода</span><span class="sxs-lookup"><span data-stu-id="1f42a-128">Completing Period-End Processes</span></span>](year-how-complete-period-end-processes.md)  
<span data-ttu-id="1f42a-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1f42a-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="1f42a-130">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="1f42a-130">General Business Functionality</span></span>](ui-across-business-areas.md)

