---
title: "Практическое руководство. Списание компонентов в соответствии с производственным выпуском | Документы Майкрософт"
description: "Для товаров, в которых применяется обратный метод списания, поведением по умолчанию является вычисление потребления компонентов во время изменения состояния запущенного производственного заказа на значение **Завершено**. Дополнительные сведения см. в разделе Метод списания."
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
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: f61e3150f1978795a20d4ad68656d6d1e72402a0
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="flush-components-according-to-operation-output"></a><span data-ttu-id="f7fe5-104">Списание компонентов в соответствии с производственным выпуском</span><span class="sxs-lookup"><span data-stu-id="f7fe5-104">Flush Components According to Operation Output</span></span>
<span data-ttu-id="f7fe5-105">Для товаров, в которых применяется обратный метод списания, поведением по умолчанию является вычисление потребления компонентов во время изменения состояния запущенного производственного заказа на значение **Завершено**.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-105">For items that are set up with backward flushing method, the default behavior is to calculate and post component consumption when you change the status of a released production order to **Finished**.</span></span>  

<span data-ttu-id="f7fe5-106">Если задаются также коды связей маршрута, по окончании каждой операции происходит расчет и учет, и учитывается количество, которое было фактически использовано в операции.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-106">If you also define routing link codes, then calculation and posting occurs when each operation is finished, and the quantity that was actually consumed in the operation is posted.</span></span> <span data-ttu-id="f7fe5-107">Дополнительные сведения см. в разделе [Создание маршрутов](production-how-to-create-routings.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe5-107">For more information, see [Create Routings](production-how-to-create-routings.md).</span></span>  

<span data-ttu-id="f7fe5-108">Например, если для заказа на производство 800 метров требуется 8 кг компонента, то при указании 200 метров на выходе, 2 кг автоматически учитываются как потребление.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-108">For example, if a production order to produce 800 meters requires 8 kg of a component, then when you post 200 meters as output, 2 kg are automatically posted as consumption.</span></span>  

<span data-ttu-id="f7fe5-109">Эта функция полезна по следующим причинам:</span><span class="sxs-lookup"><span data-stu-id="f7fe5-109">This functionality is useful for the following reasons:</span></span>  

-   <span data-ttu-id="f7fe5-110">**Оценка стоимости запасов** — операции стоимости для выхода и потребления создаются параллельно по мере выполнения производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-110">**Inventory Valuation** - Value entries for output and consumption are created in parallel as the production order progresses.</span></span> <span data-ttu-id="f7fe5-111">Без кодов связи маршрута инвентарная стоимость увеличивается по мере учета выхода, а затем одномоментно уменьшается, учитывается потребление компонентов вместе с завершенным производственным заказом.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-111">Without routing link codes, the inventory value will increase as output is posted and then decrease at a later point in time when the value of component consumption is posted together with the finished production order.</span></span>  
-   <span data-ttu-id="f7fe5-112">**Запасы — наличие** — при постепенном учете потребления сведения о наличии компонентов более точные, что важно для поддержания внутреннего баланса между спросом и предложением.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-112">**Inventory Availability** - With gradual consumption posting, the availability of component items is more up-to-date, which is important to maintain the internal balance between demand and supply.</span></span> <span data-ttu-id="f7fe5-113">Без кодов связи маршрута при проч. запросах компонента может считаться, что он доступен, при том, что он находится на удержании задержанного учета потребления.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-113">Without routing link codes, other demands for the component may believe that it is available as long as it is pending a delayed consumption posting.</span></span>  
-   <span data-ttu-id="f7fe5-114">**Just-in-Time** — благодаря возможности настроить продукты согласно запросам клиента можно сократить потери за счет того, что изменения работы и системы происходят только при необходимости.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-114">**Just-in-Time** – With the ability to customize products to customer requests, you can minimize waste by making sure that work and system changes only occur when it is necessary.</span></span>  

<span data-ttu-id="f7fe5-115">Следующая процедура описывает комбинирование обратного списания и кодов маршрутных ссылок, чтобы количество, списываемое за одну производственную операцию, было пропорционально фактическому выходу завершенной операции.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-115">The following procedure shows how to combine backward flushing and routing link codes so that the quantity that is flushed for each operation is proportional to the actual output of the finished operation.</span></span>  

## <a name="to-flush-components-according-to-operation-output"></a><span data-ttu-id="f7fe5-116">Списание компонентов в соответствии с производственным выпуском</span><span class="sxs-lookup"><span data-stu-id="f7fe5-116">To flush components according to operation output</span></span>  
1.  <span data-ttu-id="f7fe5-117">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Товары**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f7fe5-118">Выберите действие **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-118">Choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="f7fe5-119">На экспресс-вкладке **Пополнение** в поле **Метод списания** выберите **Вперед**.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-119">On the **Replenishment** FastTab, in the **Flushing Method** field, select **Forward**.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="f7fe5-120">Выберите **Подбор + прямой**, если компонент используется на данном складе, который настроен расширенного подбора и размещения.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-120">Select **Pick+ Forward** if the component is used in a location that is set up for directed put-away and pick.</span></span>  

4.  <span data-ttu-id="f7fe5-121">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Маршруты**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Routings**, and then choose the related link.</span></span>  
5.  <span data-ttu-id="f7fe5-122">Определите коды связи маршрута для каждой операции, которая потребляет компонент.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-122">Define routing link codes for every operation that consumes the component.</span></span> <span data-ttu-id="f7fe5-123">Дополнительные сведения см. в разделе [Создание маршрутов](production-how-to-create-routings.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe5-123">For more information, see [Create Routings ](production-how-to-create-routings.md).</span></span>  
6.  <span data-ttu-id="f7fe5-124">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Производственная спецификация**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Production BOM**, and then choose the related link.</span></span>  
7.  <span data-ttu-id="f7fe5-125">Определите коды связи маршрута от каждого экземпляра компонента к операции, где он потребляется.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-125">Define routing link codes from each instance of the component to the operation where it is consumed.</span></span>

    > [!IMPORTANT]  
    >  <span data-ttu-id="f7fe5-126">Компонент должен иметь маршрутную ссылку на последнюю производственную операцию в маршруте.</span><span class="sxs-lookup"><span data-stu-id="f7fe5-126">The component must have a routing link to the last operation in the routing.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f7fe5-127">См. также</span><span class="sxs-lookup"><span data-stu-id="f7fe5-127">See Also</span></span>  
[<span data-ttu-id="f7fe5-128">Создание производственных спецификаций</span><span class="sxs-lookup"><span data-stu-id="f7fe5-128">Create Production BOMs</span></span>](production-how-to-create-production-boms.md)  
[<span data-ttu-id="f7fe5-129">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="f7fe5-129">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="f7fe5-130">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="f7fe5-130">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="f7fe5-131">[Планирование](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="f7fe5-131">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="f7fe5-132">Наличие</span><span class="sxs-lookup"><span data-stu-id="f7fe5-132">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="f7fe5-133">Покупки</span><span class="sxs-lookup"><span data-stu-id="f7fe5-133">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="f7fe5-134">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f7fe5-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

