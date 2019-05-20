---
title: Изменение внешнего вида отчета путем выбора другого макета | Документы Майкрософт
description: Вы можете использовать различные макеты для отчетов и переключаться между ними, чтобы изменять внешний вид отчета.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: f24f1cd24a31ddbd0b455b876821ae0173a677c3
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1249444"
---
# <a name="change-which-layout-is-currently-used-on-a-report"></a><span data-ttu-id="2243a-103">Изменение макета, в настоящее время используемого в отчете</span><span class="sxs-lookup"><span data-stu-id="2243a-103">Change Which Layout is Currently Used on a Report</span></span>
<span data-ttu-id="2243a-104">Отчет можно настроить с использованием нескольких макетов, между которыми затем при необходимости можно будет переключаться.</span><span class="sxs-lookup"><span data-stu-id="2243a-104">A report can be set up with more than one report layout, which you can then switch among as needed.</span></span>

<span data-ttu-id="2243a-105">В зависимости от доступных для отчета макетов можно принять решение об использовании встроенного макета отчета RDLC, встроенного макета отчета Word или пользовательского макета.</span><span class="sxs-lookup"><span data-stu-id="2243a-105">Depending on the layouts that are available for a report, you can choose to use a built-in RDLC report layout, a built-in Word report layout, or a custom layout.</span></span> <span data-ttu-id="2243a-106">Дополнительные сведения о макетах отчетов RDLC и Word, встроенных и пользовательских макетах и др. см. в разделе [Управление макетами отчетов](ui-manage-report-layouts.md).</span><span class="sxs-lookup"><span data-stu-id="2243a-106">For more information about RDLC and Word report layouts, built-in and custom layouts, and more, see [Manage Report Layouts](ui-manage-report-layouts.md).</span></span>

> [!TIP]  
> <span data-ttu-id="2243a-107">Отчеты о документах (не списки), в которых используется макет отчета Word, обычно быстрее, чем те, в которых используется макет отчета RDLC.</span><span class="sxs-lookup"><span data-stu-id="2243a-107">Document reports (not lists) that use a Word report layout are typically faster than those that use an RDLC report layout.</span></span> <span data-ttu-id="2243a-108">Поэтому если имеется выбор между макетом отчета Word или RDLC для отчета по документам, используйте макет отчета Word для оптимальной производительности.</span><span class="sxs-lookup"><span data-stu-id="2243a-108">So if you have the option to choose between a Word or RDLC report layout for a document report, use the Word report layout for the best performance.</span></span>  

## <a name="to-change-the-layout-that-is-used-on-a-report"></a><span data-ttu-id="2243a-109">Изменение макета, используемого в отчете</span><span class="sxs-lookup"><span data-stu-id="2243a-109">To change the layout that is used on a report</span></span>
1. <span data-ttu-id="2243a-110">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Выбор макета отчета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2243a-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Layout Selection**, and then choose the related link.</span></span>  
   <span data-ttu-id="2243a-111">На странице **Выбор макета отчета** перечисляются все доступные отчеты для организации, которая указана в поле "Организация" в верхней части страницы.</span><span class="sxs-lookup"><span data-stu-id="2243a-111">The **Report Layout Selection** page lists all the reports that are available for the company that is specified in the Company field at the top of the page.</span></span> <span data-ttu-id="2243a-112">Поле "Выбранный макет" задает макет, который в настоящее время используется в отчете.</span><span class="sxs-lookup"><span data-stu-id="2243a-112">The Selected Layout field specifies the layout that is currently used on the report.</span></span>
