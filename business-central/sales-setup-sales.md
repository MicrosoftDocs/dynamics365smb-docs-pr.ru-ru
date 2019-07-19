---
title: Обзор задач по настройке процессов продаж | Microsoft Docs
description: Описываются задачи по настройке правил и значений для определения политик и процессов продаж.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell, configure
ms.date: 06/17/2019
ms.author: sgroespe
ms.openlocfilehash: 3ece1edb7ba18cb96099cba34065c96164390e82
ms.sourcegitcommit: 6dc83b27ac47f3b39a7b84cfb7446e7f48b8ce63
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2019
ms.locfileid: "1632710"
---
# <a name="setting-up-sales"></a><span data-ttu-id="328a9-103">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="328a9-103">Setting Up Sales</span></span>
<span data-ttu-id="328a9-104">Прежде чем приступать к управлению процессами продажи, необходимо настроить правила и значения, которые определяют политики продажи в организации.</span><span class="sxs-lookup"><span data-stu-id="328a9-104">Before you can manage sales processes, you must configure the rules and values that define the company's sales policies.</span></span>

<span data-ttu-id="328a9-105">Необходимо определить общие параметры настройки, например необходимые документы продажи и порядок учета их значений.</span><span class="sxs-lookup"><span data-stu-id="328a9-105">You must define the general setup, such as which sales documents are required and how their values are posted.</span></span> <span data-ttu-id="328a9-106">Эта общая настройка обычно выполняется один раз в ходе начального внедрения.</span><span class="sxs-lookup"><span data-stu-id="328a9-106">This general setup is typically performed once during the initial implementation.</span></span>

<span data-ttu-id="328a9-107">Отдельная серия задач, связанных с регистрацией новых клиентов, заключается в регистрации любых соглашений по цене и предоставлению скидок, заключенных с каждым клиентом.</span><span class="sxs-lookup"><span data-stu-id="328a9-107">A separate series of tasks related to registering new customers is to record any special price or discount agreements that you have with each customer.</span></span>

<span data-ttu-id="328a9-108">Настройка параметров продаж, связанных с финансами, например способов оплаты и валют, рассмотрены в разделе "Настройка финансов".</span><span class="sxs-lookup"><span data-stu-id="328a9-108">Finance-related sales setup, such as payment methods and currencies, are covered in the Finance Setup section.</span></span> <span data-ttu-id="328a9-109">Дополнительные сведения см. в разделе [Настройка финансов](finance-setup-finance.md).</span><span class="sxs-lookup"><span data-stu-id="328a9-109">For more information, see [Setting Up Finance](finance-setup-finance.md).</span></span>

