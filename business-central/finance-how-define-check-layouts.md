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
ms.date: 02/20/2020
ms.author: edupont
ms.openlocfilehash: df141f15eda20b1c3ce17e12e726f79a20532915
ms.sourcegitcommit: 35552b250b37c97772129d1cb9fd9e2537c83824
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2020
ms.locfileid: "3097748"
---
# <a name="select-a-check-layout"></a><span data-ttu-id="05d27-103">Выбор макета платежного документа</span><span class="sxs-lookup"><span data-stu-id="05d27-103">Select a Check Layout</span></span>
<span data-ttu-id="05d27-104">Вы можете разработать платежные документы в соответствии со стандартами, установленными местными органами власти.</span><span class="sxs-lookup"><span data-stu-id="05d27-104">You can design your checks to conform with the standards set by the local authorities.</span></span> <span data-ttu-id="05d27-105">Изображения платежных документов можно печатать на английском, французском или испанском языке.</span><span class="sxs-lookup"><span data-stu-id="05d27-105">Check images can be printed in English, French, or Spanish.</span></span>

<span data-ttu-id="05d27-106">Платежные документы разрабатываются для печати в форматах изображений платежных документов США и Канады в формате "платежный документ-бланк-платежный документ" или "бланк-бланк-платежный документ".</span><span class="sxs-lookup"><span data-stu-id="05d27-106">Checks are designed to print in both the United States and Canadian check image formats in either a check-stub-check format or a stub-stub-check format.</span></span>

## <a name="to-select-a-check-layout"></a><span data-ttu-id="05d27-107">Чтобы выбрать макет платежного документа</span><span class="sxs-lookup"><span data-stu-id="05d27-107">To select a check layout</span></span>
1. <span data-ttu-id="05d27-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Выбор отчета - банковский счет**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="05d27-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Selections Bank Account**, and then choose the related link.</span></span>
2. <span data-ttu-id="05d27-109">На странице **Выбор отчета - банковский счет** в поле **Использование** выберите **Платежный документ**.</span><span class="sxs-lookup"><span data-stu-id="05d27-109">On the **Report Selection - Bank Acc.** page, in the **Usage** field, select **Check**.</span></span>
3. <span data-ttu-id="05d27-110">Выберите один из следующих кодов отчетов.</span><span class="sxs-lookup"><span data-stu-id="05d27-110">Select one of the following report IDs.</span></span>

| <span data-ttu-id="05d27-111">Код отчета</span><span class="sxs-lookup"><span data-stu-id="05d27-111">Report ID</span></span> | <span data-ttu-id="05d27-112">Название отчета</span><span class="sxs-lookup"><span data-stu-id="05d27-112">Report Name</span></span> | <span data-ttu-id="05d27-113">Описание</span><span class="sxs-lookup"><span data-stu-id="05d27-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="05d27-114">1401</span><span class="sxs-lookup"><span data-stu-id="05d27-114">1401</span></span> |<span data-ttu-id="05d27-115">Платежный документ</span><span class="sxs-lookup"><span data-stu-id="05d27-115">Check</span></span> |<span data-ttu-id="05d27-116">Это отчет по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="05d27-116">This is the default report.</span></span> |
| <span data-ttu-id="05d27-117">10411</span><span class="sxs-lookup"><span data-stu-id="05d27-117">10411</span></span> |<span data-ttu-id="05d27-118">Платежный документ (Бланк/Бланк/Платежный документ)</span><span class="sxs-lookup"><span data-stu-id="05d27-118">Check (Stub/Stub/Check)</span></span> |<span data-ttu-id="05d27-119">Этот отчет предназначен для печати платежных документов в формате "бланк/бланк/платежный документ".</span><span class="sxs-lookup"><span data-stu-id="05d27-119">This report is designed to print checks in a stub/stub/check format.</span></span> |
| <span data-ttu-id="05d27-120">10412</span><span class="sxs-lookup"><span data-stu-id="05d27-120">10412</span></span> |<span data-ttu-id="05d27-121">Платежный документ (Бланк/Платежный документ/Бланк)</span><span class="sxs-lookup"><span data-stu-id="05d27-121">Check (Stub/Check/Stub)</span></span> |<span data-ttu-id="05d27-122">Этот отчет предназначен для печати платежных документов в формате "бланк/платежный документ/бланк".</span><span class="sxs-lookup"><span data-stu-id="05d27-122">This report is designed to print checks in a stub/check/stub format.</span></span> |
| <span data-ttu-id="05d27-123">10413</span><span class="sxs-lookup"><span data-stu-id="05d27-123">10413</span></span> |<span data-ttu-id="05d27-124">Три платежных документа на страницу</span><span class="sxs-lookup"><span data-stu-id="05d27-124">Three Checks per Page</span></span> |<span data-ttu-id="05d27-125">Этот отчет предназначен для печати трех платежных документов на каждой странице.</span><span class="sxs-lookup"><span data-stu-id="05d27-125">This report is designed to print three checks on each page.</span></span> |

