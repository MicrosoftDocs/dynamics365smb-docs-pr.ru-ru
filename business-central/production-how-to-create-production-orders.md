---
title: Практическое руководство. Создание заголовков производственных заказов | Документы Майкрософт
description: Производственный заказ можно создать вручную. Для этого сначала необходимо создать заголовок производственного заказа.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 70a6f2e583e5ba78eecae0a25d6533d8265414ca
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1253313"
---
# <a name="create-production-order-headers"></a><span data-ttu-id="55139-103">Создание заголовков производственных заказов</span><span class="sxs-lookup"><span data-stu-id="55139-103">Create Production Order Headers</span></span>
<span data-ttu-id="55139-104">Производственный заказ можно создать вручную. Для этого сначала необходимо создать заголовок производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="55139-104">You can create a production order manually, and the first step is to create a production order header.</span></span>

<span data-ttu-id="55139-105">Производственные заказы обычно создаются автоматически функцией планирования для удовлетворения известного спроса.</span><span class="sxs-lookup"><span data-stu-id="55139-105">Production orders are typically created automatically by a planning function to fulfill a known demand.</span></span> <span data-ttu-id="55139-106">Дополнительные сведения см. в разделе [Планирование](production-planning.md).</span><span class="sxs-lookup"><span data-stu-id="55139-106">For more information, see [Planning](production-planning.md).</span></span>   

<span data-ttu-id="55139-107">В следующей процедуре показан способ создания утвержденного производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="55139-107">In the following procedure, a firm planned production order is created.</span></span> <span data-ttu-id="55139-108">Можно создавать производственные заказы и с другим статусом.</span><span class="sxs-lookup"><span data-stu-id="55139-108">You can also create production orders with a different status.</span></span>  

## <a name="to-create-a-production-order-header"></a><span data-ttu-id="55139-109">Создание заголовка производственного заказа</span><span class="sxs-lookup"><span data-stu-id="55139-109">To create a production order header</span></span>  
1.  <span data-ttu-id="55139-110">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Утвержд. произв. заказы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="55139-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="55139-111">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="55139-111">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="55139-112">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="55139-112">In the **No.**</span></span> <span data-ttu-id="55139-113">введите следующий номер в серии.</span><span class="sxs-lookup"><span data-stu-id="55139-113">field, insert the next number in the series.</span></span>  
4.  <span data-ttu-id="55139-114">В поле **Тип источника** выберите источник производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="55139-114">In the **Source Type** field, select the source of the production order.</span></span>

    <span data-ttu-id="55139-115">Здесь можно выбрать производство семейства товаров.</span><span class="sxs-lookup"><span data-stu-id="55139-115">Here you can select to produce for a family of items.</span></span> <span data-ttu-id="55139-116">Дополнительные сведения см. в разделе [Работа с производственными семействами](production-how-work-family.md).</span><span class="sxs-lookup"><span data-stu-id="55139-116">For more information, see [Work With Production Families](production-how-work-family.md).</span></span>
5.  <span data-ttu-id="55139-117">В поле **Номер источника** выберите номер товарной позиции, семейство или заголовок продажи, для которого будет создан производственный заказ.</span><span class="sxs-lookup"><span data-stu-id="55139-117">In the **Source No.** field, select the item number, family, or sales header for which the production order is to be generated.</span></span>  
6.  <span data-ttu-id="55139-118">Заполните поля **Кол-во** и **Дата выполнения** в соответствии со спецификациями.</span><span class="sxs-lookup"><span data-stu-id="55139-118">Fill in the **Quantity** and **Due Date** fields according to your specifications.</span></span>  

<span data-ttu-id="55139-119">При изменении производственных требований, таких как компоненты или операции, можно быстро заново спланировать производственный заказ.</span><span class="sxs-lookup"><span data-stu-id="55139-119">When production requirements change, such as components or operations, you can quickly replan the production order.</span></span> <span data-ttu-id="55139-120">Дополнительные сведения см. в разделе [Прямое перепланирование или обновление производственных заказов](production-how-to-replan-refresh-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="55139-120">For more information, see [Replan or Refresh Production Orders Directly](production-how-to-replan-refresh-production-orders.md).</span></span> 

## <a name="see-also"></a><span data-ttu-id="55139-121">См. также</span><span class="sxs-lookup"><span data-stu-id="55139-121">See Also</span></span>  
<span data-ttu-id="55139-122">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="55139-122">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="55139-123">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="55139-123">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="55139-124">[Планирование](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="55139-124">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="55139-125">Наличие</span><span class="sxs-lookup"><span data-stu-id="55139-125">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="55139-126">Покупки</span><span class="sxs-lookup"><span data-stu-id="55139-126">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="55139-127">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="55139-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
