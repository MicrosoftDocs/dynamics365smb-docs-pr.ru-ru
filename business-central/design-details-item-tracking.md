---
title: Сведения о проектировании — трассировки товара | Документация Майкрософт
description: В этом разделе приводится обзор сведений о проектировании трассировки товаров.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 50ae6f2f3538269cc7c82dd2d84644a1a31d7f56
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4751359"
---
# <a name="design-details-item-tracking"></a><span data-ttu-id="e3b93-103">Сведения о проектировании: трассировка товара</span><span class="sxs-lookup"><span data-stu-id="e3b93-103">Design Details: Item Tracking</span></span>
<span data-ttu-id="e3b93-104">По мере усложнения потока товаров в текущей цепочке поставок организациям становится все более важно иметь возможность отслеживать товары.</span><span class="sxs-lookup"><span data-stu-id="e3b93-104">As the flow of goods in today’s supply chain becomes more and more complex, the ability to keep track of items is increasingly important to the companies involved.</span></span> <span data-ttu-id="e3b93-105">Отслеживание потока транзакций по товару — это юридическое требование в сфере медицинских и химических поставок, но в других бизнес-сферах может потребоваться отслеживать продукты с гарантиями или сроками годности в целях обслуживания клиентов.</span><span class="sxs-lookup"><span data-stu-id="e3b93-105">Monitoring an item’s transaction flow is a legal requirement in the business of medical and chemical supply, but other businesses may want to monitor products with warranties or expiration dates for customer service reasons.</span></span>  

<span data-ttu-id="e3b93-106">Система трассировки товаров должна предоставлять организации простые функции обработки серийных номеров и номеров партий, учитывая особенности каждой уникальной штуки товара: время и место получения, а также время и место продажи.</span><span class="sxs-lookup"><span data-stu-id="e3b93-106">An item tracking system should provide a company with easy handling of serial and lot numbers, considering each unique piece of merchandise: when and where received, where stored, when and where sold.</span></span> <span data-ttu-id="e3b93-107">В [!INCLUDE[prod_short](includes/prod_short.md)] постепенно были добавлены функции для выполнения этого бизнес-требования, и на данный момент программа предоставляет общие для приложений функциональные возможности и надежную базу для разработки расширений.</span><span class="sxs-lookup"><span data-stu-id="e3b93-107">[!INCLUDE[prod_short](includes/prod_short.md)] has gradually expanded its coverage of this business requirement and today provides application-wide functionality and a solid core on which to develop extensions.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="e3b93-108">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="e3b93-108">In This Section</span></span>  
[<span data-ttu-id="e3b93-109">Сведения о проектировании: разработка трассировки товара</span><span class="sxs-lookup"><span data-stu-id="e3b93-109">Design Details: Item Tracking Design</span></span>](design-details-item-tracking-design.md)  
[<span data-ttu-id="e3b93-110">Сведения о проектировании: структура учета трассировки товаров</span><span class="sxs-lookup"><span data-stu-id="e3b93-110">Design Details: Item Tracking Posting Structure</span></span>](design-details-item-tracking-posting-structure.md)  
[<span data-ttu-id="e3b93-111">Сведения о проектировании: активные и исторические операции трассировки товаров</span><span class="sxs-lookup"><span data-stu-id="e3b93-111">Design Details: Active versus Historic Item Tracking Entries</span></span>](design-details-active-versus-historic-item-tracking-entries.md)  
[<span data-ttu-id="e3b93-112">Сведения о проектировании: — страница "Строки трассировки товаров"</span><span class="sxs-lookup"><span data-stu-id="e3b93-112">Design Details: Item Tracking Lines Page</span></span>](design-details-item-tracking-lines-window.md)  
[<span data-ttu-id="e3b93-113">Сведения о проектировании: доступность трассировки товара</span><span class="sxs-lookup"><span data-stu-id="e3b93-113">Design Details: Item Tracking Availability</span></span>](design-details-item-tracking-availability.md)  
[<span data-ttu-id="e3b93-114">Сведения о проектировании: трассировка и планирование товара</span><span class="sxs-lookup"><span data-stu-id="e3b93-114">Design Details: Item Tracking and Planning</span></span>](design-details-item-tracking-and-planning.md)  
[<span data-ttu-id="e3b93-115">Сведения о проектировании: трассировка и резервирование товара</span><span class="sxs-lookup"><span data-stu-id="e3b93-115">Design Details: Item Tracking and Reservations</span></span>](design-details-item-tracking-and-reservations.md)  
[<span data-ttu-id="e3b93-116">Сведения о проектировании: трассировка товара на складе</span><span class="sxs-lookup"><span data-stu-id="e3b93-116">Design Details: Item Tracking in the Warehouse</span></span>](design-details-item-tracking-in-the-warehouse.md)
