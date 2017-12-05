---
title: "Выставление счетов по резервированиям в Dynamics 365 | Microsoft Docs"
description: "Узнайте, как массово выставлять счета из Microsoft Bookings в Dynamics 365 Business edition."
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
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 154a4719cdd0e28280c5b0a5de85479beb0b9262
ms.contentlocale: ru-ru
ms.lasthandoff: 11/10/2017

---
# <a name="bulk-invoicing-for-microsoft-bookings-in-included365finincludesd365finmdmd"></a>Массовое выставление счетов для Microsoft Bookings в [!INCLUDE[d365fin](includes/d365fin_md.md)]
Если ваша организация использует приложение Bookings в Office 365, вы можете массово выставлять счета для назначений. На странице **Bookings без выставления счета** в [!INCLUDE[d365fin](includes/d365fin_md.md)] представлен список завершенных резервирований организации. На этой странице можно быстро выбрать назначения, по которым требуется создать счет, и создать черновики счетов за оказанные услуги.  

## <a name="connect-to-bookings"></a>Подклчюение к Bookings
Чтобы связать [!INCLUDE[d365fin](includes/d365fin_md.md)] с Bookings, следует указать свою организацию Bookings, которую нужно синхронизировать с Bookings, периодичность синхронизации и шаблоны, которые требуется использовать. Эти сведения настраиваются на странице **Настройка синхронизации Bookings**, которую можно запустить со страницы **Настройка синхронизации с Exchange**, которую можно найти в разделе [Поиск](ui-search.md).  

Например, если вы хотите синхронизировать клиентов между Bookings и [!INCLUDE[d365fin](includes/d365fin_md.md)], следует задать шаблон по умолчанию, который будет использоваться для добавления клиентов в [!INCLUDE[d365fin](includes/d365fin_md.md)] на основании клиентов из организации Bookings.  

## <a name="invoice-appointments"></a>Выставить счета по назначениям
Когда придет время отправки счетов за завершенные резервирования, откройте страницу **Bookings без выставления счета**. В зависимости от того, как часто синхронизируется информация, список может быть длинным или коротким. Вы можете создать счета для всех резервирований в списке или по одному резервированию за раз. Вы можете выбрать одну или несколько операций в списке и выставить счета только по ним.  

Поддержка выставления счетов по назначениям в Bookings проще, чем полны рабочий процесс с предложениями продажи, заказами на продажу и счетами продажи. Дополнительные сведения см. в разделе [Практическое руководство. Выставление счетов продажи](sales-how-invoice-sales.md). Вы можете продавать свои услуги через [!INCLUDE[d365fin](includes/d365fin_md.md)] или выбрать Bookings в зависимости от потребностей бизнеса.  

## <a name="see-also"></a>См. также
[Финансы](finance.md)  
[Практическое руководство. Выставление счетов продажи](sales-how-invoice-sales.md)  
[Настройка продаж](sales-setup-sales.md)  
[Microsoft Bookings](https://products.office.com/en-us/business/scheduling-and-booking-app)  

