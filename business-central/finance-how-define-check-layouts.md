---
title: Определение макета чека | Документация Майкрософт
description: Вы можете разрабатывать и печатать чеки в различных форматах, чтобы они соответствовали определенным стандартам.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: ac980cb4b64a39b7ed912a49b06c179ffc7219d9
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5386503"
---
# <a name="select-a-check-layout"></a><span data-ttu-id="6036b-103">Выбор макета платежного документа</span><span class="sxs-lookup"><span data-stu-id="6036b-103">Select a Check Layout</span></span>
<span data-ttu-id="6036b-104">Вы можете разработать платежные документы в соответствии со стандартами, установленными местными органами власти.</span><span class="sxs-lookup"><span data-stu-id="6036b-104">You can design your checks to conform with the standards set by the local authorities.</span></span> <span data-ttu-id="6036b-105">Изображения платежных документов можно печатать на английском, французском или испанском языке.</span><span class="sxs-lookup"><span data-stu-id="6036b-105">Check images can be printed in English, French, or Spanish.</span></span>

<span data-ttu-id="6036b-106">Платежные документы разрабатываются для печати в форматах изображений платежных документов США и Канады в формате "платежный документ-бланк-платежный документ" или "бланк-бланк-платежный документ".</span><span class="sxs-lookup"><span data-stu-id="6036b-106">Checks are designed to print in both the United States and Canadian check image formats in either a check-stub-check format or a stub-stub-check format.</span></span>

## <a name="to-select-a-check-layout"></a><span data-ttu-id="6036b-107">Чтобы выбрать макет платежного документа</span><span class="sxs-lookup"><span data-stu-id="6036b-107">To select a check layout</span></span>
1. <span data-ttu-id="6036b-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Выбор отчета - банковский счет**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="6036b-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Selections Bank Account**, and then choose the related link.</span></span>
2. <span data-ttu-id="6036b-109">На странице **Выбор отчета - банковский счет** в поле **Использование** выберите **Платежный документ**.</span><span class="sxs-lookup"><span data-stu-id="6036b-109">On the **Report Selection - Bank Acc.** page, in the **Usage** field, select **Check**.</span></span>
3. <span data-ttu-id="6036b-110">Выберите один из следующих кодов отчетов.</span><span class="sxs-lookup"><span data-stu-id="6036b-110">Select one of the following report IDs.</span></span>

| <span data-ttu-id="6036b-111">Код отчета</span><span class="sxs-lookup"><span data-stu-id="6036b-111">Report ID</span></span> | <span data-ttu-id="6036b-112">Название отчета</span><span class="sxs-lookup"><span data-stu-id="6036b-112">Report Name</span></span> | <span data-ttu-id="6036b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6036b-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="6036b-114">1401</span><span class="sxs-lookup"><span data-stu-id="6036b-114">1401</span></span> |<span data-ttu-id="6036b-115">Платежный документ</span><span class="sxs-lookup"><span data-stu-id="6036b-115">Check</span></span> |<span data-ttu-id="6036b-116">Это отчет по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6036b-116">This is the default report.</span></span> |
| <span data-ttu-id="6036b-117">10411</span><span class="sxs-lookup"><span data-stu-id="6036b-117">10411</span></span> |<span data-ttu-id="6036b-118">Платежный документ (Бланк/Бланк/Платежный документ)</span><span class="sxs-lookup"><span data-stu-id="6036b-118">Check (Stub/Stub/Check)</span></span> |<span data-ttu-id="6036b-119">Этот отчет предназначен для печати платежных документов в формате "бланк/бланк/платежный документ".</span><span class="sxs-lookup"><span data-stu-id="6036b-119">This report is designed to print checks in a stub/stub/check format.</span></span> |
| <span data-ttu-id="6036b-120">10412</span><span class="sxs-lookup"><span data-stu-id="6036b-120">10412</span></span> |<span data-ttu-id="6036b-121">Платежный документ (Бланк/Платежный документ/Бланк)</span><span class="sxs-lookup"><span data-stu-id="6036b-121">Check (Stub/Check/Stub)</span></span> |<span data-ttu-id="6036b-122">Этот отчет предназначен для печати платежных документов в формате "бланк/платежный документ/бланк".</span><span class="sxs-lookup"><span data-stu-id="6036b-122">This report is designed to print checks in a stub/check/stub format.</span></span> |
| <span data-ttu-id="6036b-123">10413</span><span class="sxs-lookup"><span data-stu-id="6036b-123">10413</span></span> |<span data-ttu-id="6036b-124">Три платежных документа на страницу</span><span class="sxs-lookup"><span data-stu-id="6036b-124">Three Checks per Page</span></span> |<span data-ttu-id="6036b-125">Этот отчет предназначен для печати трех платежных документов на каждой странице.</span><span class="sxs-lookup"><span data-stu-id="6036b-125">This report is designed to print three checks on each page.</span></span> |

