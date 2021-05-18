---
title: Выбор отчета в Business Central
description: Узнайте, как настроить отчеты, которые вы используете для печати различных типов документов в Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: setup, reporting
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: ba15a65317ebf52579c285c93dd59eba1b65ae1b
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5787111"
---
# <a name="report-selection-in-business-central"></a><span data-ttu-id="cb663-103">Выбор отчета в Business Central</span><span class="sxs-lookup"><span data-stu-id="cb663-103">Report Selection in Business Central</span></span>

<span data-ttu-id="cb663-104">Вы можете настроить отчеты по умолчанию, которые будут использоваться для печати различных документов для покупок и продаж, таких как заказы, предложения, счета и кредит-ноты.</span><span class="sxs-lookup"><span data-stu-id="cb663-104">You can set up default reports that will be used to print the various documents for sales and purchases, such as orders, quotes, invoices, and credit memos.</span></span> <span data-ttu-id="cb663-105">Например, если у вас есть особый макет для счетов на продажу, вы можете указать этот отчет на странице **Выбор отчетов — продажи**, чтобы его можно было использовать для отправки или печати счетов на продажу.</span><span class="sxs-lookup"><span data-stu-id="cb663-105">For example, if you have a specific layout for sales invoices, you can specify that report in the **Report Selections - Sales** page so that it will be used to send or print sales invoices.</span></span>  

<span data-ttu-id="cb663-106">Страницы **Выбор отчета** указывают, какие отчеты будут распечатаны в различных ситуациях.</span><span class="sxs-lookup"><span data-stu-id="cb663-106">The **Report Selections** pages specify which report will be printed in different situations.</span></span> <span data-ttu-id="cb663-107">[!INCLUDE [prod_short](includes/prod_short.md)] включает конфигурации по умолчанию, но, конечно, вы можете изменить эти значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cb663-107">[!INCLUDE [prod_short](includes/prod_short.md)] includes default configurations, but of course you can change these defaults.</span></span> <span data-ttu-id="cb663-108">Можно также добавлять отчеты на страницы **Выбор отчета**, если вы хотите печатать более одного отчета на каждый тип документов, например.</span><span class="sxs-lookup"><span data-stu-id="cb663-108">You can also add reports to the **Report Selection** pages if you want to print more than one report per document type, for example.</span></span>  

## <a name="available-report-selections"></a><span data-ttu-id="cb663-109">Доступный выбор отчетов</span><span class="sxs-lookup"><span data-stu-id="cb663-109">Available report selections</span></span>

<span data-ttu-id="cb663-110">[!INCLUDE [prod_short](includes/prod_short.md)] включает в себя различные страницы **Выбор отчета** для разных областей.</span><span class="sxs-lookup"><span data-stu-id="cb663-110">[!INCLUDE [prod_short](includes/prod_short.md)] includes different **Report Selection** pages for different areas.</span></span> <span data-ttu-id="cb663-111">В следующих таблицах описано, где можно найти информацию о различных страницах.</span><span class="sxs-lookup"><span data-stu-id="cb663-111">The following tables describes where you can find information about the different pages.</span></span>  

