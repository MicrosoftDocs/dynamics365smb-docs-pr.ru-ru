---
title: "Сведения о проектировании — планирование поставок | Документы Майкрософт"
description: "Этот раздел содержит обзор концепций и принципов, используемых в функциях планирования поставок в [!INCLUDE[d365fin](includes/d365fin_md.md)]."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, supply, planning, reordering, replenishment
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: b8a44ff374338c79bd2e1aa31ee60e172f06da5e
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-supply-planning"></a><span data-ttu-id="3bd9e-103">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="3bd9e-103">Design Details: Supply Planning</span></span>
<span data-ttu-id="3bd9e-104">Документация содержит подробные технические сведения о концепциях и принципах, используемых в функциях планирования поставок в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3bd9e-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Supply Planning features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="3bd9e-105">В ней описывается, как работает система планирования и как скорректировать алгоритмы для выполнения требований планирования в различных средах.</span><span class="sxs-lookup"><span data-stu-id="3bd9e-105">It explains how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span></span> <span data-ttu-id="3bd9e-106">Сначала приводятся основные понятия решений, а затем описывается логика центрального механизма, балансировка поставок и выполнение планирования запасов с использованием политик дозаказа.</span><span class="sxs-lookup"><span data-stu-id="3bd9e-106">It first introduces central solution concepts and then describes the logic of the central mechanism, supply balancing, before proceeding to explain how inventory planning is performed with the use of reordering policies.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="3bd9e-107">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="3bd9e-107">In This Section</span></span>  
[<span data-ttu-id="3bd9e-108">Сведения о проектировании: основные понятия системы планирования</span><span class="sxs-lookup"><span data-stu-id="3bd9e-108">Design Details: Central Concepts of the Planning System</span></span>](design-details-central-concepts-of-the-planning-system.md)  
[<span data-ttu-id="3bd9e-109">Сведения о проектировании: резервирование, трассировка заказов и отправка сообщений о действиях</span><span class="sxs-lookup"><span data-stu-id="3bd9e-109">Design Details: Reservation, Order Tracking, and Action Messaging</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
[<span data-ttu-id="3bd9e-110">Сведения о проектировании: балансировка спроса и поставки</span><span class="sxs-lookup"><span data-stu-id="3bd9e-110">Design Details: Balancing Demand and Supply</span></span>](design-details-balancing-demand-and-supply.md)  
[<span data-ttu-id="3bd9e-111">Сведения о проектировании: обработка политик дозаказа</span><span class="sxs-lookup"><span data-stu-id="3bd9e-111">Design Details: Handling Reordering Policies</span></span>](design-details-handling-reordering-policies.md)  
[<span data-ttu-id="3bd9e-112">Сведения о проектировании: параметры планирования</span><span class="sxs-lookup"><span data-stu-id="3bd9e-112">Design Details: Planning Parameters</span></span>](design-details-planning-parameters.md)  
[<span data-ttu-id="3bd9e-113">Сведения о проектировании: таблица "Назначение произ. плана"</span><span class="sxs-lookup"><span data-stu-id="3bd9e-113">Design Details: Planning Assignment Table</span></span>](design-details-planning-assignment-table.md)  
[<span data-ttu-id="3bd9e-114">Сведения о проектировании: спрос на пустом складе</span><span class="sxs-lookup"><span data-stu-id="3bd9e-114">Design Details: Demand at Blank Location</span></span>](design-details-demand-at-blank-location.md)  
[<span data-ttu-id="3bd9e-115">Сведения о проектировании: перемещения при планировании</span><span class="sxs-lookup"><span data-stu-id="3bd9e-115">Design Details: Transfers in Planning</span></span>](design-details-transfers-in-planning.md)