<span data-ttu-id="6036b-126">После настройки макетов платежных документов их можно распечатывать со страницы **Журнал платежей**.</span><span class="sxs-lookup"><span data-stu-id="6036b-126">When you have set up check layouts, you can print checks from the **Payment Journal** page.</span></span> <span data-ttu-id="6036b-127">Дополнительные сведения см. в разделе [Работа с платежными документами](payables-how-work-checks.md).</span><span class="sxs-lookup"><span data-stu-id="6036b-127">For more information, see [Work with Checks](payables-how-work-checks.md).</span></span>

<span data-ttu-id="6036b-128">Чтобы изменить один из этих макетов платежного документа по умолчанию, выберите Word, либо интеграцию RDLC.</span><span class="sxs-lookup"><span data-stu-id="6036b-128">To change one of these default check layouts, use either the Word or the RDLC integration to do so.</span></span> <span data-ttu-id="6036b-129">Дополнительные сведения см. в разделе [Создание и изменение пользовательских макетов отчетов](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="6036b-129">For more information, see [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).</span></span>

## <a name="using-micr-and-security-fonts"></a><span data-ttu-id="6036b-130">Использование шрифтов безопасности и MICR</span><span class="sxs-lookup"><span data-stu-id="6036b-130">Using MICR and Security Fonts</span></span>
<span data-ttu-id="6036b-131">Онлайн-версия [!INCLUDE[prod_short](includes/prod_short.md)] содержит предварительно установленные шрифты на серверах, которые можно использовать при определении макетов чеков.</span><span class="sxs-lookup"><span data-stu-id="6036b-131">The online version of [!INCLUDE[prod_short](includes/prod_short.md)] contains pre-installed fonts on the servers that can be used when defining check layouts.</span></span> <span data-ttu-id="6036b-132">Ниже описывается, какие шрифты доступны, и приведены ссылки на подробную информацию сторонних поставщиков шрифтов.</span><span class="sxs-lookup"><span data-stu-id="6036b-132">The following outlines which fonts are available and has links to detailed information by the 3rd-party suppliers of the fonts.</span></span>

> [!Important]
> <span data-ttu-id="6036b-133">Шрифты безопасности чеков и MICR в Microsoft Dynamics [!INCLUDE[prod_short](includes/prod_short.md)] лицензированы в пакете шрифтов IDAutomation.com, Inc. Эти продукты могут использоваться только как часть или в связи с Microsoft Dynamics [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="6036b-133">MICR and check security fonts in Microsoft Dynamics [!INCLUDE[prod_short](includes/prod_short.md)] are licensed in a font package from IDAutomation.com, Inc. These products may only be used as part of and in connection with Microsoft Dynamics [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

<span data-ttu-id="6036b-134">В обновлении 15.3 и новее шрифты установлены и доступны для использования шрифты Magnetic Ink Character Recognition (MICR).</span><span class="sxs-lookup"><span data-stu-id="6036b-134">In update 15.3 and newer, Magnetic Ink Character Recognition (MICR) fonts are installed and available to use.</span></span> <span data-ttu-id="6036b-135">Поддерживаются стандарты E-13B и CMC-7.</span><span class="sxs-lookup"><span data-stu-id="6036b-135">Both the E-13B and the CMC-7 standards are supported.</span></span> <span data-ttu-id="6036b-136">Помимо шрифтов MICR доступны специальные шрифты безопасности для генерации текста, имен, сумм и символов валюты доллара, евро, фунта и йены, которые трудно подделать после печати чека.</span><span class="sxs-lookup"><span data-stu-id="6036b-136">In addition to MICR fonts, special security fonts are available to generate text, names, amounts, and the currency symbols Dollar, Euro, Pound, and Yen, which are hard to tamper with once a check has been printed.</span></span>

> [!NOTE]
> <span data-ttu-id="6036b-137">В целях безопасности и по юридическим причинам вы не можете загружать пользовательские шрифты в среду [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="6036b-137">For security and legal reasons, you cannot upload custom fonts to the [!INCLUDE[prod_short](includes/prod_short.md)] environment.</span></span>

### <a name="micr-e-13b-specifications"></a><span data-ttu-id="6036b-138">Спецификации MICR E-13B</span><span class="sxs-lookup"><span data-stu-id="6036b-138">MICR E-13B Specifications</span></span>
<span data-ttu-id="6036b-139">Ниже приведено краткое описание спецификаций для шрифтов MICR E-13B, которые могут быть полезны при калибровке шрифтов в макетах чеков с определенными принтерами MICR.</span><span class="sxs-lookup"><span data-stu-id="6036b-139">The following summarizes specifications for the MICR E-13B fonts that may be useful when calibrating fonts to be on check layouts with specific MICR printers.</span></span>

<span data-ttu-id="6036b-140">![Спецификации MICR E-13B](media/font_MICR_E-13B_Specifications.png "Спецификации MICR E-13B")</span><span class="sxs-lookup"><span data-stu-id="6036b-140">![MICR E-13B Specifications](media/font_MICR_E-13B_Specifications.png "MICR E-13B Specifications")</span></span>

### <a name="delimiter-characters"></a><span data-ttu-id="6036b-141">Символы-разделители</span><span class="sxs-lookup"><span data-stu-id="6036b-141">Delimiter characters</span></span>
<span data-ttu-id="6036b-142">![Символы-разделители](media/font-micr-letters.png "Символы-разделители")</span><span class="sxs-lookup"><span data-stu-id="6036b-142">![Delimiter characters](media/font-micr-letters.png "Delimiter characters")</span></span>

<span data-ttu-id="6036b-143">Полную спецификацию шрифтов MICR E-13B можно найти в документации поставщика здесь: ( https://www.idautomation.com/micr-fonts/e13b/).</span><span class="sxs-lookup"><span data-stu-id="6036b-143">The full specification of MICR E-13B fonts can be found in the supplier's documentation here: (https://www.idautomation.com/micr-fonts/e13b/).</span></span>

### <a name="micr-cmc-7-specifications"></a><span data-ttu-id="6036b-144">Спецификации MICR CMC-7</span><span class="sxs-lookup"><span data-stu-id="6036b-144">MICR CMC-7 Specifications</span></span>
<span data-ttu-id="6036b-145">Следующие шрифты CMC-7 доступны в [!INCLUDE[prod_short](includes/prod_short.md)] online:</span><span class="sxs-lookup"><span data-stu-id="6036b-145">The following CMC-7 fonts are available in [!INCLUDE[prod_short](includes/prod_short.md)] online:</span></span>

- <span data-ttu-id="6036b-146">IDAutomationCMC7</span><span class="sxs-lookup"><span data-stu-id="6036b-146">IDAutomationCMC7</span></span>
- <span data-ttu-id="6036b-147">IDAutomationCMC7n10</span><span class="sxs-lookup"><span data-stu-id="6036b-147">IDAutomationCMC7n10</span></span>
- <span data-ttu-id="6036b-148">IDAutomationCMC7n25</span><span class="sxs-lookup"><span data-stu-id="6036b-148">IDAutomationCMC7n25</span></span>
-   <span data-ttu-id="6036b-149">IDAutomationCMC7n40</span><span class="sxs-lookup"><span data-stu-id="6036b-149">IDAutomationCMC7n40</span></span>

<span data-ttu-id="6036b-150">Ниже приведено краткое описание спецификаций для шрифтов MICR CMC-7 которые могут быть полезны при калибровке шрифтов в макетах чеков с определенными принтерами MICR.</span><span class="sxs-lookup"><span data-stu-id="6036b-150">The following summarizes specifications for the MICR CMC-7 fonts that may be useful when calibrating fonts to be on check layouts with specific MICR printers.</span></span>

<span data-ttu-id="6036b-151">![Спецификации MICR CMC-7](media/font_MICR_CMC-7_Specifications.png "Спецификации MICR CMC-7")</span><span class="sxs-lookup"><span data-stu-id="6036b-151">![MICR CMC-7 Specifications](media/font_MICR_CMC-7_Specifications.png "MICR CMC-7 Specifications")</span></span>

### <a name="delimiter-characters"></a><span data-ttu-id="6036b-152">Символы-разделители</span><span class="sxs-lookup"><span data-stu-id="6036b-152">Delimiter characters</span></span>
<span data-ttu-id="6036b-153">![Символы-разделители](media/font-cmc7-letters.png "Символы-разделители")</span><span class="sxs-lookup"><span data-stu-id="6036b-153">![Delimiter characters](media/font-cmc7-letters.png "Delimiter characters")</span></span>

<span data-ttu-id="6036b-154">Полную спецификацию шрифтов MICR CMC-7 можно найти в документации поставщика здесь: ( http://www.idautomation.com/micr-fonts/cmc7/).</span><span class="sxs-lookup"><span data-stu-id="6036b-154">The full specification of MICR CMC-7 fonts can be found in the supplier's documentation here: (http://www.idautomation.com/micr-fonts/cmc7/).</span></span>

### <a name="secure-font-specifications"></a><span data-ttu-id="6036b-155">Спецификации безопасных шрифтов</span><span class="sxs-lookup"><span data-stu-id="6036b-155">Secure Font Specifications</span></span>
<span data-ttu-id="6036b-156">Ниже приведено краткое описание спецификаций шрифтов безопасности чеков, которые могут быть полезны при калибровке шрифтов в макетах чеков с определенными принтерами MICR.</span><span class="sxs-lookup"><span data-stu-id="6036b-156">The following summarizes specifications for check security fonts that may be useful when calibrating fonts to be on check layouts with specific MICR printers.</span></span>

<span data-ttu-id="6036b-157">![Спецификации шрифтов безопасности чеков](media/font_check-security-font_Specifications.png "Спецификации шрифтов безопасности чеков")</span><span class="sxs-lookup"><span data-stu-id="6036b-157">![Check Security Font Specifications](media/font_check-security-font_Specifications.png "Check Security Font Specifications")</span></span>

<span data-ttu-id="6036b-158">Полную спецификацию шрифтов безопасности чеков можно найти в документации поставщика здесь: ( https://www.idautomation.com/security-fonts/).</span><span class="sxs-lookup"><span data-stu-id="6036b-158">The full specification of check security fonts can be found in the supplier's documentation here: (https://www.idautomation.com/security-fonts/).</span></span>

<span data-ttu-id="6036b-159">Шрифты для других целей также доступны в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="6036b-159">Fonts for other purposes are also available in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="6036b-160">Для получения дополнительной информации см. [Доступные шрифты](ui-fonts.md)</span><span class="sxs-lookup"><span data-stu-id="6036b-160">For more information, see [Available Fonts](ui-fonts.md)</span></span>

## <a name="see-also"></a><span data-ttu-id="6036b-161">См. также</span><span class="sxs-lookup"><span data-stu-id="6036b-161">See Also</span></span>
[<span data-ttu-id="6036b-162">Создание и изменение пользовательских макетов отчетов</span><span class="sxs-lookup"><span data-stu-id="6036b-162">Create and Modify Custom Report Layouts</span></span>](ui-how-create-custom-report-layout.md)  
[<span data-ttu-id="6036b-163">Шрифты в Business Central</span><span class="sxs-lookup"><span data-stu-id="6036b-163">Fonts in Business Central</span></span>](ui-fonts.md)  
[<span data-ttu-id="6036b-164">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="6036b-164">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="6036b-165">[Выверка банковских счетов](bank-manage-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="6036b-165">[Reconciling Bank Accounts](bank-manage-bank-accounts.md) </span></span>  
[<span data-ttu-id="6036b-166">Выполнение процессов завершения периода</span><span class="sxs-lookup"><span data-stu-id="6036b-166">Completing Period-End Processes</span></span>](year-how-complete-period-end-processes.md)  
<span data-ttu-id="6036b-167">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6036b-167">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="6036b-168">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="6036b-168">General Business Functionality</span></span>](ui-across-business-areas.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]