|<span data-ttu-id="cb663-112">Область или задача</span><span class="sxs-lookup"><span data-stu-id="cb663-112">Area or task</span></span>  |<span data-ttu-id="cb663-113">Узнать больше</span><span class="sxs-lookup"><span data-stu-id="cb663-113">Learn more</span></span>|
|--------------|----------|
|<span data-ttu-id="cb663-114">Пример того, как работает выбор отчета (продажи)</span><span class="sxs-lookup"><span data-stu-id="cb663-114">Example of how report selection works (Sales)</span></span>|[<span data-ttu-id="cb663-115">Выбор отчета для документов на продажу</span><span class="sxs-lookup"><span data-stu-id="cb663-115">Report selection for sales documents</span></span>](#example-report-selection-for-sales-documents)|
|<span data-ttu-id="cb663-116">Макет по умолчанию для сообщений электронной почты с документами на продажу или покупку</span><span class="sxs-lookup"><span data-stu-id="cb663-116">Default layout for emails with sales and purchase documents</span></span>  |[<span data-ttu-id="cb663-117">Настройка многоразовых текстов и макетов электронной почты для документов продажи и закупок</span><span class="sxs-lookup"><span data-stu-id="cb663-117">Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents</span></span>](admin-how-setup-email.md#set-up-reusable-email-texts-and-layouts-for-sales-and-purchase-documents) |
|<span data-ttu-id="cb663-118">Определение макетов платежных документов</span><span class="sxs-lookup"><span data-stu-id="cb663-118">Define check layouts</span></span>     |[<span data-ttu-id="cb663-119">Выбор макета платежного документа</span><span class="sxs-lookup"><span data-stu-id="cb663-119">Select a Check Layout</span></span>](finance-how-define-check-layouts.md) |
|<span data-ttu-id="cb663-120">Определение отчетов для отчетности по НДС (Германия)</span><span class="sxs-lookup"><span data-stu-id="cb663-120">Define reports for VAT reporting (Germany)</span></span>|[<span data-ttu-id="cb663-121">Настройка отчетов по НДС и Интрастат</span><span class="sxs-lookup"><span data-stu-id="cb663-121">Set Up Reports for VAT and Intrastat</span></span>](LocalFunctionality/Germany/how-to-set-up-reports-for-vat-and-intrastat.md) |

> [!TIP]
> <span data-ttu-id="cb663-122">Ваш [!INCLUDE [prod_short](includes/prod_short.md)] может включать дополнительные страницы **Выбор отчета**, например, в зависимости от вашего местоположения и отрасли.</span><span class="sxs-lookup"><span data-stu-id="cb663-122">Your [!INCLUDE [prod_short](includes/prod_short.md)] can include additional **Report Selection** pages, depending on your location and industry, for example.</span></span> <span data-ttu-id="cb663-123">Вы всегда можете проверить свою настройку, выбрав значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Выбор отчетов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="cb663-123">You can always check your setup by choosing the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, entering **Report Selections**, and then choose the relevant link.</span></span>

<span data-ttu-id="cb663-124">Версия по умолчанию [!INCLUDE [prod_short](includes/prod_short.md)] включает следующие страницы **Раздел отчета**:</span><span class="sxs-lookup"><span data-stu-id="cb663-124">The default version of [!INCLUDE [prod_short](includes/prod_short.md)] includes the following **Report Section** pages:</span></span>

* <span data-ttu-id="cb663-125">**Выбор отчета - продажи**</span><span class="sxs-lookup"><span data-stu-id="cb663-125">**Report Selection - Sales**</span></span>  
* <span data-ttu-id="cb663-126">**Выбор отчета - покупка**</span><span class="sxs-lookup"><span data-stu-id="cb663-126">**Report Selection - Purchase**</span></span>  
* <span data-ttu-id="cb663-127">**Выбор отчетов - склад**</span><span class="sxs-lookup"><span data-stu-id="cb663-127">**Report Selection - Inventory**</span></span>  
* <span data-ttu-id="cb663-128">**Выбор отчета - движение денежных средств**</span><span class="sxs-lookup"><span data-stu-id="cb663-128">**Report Selection - Cash Flow**</span></span>  
* <span data-ttu-id="cb663-129">**Выбор отчета — склад**</span><span class="sxs-lookup"><span data-stu-id="cb663-129">**Report Selection - Warehouse**</span></span>  
* <span data-ttu-id="cb663-130">**Выбор отчета — банковский счет**</span><span class="sxs-lookup"><span data-stu-id="cb663-130">**Report Selection - Bank Account**</span></span>  
* <span data-ttu-id="cb663-131">**Выбор отчетов — напоминание/процент-нота**</span><span class="sxs-lookup"><span data-stu-id="cb663-131">**Report Selections Reminder/Finance Charge**</span></span>  

## <a name="example-report-selection-for-sales-documents"></a><span data-ttu-id="cb663-132">Пример. Выбор отчета для документов на продажу</span><span class="sxs-lookup"><span data-stu-id="cb663-132">Example: Report selection for sales documents</span></span>

<span data-ttu-id="cb663-133">Страница **Выбор отчета - продажи** определяет отчеты по умолчанию, которые будут использоваться в различных сценариях для каждого связанного типа документа.</span><span class="sxs-lookup"><span data-stu-id="cb663-133">The **Report Selection - Sales** page defines the default reports to use in different scenarios for each related document type.</span></span> <span data-ttu-id="cb663-134">Выберите тип документа в поле **Применение**, затем добавьте или просмотрите выбранный отчет.</span><span class="sxs-lookup"><span data-stu-id="cb663-134">Choose a document type in the **Usage** field, and then add or review the report selection.</span></span> <span data-ttu-id="cb663-135">Вы можете настроить более одного отчета и порядок их отправки или распечатки.</span><span class="sxs-lookup"><span data-stu-id="cb663-135">You can set up more than one report and the order of sequence that the reports must be sent or printed in.</span></span>  

[!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="cb663-136">Некоторые типы документов могут быть отправлены как вложения электронной почты, а другие — нет.</span><span class="sxs-lookup"><span data-stu-id="cb663-136">Some types of document can be sent as email attachments, and others cannot.</span></span> <span data-ttu-id="cb663-137">Каждая страница **Выбор отчета** показывает дополнительные поля, если тип поддерживает электронную почту из коробки.</span><span class="sxs-lookup"><span data-stu-id="cb663-137">Each **Report Selection** page shows additional fields if the type support email out of the box.</span></span>  

<span data-ttu-id="cb663-138">Например, на страницах **Выбор отчета - продажи** и **Выбор отчета - покупка**, следующие поля помогут вам настроить электронную почту:</span><span class="sxs-lookup"><span data-stu-id="cb663-138">For example, in the **Report Selection - Sales** and **Report Selection - Purchase** pages, the following fields help you set up emailing:</span></span>

|<span data-ttu-id="cb663-139">Имя поля</span><span class="sxs-lookup"><span data-stu-id="cb663-139">Field name</span></span> |<span data-ttu-id="cb663-140">Описание</span><span class="sxs-lookup"><span data-stu-id="cb663-140">Description</span></span>  |
|-----------|-------------|
|<span data-ttu-id="cb663-141">**Использовать для содержания сообщения электронной почты**</span><span class="sxs-lookup"><span data-stu-id="cb663-141">**Use for Email Body**</span></span>| <span data-ttu-id="cb663-142">Определяет сводные сведения, такие как номер счета, срок оплаты, ссылка на службу платежей, которые будут вставлены в текст отправляемого сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cb663-142">Specifies that summarized information, such as invoice number, due date, and payment service link, will be inserted in the body of the email that you send.</span></span>        |
|<span data-ttu-id="cb663-143">**Использовать для вложения в сообщение электронной почты**</span><span class="sxs-lookup"><span data-stu-id="cb663-143">**Use for Email Attachment**</span></span>| <span data-ttu-id="cb663-144">Указывает, что связанный документ будет вложен в сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cb663-144">Specifies that the related document will be attached to the email.</span></span>|
|<span data-ttu-id="cb663-145">**Описание макета содержания сообщения электронной почты**</span><span class="sxs-lookup"><span data-stu-id="cb663-145">**Email Body Layout Description**</span></span>|<span data-ttu-id="cb663-146">Задает используемый макет текста сообщения электронной почты, обычно это настраиваемый макет отчета.</span><span class="sxs-lookup"><span data-stu-id="cb663-146">Specifies the email body layout that is used, typically a custom report layout.</span></span> |

## <a name="see-also"></a><span data-ttu-id="cb663-147">См. также</span><span class="sxs-lookup"><span data-stu-id="cb663-147">See also</span></span>

[<span data-ttu-id="cb663-148">Настройка многоразовых текстов и макетов электронной почты для документов продажи и закупок</span><span class="sxs-lookup"><span data-stu-id="cb663-148">Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents</span></span>](admin-how-setup-email.md#set-up-reusable-email-texts-and-layouts-for-sales-and-purchase-documents)  
[<span data-ttu-id="cb663-149">Выбор макета платежного документа</span><span class="sxs-lookup"><span data-stu-id="cb663-149">Select a Check Layout</span></span>](finance-how-define-check-layouts.md)  
[<span data-ttu-id="cb663-150">Настройка отчетов по НДС и Интрастат (Германия)</span><span class="sxs-lookup"><span data-stu-id="cb663-150">Set Up Reports for VAT and Intrastat (Germany)</span></span>](LocalFunctionality/Germany/how-to-set-up-reports-for-vat-and-intrastat.md)  
[<span data-ttu-id="cb663-151">Управление макетами отчетов и документов</span><span class="sxs-lookup"><span data-stu-id="cb663-151">Managing Report and Document Layouts</span></span>](ui-manage-report-layouts.md)  
[<span data-ttu-id="cb663-152">Определение макетов документов для клиентов и поставщиков</span><span class="sxs-lookup"><span data-stu-id="cb663-152">Define Document Layouts for Customers and Vendors</span></span>](ui-define-customer-vendor-document-layouts.md)  
[<span data-ttu-id="cb663-153">Настройка принтеров</span><span class="sxs-lookup"><span data-stu-id="cb663-153">Set Up Printers</span></span>](ui-specify-printer-selection-reports.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]