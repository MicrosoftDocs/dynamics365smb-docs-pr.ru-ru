---
title: "Сведения о проектировании — себестоимость запасов | Документы Майкрософт"
description: "Документация содержит подробные технические сведения о концепциях и принципах, используемых в функциях учета стоимости товаров в Finance and Operations, Business edition."
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, inventory, costing
ms.date: 11/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 2ee8988a89e4bd01683a6945e66e08ab9608af2e
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-inventory-costing"></a><span data-ttu-id="5c9d2-103">Сведения о проектировании: себестоимость запасов</span><span class="sxs-lookup"><span data-stu-id="5c9d2-103">Design Details: Inventory Costing</span></span>
<span data-ttu-id="5c9d2-104">Документация содержит подробные технические сведения о концепциях и принципах, используемых в функциях учета стоимости товаров в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5c9d2-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="5c9d2-105">Учет себестоимости запасов, который также называют управлением затратами, связан с записью и отчетностью по текущим бизнес-расходам.</span><span class="sxs-lookup"><span data-stu-id="5c9d2-105">Inventory costing, also referred to as cost management, is concerned with recording and reporting business operating costs.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="5c9d2-106">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="5c9d2-106">In This Section</span></span>  
[<span data-ttu-id="5c9d2-107">Сведения о проектировании: методы учета себестоимости</span><span class="sxs-lookup"><span data-stu-id="5c9d2-107">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)  
[<span data-ttu-id="5c9d2-108">Сведения о проектировании: применение товара</span><span class="sxs-lookup"><span data-stu-id="5c9d2-108">Design Details: Item Application</span></span>](design-details-item-application.md)  
[<span data-ttu-id="5c9d2-109">Сведения о проектировании: известная проблема применения товара</span><span class="sxs-lookup"><span data-stu-id="5c9d2-109">Design Details: Known Item Application Issue</span></span>](design-details-inventory-zero-level-open-item-ledger-entries.md)  
[<span data-ttu-id="5c9d2-110">Сведения о проектировании: коррекция себестоимости</span><span class="sxs-lookup"><span data-stu-id="5c9d2-110">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)  
[<span data-ttu-id="5c9d2-111">Подробности разработки: дата учета для операции коррекции стоимости</span><span class="sxs-lookup"><span data-stu-id="5c9d2-111">Design Details: Posting Date on Adjustment Value Entry</span></span>](design-details-inventory-adjustment-value-entry-posting-date.md)  
[<span data-ttu-id="5c9d2-112">Сведения о проектировании: учет ожидаемой себестоимости</span><span class="sxs-lookup"><span data-stu-id="5c9d2-112">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)  
[<span data-ttu-id="5c9d2-113">Сведения о проектировании: средняя себестоимость</span><span class="sxs-lookup"><span data-stu-id="5c9d2-113">Design Details: Average Cost</span></span>](design-details-average-cost.md)  
[<span data-ttu-id="5c9d2-114">Сведения о проектировании: отклонение</span><span class="sxs-lookup"><span data-stu-id="5c9d2-114">Design Details: Variance</span></span>](design-details-variance.md)  
[<span data-ttu-id="5c9d2-115">Сведения о проектировании: округление</span><span class="sxs-lookup"><span data-stu-id="5c9d2-115">Design Details: Rounding</span></span>](design-details-rounding.md)  
[<span data-ttu-id="5c9d2-116">Сведения о проектировании: компоненты себестоимости</span><span class="sxs-lookup"><span data-stu-id="5c9d2-116">Design Details: Cost Components</span></span>](design-details-cost-components.md)  
[<span data-ttu-id="5c9d2-117">Сведения о проектировании: периоды учета запасов</span><span class="sxs-lookup"><span data-stu-id="5c9d2-117">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="5c9d2-118">Сведения о проектировании: учет запасов</span><span class="sxs-lookup"><span data-stu-id="5c9d2-118">Design Details: Inventory Posting</span></span>](design-details-inventory-posting.md)  
[<span data-ttu-id="5c9d2-119">Сведения о проектировании: учет производственного заказа</span><span class="sxs-lookup"><span data-stu-id="5c9d2-119">Design Details: Production Order Posting</span></span>](design-details-production-order-posting.md)  
[<span data-ttu-id="5c9d2-120">Сведения о проектировании: учет заказа на сборку</span><span class="sxs-lookup"><span data-stu-id="5c9d2-120">Design Details: Assembly Order Posting</span></span>](design-details-assembly-order-posting.md)  
[<span data-ttu-id="5c9d2-121">Сведения о проектировании: выверка с главной книгой</span><span class="sxs-lookup"><span data-stu-id="5c9d2-121">Design Details: Reconciliation with the General Ledger</span></span>](design-details-reconciliation-with-the-general-ledger.md)  
[<span data-ttu-id="5c9d2-122">Сведения о проектировании: счета в главной книге</span><span class="sxs-lookup"><span data-stu-id="5c9d2-122">Design Details: Accounts in the General Ledger</span></span>](design-details-accounts-in-the-general-ledger.md)  
[<span data-ttu-id="5c9d2-123">Сведения о проектировании: переоценка</span><span class="sxs-lookup"><span data-stu-id="5c9d2-123">Design Details: Revaluation</span></span>](design-details-revaluation.md)

