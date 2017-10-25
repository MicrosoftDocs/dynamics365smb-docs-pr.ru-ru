---
title: "Практическое руководство. Создание заголовков производственных заказов | Документы Майкрософт"
description: "Производственный заказ можно создать вручную. Для этого сначала необходимо создать заголовок производственного заказа."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 0c792dbb7d7261e8f8b89ca4f3d39d875142c4eb
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-create-production-order-headers"></a><span data-ttu-id="738fd-103">Практическое руководство. Создание заголовков производственных заказов</span><span class="sxs-lookup"><span data-stu-id="738fd-103">How to: Create Production Order Headers</span></span>
<span data-ttu-id="738fd-104">Производственный заказ можно создать вручную. Для этого сначала необходимо создать заголовок производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="738fd-104">You can create a production order manually, and the first step is to create a production order header.</span></span>

<span data-ttu-id="738fd-105">Производственные заказы обычно создаются автоматически функцией планирования для удовлетворения известного спроса.</span><span class="sxs-lookup"><span data-stu-id="738fd-105">Production orders are typically created automatically by a planning function to fulfill a known demand.</span></span> <span data-ttu-id="738fd-106">Дополнительные сведения см. в разделе [Планирование](production-planning.md).</span><span class="sxs-lookup"><span data-stu-id="738fd-106">For more information, see [Planning](production-planning.md).</span></span>   

<span data-ttu-id="738fd-107">В следующей процедуре показан способ создания утвержденного производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="738fd-107">In the following procedure, a firm planned production order is created.</span></span> <span data-ttu-id="738fd-108">Можно создавать производственные заказы и с другим статусом.</span><span class="sxs-lookup"><span data-stu-id="738fd-108">You can also create production orders with a different status.</span></span>  

## <a name="to-create-a-production-order-header"></a><span data-ttu-id="738fd-109">Создание заголовка производственного заказа</span><span class="sxs-lookup"><span data-stu-id="738fd-109">To create a production order header</span></span>  
1.  <span data-ttu-id="738fd-110">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Утвержд. произв. заказы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="738fd-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="738fd-111">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="738fd-111">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="738fd-112">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="738fd-112">In the **No.**</span></span> <span data-ttu-id="738fd-113">введите следующий номер в серии.</span><span class="sxs-lookup"><span data-stu-id="738fd-113">field, insert the next number in the series.</span></span>  
4.  <span data-ttu-id="738fd-114">В поле **Тип источника** выберите источник производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="738fd-114">In the **Source Type** field, select the source of the production order.</span></span>

    <span data-ttu-id="738fd-115">Здесь можно выбрать производство семейства товаров.</span><span class="sxs-lookup"><span data-stu-id="738fd-115">Here you can select to produce for a family of items.</span></span> <span data-ttu-id="738fd-116">Дополнительные сведения см. в разделе [Практическое руководство. Работа с производственными семействами](production-how-work-family.md).</span><span class="sxs-lookup"><span data-stu-id="738fd-116">For more information, see [How to: Work With Production Families](production-how-work-family.md).</span></span>
5.  <span data-ttu-id="738fd-117">В поле **Номер источника** выберите номер товарной позиции, семейство или заголовок продажи, для которого будет создан производственный заказ.</span><span class="sxs-lookup"><span data-stu-id="738fd-117">In the **Source No.** field, select the item number, family, or sales header for which the production order is to be generated.</span></span>  
6.  <span data-ttu-id="738fd-118">Заполните поля **Кол-во** и **Дата выполнения** в соответствии со спецификациями.</span><span class="sxs-lookup"><span data-stu-id="738fd-118">Fill in the **Quantity** and **Due Date** fields according to your specifications.</span></span>  

<span data-ttu-id="738fd-119">При изменении производственных требований, таких как компоненты или операции, можно быстро заново спланировать производственный заказ.</span><span class="sxs-lookup"><span data-stu-id="738fd-119">When production requirements change, such as components or operations, you can quickly replan the production order.</span></span> <span data-ttu-id="738fd-120">Дополнительные сведения см. в разделе [Практическое руководство. Непосредственное перепланирование или обновление производственных заказов](production-how-to-replan-refresh-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="738fd-120">For more information, see [How to: Replan or Refresh Production Orders Directly](production-how-to-replan-refresh-production-orders.md).</span></span> 

## <a name="see-also"></a><span data-ttu-id="738fd-121">См. также</span><span class="sxs-lookup"><span data-stu-id="738fd-121">See Also</span></span>  
<span data-ttu-id="738fd-122">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="738fd-122">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="738fd-123">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="738fd-123">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="738fd-124">[Планирование](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="738fd-124">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="738fd-125">Наличие</span><span class="sxs-lookup"><span data-stu-id="738fd-125">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="738fd-126">Покупки</span><span class="sxs-lookup"><span data-stu-id="738fd-126">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="738fd-127">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="738fd-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

