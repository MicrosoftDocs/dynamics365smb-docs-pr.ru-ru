---
title: Создание производственных заказов из заказов на продажу
description: Вы можете создать производственные заказы из заказов на продажу.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 05/28/2021
ms.author: edupont
ms.openlocfilehash: 438f4d4e1833ba607ceedb9f5d9450c0a4dbb680
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "6115240"
---
# <a name="create-production-orders-from-sales-orders"></a><span data-ttu-id="feb54-103">Создание производственных заказов из заказов на продажу</span><span class="sxs-lookup"><span data-stu-id="feb54-103">Create Production Orders from Sales Orders</span></span>
<span data-ttu-id="feb54-104">Можно создавать производственные заказы для произведенных товаров непосредственно из заказов на продажу.</span><span class="sxs-lookup"><span data-stu-id="feb54-104">You can create production orders for produced items directly from sales orders.</span></span>  

## <a name="to-create-a-production-order-from-a-sales-order"></a><span data-ttu-id="feb54-105">Создание производственного заказа из заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="feb54-105">To create a production order from a sales order</span></span>  

1.  <span data-ttu-id="feb54-106">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="feb54-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="feb54-107">Выберите заказ на продажу, для которого будет создан производственный заказ.</span><span class="sxs-lookup"><span data-stu-id="feb54-107">Select the sales order you want to create a production order for.</span></span>  
3.  <span data-ttu-id="feb54-108">Выберите действие **Планирование**.</span><span class="sxs-lookup"><span data-stu-id="feb54-108">Choose the **Planning** action.</span></span> <span data-ttu-id="feb54-109">На странице **Планирование заказа на продажу** можно просмотреть наличие товаров, указанных в заказе на продажу.</span><span class="sxs-lookup"><span data-stu-id="feb54-109">On the **Sales Order Planning** page, you can view the availability of the sales order item.</span></span>  
4.  <span data-ttu-id="feb54-110">Выберите действие **Создать произв. заказ**.</span><span class="sxs-lookup"><span data-stu-id="feb54-110">Choose the **Create Prod. Order** action.</span></span>  
5.  <span data-ttu-id="feb54-111">Выберите статус и тип заказа.</span><span class="sxs-lookup"><span data-stu-id="feb54-111">Select the status and order type.</span></span>  
6.  <span data-ttu-id="feb54-112">Выберите кнопку **Да**, чтобы создать один или несколько производственных заказов для строк, у которых есть **Произв. заказ** в поле **Метод пополнения**.</span><span class="sxs-lookup"><span data-stu-id="feb54-112">Choose the **Yes** button to create one or more production orders for the lines that have **Prod. Order** in their **Replenishment System** field.</span></span>


> [!NOTE]  
> <span data-ttu-id="feb54-113">Строки спроса в созданном производственном заказе проекта, которые в поле **Метод пополнения** имеют значение **Произв. заказ**, представляют подчиненные производственные заказы.</span><span class="sxs-lookup"><span data-stu-id="feb54-113">Demand lines in the created production order that have **Prod. Order** in their **Replenishment System** field represent underlying production orders.</span></span> <span data-ttu-id="feb54-114">После формирования этих производственных заказов необходимо определить невыполненный спрос компонента для них на странице **Планирование заказов** или с помощью функции **Перепланировать**.</span><span class="sxs-lookup"><span data-stu-id="feb54-114">After you have generated these production orders, remember to identify any unfulfilled component demand for them using the **Order Planning** page or the **Replan** function from created orders.</span></span> 

## <a name="order-type"></a><span data-ttu-id="feb54-115">Тип заказа</span><span class="sxs-lookup"><span data-stu-id="feb54-115">Order type</span></span>  
<span data-ttu-id="feb54-116">Вы можете выбрать один из двух способов создания производственных заказов, как показано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="feb54-116">You can choose between two ways to create the production orders as outlined in the following table.</span></span>

|<span data-ttu-id="feb54-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="feb54-117">Option</span></span>|<span data-ttu-id="feb54-118">Описание</span><span class="sxs-lookup"><span data-stu-id="feb54-118">Description</span></span>|
|------|-----------|
|<span data-ttu-id="feb54-119">Товарный заказ</span><span class="sxs-lookup"><span data-stu-id="feb54-119">Item Order</span></span>|<span data-ttu-id="feb54-120">Один производственный заказ создается для каждого нужного производственного заказы, который представлен строкой в окне **Планирование заказа на продажу**.</span><span class="sxs-lookup"><span data-stu-id="feb54-120">One production order is created for each needed production order that is represented by a line in the **Sales Order Planning** window.</span></span>|
|<span data-ttu-id="feb54-121">Проектный заказ</span><span class="sxs-lookup"><span data-stu-id="feb54-121">Project Order</span></span>|<span data-ttu-id="feb54-122">Один производственный заказ создается для всех нужных производственных заказов, которые представлены строками в окне **Планирование заказа на продажу**.</span><span class="sxs-lookup"><span data-stu-id="feb54-122">One production order is created for all needed production orders order that are represented by lines in the **Sales Order Planning** window.</span></span> |

<span data-ttu-id="feb54-123">При использовании проектных заказов поле **Тип источника** производственного заказа содержит **Продажи - заголовок**, а заказ содержит несколько строк (по одной на каждую товарную позицию, которая должна быть произведена).</span><span class="sxs-lookup"><span data-stu-id="feb54-123">When you use project orders, the **Source Type** field of the production order contains **Sales Header** and the order has multiple lines, one for each sales line item that must be produced.</span></span>  


## <a name="see-also"></a><span data-ttu-id="feb54-124">См. также</span><span class="sxs-lookup"><span data-stu-id="feb54-124">See Also</span></span>  
[<span data-ttu-id="feb54-125">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="feb54-125">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="feb54-126">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="feb54-126">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="feb54-127">Запасы</span><span class="sxs-lookup"><span data-stu-id="feb54-127">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="feb54-128">Покупки</span><span class="sxs-lookup"><span data-stu-id="feb54-128">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="feb54-129">[Сведения о проектировании: планирование поставок](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="feb54-129">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="feb54-130">Рекомендации по настройке. Планирование поставок</span><span class="sxs-lookup"><span data-stu-id="feb54-130">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="feb54-131">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="feb54-131">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]
