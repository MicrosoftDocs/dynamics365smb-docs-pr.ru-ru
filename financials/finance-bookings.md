---
title: "Выставление счетов по резервированиям в Dynamics 365 | Документы Майкрософт"
description: "Узнайте, как массово выставлять счета из Microsoft Bookings в Dynamics 365 for Financials."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: invoicing, bookings
ms.date: 06/14/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 1f1a1645ba27a3b42d67c11f7472c283ca44dbd1
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="bulk-invoicing-for-microsoft-bookings-in-included365finincludesd365finmdmd"></a><span data-ttu-id="f7379-103">Массовое выставление счетов для Microsoft Bookings в [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="f7379-103">Bulk Invoicing for Microsoft Bookings in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
<span data-ttu-id="f7379-104">Если ваша организация использует приложение Bookings в Office 365, вы можете массово выставлять счета для назначений.</span><span class="sxs-lookup"><span data-stu-id="f7379-104">If your company uses the Bookings app in Office 365, you can do bulk invoicing for appointments.</span></span> <span data-ttu-id="f7379-105">На странице **Bookings без выставления счета** в [!INCLUDE[d365fin](includes/d365fin_md.md)] представлен список завершенных резервирований организации.</span><span class="sxs-lookup"><span data-stu-id="f7379-105">The **Uninvoiced Bookings** page in [!INCLUDE[d365fin](includes/d365fin_md.md)] provides a list of the company's completed bookings.</span></span> <span data-ttu-id="f7379-106">На этой странице можно быстро выбрать назначения, по которым требуется создать счет, и создать черновики счетов за оказанные услуги.</span><span class="sxs-lookup"><span data-stu-id="f7379-106">In this page you can quickly select the appointments that you want to invoice and create draft invoices for the services provided.</span></span>  

## <a name="connect-to-bookings"></a><span data-ttu-id="f7379-107">Подклчюение к Bookings</span><span class="sxs-lookup"><span data-stu-id="f7379-107">Connect to Bookings</span></span>
<span data-ttu-id="f7379-108">Чтобы связать [!INCLUDE[d365fin](includes/d365fin_md.md)] с Bookings, следует указать свою организацию Bookings, которую нужно синхронизировать с Bookings, периодичность синхронизации и шаблоны, которые требуется использовать.</span><span class="sxs-lookup"><span data-stu-id="f7379-108">To connect your [!INCLUDE[d365fin](includes/d365fin_md.md)] with Bookings, you must specify your Bookings company, what to synchronize with Bookings, how often to synchronize, and which templates to use.</span></span> <span data-ttu-id="f7379-109">Эти сведения настраиваются на странице **Настройка синхронизации Bookings**, которую можно запустить со страницы **Настройка синхронизации с Exchange**, которую можно найти в разделе [Поиск](ui-search.md).</span><span class="sxs-lookup"><span data-stu-id="f7379-109">You set up this information in the **Booking Sync. Setup** page, which you can launch from the **Exchange Sync. Setup** page, which you can find through [Search](ui-search.md).</span></span>  

<span data-ttu-id="f7379-110">Например, если вы хотите синхронизировать клиентов между Bookings и [!INCLUDE[d365fin](includes/d365fin_md.md)], следует задать шаблон по умолчанию, который будет использоваться для добавления клиентов в [!INCLUDE[d365fin](includes/d365fin_md.md)] на основании клиентов из организации Bookings.</span><span class="sxs-lookup"><span data-stu-id="f7379-110">For example, if you want to synchronize customers between Bookings and [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the default template to use to add new customers in [!INCLUDE[d365fin](includes/d365fin_md.md)] based on the customers in your Bookings company.</span></span>  

## <a name="invoice-appointments"></a><span data-ttu-id="f7379-111">Выставить счета по назначениям</span><span class="sxs-lookup"><span data-stu-id="f7379-111">Invoice Appointments</span></span>
<span data-ttu-id="f7379-112">Когда придет время отправки счетов за завершенные резервирования, откройте страницу **Bookings без выставления счета**.</span><span class="sxs-lookup"><span data-stu-id="f7379-112">When it is time to send invoices for the completed bookings, you go to the **Uninvoiced Bookings** page.</span></span> <span data-ttu-id="f7379-113">В зависимости от того, как часто синхронизируется информация, список может быть длинным или коротким.</span><span class="sxs-lookup"><span data-stu-id="f7379-113">Depending on how often the information is synchronized, the list is long or short.</span></span> <span data-ttu-id="f7379-114">Вы можете создать счета для всех резервирований в списке или по одному резервированию за раз.</span><span class="sxs-lookup"><span data-stu-id="f7379-114">You can create invoices for all bookings in the list or one booking at a time.</span></span> <span data-ttu-id="f7379-115">Вы можете выбрать одну или несколько операций в списке и выставить счета только по ним.</span><span class="sxs-lookup"><span data-stu-id="f7379-115">You can select one or more entries in the list and invoice those only.</span></span>  

<span data-ttu-id="f7379-116">Поддержка выставления счетов по назначениям в Bookings проще, чем полны рабочий процесс с предложениями продажи, заказами на продажу и счетами продажи.</span><span class="sxs-lookup"><span data-stu-id="f7379-116">The support for invoicing appointments from Bookings is simpler than the fuller workflow of working with sales quotes, sales orders, and sales invoices.</span></span> <span data-ttu-id="f7379-117">Дополнительные сведения см. в разделе [Практическое руководство. Выставление счетов продажи](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="f7379-117">For more information, see [How to: Invoice Sales](sales-how-invoice-sales.md).</span></span> <span data-ttu-id="f7379-118">Вы можете продавать свои услуги через [!INCLUDE[d365fin](includes/d365fin_md.md)] или выбрать Bookings в зависимости от потребностей бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f7379-118">You can choose to sell your services using [!INCLUDE[d365fin](includes/d365fin_md.md)] or choose to use Bookings, depending on your business needs.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f7379-119">См. также</span><span class="sxs-lookup"><span data-stu-id="f7379-119">See Also</span></span>
[<span data-ttu-id="f7379-120">Финансы</span><span class="sxs-lookup"><span data-stu-id="f7379-120">Finance</span></span>](finance.md)  
[<span data-ttu-id="f7379-121">Практическое руководство. Выставление счетов продажи</span><span class="sxs-lookup"><span data-stu-id="f7379-121">How to: Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="f7379-122">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="f7379-122">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="f7379-123">Microsoft Bookings</span><span class="sxs-lookup"><span data-stu-id="f7379-123">Microsoft Bookings</span></span>](https://products.office.com/en-us/business/scheduling-and-booking-app)  

