---
title: Обзор задач по настройке процессов продаж | Документация Майкрософт
description: Описываются задачи по настройке правил и значений для определения политик и процессов продаж.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell, configure
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: f344fb03f1447681676d5e1e13294bc7cefccb96
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775404"
---
# <a name="setting-up-sales"></a><span data-ttu-id="67c7c-103">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="67c7c-103">Setting Up Sales</span></span>
<span data-ttu-id="67c7c-104">Прежде чем приступать к управлению процессами продажи, необходимо настроить правила и значения, которые определяют политики продажи в организации.</span><span class="sxs-lookup"><span data-stu-id="67c7c-104">Before you can manage sales processes, you must configure the rules and values that define the company's sales policies.</span></span>

<span data-ttu-id="67c7c-105">Необходимо определить общие параметры настройки, например необходимые документы продажи и порядок учета их значений.</span><span class="sxs-lookup"><span data-stu-id="67c7c-105">You must define the general setup, such as which sales documents are required and how their values are posted.</span></span> <span data-ttu-id="67c7c-106">Эта общая настройка обычно выполняется один раз в ходе начального внедрения.</span><span class="sxs-lookup"><span data-stu-id="67c7c-106">This general setup is typically performed once during the initial implementation.</span></span>

<span data-ttu-id="67c7c-107">Отдельная серия задач, связанных с регистрацией новых клиентов, заключается в регистрации любых соглашений по цене и предоставлению скидок, заключенных с каждым клиентом.</span><span class="sxs-lookup"><span data-stu-id="67c7c-107">A separate series of tasks related to registering new customers is to record any special price or discount agreements that you have with each customer.</span></span>

<span data-ttu-id="67c7c-108">Настройка параметров продаж, связанных с финансами, например способов оплаты и валют, рассмотрены в разделе "Настройка финансов".</span><span class="sxs-lookup"><span data-stu-id="67c7c-108">Finance-related sales setup, such as payment methods and currencies, are covered in the Finance Setup section.</span></span> <span data-ttu-id="67c7c-109">Дополнительные сведения см. в разделе [Настройка финансов](finance-setup-finance.md).</span><span class="sxs-lookup"><span data-stu-id="67c7c-109">For more information, see [Setting Up Finance](finance-setup-finance.md).</span></span>

