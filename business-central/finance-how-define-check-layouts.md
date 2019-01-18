---
title: "Определение макета чека | Документы Майкрософт"
description: "Вы можете разрабатывать и печатать чеки в различных форматах, чтобы они соответствовали определенным стандартам."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 743cf7ecbed4157dc9283a97baa956e69ec0c6b5
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="define-check-layouts"></a><span data-ttu-id="d44c1-103">Определение макетов платежных документов</span><span class="sxs-lookup"><span data-stu-id="d44c1-103">Define Check Layouts</span></span>
<span data-ttu-id="d44c1-104">Вы можете разработать платежные документы в соответствии со стандартами, установленными местными органами власти.</span><span class="sxs-lookup"><span data-stu-id="d44c1-104">You can design your checks to conform with the standards set by the local authorities.</span></span> <span data-ttu-id="d44c1-105">Изображения платежных документов можно печатать на английском, французском или испанском языке.</span><span class="sxs-lookup"><span data-stu-id="d44c1-105">Check images can be printed in English, French, or Spanish.</span></span>

<span data-ttu-id="d44c1-106">Платежные документы разрабатываются для печати в форматах изображений платежных документов США и Канады в формате "платежный документ-бланк-платежный документ" или "бланк-бланк-платежный документ".</span><span class="sxs-lookup"><span data-stu-id="d44c1-106">Checks are designed to print in both the United States and Canadian check image formats in either a check-stub-check format or a stub-stub-check format.</span></span>

## <a name="to-define-check-layouts"></a><span data-ttu-id="d44c1-107">Определение макетов платежных документов</span><span class="sxs-lookup"><span data-stu-id="d44c1-107">To define check layouts</span></span>
1. <span data-ttu-id="d44c1-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Выбор отчета - банковский счет**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d44c1-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Selections Bank Account**, and then choose the related link.</span></span>
2. <span data-ttu-id="d44c1-109">На странице **Выбор отчета - банковский счет** в поле **Использование** выберите **Платежный документ**.</span><span class="sxs-lookup"><span data-stu-id="d44c1-109">On the **Report Selection - Bank Acc.** page, in the **Usage** field, select **Check**.</span></span>
3. <span data-ttu-id="d44c1-110">Выберите один из следующих кодов отчетов.</span><span class="sxs-lookup"><span data-stu-id="d44c1-110">Select one of the following report IDs.</span></span>

| <span data-ttu-id="d44c1-111">Код отчета</span><span class="sxs-lookup"><span data-stu-id="d44c1-111">Report ID</span></span> | <span data-ttu-id="d44c1-112">Название отчета</span><span class="sxs-lookup"><span data-stu-id="d44c1-112">Report Name</span></span> | <span data-ttu-id="d44c1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d44c1-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="d44c1-114">1401</span><span class="sxs-lookup"><span data-stu-id="d44c1-114">1401</span></span> |<span data-ttu-id="d44c1-115">Платежный документ</span><span class="sxs-lookup"><span data-stu-id="d44c1-115">Check</span></span> |<span data-ttu-id="d44c1-116">Это отчет по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d44c1-116">This is the default report.</span></span> |
| <span data-ttu-id="d44c1-117">10401</span><span class="sxs-lookup"><span data-stu-id="d44c1-117">10401</span></span> |<span data-ttu-id="d44c1-118">Платежный документ (Бланк/Бланк/Платежный документ)</span><span class="sxs-lookup"><span data-stu-id="d44c1-118">Check (Stub/Stub/Check)</span></span> |<span data-ttu-id="d44c1-119">Этот отчет предназначен для печати платежных документов в формате "бланк/бланк/платежный документ".</span><span class="sxs-lookup"><span data-stu-id="d44c1-119">This report is designed to print checks in a stub/stub/check format.</span></span> |
| <span data-ttu-id="d44c1-120">10411</span><span class="sxs-lookup"><span data-stu-id="d44c1-120">10411</span></span> |<span data-ttu-id="d44c1-121">Платежный документ (Бланк/Платежный документ/Бланк)</span><span class="sxs-lookup"><span data-stu-id="d44c1-121">Check (Stub/Check/Stub)</span></span> |<span data-ttu-id="d44c1-122">Этот отчет предназначен для печати платежных документов в формате "платежный документ/бланк/платежный документ".</span><span class="sxs-lookup"><span data-stu-id="d44c1-122">This report is designed to print checks in a check/stub/check format.</span></span> |

<span data-ttu-id="d44c1-123">После настройки макетов платежных документов их можно распечатывать со страницы **Журнал платежей**.</span><span class="sxs-lookup"><span data-stu-id="d44c1-123">When you have set up check layouts, you can print checks from the **Payment Journal** page.</span></span> <span data-ttu-id="d44c1-124">Дополнительные сведения см. в разделе [Работа с платежными документами](payables-how-work-checks.md).</span><span class="sxs-lookup"><span data-stu-id="d44c1-124">For more information, see [Work with Checks](payables-how-work-checks.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="d44c1-125">См. также</span><span class="sxs-lookup"><span data-stu-id="d44c1-125">See Also</span></span>
[<span data-ttu-id="d44c1-126">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="d44c1-126">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="d44c1-127">[Управление банковскими счетами](bank-manage-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="d44c1-127">[Managing Bank Accounts](bank-manage-bank-accounts.md) </span></span>  
[<span data-ttu-id="d44c1-128">Выполнение процессов завершения периода</span><span class="sxs-lookup"><span data-stu-id="d44c1-128">Completing Period-End Processes</span></span>](year-how-complete-period-end-processes.md)  
<span data-ttu-id="d44c1-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d44c1-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="d44c1-130">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="d44c1-130">General Business Functionality</span></span>](ui-across-business-areas.md)

