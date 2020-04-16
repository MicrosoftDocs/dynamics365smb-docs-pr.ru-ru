---
title: О затратах на завершенные производственные заказы | Документация Майкрософт
description: Завершение производственного заказа - это важная задача в выполнении жизненного цикла изготавливаемого товара. Окончательные издержки, включая отклонения в среде стандартной себестоимости, фактические данные в среде себестоимости FIFO, средней себестоимости или себестоимости LIFO, вычисляются с помощью пакетного задания Коррекция себест. запасов.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: b33c0aae12374722a3ef5c73db50bbf53a35f39c
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3184128"
---
# <a name="about-finished-production-order-costs"></a><span data-ttu-id="d41d4-104">О затратах на завершенные производственные заказы</span><span class="sxs-lookup"><span data-stu-id="d41d4-104">About Finished Production Order Costs</span></span>
<span data-ttu-id="d41d4-105">Завершение производственного заказа - это важная задача в выполнении жизненного цикла изготавливаемого товара.</span><span class="sxs-lookup"><span data-stu-id="d41d4-105">Finishing the production order is an important task in completing the costing lifecycle of the item that is being produced.</span></span> <span data-ttu-id="d41d4-106">Окончательные издержки, включая отклонения в среде стандартной себестоимости, фактические данные в среде себестоимости FIFO, средней себестоимости или себестоимости LIFO, вычисляются с помощью пакетного задания **Коррекция себест. запасов**, которое допускает финансовую выверку себестоимости производства товара.</span><span class="sxs-lookup"><span data-stu-id="d41d4-106">Final costs, including variances in a standard cost environment, actuals in a FIFO, Average, or LIFO cost environment, are calculated using the **Adjust Cost - Item Entries** batch job, which allows for financial reconciliation of the costs of item production.</span></span> <span data-ttu-id="d41d4-107">Чтобы производственный заказ считался заказом, подлежащим коррекции себестоимости, его статус должен быть **Завершен**.</span><span class="sxs-lookup"><span data-stu-id="d41d4-107">For a production order to be considered for cost adjustment, the status must be **Finished**.</span></span> <span data-ttu-id="d41d4-108">Поэтому очень важно, чтобы при завершении статус производственного заказа менялся на **Завершен**.</span><span class="sxs-lookup"><span data-stu-id="d41d4-108">It is therefore critical that upon completion, the status of a production order is changed to **Finished**.</span></span>  

## <a name="example"></a><span data-ttu-id="d41d4-109">Пример</span><span class="sxs-lookup"><span data-stu-id="d41d4-109">Example</span></span>  
 <span data-ttu-id="d41d4-110">В среде стандартной себестоимости при потреблении материалов для производства товара, себестоимость товара плюс оплата труда и накладные расходы учитываются в НЗП.</span><span class="sxs-lookup"><span data-stu-id="d41d4-110">In a standard cost environment, when you consume material to produce an item, stated simply, the cost of the item plus labor and overhead go into WIP.</span></span> <span data-ttu-id="d41d4-111">Когда товар будет произведен, НЗП уменьшается на сумму стандартной себестоимости товара.</span><span class="sxs-lookup"><span data-stu-id="d41d4-111">When the item is produced, WIP is reduced by the amount of the standard cost of the item.</span></span> <span data-ttu-id="d41d4-112">Обычно эти издержки не дают в итоге нулевое значение.</span><span class="sxs-lookup"><span data-stu-id="d41d4-112">Typically, these costs do not net to zero.</span></span> <span data-ttu-id="d41d4-113">Чтобы эти издержки стали нулевыми, необходимо выполнить пакетное задание **Коррекция себест. запасов**, при этом для корректировки будут учитываться только производственные заказы со статусом **Завершено**.</span><span class="sxs-lookup"><span data-stu-id="d41d4-113">So that these costs can net to zero, you must run the **Adjust Cost - Item Entries** batch job, noting that only production orders with the status of **Finished** will be considered for adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d41d4-114">См. также</span><span class="sxs-lookup"><span data-stu-id="d41d4-114">See Also</span></span>  
[<span data-ttu-id="d41d4-115">Управление себестоимостью товаров</span><span class="sxs-lookup"><span data-stu-id="d41d4-115">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="d41d4-116">Производство</span><span class="sxs-lookup"><span data-stu-id="d41d4-116">Manufacturing</span></span>](production-manage-manufacturing.md)  
<span data-ttu-id="d41d4-117">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d41d4-117">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
