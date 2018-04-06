---
title: "Практическое руководство. Учет потребления в пакетном режиме | Документы Майкрософт"
description: "Если выбран метод списания **Вручную**, учет компонентов производится вручную с использованием журнала потребления."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 4058d16ee3bdfc10933e1f3a01c84fbc5d0b0ebb
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="batch-post-production-consumption"></a><span data-ttu-id="97bcb-103">Учет потребления для производства в пакетном режиме</span><span class="sxs-lookup"><span data-stu-id="97bcb-103">Batch Post Production Consumption</span></span>
<span data-ttu-id="97bcb-104">Если выбран метод списания **Вручную**, учет компонентов производится вручную с использованием журнала потребления.</span><span class="sxs-lookup"><span data-stu-id="97bcb-104">If the flushing method is **Manual**, you must post the components manually, using a consumption journal.</span></span>

<span data-ttu-id="97bcb-105">Можно также настроить систему для автоматического учета (*списания*) компонентов при запуске или завершении производственных заказов.</span><span class="sxs-lookup"><span data-stu-id="97bcb-105">You can also set the system up to automatically post (*flush*) components when you start or finish production orders.</span></span> <span data-ttu-id="97bcb-106">Дополнительные сведения см. в разделе [Включение списания компонентов в соответствии с производственным выпуском](production-how-to-flush-components-according-to-operation-output.md).</span><span class="sxs-lookup"><span data-stu-id="97bcb-106">For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).</span></span>

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a><span data-ttu-id="97bcb-107">Учет потребления для одной или нескольких строк производственного заказа</span><span class="sxs-lookup"><span data-stu-id="97bcb-107">To post consumption for one or more production order lines</span></span>  
1.  <span data-ttu-id="97bcb-108">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журнал потребления**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="97bcb-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Consumption Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="97bcb-109">Заполните поля данными производственного заказа и данными о потреблении.</span><span class="sxs-lookup"><span data-stu-id="97bcb-109">Fill in the fields with the production order data and the consumption data.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    <span data-ttu-id="97bcb-110">Если склад, на котором хранятся компоненты, настроен на использование ячеек, но не требует обработки подбора, присвойте код ячейки строке журнала для указания места на складе, откуда должны забираться товары.</span><span class="sxs-lookup"><span data-stu-id="97bcb-110">If the warehouse location where the components are stored is set up to use bins but does not require pick processing, assign a bin code to the journal line to indicate where the items should be taken from in the warehouse.</span></span> <span data-ttu-id="97bcb-111">Дополнительные сведения см. в разделе [Подбор для производства или сборки](warehouse-how-to-pick-for-production.md).</span><span class="sxs-lookup"><span data-stu-id="97bcb-111">For more information, see [Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).</span></span>  
3.  <span data-ttu-id="97bcb-112">Выберите действие **Учесть**, чтобы учесть потребление.</span><span class="sxs-lookup"><span data-stu-id="97bcb-112">Choose the **Post** action to post the consumption.</span></span> <span data-ttu-id="97bcb-113">Соответствующие операции в книге товаров уменьшаются.</span><span class="sxs-lookup"><span data-stu-id="97bcb-113">The related item ledger entries are reduced.</span></span>

## <a name="see-also"></a><span data-ttu-id="97bcb-114">См. также</span><span class="sxs-lookup"><span data-stu-id="97bcb-114">See Also</span></span>  
<span data-ttu-id="97bcb-115">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="97bcb-115">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="97bcb-116">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="97bcb-116">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="97bcb-117">[Планирование](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="97bcb-117">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="97bcb-118">Наличие</span><span class="sxs-lookup"><span data-stu-id="97bcb-118">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="97bcb-119">Покупки</span><span class="sxs-lookup"><span data-stu-id="97bcb-119">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="97bcb-120">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="97bcb-120">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

