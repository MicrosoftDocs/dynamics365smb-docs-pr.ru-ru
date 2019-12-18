---
title: Определение макета чека | Документация Майкрософт
description: Вы можете разрабатывать и печатать чеки в различных форматах, чтобы они соответствовали определенным стандартам.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: d4818c9dfe96f7e890d84a16c717d4451f56497a
ms.sourcegitcommit: 893e13fa75b2d04dedd4a29abda216e3e54b24ae
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "2808581"
---
# <a name="select-a-check-layout"></a><span data-ttu-id="c6e66-103">Выбор макета платежного документа</span><span class="sxs-lookup"><span data-stu-id="c6e66-103">Select a Check Layout</span></span>
<span data-ttu-id="c6e66-104">Вы можете разработать платежные документы в соответствии со стандартами, установленными местными органами власти.</span><span class="sxs-lookup"><span data-stu-id="c6e66-104">You can design your checks to conform with the standards set by the local authorities.</span></span> <span data-ttu-id="c6e66-105">Изображения платежных документов можно печатать на английском, французском или испанском языке.</span><span class="sxs-lookup"><span data-stu-id="c6e66-105">Check images can be printed in English, French, or Spanish.</span></span>

<span data-ttu-id="c6e66-106">Платежные документы разрабатываются для печати в форматах изображений платежных документов США и Канады в формате "платежный документ-бланк-платежный документ" или "бланк-бланк-платежный документ".</span><span class="sxs-lookup"><span data-stu-id="c6e66-106">Checks are designed to print in both the United States and Canadian check image formats in either a check-stub-check format or a stub-stub-check format.</span></span>

## <a name="to-select-a-check-layout"></a><span data-ttu-id="c6e66-107">Чтобы выбрать макет платежного документа</span><span class="sxs-lookup"><span data-stu-id="c6e66-107">To select a check layout</span></span>
1. <span data-ttu-id="c6e66-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Выбор отчета - банковский счет**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="c6e66-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Selections Bank Account**, and then choose the related link.</span></span>
2. <span data-ttu-id="c6e66-109">На странице **Выбор отчета - банковский счет** в поле **Использование** выберите **Платежный документ**.</span><span class="sxs-lookup"><span data-stu-id="c6e66-109">On the **Report Selection - Bank Acc.** page, in the **Usage** field, select **Check**.</span></span>
3. <span data-ttu-id="c6e66-110">Выберите один из следующих кодов отчетов.</span><span class="sxs-lookup"><span data-stu-id="c6e66-110">Select one of the following report IDs.</span></span>

| <span data-ttu-id="c6e66-111">Код отчета</span><span class="sxs-lookup"><span data-stu-id="c6e66-111">Report ID</span></span> | <span data-ttu-id="c6e66-112">Название отчета</span><span class="sxs-lookup"><span data-stu-id="c6e66-112">Report Name</span></span> | <span data-ttu-id="c6e66-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c6e66-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="c6e66-114">1401</span><span class="sxs-lookup"><span data-stu-id="c6e66-114">1401</span></span> |<span data-ttu-id="c6e66-115">Платежный документ</span><span class="sxs-lookup"><span data-stu-id="c6e66-115">Check</span></span> |<span data-ttu-id="c6e66-116">Это отчет по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c6e66-116">This is the default report.</span></span> |
| <span data-ttu-id="c6e66-117">10411</span><span class="sxs-lookup"><span data-stu-id="c6e66-117">10411</span></span> |<span data-ttu-id="c6e66-118">Платежный документ (Бланк/Бланк/Платежный документ)</span><span class="sxs-lookup"><span data-stu-id="c6e66-118">Check (Stub/Stub/Check)</span></span> |<span data-ttu-id="c6e66-119">Этот отчет предназначен для печати платежных документов в формате "бланк/бланк/платежный документ".</span><span class="sxs-lookup"><span data-stu-id="c6e66-119">This report is designed to print checks in a stub/stub/check format.</span></span> |
| <span data-ttu-id="c6e66-120">10412</span><span class="sxs-lookup"><span data-stu-id="c6e66-120">10412</span></span> |<span data-ttu-id="c6e66-121">Платежный документ (Бланк/Платежный документ/Бланк)</span><span class="sxs-lookup"><span data-stu-id="c6e66-121">Check (Stub/Check/Stub)</span></span> |<span data-ttu-id="c6e66-122">Этот отчет предназначен для печати платежных документов в формате "бланк/платежный документ/бланк".</span><span class="sxs-lookup"><span data-stu-id="c6e66-122">This report is designed to print checks in a stub/check/stub format.</span></span> |
| <span data-ttu-id="c6e66-123">10413</span><span class="sxs-lookup"><span data-stu-id="c6e66-123">10413</span></span> |<span data-ttu-id="c6e66-124">Три платежных документа на страницу</span><span class="sxs-lookup"><span data-stu-id="c6e66-124">Three Checks per Page</span></span> |<span data-ttu-id="c6e66-125">Этот отчет предназначен для печати трех платежных документов на каждой странице.</span><span class="sxs-lookup"><span data-stu-id="c6e66-125">This report is designed to print three checks on each page.</span></span> |

<span data-ttu-id="c6e66-126">После настройки макетов платежных документов их можно распечатывать со страницы **Журнал платежей**.</span><span class="sxs-lookup"><span data-stu-id="c6e66-126">When you have set up check layouts, you can print checks from the **Payment Journal** page.</span></span> <span data-ttu-id="c6e66-127">Дополнительные сведения см. в разделе [Работа с платежными документами](payables-how-work-checks.md).</span><span class="sxs-lookup"><span data-stu-id="c6e66-127">For more information, see [Work with Checks](payables-how-work-checks.md).</span></span>

<span data-ttu-id="c6e66-128">Чтобы изменить один из этих макетов платежного документа по умолчанию, выберите Word, либо интеграцию RDLC.</span><span class="sxs-lookup"><span data-stu-id="c6e66-128">To change one of these default check layouts, use either the Word or the RDLC integration to do so.</span></span> <span data-ttu-id="c6e66-129">Дополнительные сведения см. в разделе [Создание и изменение пользовательских макетов отчетов](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="c6e66-129">For more information, see [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="c6e66-130">См. также</span><span class="sxs-lookup"><span data-stu-id="c6e66-130">See Also</span></span>
[<span data-ttu-id="c6e66-131">Создание и изменение пользовательских макетов отчетов</span><span class="sxs-lookup"><span data-stu-id="c6e66-131">Create and Modify Custom Report Layouts</span></span>](ui-how-create-custom-report-layout.md)  
[<span data-ttu-id="c6e66-132">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="c6e66-132">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="c6e66-133">[Управление банковскими счетами](bank-manage-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="c6e66-133">[Managing Bank Accounts](bank-manage-bank-accounts.md) </span></span>  
[<span data-ttu-id="c6e66-134">Выполнение процессов завершения периода</span><span class="sxs-lookup"><span data-stu-id="c6e66-134">Completing Period-End Processes</span></span>](year-how-complete-period-end-processes.md)  
<span data-ttu-id="c6e66-135">[Работа с [!INCLUDE[prodshort](includes/prodshort.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c6e66-135">[Working with [!INCLUDE[prodshort](includes/prodshort.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="c6e66-136">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="c6e66-136">General Business Functionality</span></span>](ui-across-business-areas.md)