2. <span data-ttu-id="2243a-113">Укажите в поле **Организация** в верхней части страницы организацию, которую требуется включить в отчет.</span><span class="sxs-lookup"><span data-stu-id="2243a-113">Set the **Company** field at the top of the page to the company that includes the report.</span></span>
3. <span data-ttu-id="2243a-114">Чтобы изменить макет отчета, в строке отчета в списке настройте в поле **Выбранный отчет** один из следующих вариантов.</span><span class="sxs-lookup"><span data-stu-id="2243a-114">To change the layout that is used by a report, in the row for the report in the list, set the **Selected Layout** field to one of the following options:</span></span>
   * <span data-ttu-id="2243a-115">RDLC (встроенный), использует встроенный макет отчета RDLC.</span><span class="sxs-lookup"><span data-stu-id="2243a-115">RDLC (built-in), uses the built-in RDLC report layout on the report.</span></span>
   * <span data-ttu-id="2243a-116">Word (встроенный), использует встроенный макет отчета Word.</span><span class="sxs-lookup"><span data-stu-id="2243a-116">Word (built-in), uses the built-in Word report layout on the report.</span></span>
   * <span data-ttu-id="2243a-117">Пользовательский, использует пользовательский макет отчета.</span><span class="sxs-lookup"><span data-stu-id="2243a-117">Custom, uses a custom layout on the report.</span></span>  
     <span data-ttu-id="2243a-118">Можно просмотреть, какие пользовательские отчеты доступны для отчета на информационной панели "Часть макетов отчета".</span><span class="sxs-lookup"><span data-stu-id="2243a-118">You can see which custom layouts are available for the report in the Report Layouts Part FactBox.</span></span> <span data-ttu-id="2243a-119">Если отсутствуют пользовательские макеты для отчета, сначала необходимо создать их.</span><span class="sxs-lookup"><span data-stu-id="2243a-119">If there are no custom layouts for the report, then you will have to create one first.</span></span> <span data-ttu-id="2243a-120">Если выбрать этот вариант, перейдите к следующей процедуре, чтобы задать пользовательский макет, который требуется использовать.</span><span class="sxs-lookup"><span data-stu-id="2243a-120">If you choose this option, go to the next procedure to specify the custom layout that you want to use.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="2243a-121">Если выбрано значение **RDLC (встроенный)** или **Word (встроенный)** и пользователь получает сообщение об ошибке, что этот отчет не имеет макета заданного типа, необходимо выбрать другой макет или создать пользовательский макет отчета нужного типа.</span><span class="sxs-lookup"><span data-stu-id="2243a-121">If you choose **RDLC (built-in)** or **Word (built-in)** and you get an error message that the report does not have a layout of the specified type, then you must choose another layout option or create a custom report layout of the type that you want to use.</span></span>

<span data-ttu-id="2243a-122">Если выбран встроенный макет отчета RDLC или Word, никакие дальнейшие действия не требуются, а макет будет использоваться при следующем выполнении отчета.</span><span class="sxs-lookup"><span data-stu-id="2243a-122">If you selected a built-in RDLC or Word report layout, then no further action is required and the layout will be used the next time the report is run.</span></span>

## <a name="to-specify-a-custom-layout-on-a-report"></a><span data-ttu-id="2243a-123">Определение пользовательского макета отчета</span><span class="sxs-lookup"><span data-stu-id="2243a-123">To specify a custom layout on a report</span></span>
1. <span data-ttu-id="2243a-124">Вы указываете, какой пользовательский макет нужно использовать в отчете со страницы **Пользовательские макеты отчетов**.</span><span class="sxs-lookup"><span data-stu-id="2243a-124">You specify which custom layout to use on the report from the **Custom Report Layouts** page.</span></span> <span data-ttu-id="2243a-125">Если страница **Пользовательские макеты отчетов** не открыта, нажмите кнопку выбора в поле **Описание макета отчета**.</span><span class="sxs-lookup"><span data-stu-id="2243a-125">If the **Custom Report Layouts** page is not open, then in the **Report Layout Description** field, choose the lookup button.</span></span>
2. <span data-ttu-id="2243a-126">На странице **Пользовательские макеты отчетов** выберите строку для пользовательского макета, который требуется использовать, затем закройте страницу.</span><span class="sxs-lookup"><span data-stu-id="2243a-126">On the **Custom Report Layouts** page, select the row for custom layout that you want to use, and then close the page.</span></span>

<span data-ttu-id="2243a-127">Вы вернетесь на страницу **Выбор макета отчета**.</span><span class="sxs-lookup"><span data-stu-id="2243a-127">You return to the **Report Layout Selection** page.</span></span> <span data-ttu-id="2243a-128">Имя выбранного пользовательского макета отображается в поле **Описание пользовательского макета**.</span><span class="sxs-lookup"><span data-stu-id="2243a-128">The name of the selected custom layout displays in the **Custom Layout Description** field.</span></span> <span data-ttu-id="2243a-129">Пользовательский макет будет использован при следующем выполнении отчета.</span><span class="sxs-lookup"><span data-stu-id="2243a-129">The custom layout will be used the next time that you run the report.</span></span>

## <a name="see-also"></a><span data-ttu-id="2243a-130">См. также</span><span class="sxs-lookup"><span data-stu-id="2243a-130">See Also</span></span>
[<span data-ttu-id="2243a-131">Управление макетами отчетов</span><span class="sxs-lookup"><span data-stu-id="2243a-131">Managing Report Layouts</span></span>](ui-manage-report-layouts.md)  
<span data-ttu-id="2243a-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2243a-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
