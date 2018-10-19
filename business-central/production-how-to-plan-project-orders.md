---
title: "Как планировать заказы проекта | Документы Майкрософт"
description: "Выполнение этой задачи планирования начинается с заказа на продажу и производится в окне **Планирование заказа на продажу**. После создания проектного производственного заказа его планирование может быть продолжено в окне **Планирование заказов**."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 08cd8c323e8f5221bd6915618582441a739e77c8
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="plan-project-orders"></a><span data-ttu-id="4cd7e-104">Планирование заказов проекта</span><span class="sxs-lookup"><span data-stu-id="4cd7e-104">Plan Project Orders</span></span>
<span data-ttu-id="4cd7e-105">Выполнение этой задачи планирования начинается с заказа на продажу и производится в окне **Планирование заказа на продажу**.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-105">This planning task starts from a sales order and uses the **Sales Order Planning** window.</span></span> <span data-ttu-id="4cd7e-106">После создания проектного производственного заказа его планирование может быть продолжено в окне **Планирование заказов**.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-106">Once you have created a project production order, you can plan it further by using the **Order Planning** window.</span></span>  

## <a name="to-create-a-project-production-order"></a><span data-ttu-id="4cd7e-107">Создание проектного производственного заказа</span><span class="sxs-lookup"><span data-stu-id="4cd7e-107">To create a project production order</span></span>  

1.  <span data-ttu-id="4cd7e-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4cd7e-109">Выберите заказ на продажу, который представляет производственный проект, затем выберите действие **Планирование**.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-109">Select the sales order that represents the production project, and then choose the **Planning** action.</span></span>  
4.  <span data-ttu-id="4cd7e-110">В окне **Планирование заказа на продажу** выберите действие **Создать произв. заказ**.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-110">In the **Sales Order Planning** window, choose  the **Create Prod. Order** action.</span></span>  
5.  <span data-ttu-id="4cd7e-111">В окне **Создание заказа из продажи** в поле **Тип заказа** выберите **Проектный заказ**.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-111">In the **Create Order from Sales** window, in the **Order Type** field, select **Project Order**.</span></span>  
6.  <span data-ttu-id="4cd7e-112">Нажмите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-112">Choose the **Yes** button.</span></span>  
7.  <span data-ttu-id="4cd7e-113">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Производственные заказы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Production Orders**, and then choose the related link.</span></span>
8. <span data-ttu-id="4cd7e-114">Откройте только что созданный производственный заказ.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-114">Open the production order just created.</span></span>  

    <span data-ttu-id="4cd7e-115">Обратите внимание, что поле **Тип источника** производственного заказа содержит **Продажи - заголовок**, а заказ содержит несколько строк (по одной на каждую товарную позицию, которая должна быть произведена).</span><span class="sxs-lookup"><span data-stu-id="4cd7e-115">Notice that the **Source Type** field of the production order contains **Sales Header** and the order has multiple lines, one for each sales line item that must be produced.</span></span>  
9. <span data-ttu-id="4cd7e-116">Выберите действие **Планирование**.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-116">Choose the **Planning** action.</span></span>
10. <span data-ttu-id="4cd7e-117">В окне **Планирование заказов** выберите действие **Обновить**, чтобы рассчитать новый спрос.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-117">In the **Order Planning** window, choose the **Refresh** action to calculate new demand.</span></span>  

<span data-ttu-id="4cd7e-118">Строка заголовка проектного заказа отображается в развернутом виде со всеми невыполненными строками требования.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-118">The order header line for the project order is displayed with all unfulfilled demand lines expanded under it.</span></span> <span data-ttu-id="4cd7e-119">Хотя производственный заказ содержит строки для нескольких производимых товаров, общее требование для всех строк производственного заказа вместе с названием исходного клиента отображается под одной строкой заголовка заказа в окне **Планирование заказов**.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-119">Although the production order contains lines for several produced items, the total demand for all production order lines is listed under one order header line in the **Order Planning** window, and the original customer name is displayed.</span></span> <span data-ttu-id="4cd7e-120">Теперь можно приступать к планированию спроса, как описано в разделе [Планирование нового спроса по заказам](production-how-to-plan-for-new-demand.md).</span><span class="sxs-lookup"><span data-stu-id="4cd7e-120">You can now proceed to plan for the demand as described in [Plan for New Demand Order by Order](production-how-to-plan-for-new-demand.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="4cd7e-121">Строки спроса в производственном заказе проекта, которые в поле **Метод пополнения** имеют значение **Произв. заказ**, представляют подчиненные производственные заказы.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-121">Demand lines in the project production order that have **Prod. Order** in their **Replenishment System** field represent underlying production orders.</span></span> <span data-ttu-id="4cd7e-122">После формирования этих производственных заказов необходимо снова вычислить план в окне **Планирование заказов** для определения возможного невыполненного требования компонента для них.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-122">After you have generated these production orders, you must again calculate a plan in the **Order Planning** window to identify any unfulfilled component demand for them.</span></span> <span data-ttu-id="4cd7e-123">В этом случае они отображаются в виде строк спроса под обычной строкой заголовка производственного заказа, обозначая, что связь проекта более не отображается в окне.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-123">In that case, they are displayed as demand lines under a normal production order header line, meaning, the project relation is no longer visible in the window.</span></span> <span data-ttu-id="4cd7e-124">Если используется "Трассировка заказов", можно пролистать назад и вперед все заказы на поставку, созданные под исходным заказом на продажу.</span><span class="sxs-lookup"><span data-stu-id="4cd7e-124">However, if you are using the Order Tracking feature, then you can look back and forth to all supply orders made under the original sales order.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4cd7e-125">См. также</span><span class="sxs-lookup"><span data-stu-id="4cd7e-125">See Also</span></span>
<span data-ttu-id="4cd7e-126">[Планирование](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="4cd7e-126">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="4cd7e-127">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="4cd7e-127">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="4cd7e-128">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="4cd7e-128">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="4cd7e-129">Наличие</span><span class="sxs-lookup"><span data-stu-id="4cd7e-129">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="4cd7e-130">Покупки</span><span class="sxs-lookup"><span data-stu-id="4cd7e-130">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="4cd7e-131">[Сведения о проектировании: планирование поставок](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="4cd7e-131">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="4cd7e-132">Рекомендации по настройке. Планирование поставок</span><span class="sxs-lookup"><span data-stu-id="4cd7e-132">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="4cd7e-133">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4cd7e-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

