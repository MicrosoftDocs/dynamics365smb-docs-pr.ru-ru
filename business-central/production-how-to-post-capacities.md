---
title: Практическое руководство. Учет производственных мощностей | Документы Майкрософт
description: Учет используемых производственных мощностей, не присвоенных производственному заказу, осуществляется в журнале производственных мощностей. Например, работы по обслуживанию должны быть приписаны к производственным мощностям, а не к производственному заказу.
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
ms.openlocfilehash: 58005b8b4d401f5eab8a934d7b00b610b64b4281
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "928304"
---
# <a name="post-capacities"></a><span data-ttu-id="4980f-104">Учет производственных мощностей</span><span class="sxs-lookup"><span data-stu-id="4980f-104">Post Capacities</span></span>
<span data-ttu-id="4980f-105">Учет используемых производственных мощностей, не присвоенных производственному заказу, осуществляется в журнале производственных мощностей.</span><span class="sxs-lookup"><span data-stu-id="4980f-105">In the capacity journal, you post consumed capacities that are not assigned to the production order.</span></span> <span data-ttu-id="4980f-106">Например, работы по обслуживанию должны быть приписаны к производственным мощностям, а не к производственному заказу.</span><span class="sxs-lookup"><span data-stu-id="4980f-106">For example, maintenance work must be assigned to capacity, but not to a production order.</span></span>  

## <a name="to-post-capacities"></a><span data-ttu-id="4980f-107">Учет произв. мощностей</span><span class="sxs-lookup"><span data-stu-id="4980f-107">To post capacities</span></span>  
1.  <span data-ttu-id="4980f-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы произв. мощностей**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="4980f-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Capacity Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4980f-109">Заполните поля **Дата учета** и **Номер документа**.</span><span class="sxs-lookup"><span data-stu-id="4980f-109">Fill in the **Posting Date** and **Document No.** fields.</span></span>  
3.  <span data-ttu-id="4980f-110">В поле **Тип** введите тип производственных мощностей — **Машинный центр** или **Рабочий центр**, — учет которых необходимо осуществить.</span><span class="sxs-lookup"><span data-stu-id="4980f-110">In the **Type** field, enter the type of the capacity, either **Machine Center** or **Work Center**, that you are posting.</span></span>  
4.  <span data-ttu-id="4980f-111">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="4980f-111">In the **No.**</span></span> <span data-ttu-id="4980f-112">введите номер машинного или производственного центра.</span><span class="sxs-lookup"><span data-stu-id="4980f-112">field, enter the number of the machine center or work center.</span></span>  
5.  <span data-ttu-id="4980f-113">Введите необходимые данные в остальные поля, такие как **Время начала**, **Время окончания**, **Кол-во** и **Брак**.</span><span class="sxs-lookup"><span data-stu-id="4980f-113">Enter the relevant data in the other fields, such as **Starting Time**, **Ending Time**, **Quantity**, and **Scrap**.</span></span>  
6.  <span data-ttu-id="4980f-114">Выберите действие **Учесть**, чтобы учесть производственные мощности.</span><span class="sxs-lookup"><span data-stu-id="4980f-114">Choose the **Post** action to post the capacities.</span></span>  

## <a name="to-view-work-center-ledger-entries"></a><span data-ttu-id="4980f-115">Для просмотра операций книги рабочего центра:</span><span class="sxs-lookup"><span data-stu-id="4980f-115">To view work center ledger entries</span></span>  
<span data-ttu-id="4980f-116">На страницах **Карточка производственного центра** и **Карточка машинного центра** можно просмотреть учтенные производственные мощности как результат завершенных производственных заказов.</span><span class="sxs-lookup"><span data-stu-id="4980f-116">In the **Work Center Card** and **Machine Center Card** pages, you can view the posted capacities as a result of finished production orders.</span></span>    
1.  <span data-ttu-id="4980f-117">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Рабочие центры**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="4980f-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Work Centers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4980f-118">Откройте соответствующую карточку **Производственный центр** из списка, затем выберите действие **Книга операций по произв. мощностям**.</span><span class="sxs-lookup"><span data-stu-id="4980f-118">Open the relevant **Work Center** card from the list, and then choose the **Capacity Ledger Entries** action.</span></span>  

<span data-ttu-id="4980f-119">На странице **Произв. мощности - книга операций** перечисляются учтенные операции рабочего центра в порядке их учета.</span><span class="sxs-lookup"><span data-stu-id="4980f-119">The **Capacity Ledger Entries** page displays the posted entries from the work center in the order they were posted.</span></span>   

## <a name="see-also"></a><span data-ttu-id="4980f-120">См. также</span><span class="sxs-lookup"><span data-stu-id="4980f-120">See Also</span></span>  
<span data-ttu-id="4980f-121">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="4980f-121">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="4980f-122">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="4980f-122">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="4980f-123">[Планирование](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="4980f-123">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="4980f-124">Наличие</span><span class="sxs-lookup"><span data-stu-id="4980f-124">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="4980f-125">Покупки</span><span class="sxs-lookup"><span data-stu-id="4980f-125">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="4980f-126">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4980f-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
