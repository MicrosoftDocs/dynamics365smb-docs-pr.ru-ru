---
title: Практическое руководство. Предложения продажи сборки на заказ | Документация Майкрософт
description: Можно использовать функцию управления сборкой, чтобы настроить сборочный элемент по запросу клиента во время процесса продаж.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: kit, kitting
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 807c924e64764e7ac1932321603a415101e3bbf3
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5386653"
---
# <a name="quote-an-assemble-to-order-sale"></a><span data-ttu-id="a89ed-103">Предложения продажи сборки на заказ</span><span class="sxs-lookup"><span data-stu-id="a89ed-103">Quote an Assemble-to-Order Sale</span></span>
<span data-ttu-id="a89ed-104">Можно использовать функцию управления сборкой, чтобы настроить сборочный элемент по запросу клиента во время процесса продаж.</span><span class="sxs-lookup"><span data-stu-id="a89ed-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span></span> <span data-ttu-id="a89ed-105">Дополнительные сведения см. в разделе [Продажа товара, собранного на заказ](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="a89ed-105">For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>  

<span data-ttu-id="a89ed-106">Как при продаже любого другого типа товара, можно также создать предложение по продаже для настраиваемого сборочного элемента до его преобразования в заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="a89ed-106">As when you sell any other type of item, you can also create a sales quote for a customized assembly item before converting it to a sales order.</span></span> <span data-ttu-id="a89ed-107">Этот процесс включает несколько дополнительных этапов при его сравнении с созданием обычного предложения по продаже, и он использует разновидность связанного сборочного заказа, которой является предложение по сборке.</span><span class="sxs-lookup"><span data-stu-id="a89ed-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span></span>

> [!NOTE]  
>  <span data-ttu-id="a89ed-108">Как и во всех типах предложений, количества в предложениях по сборке не используются в расчетах наличия, планирования или резервирования.</span><span class="sxs-lookup"><span data-stu-id="a89ed-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span></span>  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a><span data-ttu-id="a89ed-109">Создание предложения по продаже для товара сборки на заказ</span><span class="sxs-lookup"><span data-stu-id="a89ed-109">To create a sales quote for an assemble-to-order item</span></span>  
1.  <span data-ttu-id="a89ed-110">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Предложение по продаже**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="a89ed-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Quote**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a89ed-111">Создайте строку предложения по продаже с одной строкой для сборочного элемента.</span><span class="sxs-lookup"><span data-stu-id="a89ed-111">Create a sales quote line with one line for an assembly item.</span></span> <span data-ttu-id="a89ed-112">Дополнительные сведения см. в разделе [Создание предложений по продаже](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="a89ed-112">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span></span>  
3.  <span data-ttu-id="a89ed-113">В поле **Количество для сборки на заказ** введите полное количество.</span><span class="sxs-lookup"><span data-stu-id="a89ed-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="a89ed-114">Не следует отправлять предложение по частичному количеству.</span><span class="sxs-lookup"><span data-stu-id="a89ed-114">You should not quote a partial quantity.</span></span> <span data-ttu-id="a89ed-115">Поэтому необходимо ввести то же количество, введенное в поле **Кол-во**, в строку предложения по продаже.</span><span class="sxs-lookup"><span data-stu-id="a89ed-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span></span>  

4.  <span data-ttu-id="a89ed-116">На экспресс-вкладке **Строки** выберите **Строка**, выберите **Сборка на заказ**, а затем выберите **Строки сборки на заказ**.</span><span class="sxs-lookup"><span data-stu-id="a89ed-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span></span> <span data-ttu-id="a89ed-117">В качестве альтернативы выберите поле **Количество для сборки на заказ** в строке.</span><span class="sxs-lookup"><span data-stu-id="a89ed-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span></span>  
5.  <span data-ttu-id="a89ed-118">На странице **Строки сборки на заказ** просмотрите или измените строки сборочного заказа в соответствии с предложением по продаже, которое запросил клиент.</span><span class="sxs-lookup"><span data-stu-id="a89ed-118">On the **Assemble-to-Order Lines** page, review or modify the assembly order lines according to the quote that the customer is requesting.</span></span> <span data-ttu-id="a89ed-119">Если необходимо просмотреть дополнительные сведения, выберите действие **Показать документ**, чтобы открыть полный общий предложенный заказ.</span><span class="sxs-lookup"><span data-stu-id="a89ed-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span></span> <span data-ttu-id="a89ed-120">Изменить содержимое большинства полей и учесть их невозможно.</span><span class="sxs-lookup"><span data-stu-id="a89ed-120">You cannot change the contents of most fields, and you cannot post.</span></span>  
6.  <span data-ttu-id="a89ed-121">При регулировке строк сборочного заказа в соответствии с предложением закройте окно **Строки сборки на заказ**, чтобы вернуться на страницу **Предложение**.</span><span class="sxs-lookup"><span data-stu-id="a89ed-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** page to return to the **Sales Quote** page.</span></span>  
7.  <span data-ttu-id="a89ed-122">Если клиент принимает предложение, создайте заказ на продажу оцененного сборочного элемента.</span><span class="sxs-lookup"><span data-stu-id="a89ed-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span></span> <span data-ttu-id="a89ed-123">Дополнительные сведения см. в разделе [Создание предложений по продаже](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="a89ed-123">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span></span> <span data-ttu-id="a89ed-124">Связанное предложение по сборке и все настройки связаны с новым заказом на продажу для подготовки сборки товара или товаров, которые должны быть проданы.</span><span class="sxs-lookup"><span data-stu-id="a89ed-124">The linked assembly quote and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a89ed-125">См. также</span><span class="sxs-lookup"><span data-stu-id="a89ed-125">See Also</span></span>  
[<span data-ttu-id="a89ed-126">Управление сборкой</span><span class="sxs-lookup"><span data-stu-id="a89ed-126">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="a89ed-127">Работа со спецификациями</span><span class="sxs-lookup"><span data-stu-id="a89ed-127">Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="a89ed-128">Запасы</span><span class="sxs-lookup"><span data-stu-id="a89ed-128">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="a89ed-129">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="a89ed-129">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="a89ed-130">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a89ed-130">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]