---
title: "Практическое руководство. Предложения продажи сборки на заказ | Документы Майкрософт"
description: "Можно использовать функцию управления сборкой, чтобы настроить сборочный элемент по запросу клиента во время процесса продаж."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 402745a9c90d1b82779e436f4a6533d2aed1b344
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="quote-an-assemble-to-order-sale"></a><span data-ttu-id="b746e-103">Предложения продажи сборки на заказ</span><span class="sxs-lookup"><span data-stu-id="b746e-103">Quote an Assemble-to-Order Sale</span></span>
<span data-ttu-id="b746e-104">Можно использовать функцию управления сборкой, чтобы настроить сборочный элемент по запросу клиента во время процесса продаж.</span><span class="sxs-lookup"><span data-stu-id="b746e-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span></span> <span data-ttu-id="b746e-105">Дополнительные сведения см. в разделе [Продажа товара, собранного на заказ](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="b746e-105">For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>  

<span data-ttu-id="b746e-106">Как при продаже любого другого типа товара, можно также создать предложение по продаже для настраиваемого сборочного элемента до его преобразования в заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="b746e-106">As when you sell any other type of item, you can also create a sales quote for a customized assembly item before converting it to a sales order.</span></span> <span data-ttu-id="b746e-107">Этот процесс включает несколько дополнительных этапов при его сравнении с созданием обычного предложения по продаже, и он использует разновидность связанного сборочного заказа, которой является предложение по сборке.</span><span class="sxs-lookup"><span data-stu-id="b746e-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span></span>

> [!NOTE]  
>  <span data-ttu-id="b746e-108">Как и во всех типах предложений, количества в предложениях по сборке не используются в расчетах наличия, планирования или резервирования.</span><span class="sxs-lookup"><span data-stu-id="b746e-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span></span>  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a><span data-ttu-id="b746e-109">Создание предложения по продаже для товара сборки на заказ</span><span class="sxs-lookup"><span data-stu-id="b746e-109">To create a sales quote for an assemble-to-order item</span></span>  
1.  <span data-ttu-id="b746e-110">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Предложение по продаже**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="b746e-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Quote**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b746e-111">Создайте строку предложения по продаже с одной строкой для сборочного элемента.</span><span class="sxs-lookup"><span data-stu-id="b746e-111">Create a sales quote line with one line for an assembly item.</span></span> <span data-ttu-id="b746e-112">Дополнительные сведения см. в разделе [Создание предложений](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="b746e-112">For more information, see [Make Offers](sales-how-make-offers.md).</span></span>  
3.  <span data-ttu-id="b746e-113">В поле **Количество для сборки на заказ** введите полное количество.</span><span class="sxs-lookup"><span data-stu-id="b746e-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="b746e-114">Не следует отправлять предложение по частичному количеству.</span><span class="sxs-lookup"><span data-stu-id="b746e-114">You should not quote a partial quantity.</span></span> <span data-ttu-id="b746e-115">Поэтому необходимо ввести то же количество, введенное в поле **Кол-во**, в строку предложения по продаже.</span><span class="sxs-lookup"><span data-stu-id="b746e-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span></span>  

4.  <span data-ttu-id="b746e-116">На экспресс-вкладке **Строки** выберите **Строка**, выберите **Сборка на заказ**, а затем выберите **Строки сборки на заказ**.</span><span class="sxs-lookup"><span data-stu-id="b746e-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span></span> <span data-ttu-id="b746e-117">В качестве альтернативы выберите поле **Количество для сборки на заказ** в строке.</span><span class="sxs-lookup"><span data-stu-id="b746e-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span></span>  
5.  <span data-ttu-id="b746e-118">В окне **Строки сборки на заказ** просмотрите или измените строки сборочного заказа в соответствии с предложением по продаже, которое запросил клиент.</span><span class="sxs-lookup"><span data-stu-id="b746e-118">In the **Assemble-to-Order Lines** window, review or modify the assembly order lines according to the quote that the customer is requesting.</span></span> <span data-ttu-id="b746e-119">Если необходимо просмотреть дополнительные сведения, выберите действие **Показать документ**, чтобы открыть полный общий предложенный заказ.</span><span class="sxs-lookup"><span data-stu-id="b746e-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span></span> <span data-ttu-id="b746e-120">Изменить содержимое большинства полей и учесть их невозможно.</span><span class="sxs-lookup"><span data-stu-id="b746e-120">You cannot change the contents of most fields, and you cannot post.</span></span>  
6.  <span data-ttu-id="b746e-121">При регулировке строк сборочного заказа в соответствии с предложением закройте окно **Строки сборки на заказ**, чтобы вернуться в окно **Предложение**.</span><span class="sxs-lookup"><span data-stu-id="b746e-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** window to return to the **Sales Quote** window.</span></span>  
7.  <span data-ttu-id="b746e-122">Если клиент принимает предложение, создайте заказ на продажу оцененного сборочного элемента.</span><span class="sxs-lookup"><span data-stu-id="b746e-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span></span> <span data-ttu-id="b746e-123">Дополнительные сведения см. в разделе [Создание предложений](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="b746e-123">For more information, see [Make Offers](sales-how-make-offers.md).</span></span> <span data-ttu-id="b746e-124">Связанное предложение по сборке и все настройки связаны с новым заказом на продажу для подготовки сборки товара или товаров, которые должны быть проданы.</span><span class="sxs-lookup"><span data-stu-id="b746e-124">The linked assembly quote and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b746e-125">См. также</span><span class="sxs-lookup"><span data-stu-id="b746e-125">See Also</span></span>  
[<span data-ttu-id="b746e-126">Управление сборкой</span><span class="sxs-lookup"><span data-stu-id="b746e-126">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="b746e-127">Работа со спецификациями</span><span class="sxs-lookup"><span data-stu-id="b746e-127">Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="b746e-128">Наличие</span><span class="sxs-lookup"><span data-stu-id="b746e-128">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="b746e-129">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="b746e-129">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="b746e-130">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b746e-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

