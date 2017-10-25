---
title: "Практическое руководство. Предложения продажи сборки на заказ | Документы Майкрософт"
description: "Можно использовать функцию управления сборкой, чтобы настроить сборочный элемент по запросу клиента во время процесса продаж."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7602b067e4b3fc99815a581c851138d7cc3ff41e
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-quote-an-assemble-to-order-sale"></a><span data-ttu-id="d45cc-103">Практическое руководство. Предложения продажи сборки на заказ</span><span class="sxs-lookup"><span data-stu-id="d45cc-103">How to: Quote an Assemble-to-Order Sale</span></span>
<span data-ttu-id="d45cc-104">Можно использовать функцию управления сборкой, чтобы настроить сборочный элемент по запросу клиента во время процесса продаж.</span><span class="sxs-lookup"><span data-stu-id="d45cc-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span></span> <span data-ttu-id="d45cc-105">Дополнительные сведения см. в разделе [Практическое руководство. Продажа товара, собранного на заказ](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="d45cc-105">For more information, see [How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>  

<span data-ttu-id="d45cc-106">Как при продаже любого другого типа товара, можно также создать предложение по продаже для настраиваемого сборочного элемента до его преобразования в заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="d45cc-106">As when you sell any other type of item, you can also create a sales quote for a customized assembly item before converting it to a sales order.</span></span> <span data-ttu-id="d45cc-107">Этот процесс включает несколько дополнительных этапов при его сравнении с созданием обычного предложения по продаже, и он использует разновидность связанного сборочного заказа, которой является предложение по сборке.</span><span class="sxs-lookup"><span data-stu-id="d45cc-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span></span>

> [!NOTE]  
>  <span data-ttu-id="d45cc-108">Как и во всех типах предложений, количества в предложениях по сборке не используются в расчетах наличия, планирования или резервирования.</span><span class="sxs-lookup"><span data-stu-id="d45cc-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span></span>  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a><span data-ttu-id="d45cc-109">Создание предложения по продаже для товара сборки на заказ</span><span class="sxs-lookup"><span data-stu-id="d45cc-109">To create a sales quote for an assemble-to-order item</span></span>  
1.  <span data-ttu-id="d45cc-110">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Предложение по продаже**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d45cc-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Quote**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d45cc-111">Создайте строку предложения по продаже с одной строкой для сборочного элемента.</span><span class="sxs-lookup"><span data-stu-id="d45cc-111">Create a sales quote line with one line for an assembly item.</span></span> <span data-ttu-id="d45cc-112">Дополнительные сведения см. в разделе [Практическое руководство. Создание предложений](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="d45cc-112">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span></span>  
3.  <span data-ttu-id="d45cc-113">В поле **Количество для сборки на заказ** введите полное количество.</span><span class="sxs-lookup"><span data-stu-id="d45cc-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="d45cc-114">Не следует отправлять предложение по частичному количеству.</span><span class="sxs-lookup"><span data-stu-id="d45cc-114">You should not quote a partial quantity.</span></span> <span data-ttu-id="d45cc-115">Поэтому необходимо ввести то же количество, введенное в поле **Кол-во**, в строку предложения по продаже.</span><span class="sxs-lookup"><span data-stu-id="d45cc-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span></span>  

4.  <span data-ttu-id="d45cc-116">На экспресс-вкладке **Строки** выберите **Строка**, выберите **Сборка на заказ**, а затем выберите **Строки сборки на заказ**.</span><span class="sxs-lookup"><span data-stu-id="d45cc-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span></span> <span data-ttu-id="d45cc-117">В качестве альтернативы выберите поле **Количество для сборки на заказ** в строке.</span><span class="sxs-lookup"><span data-stu-id="d45cc-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span></span>  
5.  <span data-ttu-id="d45cc-118">В окне **Строки сборки на заказ** просмотрите или измените строки сборочного заказа в соответствии с предложением по продаже, которое запросил клиент.</span><span class="sxs-lookup"><span data-stu-id="d45cc-118">In the **Assemble-to-Order Lines** window, review or modify the assembly order lines according to the quote that the customer is requesting.</span></span> <span data-ttu-id="d45cc-119">Если необходимо просмотреть дополнительные сведения, выберите действие **Показать документ**, чтобы открыть полный общий предложенный заказ.</span><span class="sxs-lookup"><span data-stu-id="d45cc-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span></span> <span data-ttu-id="d45cc-120">Изменить содержимое большинства полей и учесть их невозможно.</span><span class="sxs-lookup"><span data-stu-id="d45cc-120">You cannot change the contents of most fields, and you cannot post.</span></span>  
6.  <span data-ttu-id="d45cc-121">При регулировке строк сборочного заказа в соответствии с предложением закройте окно **Строки сборки на заказ**, чтобы вернуться в окно **Предложение**.</span><span class="sxs-lookup"><span data-stu-id="d45cc-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** window to return to the **Sales Quote** window.</span></span>  
7.  <span data-ttu-id="d45cc-122">Если клиент принимает предложение, создайте заказ на продажу оцененного сборочного элемента.</span><span class="sxs-lookup"><span data-stu-id="d45cc-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span></span> <span data-ttu-id="d45cc-123">Дополнительные сведения см. в разделе [Практическое руководство. Создание предложений](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="d45cc-123">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span></span> <span data-ttu-id="d45cc-124">Связанное предложение по сборке и все настройки связаны с новым заказом на продажу для подготовки сборки товара или товаров, которые должны быть проданы.</span><span class="sxs-lookup"><span data-stu-id="d45cc-124">The linked assembly quote and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d45cc-125">См. также</span><span class="sxs-lookup"><span data-stu-id="d45cc-125">See Also</span></span>  
[<span data-ttu-id="d45cc-126">Управление сборкой</span><span class="sxs-lookup"><span data-stu-id="d45cc-126">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="d45cc-127">Практическое руководство. Работа со спецификациями</span><span class="sxs-lookup"><span data-stu-id="d45cc-127">How to: Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="d45cc-128">Наличие</span><span class="sxs-lookup"><span data-stu-id="d45cc-128">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="d45cc-129">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="d45cc-129">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="d45cc-130">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d45cc-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