| <span data-ttu-id="67c7c-110">Действие</span><span class="sxs-lookup"><span data-stu-id="67c7c-110">To</span></span> | <span data-ttu-id="67c7c-111">Ссылка</span><span class="sxs-lookup"><span data-stu-id="67c7c-111">See</span></span> |
| --- | --- |
| <span data-ttu-id="67c7c-112">Создание карточки клиента для каждого клиента, которому осуществляется продажа.</span><span class="sxs-lookup"><span data-stu-id="67c7c-112">Create a customer card for each customer that you sell to.</span></span> |[<span data-ttu-id="67c7c-113">Регистрация новых клиентов</span><span class="sxs-lookup"><span data-stu-id="67c7c-113">Register New Customers</span></span>](sales-how-register-new-customers.md) |
| <span data-ttu-id="67c7c-114">Разрешите клиентам платить через PayPal, выбрав значок PayPal на документах продажи.</span><span class="sxs-lookup"><span data-stu-id="67c7c-114">Enable customers to pay through PayPal by choosing the PayPal logo on sales documents.</span></span> |[<span data-ttu-id="67c7c-115">Включение платежей клиентов через PayPal</span><span class="sxs-lookup"><span data-stu-id="67c7c-115">Enable Customer Payment Through PayPal</span></span>](sales-how-enable-payment-service-extensions.md) |
| <span data-ttu-id="67c7c-116">Ввод различных скидок и специальных цен, которые применяются к клиентам в зависимости от товара, количества и/или даты.</span><span class="sxs-lookup"><span data-stu-id="67c7c-116">Enter the different discounts and special prices that you grant to customers depending on item, quantities, and/or date.</span></span> |[<span data-ttu-id="67c7c-117">Регистрация соглашений о цене продажи, скидках и платежах</span><span class="sxs-lookup"><span data-stu-id="67c7c-117">Record Sales Price, Discount, and Payment Agreements</span></span>](sales-how-record-sales-price-discount-payment-agreements.md) |
| <span data-ttu-id="67c7c-118">Настройте менеджеров по продажам таким образом, чтобы вы могли назначать их контактным лицам клиента и изменять производительность менеджеров для расчета комиссионных от продажи или премий.</span><span class="sxs-lookup"><span data-stu-id="67c7c-118">Set up salespeople so that you can assign them to customer contacts or measure salespeople's performance as a basis for calculating the sales commission or bonus.</span></span> |[<span data-ttu-id="67c7c-119">Настройка менеджеров по продажам</span><span class="sxs-lookup"><span data-stu-id="67c7c-119">Set Up Salespeople</span></span>](sales-how-setup-salespeople.md) |
| <span data-ttu-id="67c7c-120">Определите для отдельных клиентов или для всех клиентов, как документы продажи должны по умолчанию отправлять при выборе действия **Учесть и отправить**.</span><span class="sxs-lookup"><span data-stu-id="67c7c-120">Specify for individual customers or for all customers how sales documents are sent by default when you choose the **Post and Send** action.</span></span> |[<span data-ttu-id="67c7c-121">Настройка профилей отправки документов</span><span class="sxs-lookup"><span data-stu-id="67c7c-121">Set Up Document Sending Profiles</span></span>](sales-how-setup-document-send-profiles.md) |
| <span data-ttu-id="67c7c-122">Настройте электронную почту, чтобы она содержала сводные сведения об отправляемом документе продажи.</span><span class="sxs-lookup"><span data-stu-id="67c7c-122">Set your email up to contain a summary of information in the sales document that is being sent.</span></span> |<span data-ttu-id="67c7c-123">[Отправка документов по электронной почте](ui-how-send-documents-email.md).</span><span class="sxs-lookup"><span data-stu-id="67c7c-123">[Send Documents by Email](ui-how-send-documents-email.md).</span></span> |
|<span data-ttu-id="67c7c-124">Использование веб-службы ЕС для проверки ИНН клиента.</span><span class="sxs-lookup"><span data-stu-id="67c7c-124">Use an EU web service to verify a customer's VAT registration number.</span></span>|[<span data-ttu-id="67c7c-125">Проверка регистрационных номеров НДС</span><span class="sxs-lookup"><span data-stu-id="67c7c-125">Verify VAT Registration Numbers</span></span>](finance-setup-vat.md)|
|<span data-ttu-id="67c7c-126">Определите различные условия, которые вы предлагаете клиентам или которые предлагают вам ваши поставщики.</span><span class="sxs-lookup"><span data-stu-id="67c7c-126">Define the different incoterms that you offer to customers or that your vendors offer you.</span></span>|[<span data-ttu-id="67c7c-127">Настройка методов отгрузки</span><span class="sxs-lookup"><span data-stu-id="67c7c-127">Set Up Shipment Methods</span></span>](sales-how-set-up-shipment-methods.md)|
|<span data-ttu-id="67c7c-128">Ввести сведения о различных используемых перевозчиках, включая ссылки на их службу отслеживания пакетов.</span><span class="sxs-lookup"><span data-stu-id="67c7c-128">Enter information about the different transportation vendors you use, including a link to their package tracking service.</span></span>|[<span data-ttu-id="67c7c-129">Настройка экспедиторов</span><span class="sxs-lookup"><span data-stu-id="67c7c-129">Set Up Shipping Agents</span></span>](sales-how-to-set-up-shipping-agents.md)|
|<span data-ttu-id="67c7c-130">Укажите отчеты по умолчанию, которые будут использоваться для различных типов документов.</span><span class="sxs-lookup"><span data-stu-id="67c7c-130">Specify default reports to be used for different document types.</span></span>|[<span data-ttu-id="67c7c-131">Выбор отчета в Business Central</span><span class="sxs-lookup"><span data-stu-id="67c7c-131">Report Selection in Business Central</span></span>](across-report-selections.md)|

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="67c7c-132">См. соответствующее обучение на странице [Microsoft Learn](/learn/paths/trade-get-started-dynamics-365-business-central/)</span><span class="sxs-lookup"><span data-stu-id="67c7c-132">See Related Training at [Microsoft Learn](/learn/paths/trade-get-started-dynamics-365-business-central/)</span></span>

## <a name="see-also"></a><span data-ttu-id="67c7c-133">См. также</span><span class="sxs-lookup"><span data-stu-id="67c7c-133">See Also</span></span>
[<span data-ttu-id="67c7c-134">Продажи</span><span class="sxs-lookup"><span data-stu-id="67c7c-134">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="67c7c-135">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="67c7c-135">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]