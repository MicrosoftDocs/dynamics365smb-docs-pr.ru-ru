---
title: "Выставление счетов по резервированиям в Finance and Operations, Business edition | Microsoft Docs"
description: "Узнайте, как массово выставлять счета из Microsoft Bookings в Finance and Operations, Business edition."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: invoicing, bookings
ms.date: 06/14/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: d387bbbf59550a6ca11dff534b76683a07808ca4
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="bulk-invoicing-for-microsoft-bookings-in-included365finincludesd365finmdmd"></a><span data-ttu-id="56349-103">Массовое выставление счетов для Microsoft Bookings в [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="56349-103">Bulk Invoicing for Microsoft Bookings in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
<span data-ttu-id="56349-104">Если ваша организация использует приложение Bookings в Office 365, вы можете массово выставлять счета для назначений.</span><span class="sxs-lookup"><span data-stu-id="56349-104">If your company uses the Bookings app in Office 365, you can do bulk invoicing for appointments.</span></span> <span data-ttu-id="56349-105">На странице **Bookings без выставления счета** в [!INCLUDE[d365fin](includes/d365fin_md.md)] представлен список завершенных резервирований организации.</span><span class="sxs-lookup"><span data-stu-id="56349-105">The **Uninvoiced Bookings** page in [!INCLUDE[d365fin](includes/d365fin_md.md)] provides a list of the company's completed bookings.</span></span> <span data-ttu-id="56349-106">На этой странице можно быстро выбрать назначения, по которым требуется создать счет, и создать черновики счетов за оказанные услуги.</span><span class="sxs-lookup"><span data-stu-id="56349-106">In this page you can quickly select the appointments that you want to invoice and create draft invoices for the services provided.</span></span>  

## <a name="connect-to-bookings"></a><span data-ttu-id="56349-107">Подклчюение к Bookings</span><span class="sxs-lookup"><span data-stu-id="56349-107">Connect to Bookings</span></span>
<span data-ttu-id="56349-108">Чтобы связать [!INCLUDE[d365fin](includes/d365fin_md.md)] с Bookings, следует указать свою организацию Bookings, которую нужно синхронизировать с Bookings, периодичность синхронизации и шаблоны, которые требуется использовать.</span><span class="sxs-lookup"><span data-stu-id="56349-108">To connect your [!INCLUDE[d365fin](includes/d365fin_md.md)] with Bookings, you must specify your Bookings company, what to synchronize with Bookings, how often to synchronize, and which templates to use.</span></span> <span data-ttu-id="56349-109">Эти сведения настраиваются на странице **Настройка синхронизации Bookings**, которую можно запустить со страницы **Настройка синхронизации с Exchange**, которую можно найти в разделе [Поиск](ui-search.md).</span><span class="sxs-lookup"><span data-stu-id="56349-109">You set up this information in the **Booking Sync. Setup** page, which you can launch from the **Exchange Sync. Setup** page, which you can find through [Search](ui-search.md).</span></span>  

<span data-ttu-id="56349-110">Например, если вы хотите синхронизировать клиентов между Bookings и [!INCLUDE[d365fin](includes/d365fin_md.md)], следует задать шаблон по умолчанию, который будет использоваться для добавления клиентов в [!INCLUDE[d365fin](includes/d365fin_md.md)] на основании клиентов из организации Bookings.</span><span class="sxs-lookup"><span data-stu-id="56349-110">For example, if you want to synchronize customers between Bookings and [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the default template to use to add new customers in [!INCLUDE[d365fin](includes/d365fin_md.md)] based on the customers in your Bookings company.</span></span>  

## <a name="invoice-appointments"></a><span data-ttu-id="56349-111">Выставить счета по назначениям</span><span class="sxs-lookup"><span data-stu-id="56349-111">Invoice Appointments</span></span>
<span data-ttu-id="56349-112">Когда придет время отправки счетов за завершенные резервирования, откройте страницу **Bookings без выставления счета**.</span><span class="sxs-lookup"><span data-stu-id="56349-112">When it is time to send invoices for the completed bookings, you go to the **Uninvoiced Bookings** page.</span></span> <span data-ttu-id="56349-113">В зависимости от того, как часто синхронизируется информация, список может быть длинным или коротким.</span><span class="sxs-lookup"><span data-stu-id="56349-113">Depending on how often the information is synchronized, the list is long or short.</span></span> <span data-ttu-id="56349-114">Вы можете создать счета для всех резервирований в списке или по одному резервированию за раз.</span><span class="sxs-lookup"><span data-stu-id="56349-114">You can create invoices for all bookings in the list or one booking at a time.</span></span> <span data-ttu-id="56349-115">Вы можете выбрать одну или несколько операций в списке и выставить счета только по ним.</span><span class="sxs-lookup"><span data-stu-id="56349-115">You can select one or more entries in the list and invoice those only.</span></span>  

<span data-ttu-id="56349-116">Поддержка выставления счетов по назначениям в Bookings проще, чем полны рабочий процесс с предложениями продажи, заказами на продажу и счетами продажи.</span><span class="sxs-lookup"><span data-stu-id="56349-116">The support for invoicing appointments from Bookings is simpler than the fuller workflow of working with sales quotes, sales orders, and sales invoices.</span></span> <span data-ttu-id="56349-117">Дополнительные сведения см. в разделе [Выставление счетов продажи](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="56349-117">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span></span> <span data-ttu-id="56349-118">Вы можете продавать свои услуги через [!INCLUDE[d365fin](includes/d365fin_md.md)] или выбрать Bookings в зависимости от потребностей бизнеса.</span><span class="sxs-lookup"><span data-stu-id="56349-118">You can choose to sell your services using [!INCLUDE[d365fin](includes/d365fin_md.md)] or choose to use Bookings, depending on your business needs.</span></span>  

## <a name="see-also"></a><span data-ttu-id="56349-119">См. также</span><span class="sxs-lookup"><span data-stu-id="56349-119">See Also</span></span>
[<span data-ttu-id="56349-120">Финансы</span><span class="sxs-lookup"><span data-stu-id="56349-120">Finance</span></span>](finance.md)  
[<span data-ttu-id="56349-121">Выставление счетов продажи</span><span class="sxs-lookup"><span data-stu-id="56349-121">Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="56349-122">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="56349-122">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="56349-123">Microsoft Bookings</span><span class="sxs-lookup"><span data-stu-id="56349-123">Microsoft Bookings</span></span>](https://products.office.com/en-us/business/scheduling-and-booking-app)  

