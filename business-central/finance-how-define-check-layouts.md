---
title: Определение макета чека | Документы Майкрософт
description: Вы можете разрабатывать и печатать чеки в различных форматах, чтобы они соответствовали определенным стандартам.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 04/24/2019
ms.author: edupont
ms.openlocfilehash: f2b7fa01cff36e3aab335f7d5921954343c69b74
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1243599"
---
# <a name="define-check-layouts"></a><span data-ttu-id="70e93-103">Определение макетов платежных документов</span><span class="sxs-lookup"><span data-stu-id="70e93-103">Define Check Layouts</span></span>
<span data-ttu-id="70e93-104">Вы можете разработать платежные документы в соответствии со стандартами, установленными местными органами власти.</span><span class="sxs-lookup"><span data-stu-id="70e93-104">You can design your checks to conform with the standards set by the local authorities.</span></span> <span data-ttu-id="70e93-105">Изображения платежных документов можно печатать на английском, французском или испанском языке.</span><span class="sxs-lookup"><span data-stu-id="70e93-105">Check images can be printed in English, French, or Spanish.</span></span>

<span data-ttu-id="70e93-106">Платежные документы разрабатываются для печати в форматах изображений платежных документов США и Канады в формате "платежный документ-бланк-платежный документ" или "бланк-бланк-платежный документ".</span><span class="sxs-lookup"><span data-stu-id="70e93-106">Checks are designed to print in both the United States and Canadian check image formats in either a check-stub-check format or a stub-stub-check format.</span></span>

## <a name="to-define-check-layouts"></a><span data-ttu-id="70e93-107">Определение макетов платежных документов</span><span class="sxs-lookup"><span data-stu-id="70e93-107">To define check layouts</span></span>
1. <span data-ttu-id="70e93-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Выбор отчета - банковский счет**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="70e93-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Selections Bank Account**, and then choose the related link.</span></span>
2. <span data-ttu-id="70e93-109">На странице **Выбор отчета - банковский счет** в поле **Использование** выберите **Платежный документ**.</span><span class="sxs-lookup"><span data-stu-id="70e93-109">On the **Report Selection - Bank Acc.** page, in the **Usage** field, select **Check**.</span></span>
3. <span data-ttu-id="70e93-110">Выберите один из следующих кодов отчетов.</span><span class="sxs-lookup"><span data-stu-id="70e93-110">Select one of the following report IDs.</span></span>

  | <span data-ttu-id="70e93-111">Код отчета</span><span class="sxs-lookup"><span data-stu-id="70e93-111">Report ID</span></span> | <span data-ttu-id="70e93-112">Название отчета</span><span class="sxs-lookup"><span data-stu-id="70e93-112">Report Name</span></span> | <span data-ttu-id="70e93-113">Описанием</span><span class="sxs-lookup"><span data-stu-id="70e93-113">Description</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="70e93-114">1401</span><span class="sxs-lookup"><span data-stu-id="70e93-114">1401</span></span> |<span data-ttu-id="70e93-115">Платежный документ</span><span class="sxs-lookup"><span data-stu-id="70e93-115">Check</span></span> |<span data-ttu-id="70e93-116">Это отчет по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70e93-116">This is the default report.</span></span> |
  | <span data-ttu-id="70e93-117">10411</span><span class="sxs-lookup"><span data-stu-id="70e93-117">10411</span></span> |<span data-ttu-id="70e93-118">Платежный документ (Бланк/Бланк/Платежный документ)</span><span class="sxs-lookup"><span data-stu-id="70e93-118">Check (Stub/Stub/Check)</span></span> |<span data-ttu-id="70e93-119">Этот отчет предназначен для печати платежных документов в формате "бланк/бланк/платежный документ".</span><span class="sxs-lookup"><span data-stu-id="70e93-119">This report is designed to print checks in a stub/stub/check format.</span></span> |
  | <span data-ttu-id="70e93-120">10412</span><span class="sxs-lookup"><span data-stu-id="70e93-120">10412</span></span> |<span data-ttu-id="70e93-121">Платежный документ (Бланк/Платежный документ/Бланк)</span><span class="sxs-lookup"><span data-stu-id="70e93-121">Check (Stub/Check/Stub)</span></span> |<span data-ttu-id="70e93-122">Этот отчет предназначен для печати платежных документов в формате "бланк/платежный документ/бланк".</span><span class="sxs-lookup"><span data-stu-id="70e93-122">This report is designed to print checks in a stub/check/stub format.</span></span> |
  | <span data-ttu-id="70e93-123">10413</span><span class="sxs-lookup"><span data-stu-id="70e93-123">10413</span></span> |<span data-ttu-id="70e93-124">Три платежных документа на страницу</span><span class="sxs-lookup"><span data-stu-id="70e93-124">Three Checks per Page</span></span> |<span data-ttu-id="70e93-125">Этот отчет предназначен для печати трех платежных документов на каждой странице.</span><span class="sxs-lookup"><span data-stu-id="70e93-125">This report is designed to print three checks on each page.</span></span> |

<span data-ttu-id="70e93-126">После настройки макетов платежных документов их можно распечатывать со страницы **Журнал платежей**.</span><span class="sxs-lookup"><span data-stu-id="70e93-126">When you have set up check layouts, you can print checks from the **Payment Journal** page.</span></span> <span data-ttu-id="70e93-127">Дополнительные сведения см. в разделе [Работа с платежными документами](payables-how-work-checks.md).</span><span class="sxs-lookup"><span data-stu-id="70e93-127">For more information, see [Work with Checks](payables-how-work-checks.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="70e93-128">См. также</span><span class="sxs-lookup"><span data-stu-id="70e93-128">See Also</span></span>
[<span data-ttu-id="70e93-129">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="70e93-129">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="70e93-130">[Управление банковскими счетами](bank-manage-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="70e93-130">[Managing Bank Accounts](bank-manage-bank-accounts.md) </span></span>  
[<span data-ttu-id="70e93-131">Выполнение процессов завершения периода</span><span class="sxs-lookup"><span data-stu-id="70e93-131">Completing Period-End Processes</span></span>](year-how-complete-period-end-processes.md)  
<span data-ttu-id="70e93-132">[Работа с [!INCLUDE[prodshort](includes/prodshort.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="70e93-132">[Working with [!INCLUDE[prodshort](includes/prodshort.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="70e93-133">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="70e93-133">General Business Functionality</span></span>](ui-across-business-areas.md)
