---
title: Учет потребления в пакетном режиме
description: Если выбран метод списания **Вручную**, учет компонентов производится вручную с использованием журнала потребления.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 66a19b624c74ec844806c27c490c300746b46704
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5787906"
---
# <a name="batch-post-production-consumption"></a><span data-ttu-id="03fad-103">Учет потребления для производства в пакетном режиме</span><span class="sxs-lookup"><span data-stu-id="03fad-103">Batch Post Production Consumption</span></span>

<span data-ttu-id="03fad-104">Если выбран метод списания **Вручную**, учет компонентов производится вручную с использованием журнала потребления.</span><span class="sxs-lookup"><span data-stu-id="03fad-104">If the flushing method is **Manual**, you must post the components manually, using a consumption journal.</span></span>  

>[!NOTE]
> <span data-ttu-id="03fad-105">Если в поле **Требуется подбор** в карточке товара установлен флажок для указания необходимости для данного склада обработки подбора запасов, это пакетное задание использовать не нужно.</span><span class="sxs-lookup"><span data-stu-id="03fad-105">If you have placed a check mark in the **Require Pick** field on the location card to indicate that the location requires inventory pick processing, then you do not need to use this batch job.</span></span> [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="03fad-106">будет обрабатывать потребление при учете подбора запасов.</span><span class="sxs-lookup"><span data-stu-id="03fad-106">will handle consumption when you post the inventory pick.</span></span> <span data-ttu-id="03fad-107">Дополнительные сведения см. в разделе [Подбор для производства или сборки](warehouse-how-to-pick-for-production.md#to-pick-components-in-basic-warehouse-configurations).</span><span class="sxs-lookup"><span data-stu-id="03fad-107">For more information, see [Pick for Production or Assembly](warehouse-how-to-pick-for-production.md#to-pick-components-in-basic-warehouse-configurations).</span></span> 

<span data-ttu-id="03fad-108">Можно также настроить [!INCLUDE[prod_short](includes/prod_short.md)] для автоматического учета (*списания*) компонентов при запуске или завершении производственных заказов.</span><span class="sxs-lookup"><span data-stu-id="03fad-108">You can also set up [!INCLUDE[prod_short](includes/prod_short.md)] to automatically post (*flush*) components when you start or finish production orders.</span></span> <span data-ttu-id="03fad-109">Дополнительные сведения см. в разделе [Включение списания компонентов в соответствии с производственным выпуском](production-how-to-flush-components-according-to-operation-output.md).</span><span class="sxs-lookup"><span data-stu-id="03fad-109">For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).</span></span>

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a><span data-ttu-id="03fad-110">Учет потребления для одной или нескольких строк производственного заказа</span><span class="sxs-lookup"><span data-stu-id="03fad-110">To post consumption for one or more production order lines</span></span>

1.  <span data-ttu-id="03fad-111">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал потребления**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="03fad-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Consumption Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="03fad-112">Заполните поля данными производственного заказа и данными о потреблении.</span><span class="sxs-lookup"><span data-stu-id="03fad-112">Fill in the fields with the production order data and the consumption data.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    <span data-ttu-id="03fad-113">Используйте действие **Расчет потребления** для создания строк журнала из производственных заказов на основе фактического (учтенное количество готовой продукции) или ожидаемого выпуска продукции (расчетное количество готовой продукции).</span><span class="sxs-lookup"><span data-stu-id="03fad-113">Use the **Calc. Consumption** action to generate journal lines from production orders based on the actual output (the quantity of finished goods that you have reported) or on the expected output (the quantity of finished goods that you expect to produce).</span></span>

    > [!NOTE]
    > <span data-ttu-id="03fad-114">Если вы настроили карточку местоположения так, чтобы она требовала обработки комплектования склада, то в поле **Количество** на странице **Журнал потребления** можно ввести только уже скомплектованные количества через действие склада, а не какое-либо рассчитанное количество.</span><span class="sxs-lookup"><span data-stu-id="03fad-114">If you configured the location card to require warehouse pick processing, then only quantities that are already picked through a warehouse activity can be entered in the **Quantity** field in the **Consumption Journal** page, not any calculated quantity.</span></span> <span data-ttu-id="03fad-115">Дополнительные сведения см. в разделе [Подбор для производства или сборки в расширенных конфигурациях склада](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md)</span><span class="sxs-lookup"><span data-stu-id="03fad-115">For more information, see [Pick for Production or Assembly in Advanced Warehouse Configurations](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md)</span></span>

3.  <span data-ttu-id="03fad-116">Выберите действие **Учесть**, чтобы учесть потребление.</span><span class="sxs-lookup"><span data-stu-id="03fad-116">Choose the **Post** action to post the consumption.</span></span> <span data-ttu-id="03fad-117">Соответствующие запасы уменьшаются.</span><span class="sxs-lookup"><span data-stu-id="03fad-117">The related inventories are reduced.</span></span>



## <a name="see-also"></a><span data-ttu-id="03fad-118">См. также</span><span class="sxs-lookup"><span data-stu-id="03fad-118">See Also</span></span>

<span data-ttu-id="03fad-119">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="03fad-119">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="03fad-120">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="03fad-120">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="03fad-121">[Планирование](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="03fad-121">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="03fad-122">Запасы</span><span class="sxs-lookup"><span data-stu-id="03fad-122">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="03fad-123">Покупки</span><span class="sxs-lookup"><span data-stu-id="03fad-123">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="03fad-124">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="03fad-124">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]
