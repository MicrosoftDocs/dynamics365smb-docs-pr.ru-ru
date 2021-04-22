---
title: Выставление счетов по резервированиям в Business Central | Документация Майкрософт
description: Узнайте, как массово выставлять счета из Microsoft Bookings в Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: invoicing, bookings
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 06095fdb0fac291490eeef5a085264ea75581283
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5780861"
---
# <a name="bulk-invoicing-for-microsoft-bookings-in-prod_short"></a>Пакетное выставление счетов для Microsoft Bookings в [!INCLUDE[prod_short](includes/prod_short.md)]
Если ваша организация использует приложение Bookings в Microsoft 365, вы можете массово выставлять счета для назначений. На странице **Bookings без выставления счета** в [!INCLUDE[prod_short](includes/prod_short.md)] представлен список завершенных резервирований организации. На этой странице можно быстро выбрать назначения, по которым требуется создать счет, и создать черновики счетов за оказанные услуги.  

## <a name="connect-to-bookings"></a>Подклчюение к Bookings
Чтобы связать [!INCLUDE[prod_short](includes/prod_short.md)] с Bookings, следует указать свою организацию Bookings, которую нужно синхронизировать с Bookings, периодичность синхронизации и шаблоны, которые требуется использовать. Эти сведения настраиваются на странице **Настройка синхронизации Bookings**, которую можно запустить со страницы **Настройка синхронизации с Exchange**, которую можно найти в разделе [Поиск](ui-search.md).  

Например, если вы хотите синхронизировать клиентов между Bookings и [!INCLUDE[prod_short](includes/prod_short.md)], следует задать шаблон по умолчанию, который будет использоваться для добавления клиентов в [!INCLUDE[prod_short](includes/prod_short.md)] на основании клиентов из организации Bookings.  

> [!NOTE]
> Приложение Bookings разработано для регистрации встреч для индивидуальных клиентов, а не для организаций. Синхронизация с [!INCLUDE[prod_short](includes/prod_short.md)] будет, таким образом, синхронизировать только контакты клиента с типом "Человек". Также требуется адрес электронной почты, чтобы контакт синхронизировался.  

Аналогично, если вы хотите синхронизировать сервисные товары между Bookings и [!INCLUDE[prod_short](includes/prod_short.md)], следует задать шаблон по умолчанию, который будет использоваться для добавления сервисных товаров в [!INCLUDE[prod_short](includes/prod_short.md)] на основании сервисов в вашей организации Bookings.  

> [!NOTE]
> Только товары типа *Сервис* будут синхронизированы между Bookings и [!INCLUDE[prod_short](includes/prod_short.md)]. Шаблон, настраиваемый на странице **Шаблоны конфигурации** таким образом, чтобы его можно было использовать для синхронизации товаров, должен определять тип как *Сервис*.

## <a name="invoice-appointments"></a>Выставить счета по назначениям
Когда придет время отправки счетов за завершенные резервирования, откройте страницу **Bookings без выставления счета**. В зависимости от того, как часто синхронизируется информация, список может быть длинным или коротким. Вы можете создать счета для всех резервирований в списке или по одному резервированию за раз. Вы можете выбрать одну или несколько операций в списке и выставить счета только по ним.  

Поддержка выставления счетов по назначениям в Bookings проще, чем полны рабочий процесс с предложениями продажи, заказами на продажу и счетами продажи. Дополнительные сведения см. в разделе [Выставление счетов продажи](sales-how-invoice-sales.md). Вы можете продавать свои услуги через [!INCLUDE[prod_short](includes/prod_short.md)] или выбрать Bookings в зависимости от потребностей бизнеса.  

## <a name="see-also"></a>См. также
[Финансы](finance.md)  
[Выставление счетов продажи](sales-how-invoice-sales.md)  
[Настройка продаж](sales-setup-sales.md)  
[Microsoft Bookings](https://products.office.com/business/scheduling-and-booking-app)  


[!INCLUDE[footer-include](includes/footer-banner.md)]