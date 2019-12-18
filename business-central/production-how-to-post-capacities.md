---
title: Практическое руководство. Учет производственных мощностей | Документация Майкрософт
description: Учет используемых производственных мощностей, не присвоенных производственному заказу, осуществляется в журнале производственных мощностей. Например, работы по обслуживанию должны быть приписаны к производственным мощностям, а не к производственному заказу.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: bccc43aea943fa1745d92a6bdb064307f088d1e6
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2883242"
---
# <a name="post-capacities"></a><span data-ttu-id="8c172-104">Учет производственных мощностей</span><span class="sxs-lookup"><span data-stu-id="8c172-104">Post Capacities</span></span>
<span data-ttu-id="8c172-105">Учет используемых производственных мощностей, не присвоенных производственному заказу, осуществляется в журнале производственных мощностей.</span><span class="sxs-lookup"><span data-stu-id="8c172-105">In the capacity journal, you post consumed capacities that are not assigned to the production order.</span></span> <span data-ttu-id="8c172-106">Например, работы по обслуживанию должны быть приписаны к производственным мощностям, а не к производственному заказу.</span><span class="sxs-lookup"><span data-stu-id="8c172-106">For example, maintenance work must be assigned to capacity, but not to a production order.</span></span>  

## <a name="to-post-capacities"></a><span data-ttu-id="8c172-107">Учет произв. мощностей</span><span class="sxs-lookup"><span data-stu-id="8c172-107">To post capacities</span></span>  
1.  <span data-ttu-id="8c172-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы произв. мощностей**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="8c172-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Capacity Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8c172-109">Заполните поля **Дата учета** и **Номер документа**.</span><span class="sxs-lookup"><span data-stu-id="8c172-109">Fill in the **Posting Date** and **Document No.** fields.</span></span>  
3.  <span data-ttu-id="8c172-110">В поле **Тип** введите тип производственных мощностей — **Машинный центр** или **Рабочий центр**, — учет которых необходимо осуществить.</span><span class="sxs-lookup"><span data-stu-id="8c172-110">In the **Type** field, enter the type of the capacity, either **Machine Center** or **Work Center**, that you are posting.</span></span>  
4.  <span data-ttu-id="8c172-111">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="8c172-111">In the **No.**</span></span> <span data-ttu-id="8c172-112">введите номер машинного или производственного центра.</span><span class="sxs-lookup"><span data-stu-id="8c172-112">field, enter the number of the machine center or work center.</span></span>  
5.  <span data-ttu-id="8c172-113">Введите необходимые данные в остальные поля, такие как **Время начала**, **Время окончания**, **Кол-во** и **Брак**.</span><span class="sxs-lookup"><span data-stu-id="8c172-113">Enter the relevant data in the other fields, such as **Starting Time**, **Ending Time**, **Quantity**, and **Scrap**.</span></span>  
6.  <span data-ttu-id="8c172-114">Выберите действие **Учесть**, чтобы учесть производственные мощности.</span><span class="sxs-lookup"><span data-stu-id="8c172-114">Choose the **Post** action to post the capacities.</span></span>  

## <a name="to-view-work-center-ledger-entries"></a><span data-ttu-id="8c172-115">Для просмотра операций книги рабочего центра:</span><span class="sxs-lookup"><span data-stu-id="8c172-115">To view work center ledger entries</span></span>  
<span data-ttu-id="8c172-116">На страницах **Карточка производственного центра** и **Карточка машинного центра** можно просмотреть учтенные производственные мощности как результат завершенных производственных заказов.</span><span class="sxs-lookup"><span data-stu-id="8c172-116">In the **Work Center Card** and **Machine Center Card** pages, you can view the posted capacities as a result of finished production orders.</span></span>    
1.  <span data-ttu-id="8c172-117">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Производственные центры**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="8c172-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Work Centers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8c172-118">Откройте соответствующую карточку **Производственный центр** из списка, затем выберите действие **Книга операций по произв. мощностям**.</span><span class="sxs-lookup"><span data-stu-id="8c172-118">Open the relevant **Work Center** card from the list, and then choose the **Capacity Ledger Entries** action.</span></span>  

<span data-ttu-id="8c172-119">На странице **Произв. мощности - книга операций** перечисляются учтенные операции рабочего центра в порядке их учета.</span><span class="sxs-lookup"><span data-stu-id="8c172-119">The **Capacity Ledger Entries** page displays the posted entries from the work center in the order they were posted.</span></span>   

## <a name="see-also"></a><span data-ttu-id="8c172-120">См. также</span><span class="sxs-lookup"><span data-stu-id="8c172-120">See Also</span></span>  
<span data-ttu-id="8c172-121">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="8c172-121">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="8c172-122">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="8c172-122">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="8c172-123">[Планирование](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="8c172-123">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="8c172-124">Запасы</span><span class="sxs-lookup"><span data-stu-id="8c172-124">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="8c172-125">Покупки</span><span class="sxs-lookup"><span data-stu-id="8c172-125">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="8c172-126">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8c172-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
