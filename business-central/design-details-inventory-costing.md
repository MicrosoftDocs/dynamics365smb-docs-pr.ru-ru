---
title: Сведения о проектировании — себестоимость запасов | Документация Майкрософт
description: Документация содержит подробные технические сведения о концепциях и принципах, используемых в функциях учета стоимости товаров в Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, inventory, costing
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 8bfcf2b10d9b302c9a65b7cf27c7fb336be68617
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215982"
---
# <a name="design-details-inventory-costing"></a><span data-ttu-id="02987-103">Сведения о проектировании: себестоимость запасов</span><span class="sxs-lookup"><span data-stu-id="02987-103">Design Details: Inventory Costing</span></span>
<span data-ttu-id="02987-104">Документация содержит подробные технические сведения о концепциях и принципах, используемых в функциях учета стоимости товаров в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="02987-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  

<span data-ttu-id="02987-105">Учет себестоимости запасов, который также называют управлением затратами, связан с записью и отчетностью по текущим бизнес-расходам.</span><span class="sxs-lookup"><span data-stu-id="02987-105">Inventory costing, also referred to as cost management, is concerned with recording and reporting business operating costs.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="02987-106">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="02987-106">In This Section</span></span>  
[<span data-ttu-id="02987-107">Сведения о проектировании: методы учета себестоимости</span><span class="sxs-lookup"><span data-stu-id="02987-107">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)  
[<span data-ttu-id="02987-108">Сведения о проектировании: применение товара</span><span class="sxs-lookup"><span data-stu-id="02987-108">Design Details: Item Application</span></span>](design-details-item-application.md)  
[<span data-ttu-id="02987-109">Сведения о проектировании: известная проблема применения товара</span><span class="sxs-lookup"><span data-stu-id="02987-109">Design Details: Known Item Application Issue</span></span>](design-details-inventory-zero-level-open-item-ledger-entries.md)  
[<span data-ttu-id="02987-110">Сведения о проектировании: коррекция себестоимости</span><span class="sxs-lookup"><span data-stu-id="02987-110">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)  
[<span data-ttu-id="02987-111">Подробности разработки: дата учета для операции коррекции стоимости</span><span class="sxs-lookup"><span data-stu-id="02987-111">Design Details: Posting Date on Adjustment Value Entry</span></span>](design-details-inventory-adjustment-value-entry-posting-date.md)  
[<span data-ttu-id="02987-112">Сведения о проектировании: учет ожидаемой себестоимости</span><span class="sxs-lookup"><span data-stu-id="02987-112">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)  
[<span data-ttu-id="02987-113">Сведения о проектировании: средняя себестоимость</span><span class="sxs-lookup"><span data-stu-id="02987-113">Design Details: Average Cost</span></span>](design-details-average-cost.md)  
[<span data-ttu-id="02987-114">Сведения о проектировании: отклонение</span><span class="sxs-lookup"><span data-stu-id="02987-114">Design Details: Variance</span></span>](design-details-variance.md)  
[<span data-ttu-id="02987-115">Сведения о проектировании: округление</span><span class="sxs-lookup"><span data-stu-id="02987-115">Design Details: Rounding</span></span>](design-details-rounding.md)  
[<span data-ttu-id="02987-116">Сведения о проектировании: компоненты себестоимости</span><span class="sxs-lookup"><span data-stu-id="02987-116">Design Details: Cost Components</span></span>](design-details-cost-components.md)  
[<span data-ttu-id="02987-117">Сведения о проектировании: периоды учета запасов</span><span class="sxs-lookup"><span data-stu-id="02987-117">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="02987-118">Сведения о проектировании: учет запасов</span><span class="sxs-lookup"><span data-stu-id="02987-118">Design Details: Inventory Posting</span></span>](design-details-inventory-posting.md)  
[<span data-ttu-id="02987-119">Сведения о проектировании: учет производственного заказа</span><span class="sxs-lookup"><span data-stu-id="02987-119">Design Details: Production Order Posting</span></span>](design-details-production-order-posting.md)  
[<span data-ttu-id="02987-120">Сведения о проектировании: учет заказа на сборку</span><span class="sxs-lookup"><span data-stu-id="02987-120">Design Details: Assembly Order Posting</span></span>](design-details-assembly-order-posting.md)  
[<span data-ttu-id="02987-121">Сведения о проектировании: выверка с главной книгой</span><span class="sxs-lookup"><span data-stu-id="02987-121">Design Details: Reconciliation with the General Ledger</span></span>](design-details-reconciliation-with-the-general-ledger.md)  
[<span data-ttu-id="02987-122">Сведения о проектировании: счета в главной книге</span><span class="sxs-lookup"><span data-stu-id="02987-122">Design Details: Accounts in the General Ledger</span></span>](design-details-accounts-in-the-general-ledger.md)  
[<span data-ttu-id="02987-123">Сведения о проектировании: оценка стоимости запасов</span><span class="sxs-lookup"><span data-stu-id="02987-123">Design Details: Inventory Valuation</span></span>](design-details-inventory-valuation.md)  
[<span data-ttu-id="02987-124">Сведения о проектировании: переоценка</span><span class="sxs-lookup"><span data-stu-id="02987-124">Design Details: Revaluation</span></span>](design-details-revaluation.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]