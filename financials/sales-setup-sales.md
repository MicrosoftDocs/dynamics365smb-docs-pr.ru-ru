---
title: "Обзор задач по настройке процессов продаж | Документы Майкрософт"
description: "Описываются задачи по настройке правил и значений для определения политик и процессов продаж."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell, configure
ms.date: 06/01/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 75ed584feda066a6c412f861bd624646c4c31085
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="setting-up-sales"></a><span data-ttu-id="cfab7-103">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="cfab7-103">Setting Up Sales</span></span>
<span data-ttu-id="cfab7-104">Прежде чем приступать к управлению процессами продажи, необходимо настроить правила и значения, которые определяют политики продажи в организации.</span><span class="sxs-lookup"><span data-stu-id="cfab7-104">Before you can manage sales processes, you must configure the rules and values that define the company's sales policies.</span></span>

<span data-ttu-id="cfab7-105">Необходимо определить общие параметры настройки, например необходимые документы продажи и порядок учета их значений.</span><span class="sxs-lookup"><span data-stu-id="cfab7-105">You must define the general setup, such as which sales documents are required and how their values are posted.</span></span> <span data-ttu-id="cfab7-106">Эта общая настройка обычно выполняется один раз в ходе начального внедрения.</span><span class="sxs-lookup"><span data-stu-id="cfab7-106">This general setup is typically performed once during the initial implementation.</span></span>

<span data-ttu-id="cfab7-107">Отдельная серия задач, связанных с регистрацией новых клиентов, заключается в регистрации любых соглашений по цене и предоставлению скидок, заключенных с каждым клиентом.</span><span class="sxs-lookup"><span data-stu-id="cfab7-107">A separate series of tasks related to registering new customers is to record any special price or discount agreements that you have with each customer.</span></span>

<span data-ttu-id="cfab7-108">Настройка параметров продаж, связанных с финансами, например способов оплаты и валют, рассмотрены в разделе "Настройка финансов".</span><span class="sxs-lookup"><span data-stu-id="cfab7-108">Finance-related sales setup, such as payment methods and currencies, are covered in the Finance Setup section.</span></span> <span data-ttu-id="cfab7-109">Дополнительные сведения см. в разделе [Настройка финансов](finance-setup-finance.md).</span><span class="sxs-lookup"><span data-stu-id="cfab7-109">For more information, see [Setting Up Finance](finance-setup-finance.md).</span></span>

| <span data-ttu-id="cfab7-110">Действие</span><span class="sxs-lookup"><span data-stu-id="cfab7-110">To</span></span> | <span data-ttu-id="cfab7-111">Ссылка</span><span class="sxs-lookup"><span data-stu-id="cfab7-111">See</span></span> |
| --- | --- |
| <span data-ttu-id="cfab7-112">Создание карточки клиента для каждого клиента, которому осуществляется продажа.</span><span class="sxs-lookup"><span data-stu-id="cfab7-112">Create a customer card for each customer that you sell to.</span></span> |[<span data-ttu-id="cfab7-113">Практическое руководство. Регистрация новых клиентов</span><span class="sxs-lookup"><span data-stu-id="cfab7-113">How to: Register New Customers</span></span>](sales-how-register-new-customers.md) |
| <span data-ttu-id="cfab7-114">Разрешите клиентам платить через PayPal, выбрав значок PayPal на документах продажи.</span><span class="sxs-lookup"><span data-stu-id="cfab7-114">Enable customers to pay through PayPal by choosing the PayPal logo on sales documents.</span></span> |[<span data-ttu-id="cfab7-115">Практическое руководство. Включение платежей клиентов через PayPal</span><span class="sxs-lookup"><span data-stu-id="cfab7-115">How to: Enable Customer Payment Through PayPal</span></span>](sales-how-enable-payment-service-extensions.md) |
| <span data-ttu-id="cfab7-116">Ввод различных скидок и специальных цен, которые применяются к клиентам в зависимости от товара, количества и/или даты.</span><span class="sxs-lookup"><span data-stu-id="cfab7-116">Enter the different discounts and special prices that you grant to customers depending on item, quantities, and/or date.</span></span> |[<span data-ttu-id="cfab7-117">Практическое руководство. Регистрация соглашений о цене продажи, скидках и платежах</span><span class="sxs-lookup"><span data-stu-id="cfab7-117">How to: Record Sales Price, Discount, and Payment Agreements</span></span>](sales-how-record-sales-price-discount-payment-agreements.md) |
| <span data-ttu-id="cfab7-118">Настройте менеджеров по продажам таким образом, чтобы вы могли назначать их контактным лицам клиента и изменять производительность менеджеров для расчета комиссионных от продажи или премий.</span><span class="sxs-lookup"><span data-stu-id="cfab7-118">Set up salespeople so that you can assign them to customer contacts or measure salespeople's performance as a basis for calculating the sales commission or bonus.</span></span> |[<span data-ttu-id="cfab7-119">Практическое руководство. Настройка менеджеров по продажам</span><span class="sxs-lookup"><span data-stu-id="cfab7-119">How to: Set Up Salespeople</span></span>](sales-how-setup-salespeople.md) |
| <span data-ttu-id="cfab7-120">Определите для отдельных клиентов или для всех клиентов, как документы продажи должны по умолчанию отправлять при выборе действия **Учесть и отправить**.</span><span class="sxs-lookup"><span data-stu-id="cfab7-120">Specify for individual customers or for all customers how sales documents are sent by default when you choose the **Post and Send** action.</span></span> |[<span data-ttu-id="cfab7-121">Практическое руководство. Настройка профилей отправки документов</span><span class="sxs-lookup"><span data-stu-id="cfab7-121">How to: Set Up Document Sending Profiles</span></span>](sales-how-setup-document-send-profiles.md) |
| <span data-ttu-id="cfab7-122">Настройте электронную почту, чтобы она содержала сводные сведения об отправляемом документе продажи.</span><span class="sxs-lookup"><span data-stu-id="cfab7-122">Set your email up to contain a summary of information in the sales document that is being sent.</span></span> |<span data-ttu-id="cfab7-123">[Практическое руководство. Отправка документов по электронной почте](ui-how-send-documents-email.md)</span><span class="sxs-lookup"><span data-stu-id="cfab7-123">[How to: Send Documents by Email](ui-how-send-documents-email.md).</span></span> |

## <a name="see-also"></a><span data-ttu-id="cfab7-124">См. также</span><span class="sxs-lookup"><span data-stu-id="cfab7-124">See Also</span></span>
[<span data-ttu-id="cfab7-125">Продажи</span><span class="sxs-lookup"><span data-stu-id="cfab7-125">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="cfab7-126">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="cfab7-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