| <span data-ttu-id="328a9-110">Действие</span><span class="sxs-lookup"><span data-stu-id="328a9-110">To</span></span> | <span data-ttu-id="328a9-111">Ссылка</span><span class="sxs-lookup"><span data-stu-id="328a9-111">See</span></span> |
| --- | --- |
| <span data-ttu-id="328a9-112">Создание карточки клиента для каждого клиента, которому осуществляется продажа.</span><span class="sxs-lookup"><span data-stu-id="328a9-112">Create a customer card for each customer that you sell to.</span></span> |[<span data-ttu-id="328a9-113">Регистрация новых клиентов</span><span class="sxs-lookup"><span data-stu-id="328a9-113">Register New Customers</span></span>](sales-how-register-new-customers.md) |
| <span data-ttu-id="328a9-114">Разрешите клиентам платить через PayPal, выбрав значок PayPal на документах продажи.</span><span class="sxs-lookup"><span data-stu-id="328a9-114">Enable customers to pay through PayPal by choosing the PayPal logo on sales documents.</span></span> |[<span data-ttu-id="328a9-115">Включение платежей клиентов через PayPal</span><span class="sxs-lookup"><span data-stu-id="328a9-115">Enable Customer Payment Through PayPal</span></span>](sales-how-enable-payment-service-extensions.md) |
| <span data-ttu-id="328a9-116">Ввод различных скидок и специальных цен, которые применяются к клиентам в зависимости от товара, количества и/или даты.</span><span class="sxs-lookup"><span data-stu-id="328a9-116">Enter the different discounts and special prices that you grant to customers depending on item, quantities, and/or date.</span></span> |[<span data-ttu-id="328a9-117">Регистрация соглашений о цене продажи, скидках и платежах</span><span class="sxs-lookup"><span data-stu-id="328a9-117">Record Sales Price, Discount, and Payment Agreements</span></span>](sales-how-record-sales-price-discount-payment-agreements.md) |
| <span data-ttu-id="328a9-118">Настройте менеджеров по продажам таким образом, чтобы вы могли назначать их контактным лицам клиента и изменять производительность менеджеров для расчета комиссионных от продажи или премий.</span><span class="sxs-lookup"><span data-stu-id="328a9-118">Set up salespeople so that you can assign them to customer contacts or measure salespeople's performance as a basis for calculating the sales commission or bonus.</span></span> |[<span data-ttu-id="328a9-119">Настройка менеджеров по продажам</span><span class="sxs-lookup"><span data-stu-id="328a9-119">Set Up Salespeople</span></span>](sales-how-setup-salespeople.md) |
| <span data-ttu-id="328a9-120">Определите для отдельных клиентов или для всех клиентов, как документы продажи должны по умолчанию отправлять при выборе действия **Учесть и отправить**.</span><span class="sxs-lookup"><span data-stu-id="328a9-120">Specify for individual customers or for all customers how sales documents are sent by default when you choose the **Post and Send** action.</span></span> |[<span data-ttu-id="328a9-121">Настройка профилей отправки документов</span><span class="sxs-lookup"><span data-stu-id="328a9-121">Set Up Document Sending Profiles</span></span>](sales-how-setup-document-send-profiles.md) |
| <span data-ttu-id="328a9-122">Настройте электронную почту, чтобы она содержала сводные сведения об отправляемом документе продажи.</span><span class="sxs-lookup"><span data-stu-id="328a9-122">Set your email up to contain a summary of information in the sales document that is being sent.</span></span> |<span data-ttu-id="328a9-123">[Отправка документов по электронной почте](ui-how-send-documents-email.md).</span><span class="sxs-lookup"><span data-stu-id="328a9-123">[Send Documents by Email](ui-how-send-documents-email.md).</span></span> |
|<span data-ttu-id="328a9-124">Использование веб-службы ЕС для проверки ИНН клиента.</span><span class="sxs-lookup"><span data-stu-id="328a9-124">Use an EU web service to verify a customer's VAT registration number.</span></span>|[<span data-ttu-id="328a9-125">Проверка регистрационных номеров НДС</span><span class="sxs-lookup"><span data-stu-id="328a9-125">Verify VAT Registration Numbers</span></span>](finance-setup-vat.md)|
|<span data-ttu-id="328a9-126">Определите различные условия, которые вы предлагаете клиентам или которые предлагают вам ваши поставщики.</span><span class="sxs-lookup"><span data-stu-id="328a9-126">Define the different incoterms that you offer to customers or that your vendors offer you.</span></span>|[<span data-ttu-id="328a9-127">Настройка методов отгрузки</span><span class="sxs-lookup"><span data-stu-id="328a9-127">Set Up Shipment Methods</span></span>](sales-how-set-up-shipment-methods.md)|
|<span data-ttu-id="328a9-128">Ввести сведения о различных используемых перевозчиках, включая ссылки на их службу отслеживания пакетов.</span><span class="sxs-lookup"><span data-stu-id="328a9-128">Enter information about the different transportation vendors you use, including a link to their package tracking service.</span></span>|[<span data-ttu-id="328a9-129">Настройка экспедиторов</span><span class="sxs-lookup"><span data-stu-id="328a9-129">Set Up Shipping Agents</span></span>](sales-how-to-set-up-shipping-agents.md)|

## <a name="see-also"></a><span data-ttu-id="328a9-130">См. также</span><span class="sxs-lookup"><span data-stu-id="328a9-130">See Also</span></span>
[<span data-ttu-id="328a9-131">Продажи</span><span class="sxs-lookup"><span data-stu-id="328a9-131">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="328a9-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="328a9-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
