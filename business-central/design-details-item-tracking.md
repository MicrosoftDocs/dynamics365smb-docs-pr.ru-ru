---
title: Сведения о проектировании — трассировки товара | Документация Майкрософт
description: В этом разделе приводится обзор сведений о проектировании трассировки товаров.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: b263abf09a3d74bbac4f8b94c4dde61644702bfc
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2303200"
---
# <a name="design-details-item-tracking"></a><span data-ttu-id="df285-103">Сведения о проектировании: трассировка товара</span><span class="sxs-lookup"><span data-stu-id="df285-103">Design Details: Item Tracking</span></span>
<span data-ttu-id="df285-104">По мере усложнения потока товаров в текущей цепочке поставок организациям становится все более важно иметь возможность отслеживать товары.</span><span class="sxs-lookup"><span data-stu-id="df285-104">As the flow of goods in today’s supply chain becomes more and more complex, the ability to keep track of items is increasingly important to the companies involved.</span></span> <span data-ttu-id="df285-105">Отслеживание потока транзакций по товару — это юридическое требование в сфере медицинских и химических поставок, но в других бизнес-сферах может потребоваться отслеживать продукты с гарантиями или сроками годности в целях обслуживания клиентов.</span><span class="sxs-lookup"><span data-stu-id="df285-105">Monitoring an item’s transaction flow is a legal requirement in the business of medical and chemical supply, but other businesses may want to monitor products with warranties or expiration dates for customer service reasons.</span></span>  

<span data-ttu-id="df285-106">Система трассировки товаров должна предоставлять организации простые функции обработки серийных номеров и номеров партий, учитывая особенности каждой уникальной штуки товара: время и место получения, а также время и место продажи.</span><span class="sxs-lookup"><span data-stu-id="df285-106">An item tracking system should provide a company with easy handling of serial and lot numbers, considering each unique piece of merchandise: when and where received, where stored, when and where sold.</span></span> <span data-ttu-id="df285-107">В [!INCLUDE[d365fin](includes/d365fin_md.md)] постепенно были добавлены функции для выполнения этого бизнес-требования, и на данный момент программа предоставляет общие для приложений функциональные возможности и надежную базу для разработки расширений.</span><span class="sxs-lookup"><span data-stu-id="df285-107">[!INCLUDE[d365fin](includes/d365fin_md.md)] has gradually expanded its coverage of this business requirement and today provides application-wide functionality and a solid core on which to develop extensions.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="df285-108">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="df285-108">In This Section</span></span>  
[<span data-ttu-id="df285-109">Сведения о проектировании: разработка трассировки товара</span><span class="sxs-lookup"><span data-stu-id="df285-109">Design Details: Item Tracking Design</span></span>](design-details-item-tracking-design.md)  
[<span data-ttu-id="df285-110">Сведения о проектировании: структура учета трассировки товаров</span><span class="sxs-lookup"><span data-stu-id="df285-110">Design Details: Item Tracking Posting Structure</span></span>](design-details-item-tracking-posting-structure.md)  
[<span data-ttu-id="df285-111">Сведения о проектировании: активные и исторические операции трассировки товаров</span><span class="sxs-lookup"><span data-stu-id="df285-111">Design Details: Active versus Historic Item Tracking Entries</span></span>](design-details-active-versus-historic-item-tracking-entries.md)  
[<span data-ttu-id="df285-112">Сведения о проектировании: — страница "Строки трассировки товаров"</span><span class="sxs-lookup"><span data-stu-id="df285-112">Design Details: Item Tracking Lines Page</span></span>](design-details-item-tracking-lines-window.md)  
[<span data-ttu-id="df285-113">Сведения о проектировании: доступность трассировки товара</span><span class="sxs-lookup"><span data-stu-id="df285-113">Design Details: Item Tracking Availability</span></span>](design-details-item-tracking-availability.md)  
[<span data-ttu-id="df285-114">Сведения о проектировании: трассировка и планирование товара</span><span class="sxs-lookup"><span data-stu-id="df285-114">Design Details: Item Tracking and Planning</span></span>](design-details-item-tracking-and-planning.md)  
[<span data-ttu-id="df285-115">Сведения о проектировании: трассировка и резервирование товара</span><span class="sxs-lookup"><span data-stu-id="df285-115">Design Details: Item Tracking and Reservations</span></span>](design-details-item-tracking-and-reservations.md)  
[<span data-ttu-id="df285-116">Сведения о проектировании: трассировка товара на складе</span><span class="sxs-lookup"><span data-stu-id="df285-116">Design Details: Item Tracking in the Warehouse</span></span>](design-details-item-tracking-in-the-warehouse.md)