<span data-ttu-id="05d27-126">После настройки макетов платежных документов их можно распечатывать со страницы **Журнал платежей**.</span><span class="sxs-lookup"><span data-stu-id="05d27-126">When you have set up check layouts, you can print checks from the **Payment Journal** page.</span></span> <span data-ttu-id="05d27-127">Дополнительные сведения см. в разделе [Работа с платежными документами](payables-how-work-checks.md).</span><span class="sxs-lookup"><span data-stu-id="05d27-127">For more information, see [Work with Checks](payables-how-work-checks.md).</span></span>

<span data-ttu-id="05d27-128">Чтобы изменить один из этих макетов платежного документа по умолчанию, выберите Word, либо интеграцию RDLC.</span><span class="sxs-lookup"><span data-stu-id="05d27-128">To change one of these default check layouts, use either the Word or the RDLC integration to do so.</span></span> <span data-ttu-id="05d27-129">Дополнительные сведения см. в разделе [Создание и изменение пользовательских макетов отчетов](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="05d27-129">For more information, see [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).</span></span>

## <a name="using-micr-and-security-fonts"></a><span data-ttu-id="05d27-130">Использование шрифтов безопасности и MICR</span><span class="sxs-lookup"><span data-stu-id="05d27-130">Using MICR and Security Fonts</span></span>
<span data-ttu-id="05d27-131">Онлайн-версия [!INCLUDE[d365fin](includes/d365fin_md.md)] содержит предварительно установленные шрифты на серверах, которые можно использовать при определении макетов чеков.</span><span class="sxs-lookup"><span data-stu-id="05d27-131">The online version of [!INCLUDE[d365fin](includes/d365fin_md.md)] contains pre-installed fonts on the servers that can be used when defining check layouts.</span></span> <span data-ttu-id="05d27-132">Ниже описывается, какие шрифты доступны, и приведены ссылки на подробную информацию сторонних поставщиков шрифтов.</span><span class="sxs-lookup"><span data-stu-id="05d27-132">The following outlines which fonts are available and has links to detailed information by the 3rd-party suppliers of the fonts.</span></span>

> [!Important]
> <span data-ttu-id="05d27-133">Шрифты безопасности чеков и MICR в Microsoft Dynamics [!INCLUDE[d365fin](includes/d365fin_md.md)] лицензированы в пакете шрифтов IDAutomation.com, Inc. Эти продукты могут использоваться только как часть или в связи с Microsoft Dynamics [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="05d27-133">MICR and check security fonts in Microsoft Dynamics [!INCLUDE[d365fin](includes/d365fin_md.md)] are licensed in a font package from IDAutomation.com, Inc. These products may only be used as part of and in connection with Microsoft Dynamics [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

<span data-ttu-id="05d27-134">В обновлении 15.3 и новее шрифты установлены и доступны для использования шрифты Magnetic Ink Character Recognition (MICR).</span><span class="sxs-lookup"><span data-stu-id="05d27-134">In update 15.3 and newer, Magnetic Ink Character Recognition (MICR) fonts are installed and available to use.</span></span> <span data-ttu-id="05d27-135">Поддерживаются стандарты E-13B и CMC-7.</span><span class="sxs-lookup"><span data-stu-id="05d27-135">Both the E-13B and the CMC-7 standards are supported.</span></span> <span data-ttu-id="05d27-136">Помимо шрифтов MICR доступны специальные шрифты безопасности для генерации текста, имен, сумм и символов валюты доллара, евро, фунта и йены, которые трудно подделать после печати чека.</span><span class="sxs-lookup"><span data-stu-id="05d27-136">In addition to MICR fonts, special security fonts are available to generate text, names, amounts, and the currency symbols Dollar, Euro, Pound, and Yen, which are hard to tamper with once a check has been printed.</span></span>

> [!NOTE]
> <span data-ttu-id="05d27-137">В целях безопасности и по юридическим причинам вы не можете загружать пользовательские шрифты в среду [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="05d27-137">For security and legal reasons, you cannot upload custom fonts to the [!INCLUDE[d365fin](includes/d365fin_md.md)] environment.</span></span>

### <a name="micr-e-13b-specifications"></a><span data-ttu-id="05d27-138">Спецификации MICR E-13B</span><span class="sxs-lookup"><span data-stu-id="05d27-138">MICR E-13B Specifications</span></span>
<span data-ttu-id="05d27-139">Ниже приведено краткое описание спецификаций для шрифтов MICR E-13B, которые могут быть полезны при калибровке шрифтов в макетах чеков с определенными принтерами MICR.</span><span class="sxs-lookup"><span data-stu-id="05d27-139">The following summarizes specifications for the MICR E-13B fonts that may be useful when calibrating fonts to be on check layouts with specific MICR printers.</span></span>

<span data-ttu-id="05d27-140">![Спецификации MICR E-13B](media/font_MICR_E-13B_Specifications.png "Спецификации MICR E-13B")</span><span class="sxs-lookup"><span data-stu-id="05d27-140">![MICR E-13B Specifications](media/font_MICR_E-13B_Specifications.png "MICR E-13B Specifications")</span></span>

<span data-ttu-id="05d27-141">Полную спецификацию шрифтов MICR E-13B можно найти в документации поставщика здесь: ( https://www.idautomation.com/micr-fonts/e13b/).</span><span class="sxs-lookup"><span data-stu-id="05d27-141">The full specification of MICR E-13B fonts can be found in the supplier's documentation here: (https://www.idautomation.com/micr-fonts/e13b/).</span></span>

### <a name="micr-cmc-7-specifications"></a><span data-ttu-id="05d27-142">Спецификации MICR CMC-7</span><span class="sxs-lookup"><span data-stu-id="05d27-142">MICR CMC-7 Specifications</span></span>
<span data-ttu-id="05d27-143">Следующие шрифты CMC-7 доступны в [!INCLUDE[d365fin](includes/d365fin_md.md)] online:</span><span class="sxs-lookup"><span data-stu-id="05d27-143">The following CMC-7 fonts are available in [!INCLUDE[d365fin](includes/d365fin_md.md)] online:</span></span>

- <span data-ttu-id="05d27-144">IDAutomationCMC7</span><span class="sxs-lookup"><span data-stu-id="05d27-144">IDAutomationCMC7</span></span>
- <span data-ttu-id="05d27-145">IDAutomationCMC7n10</span><span class="sxs-lookup"><span data-stu-id="05d27-145">IDAutomationCMC7n10</span></span>
- <span data-ttu-id="05d27-146">IDAutomationCMC7n25</span><span class="sxs-lookup"><span data-stu-id="05d27-146">IDAutomationCMC7n25</span></span>
-   <span data-ttu-id="05d27-147">IDAutomationCMC7n40</span><span class="sxs-lookup"><span data-stu-id="05d27-147">IDAutomationCMC7n40</span></span>

<span data-ttu-id="05d27-148">Ниже приведено краткое описание спецификаций для шрифтов MICR CMC-7 которые могут быть полезны при калибровке шрифтов в макетах чеков с определенными принтерами MICR.</span><span class="sxs-lookup"><span data-stu-id="05d27-148">The following summarizes specifications for the MICR CMC-7 fonts that may be useful when calibrating fonts to be on check layouts with specific MICR printers.</span></span>

<span data-ttu-id="05d27-149">![Спецификации MICR CMC-7](media/font_MICR_CMC-7_Specifications.png "Спецификации MICR CMC-7")</span><span class="sxs-lookup"><span data-stu-id="05d27-149">![MICR CMC-7 Specifications](media/font_MICR_CMC-7_Specifications.png "MICR CMC-7 Specifications")</span></span>

<span data-ttu-id="05d27-150">Полную спецификацию шрифтов MICR CMC-7 можно найти в документации поставщика здесь: ( http://www.idautomation.com/micr-fonts/cmc7/).</span><span class="sxs-lookup"><span data-stu-id="05d27-150">The full specification of MICR CMC-7 fonts can be found in the supplier's documentation here: (http://www.idautomation.com/micr-fonts/cmc7/).</span></span>

### <a name="secure-font-specifications"></a><span data-ttu-id="05d27-151">Спецификации безопасных шрифтов</span><span class="sxs-lookup"><span data-stu-id="05d27-151">Secure Font Specifications</span></span>
<span data-ttu-id="05d27-152">Ниже приведено краткое описание спецификаций шрифтов безопасности чеков, которые могут быть полезны при калибровке шрифтов в макетах чеков с определенными принтерами MICR.</span><span class="sxs-lookup"><span data-stu-id="05d27-152">The following summarizes specifications for check security fonts that may be useful when calibrating fonts to be on check layouts with specific MICR printers.</span></span>

<span data-ttu-id="05d27-153">![Спецификации шрифтов безопасности чеков](media/font_check-security-font_Specifications.png "Спецификации шрифтов безопасности чеков")</span><span class="sxs-lookup"><span data-stu-id="05d27-153">![Check Security Font Specifications](media/font_check-security-font_Specifications.png "Check Security Font Specifications")</span></span>

<span data-ttu-id="05d27-154">Полную спецификацию шрифтов безопасности чеков можно найти в документации поставщика здесь: ( https://www.idautomation.com/security-fonts/).</span><span class="sxs-lookup"><span data-stu-id="05d27-154">The full specification of check security fonts can be found in the supplier's documentation here: (https://www.idautomation.com/security-fonts/).</span></span>

<span data-ttu-id="05d27-155">Шрифты для других целей также доступны в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="05d27-155">Fonts for other purposes are also available in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="05d27-156">Для получения дополнительной информации см. [Доступные шрифты](ui-fonts.md)</span><span class="sxs-lookup"><span data-stu-id="05d27-156">For more information, see [Available Fonts](ui-fonts.md)</span></span>

## <a name="see-also"></a><span data-ttu-id="05d27-157">См. также</span><span class="sxs-lookup"><span data-stu-id="05d27-157">See Also</span></span>
[<span data-ttu-id="05d27-158">Создание и изменение пользовательских макетов отчетов</span><span class="sxs-lookup"><span data-stu-id="05d27-158">Create and Modify Custom Report Layouts</span></span>](ui-how-create-custom-report-layout.md)  
[<span data-ttu-id="05d27-159">Шрифты в Business Central</span><span class="sxs-lookup"><span data-stu-id="05d27-159">Fonts in Business Central</span></span>](ui-fonts.md)  
[<span data-ttu-id="05d27-160">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="05d27-160">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="05d27-161">[Выверка банковских счетов](bank-manage-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="05d27-161">[Reconciling Bank Accounts](bank-manage-bank-accounts.md) </span></span>  
[<span data-ttu-id="05d27-162">Выполнение процессов завершения периода</span><span class="sxs-lookup"><span data-stu-id="05d27-162">Completing Period-End Processes</span></span>](year-how-complete-period-end-processes.md)  
<span data-ttu-id="05d27-163">[Работа с [!INCLUDE[prodshort](includes/prodshort.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="05d27-163">[Working with [!INCLUDE[prodshort](includes/prodshort.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="05d27-164">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="05d27-164">General Business Functionality</span></span>](ui-across-business-areas.md)
