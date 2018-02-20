---
title: "О затратах на завершенные производственные заказы | Документы Майкрософт"
description: "Завершение производственного заказа - это важная задача в выполнении жизненного цикла изготавливаемого товара. Окончательные издержки, включая отклонения в среде стандартной себестоимости, фактические данные в среде себестоимости FIFO, средней себестоимости или себестоимости LIFO, вычисляются с помощью пакетного задания **Коррекция себест. запасов**."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 010d4d4568f45cbe8fe13864ac6996de1e224b76
ms.contentlocale: ru-ru
ms.lasthandoff: 12/14/2017

---
# <a name="about-finished-production-order-costs"></a><span data-ttu-id="e7fd9-104">О затратах на завершенные производственные заказы</span><span class="sxs-lookup"><span data-stu-id="e7fd9-104">About Finished Production Order Costs</span></span>
<span data-ttu-id="e7fd9-105">Завершение производственного заказа - это важная задача в выполнении жизненного цикла изготавливаемого товара.</span><span class="sxs-lookup"><span data-stu-id="e7fd9-105">Finishing the production order is an important task in completing the costing lifecycle of the item that is being produced.</span></span> <span data-ttu-id="e7fd9-106">Окончательные издержки, включая отклонения в среде стандартной себестоимости, фактические данные в среде себестоимости FIFO, средней себестоимости или себестоимости LIFO, вычисляются с помощью пакетного задания **Коррекция себест. запасов**, которое допускает финансовую выверку себестоимости производства товара.</span><span class="sxs-lookup"><span data-stu-id="e7fd9-106">Final costs, including variances in a standard cost environment, actuals in a FIFO, Average, or LIFO cost environment, are calculated using the **Adjust Cost - Item Entries** batch job, which allows for financial reconciliation of the costs of item production.</span></span> <span data-ttu-id="e7fd9-107">Чтобы производственный заказ считался заказом, подлежащим коррекции себестоимости, его статус должен быть **Завершен**.</span><span class="sxs-lookup"><span data-stu-id="e7fd9-107">For a production order to be considered for cost adjustment, the status must be **Finished**.</span></span> <span data-ttu-id="e7fd9-108">Поэтому очень важно, чтобы при завершении статус производственного заказа менялся на **Завершен**.</span><span class="sxs-lookup"><span data-stu-id="e7fd9-108">It is therefore critical that upon completion, the status of a production order is changed to **Finished**.</span></span>  

## <a name="example"></a><span data-ttu-id="e7fd9-109">Пример</span><span class="sxs-lookup"><span data-stu-id="e7fd9-109">Example</span></span>  
 <span data-ttu-id="e7fd9-110">В среде стандартной себестоимости при потреблении материалов для производства товара, себестоимость товара плюс оплата труда и накладные расходы учитываются в НЗП.</span><span class="sxs-lookup"><span data-stu-id="e7fd9-110">In a standard cost environment, when you consume material to produce an item, stated simply, the cost of the item plus labor and overhead go into WIP.</span></span> <span data-ttu-id="e7fd9-111">Когда товар будет произведен, НЗП уменьшается на сумму стандартной себестоимости товара.</span><span class="sxs-lookup"><span data-stu-id="e7fd9-111">When the item is produced, WIP is reduced by the amount of the standard cost of the item.</span></span> <span data-ttu-id="e7fd9-112">Обычно эти издержки не дают в итоге нулевое значение.</span><span class="sxs-lookup"><span data-stu-id="e7fd9-112">Typically, these costs do not net to zero.</span></span> <span data-ttu-id="e7fd9-113">Чтобы эти издержки стали нулевыми, необходимо выполнить пакетное задание **Коррекция себест. запасов**, при этом для корректировки будут учитываться только производственные заказы со статусом **Завершено**.</span><span class="sxs-lookup"><span data-stu-id="e7fd9-113">So that these costs can net to zero, you must run the **Adjust Cost - Item Entries** batch job, noting that only production orders with the status of **Finished** will be considered for adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e7fd9-114">См. также</span><span class="sxs-lookup"><span data-stu-id="e7fd9-114">See Also</span></span>  
[<span data-ttu-id="e7fd9-115">Управление себестоимостью товаров</span><span class="sxs-lookup"><span data-stu-id="e7fd9-115">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="e7fd9-116">Производство</span><span class="sxs-lookup"><span data-stu-id="e7fd9-116">Manufacturing</span></span>](production-manage-manufacturing.md)  
<span data-ttu-id="e7fd9-117">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e7fd9-117">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

