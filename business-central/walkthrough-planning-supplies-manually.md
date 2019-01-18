---
title: "Пошаговое руководство. Планирование поставок вручную | Документы Майкрософт"
description: "В этом пошаговом руководстве демонстрируется процесс планирования заказов на продажу для выполнения нового требования. Планирование поставок можно инициировать с фиксированным интервалом, например каждое утро или каждый понедельник, или при получении уведомления от отдела продаж либо с производства, в зависимости от типа требования."
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
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: d0a7088e436def55b3c7ddc3115065c66686b7fb
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="walkthrough-planning-supplies-manually"></a><span data-ttu-id="46204-104">Пошаговое руководство. Планирование поставок вручную</span><span class="sxs-lookup"><span data-stu-id="46204-104">Walkthrough: Planning Supplies Manually</span></span>
<span data-ttu-id="46204-105">В этом пошаговом руководстве демонстрируется процесс планирования заказов на продажу для выполнения нового требования.</span><span class="sxs-lookup"><span data-stu-id="46204-105">This walkthrough demonstrates the process of planning supply orders to fulfill new demand.</span></span> <span data-ttu-id="46204-106">Планирование поставок можно инициировать с фиксированным интервалом, например каждое утро или каждый понедельник, или при получении уведомления от отдела продаж либо с производства, в зависимости от типа требования.</span><span class="sxs-lookup"><span data-stu-id="46204-106">You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.</span></span> <span data-ttu-id="46204-107">В данном пошаговом руководстве будет использоваться страница **Планирование заказов** — простой инструмент планирования поставок на основе выполняемого вручную процесса принятия решений вместо автоматического планирования на основе параметров.</span><span class="sxs-lookup"><span data-stu-id="46204-107">In this walkthrough you will use the **Order Planning** page, a simple supply planning tool that is based on manual decision-making instead of parameter-based automatic planning.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="46204-108">Об этом пошаговом руководстве</span><span class="sxs-lookup"><span data-stu-id="46204-108">About This Walkthrough</span></span>  
 <span data-ttu-id="46204-109">В этом пошаговом руководстве рассматриваются следующие задачи:</span><span class="sxs-lookup"><span data-stu-id="46204-109">This walkthrough illustrates the following tasks:</span></span>  

-   <span data-ttu-id="46204-110">планирование заказа на покупку для компонентов производства;</span><span class="sxs-lookup"><span data-stu-id="46204-110">Planning a purchase order for manufacturing components.</span></span>  
-   <span data-ttu-id="46204-111">планирование заказа на перемещение для выполнения требования продаж;</span><span class="sxs-lookup"><span data-stu-id="46204-111">Planning a transfer order to fulfill sales demand.</span></span>  
-   <span data-ttu-id="46204-112">планирование производственного заказа для многоуровневого товара.</span><span class="sxs-lookup"><span data-stu-id="46204-112">Planning a production order for a multilevel item.</span></span>  

## <a name="roles"></a><span data-ttu-id="46204-113">Роли</span><span class="sxs-lookup"><span data-stu-id="46204-113">Roles</span></span>  
 <span data-ttu-id="46204-114">В этом пошаговом руководстве демонстрируются задачи, выполняемые исполнителями следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="46204-114">This walkthrough demonstrates tasks performed by the following user roles:</span></span>  

-   <span data-ttu-id="46204-115">Планировщик производства</span><span class="sxs-lookup"><span data-stu-id="46204-115">Production Planner</span></span>  
-   <span data-ttu-id="46204-116">Агент по закупкам</span><span class="sxs-lookup"><span data-stu-id="46204-116">Purchasing Agent</span></span>  
-   <span data-ttu-id="46204-117">обработчик заказов на продажу;</span><span class="sxs-lookup"><span data-stu-id="46204-117">Sales Order Processor</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="46204-118">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="46204-118">Prerequisites</span></span>  
 <span data-ttu-id="46204-119">Перед выполнением указаний этого пошагового руководства необходимо установить [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="46204-119">Before you begin this walkthrough, you must install the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="46204-120">В эту базу данных необходимо внести следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="46204-120">The following modifications must be made to the database:</span></span>  

-   <span data-ttu-id="46204-121">удалите все имеющиеся заказы на продажу велосипедов;</span><span class="sxs-lookup"><span data-stu-id="46204-121">Delete all existing sales orders for bicycles.</span></span>  
-   <span data-ttu-id="46204-122">создайте один заказ на продажу 10 велосипедов на складе «СИНИЙ»;</span><span class="sxs-lookup"><span data-stu-id="46204-122">Create one sales order for 10 bicycles at BLUE location.</span></span>  
-   <span data-ttu-id="46204-123">удалите все запланированные и утвержденные производственные заказы.</span><span class="sxs-lookup"><span data-stu-id="46204-123">Delete all planned and firm planned production orders.</span></span> <span data-ttu-id="46204-124">Не удаляйте начатые заказы с уже учтенными операциями.</span><span class="sxs-lookup"><span data-stu-id="46204-124">Do not delete started orders with entries that are already posted.</span></span>  

 <span data-ttu-id="46204-125">Как правило, в этом пошаговом руководстве следует использовать предлагаемые данные, так как они содержат необходимые записи.</span><span class="sxs-lookup"><span data-stu-id="46204-125">As a rule, use the suggested data in this walkthrough because this data has the necessary records.</span></span>  

## <a name="story"></a><span data-ttu-id="46204-126">Сюжет</span><span class="sxs-lookup"><span data-stu-id="46204-126">Story</span></span>  
 <span data-ttu-id="46204-127">Эдуард, планировщик производства производственной организации, собирается запланировать производственные заказы и заказы на покупку для выполнения нового требования продаж.</span><span class="sxs-lookup"><span data-stu-id="46204-127">Eduardo, the Production Planner of a small manufacturing company, is about to plan production and purchase orders to fulfill new sales demand.</span></span>  

 <span data-ttu-id="46204-128">Поскольку количество уровней спецификации товаров невелико, Эдуард использует страницу **Планирование заказов** для создания заказов на поставку вручную — по очереди для каждого уровня производства.</span><span class="sxs-lookup"><span data-stu-id="46204-128">Because the products have few BOM levels and the flow of orders is relatively low, Eduardo uses the **Order Planning** page to manually create supply orders, one product level at a time.</span></span>  

 <span data-ttu-id="46204-129">В более сложной производственной среде для планирования поставок используется производственный план на основе параметров товаров, например периода перепланирования, страхового запаса времени и точки повтора заказа, а также пакетные вычисления консолидированного требования по всем уровням производства.</span><span class="sxs-lookup"><span data-stu-id="46204-129">In a more complex manufacturing environment, the planning worksheet is used to plan supply based on item parameters such as rescheduling period, safety lead time, reorder point, and batch calculations of consolidated demand from all product levels.</span></span>  

## <a name="setting-up-the-sample-data"></a><span data-ttu-id="46204-130">Настройка образца данных</span><span class="sxs-lookup"><span data-stu-id="46204-130">Setting Up the Sample Data</span></span>  
 <span data-ttu-id="46204-131">В стандартной демонстрационной организации CRONUS в данный момент есть множество незапланированных требований.</span><span class="sxs-lookup"><span data-stu-id="46204-131">The standard CRONUS demonstration company currently has lots of unplanned demand.</span></span> <span data-ttu-id="46204-132">В процессе выполнения различных задач планирования этого пошагового руководства нужно будет отклониться от реалистичных потоков деловых операций, игнорируя требования с более близкими сроками выполнения и используя вместо них более поздние сроки.</span><span class="sxs-lookup"><span data-stu-id="46204-132">During the different planning tasks in this walkthrough, you will have to deviate from the realistic business flow by ignoring demand with close due dates and instead use demand with later due dates.</span></span>  

## <a name="using-the-order-planning-page"></a><span data-ttu-id="46204-133">Использование страницы «Планирование заказов»</span><span class="sxs-lookup"><span data-stu-id="46204-133">Using the Order Planning Page</span></span>  

<!-- 
The **Order Planning** page can be accessed from several different locations on the **Departments** menu in the navigation pane:  

-   Manufacturing, Planning  
-   Sales & Marketing, Order Processing  
-   Purchase, Planning  
-   In addition, you can open this page for a specific production order by choosing **Planning** on the **Navigate** tab in the **Order** group.

-->  

### <a name="to-use-the-order-planning-page"></a><span data-ttu-id="46204-134">Процедура использования страницы «Планирование заказов»</span><span class="sxs-lookup"><span data-stu-id="46204-134">To use the Order Planning page</span></span>  

1.  <span data-ttu-id="46204-135">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Планирование заказов**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="46204-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Order Planning**, and then choose the related link.</span></span>  

     <span data-ttu-id="46204-136">После первого открытия страницы **Планирование заказов** должен быть вычислен план для отражения новых требований, появившихся после последнего вычисления.</span><span class="sxs-lookup"><span data-stu-id="46204-136">When the **Order Planning** page first opens, a plan must be calculated to show the new demand since it was last calculated.</span></span>  

2.  <span data-ttu-id="46204-137">Выберите действие **Вычислить план**.</span><span class="sxs-lookup"><span data-stu-id="46204-137">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="46204-138">Система планирования проанализирует появившееся новое требование, например новые либо измененные заказы на продажу или производственные заказы.</span><span class="sxs-lookup"><span data-stu-id="46204-138">The planning system analyzes any new demand that has been introduced, such as new sales, changed sales, or production orders.</span></span>  

     <span data-ttu-id="46204-139">Количество, необходимое для каждой строки требования, вычисляется на основе общего наличия.</span><span class="sxs-lookup"><span data-stu-id="46204-139">Based on total availability, the quantity needed for each demand line is calculated.</span></span> <span data-ttu-id="46204-140">Это вычисление выполняется последовательно для каждого заказа.</span><span class="sxs-lookup"><span data-stu-id="46204-140">This calculation is performed order-by-order.</span></span> <span data-ttu-id="46204-141">То есть первым будет вычислен заказ с наиболее ранним сроком выполнения или датой поставки для строки требования.</span><span class="sxs-lookup"><span data-stu-id="46204-141">This means that the order which includes the demand line with the earliest due date or shipment date will be calculated first.</span></span> <span data-ttu-id="46204-142">После этого дополнительные строки требования будут вычисляться в том же порядке, вне зависимости от их срока выполнения или даты отгрузки.</span><span class="sxs-lookup"><span data-stu-id="46204-142">After that, additional demand lines will be calculated in the same order, regardless of the due date or shipment date.</span></span>  

3.  <span data-ttu-id="46204-143">Убедитесь, что страница **Планирование заказов** развернута, а размеры полей столбца изменены таким образом, что в них полностью видны все имена полей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="46204-143">Be sure that the **Order Planning** page is maximized and that column fields are resized to show all the default field names.</span></span>  

     <span data-ttu-id="46204-144">Когда процесс вычисления закончится, на странице отобразятся все невыполненные требования, представленные в виде свернутых строк заголовков заказов, отсортированных по самой ранней дате требования.</span><span class="sxs-lookup"><span data-stu-id="46204-144">When the calculation is completed, the page displays all unfulfilled demand as collapsed order header lines sorted by earliest demand date.</span></span>  

     <span data-ttu-id="46204-145">Обратите внимание, что в организации CRONUS есть несколько заказов с невыполненными требованиями.</span><span class="sxs-lookup"><span data-stu-id="46204-145">Notice that CRONUS has several orders with unfulfilled demand.</span></span> <span data-ttu-id="46204-146">Каждая выделенная полужирным шрифтом строка соответствует заказу, заказу на продажу или производственному заказу, содержащему по крайней мере одну строку заказа с недостаточным наличием.</span><span class="sxs-lookup"><span data-stu-id="46204-146">Each bold planning line represents an order, sales order, or production order, including at least one order line with insufficient availability.</span></span>  

4.  <span data-ttu-id="46204-147">В поле **Показать требования как** выберите фильтр **Все требования**.</span><span class="sxs-lookup"><span data-stu-id="46204-147">In the **Show Demand As** field, select the **All Demand** filter.</span></span>  

     <span data-ttu-id="46204-148">С помощью поля **Тип требования** можно выбрать типы заказов, которые должны отображаться.</span><span class="sxs-lookup"><span data-stu-id="46204-148">With the **Demand Type** field, you can choose which order types that you want to display.</span></span>  

     <span data-ttu-id="46204-149">Заказы, у которых нет проблем, наличия не отображаются.</span><span class="sxs-lookup"><span data-stu-id="46204-149">Orders that do not have availability problems are not shown.</span></span> <span data-ttu-id="46204-150">Если при вычислении плана заказы отсутствуют, отобразится сообщение, а строки планирования отображаться не будут.</span><span class="sxs-lookup"><span data-stu-id="46204-150">If no orders exist when a plan is calculated, a message will display and no planning lines will appear.</span></span>  

## <a name="planning-a-purchase-order-to-fulfill-component-demand"></a><span data-ttu-id="46204-151">Планирование заказа на покупку для выполнения требования компонента</span><span class="sxs-lookup"><span data-stu-id="46204-151">Planning a Purchase Order to Fulfill Component Demand</span></span>  
 <span data-ttu-id="46204-152">При выполнении этой процедуры будет создан заказ на покупку компонентов, необходимых для производства.</span><span class="sxs-lookup"><span data-stu-id="46204-152">In this procedure, you create a purchase order for needed manufacturing components.</span></span>  

### <a name="to-plan-a-purchase-order-to-fulfill-component-need-in-production"></a><span data-ttu-id="46204-153">Процедура планирования заказа на покупку для удовлетворения потребности в компоненте на производстве</span><span class="sxs-lookup"><span data-stu-id="46204-153">To plan a purchase order to fulfill component need in production</span></span>  

1.  <span data-ttu-id="46204-154">Разверните первую строку (выберите знак "+").</span><span class="sxs-lookup"><span data-stu-id="46204-154">Expand the first line (choose the + symbol).</span></span>  
2.  <span data-ttu-id="46204-155">Выберите первую строку требования с товаром **LSU-15**, затем выберите действие **Показать документ**.</span><span class="sxs-lookup"><span data-stu-id="46204-155">Choose the first demand line, with item **LSU-15**, and then choose the **Show Document** action.</span></span>  
3.  <span data-ttu-id="46204-156">Закройте открытый производственный заказ, чтобы вернуться на страницу **Планирование заказов**.</span><span class="sxs-lookup"><span data-stu-id="46204-156">Close the opened production order to return to the **Order Planning** page.</span></span>  
4.  <span data-ttu-id="46204-157">В поле **Метод пополнения** выберите **Покупка**.</span><span class="sxs-lookup"><span data-stu-id="46204-157">In the **Replenishment System** field, select **Purchase**.</span></span>  

     <span data-ttu-id="46204-158">По умолчанию используется значение из карточки товара или карточки единицы хранения, однако его можно изменить на одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="46204-158">The default value is from the item card, or SKU card, but you can change it to one of the following options:</span></span>  

    -   <span data-ttu-id="46204-159">**Покупка** — для создания заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="46204-159">**Purchase** – To create a purchase order.</span></span>  
    -   <span data-ttu-id="46204-160">**Перемещение** — для создания заказа на перемещение.</span><span class="sxs-lookup"><span data-stu-id="46204-160">**Transfer** – To create a transfer order.</span></span>  
    -   <span data-ttu-id="46204-161">**Произв. заказ** — для создания производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="46204-161">**Prod. Order** – To create a production order.</span></span>  

5.  <span data-ttu-id="46204-162">В поле **Поставка от** выберите один из следующих параметров в соответствии с выбранной системой пополнения.</span><span class="sxs-lookup"><span data-stu-id="46204-162">In the **Supply From** field, select one of the following options according to the selected replenishment system:</span></span>  

    -   <span data-ttu-id="46204-163">**Поставщик** – для покупки</span><span class="sxs-lookup"><span data-stu-id="46204-163">**Vendor** – For purchases</span></span>  
    -   <span data-ttu-id="46204-164">**Склад** — для перемещения</span><span class="sxs-lookup"><span data-stu-id="46204-164">**Location** – For transfers</span></span>  

     <span data-ttu-id="46204-165">Если поле не заполнено, при попытке создания заказов на поставку отобразится сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="46204-165">If the field is not filled in, an error message will display when you try to create the supply orders.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="46204-166">Если для компонентов в карточках товаров задан номер поставщика по умолчанию, в строках будут указаны предварительно заданные значения.</span><span class="sxs-lookup"><span data-stu-id="46204-166">If the components have a default vendor number set up on the item cards, the lines will be preset.</span></span>  

6.  <span data-ttu-id="46204-167">Выберите поле **Поставка от**.</span><span class="sxs-lookup"><span data-stu-id="46204-167">Choose the **Supply From**  field.</span></span>  
7.  <span data-ttu-id="46204-168">На странице **Каталог поставщиков товара** выберите действие **Создать**, затем выберите поставщика **30000**.</span><span class="sxs-lookup"><span data-stu-id="46204-168">On the **Item Vendor Catalogue** page, choose the **New** action, and then select vendor **30000**.</span></span>  
8.  <span data-ttu-id="46204-169">Нажмите кнопку **ОК**, чтобы вернуться на страницу **Планирование заказов**.</span><span class="sxs-lookup"><span data-stu-id="46204-169">Choose the **OK** button to return to the **Order Planning** page.</span></span>  
9. <span data-ttu-id="46204-170">Скопируйте номер поставщика **30000** в другие строки компонентов громкоговорителя для этого производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="46204-170">Copy vendor **30000** to the other lines for loudspeaker components on this production order.</span></span>  

     <span data-ttu-id="46204-171">Теперь можно приступать к созданию заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="46204-171">You are now ready to create a purchase order.</span></span>  

10. <span data-ttu-id="46204-172">Выберите действие **Создать заказы**.</span><span class="sxs-lookup"><span data-stu-id="46204-172">Choose the **Make Orders** action.</span></span> <span data-ttu-id="46204-173">Откроется страница **Создание заказов на поставку**.</span><span class="sxs-lookup"><span data-stu-id="46204-173">The **Make Supply Orders** page opens.</span></span>  
11. <span data-ttu-id="46204-174">В поле **Заказы на изготовление для** на экспресс-вкладке **Планирование заказов** выберите параметр **Активный заказ**.</span><span class="sxs-lookup"><span data-stu-id="46204-174">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **Active Order** option.</span></span>  
12. <span data-ttu-id="46204-175">На экспресс-вкладке **Параметры** в поле **Создать заказ на покупку** выберите параметр **Создать заказы на покупку**.</span><span class="sxs-lookup"><span data-stu-id="46204-175">On the **Options** FastTab, in the **Create Purchase Order** field, choose the **Make Purch. Order** option.</span></span>  
13. <span data-ttu-id="46204-176">Нажмите кнопку **ОК**, чтобы создать заказы на покупку для всех компонентов в заказе.</span><span class="sxs-lookup"><span data-stu-id="46204-176">Choose the **OK** button to create purchase orders for all the components of the order.</span></span>  

     <span data-ttu-id="46204-177">Теперь заказы на покупку созданы, сохранены и размещены в конце списка заказов на покупку.</span><span class="sxs-lookup"><span data-stu-id="46204-177">The purchase orders are now created and saved as the last orders in the list of purchase orders.</span></span>  

## <a name="planning-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="46204-178">Планирование заказа на перемещение для выполнения требования продаж</span><span class="sxs-lookup"><span data-stu-id="46204-178">Planning a Transfer Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="46204-179">В рамках этой процедуры будет спланировано требование, в основе которого лежит заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="46204-179">In this procedure, you will plan for demand from a sales order.</span></span> <span data-ttu-id="46204-180">Строки требования соответствуют строкам продажи, а не строкам компонента, как в случае требования производства.</span><span class="sxs-lookup"><span data-stu-id="46204-180">Demand lines represent sales lines and not component lines, as in production demand.</span></span>  

### <a name="to-plan-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="46204-181">Процедура планирования заказа на перемещение для выполнения требования продаж</span><span class="sxs-lookup"><span data-stu-id="46204-181">To plan a transfer order to fulfill sales demand</span></span>  

1.  <span data-ttu-id="46204-182">Переместите курсор в строку планирования для заказа **2008**.</span><span class="sxs-lookup"><span data-stu-id="46204-182">Move the pointer to the planning line for order **2008**.</span></span>  
2.  <span data-ttu-id="46204-183">Разверните строку и переместите указатель на строку требования.</span><span class="sxs-lookup"><span data-stu-id="46204-183">Expand the line and move the pointer to the demand line.</span></span>  

     <span data-ttu-id="46204-184">Заказ на продажу **2008** оформлен на десять громкоговорителей типа **LS-120**, заказанных страховой компанией РОСНО.</span><span class="sxs-lookup"><span data-stu-id="46204-184">Sales order **2008** is for ten loudspeakers, item **LS-120**, ordered by John Haddock Insurance Co.</span></span>  

     <span data-ttu-id="46204-185">Отобразится зависящий от товара метод пополнения и поставщик по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="46204-185">The item’s defined replenishment system and default vendor will display.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="46204-186">В нижней части страницы отображаются информационные поля.</span><span class="sxs-lookup"><span data-stu-id="46204-186">At the bottom of the page, there are four information fields.</span></span> <span data-ttu-id="46204-187">В поле **Ближайшая доступная дата** указано, что необходимые десять штук будут доступны по входящему заказу на поставку через девять дней после текущего срока выполнения.</span><span class="sxs-lookup"><span data-stu-id="46204-187">In the **Earliest Date Available** field, the ten pieces that are needed will be available, on an inbound supply order, nine days later than the current due date.</span></span> <span data-ttu-id="46204-188">Если это слишком поздно для клиента, в поле **Доступно для перемещения** указано тринадцать штук товара, находящихся на другом складе.</span><span class="sxs-lookup"><span data-stu-id="46204-188">If this is too late for the customer, the **Available for Transfer** field shows 13 pieces of the item at another location.</span></span> <span data-ttu-id="46204-189">Этот запас необходимо будет учесть в плане.</span><span class="sxs-lookup"><span data-stu-id="46204-189">You will want to plan for this stock.</span></span>  

3.  <span data-ttu-id="46204-190">Выберите поле **Доступно для перемещения**, чтобы открыть страницу **Получение альтернативной поставки**.</span><span class="sxs-lookup"><span data-stu-id="46204-190">Choose the **Available for Transfer** field to open the **Get Alternative Supply** page.</span></span>  
4.  <span data-ttu-id="46204-191">Нажмите кнопку **ОК**, чтобы забронировать десять доступных товаров.</span><span class="sxs-lookup"><span data-stu-id="46204-191">Choose the **OK** button to book the ten items that are available.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="46204-192">В строке требования предлагаемая покупка заменена перемещением со склада "ЗЕЛЕНЫЙ".</span><span class="sxs-lookup"><span data-stu-id="46204-192">In the demand line, the suggested purchase has been exchanged with a transfer from GREEN location.</span></span> <span data-ttu-id="46204-193">Функция **Заказы на изготовление** позволяет создать заказ на перемещения со склада "Зеленый" на требуемый склад.</span><span class="sxs-lookup"><span data-stu-id="46204-193">The **Make Orders** function creates a transfer order from GREEN to the demanded location.</span></span> <span data-ttu-id="46204-194">Принцип действия поля **Наличие заменителей** аналогичен.</span><span class="sxs-lookup"><span data-stu-id="46204-194">The **Substitutes Exists** field works in the same way.</span></span>  

5.  <span data-ttu-id="46204-195">Выберите действие **Создать заказы**.</span><span class="sxs-lookup"><span data-stu-id="46204-195">Choose the **Make Orders** action.</span></span> <span data-ttu-id="46204-196">Откроется страница **Создание заказов на поставку**.</span><span class="sxs-lookup"><span data-stu-id="46204-196">The **Make Supply Orders** page opens.</span></span>  
6.  <span data-ttu-id="46204-197">В поле **Заказы на изготовление для** на экспресс-вкладке **Планирование заказов** выберите параметр **Активный заказ**.</span><span class="sxs-lookup"><span data-stu-id="46204-197">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **The Active Order** option.</span></span>  
7.  <span data-ttu-id="46204-198">На экспресс-вкладке **Параметры** в поле **Создать заказ на перемещение** выберите параметр **Создать заказы на перемещение**.</span><span class="sxs-lookup"><span data-stu-id="46204-198">On the **Options** FastTab, in the **Create Transfer Order** field, select the **Make Trans. Orders** option.</span></span>  
8.  <span data-ttu-id="46204-199">Нажмите кнопку **ОК**, чтобы создать заказ на перемещение для поставки по заказу на продажу.</span><span class="sxs-lookup"><span data-stu-id="46204-199">Choose the **OK** button to create the transfer order to supply the sales order.</span></span>  

     <span data-ttu-id="46204-200">Теперь заказ на перемещение создан, сохранен и размещен в конце списка открытых заказов на перемещение.</span><span class="sxs-lookup"><span data-stu-id="46204-200">The transfer order is now created and saved in the list as the last order in the list of open transfer orders.</span></span>  

## <a name="planning-a-multilevel-production-order-to-fulfill-sales-demand"></a><span data-ttu-id="46204-201">Планирование многоуровневого производственного заказа для выполнения требования продажи</span><span class="sxs-lookup"><span data-stu-id="46204-201">Planning a Multilevel Production Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="46204-202">В рамках этой процедуры будет спланировано выполнение требования продажи для производимого товара с несколькими уровнями производства, для каждого из которых создается зависимое требование производства.</span><span class="sxs-lookup"><span data-stu-id="46204-202">In this procedure, you will plan to fulfill sales demand for a produced item with multiple product levels, each creating dependent production demand.</span></span>  

### <a name="to-plan-multilevel-production-to-fulfill-sales-demand"></a><span data-ttu-id="46204-203">Процедура планирования многоуровневого производства для выполнения требования продаж</span><span class="sxs-lookup"><span data-stu-id="46204-203">To plan multilevel production to fulfill sales demand</span></span>  

1.  <span data-ttu-id="46204-204">Выберите строку планирования со спросом по продажам для заказа **1001**, который был создан ранее в качестве предварительно требуемых данных.</span><span class="sxs-lookup"><span data-stu-id="46204-204">Select the planning line with sales demand for order **1001**, created earlier as prerequisite data.</span></span>  

     <span data-ttu-id="46204-205">Это требование является строкой продажи, однако для товара задан метод пополнения **Произв. заказ**.</span><span class="sxs-lookup"><span data-stu-id="46204-205">This demand is a sales line, but the item has a defined replenishment system of **Prod. Order**.</span></span> <span data-ttu-id="46204-206">Перейдите к добавлению дополнительного колокольчика в компонент, необходимый для каждого велосипеда.</span><span class="sxs-lookup"><span data-stu-id="46204-206">Proceed to add an extra bell to the component need of each bicycle.</span></span>  

2.  <span data-ttu-id="46204-207">Выберите действие **Компоненты**, чтобы открыть страницу **Компоненты производственного плана**.</span><span class="sxs-lookup"><span data-stu-id="46204-207">Choose the **Components** action to open the **Planning Components** page.</span></span>  
3.  <span data-ttu-id="46204-208">В строке с товаром "Колокольчик" измените заданное в поле **Кол-во в** значение **1** на **2**.</span><span class="sxs-lookup"><span data-stu-id="46204-208">On the line with the Bell item, change the **Quantity per** field from **1** to **2**.</span></span>  
4.  <span data-ttu-id="46204-209">На странице **Планирование заказов** ознакомьтесь с альтернативами планирования.</span><span class="sxs-lookup"><span data-stu-id="46204-209">On the **Order Planning** page, consider your planning alternatives.</span></span> <span data-ttu-id="46204-210">В данном случае альтернативные способы поставки отсутствуют — перемещение, замена или более поздняя доставка невозможны.</span><span class="sxs-lookup"><span data-stu-id="46204-210">In this case, you have no alternative means of supply, no transfer, substitute, or later delivery.</span></span> <span data-ttu-id="46204-211">Необходимо создать предлагаемый заказ на поставку: производственный заказ.</span><span class="sxs-lookup"><span data-stu-id="46204-211">You must create the suggested supply order, a production order.</span></span>  
5.  <span data-ttu-id="46204-212">Выберите действие **Создать заказы**, чтобы создать производственный заказ.</span><span class="sxs-lookup"><span data-stu-id="46204-212">Choose the **Make Orders** action to create the production order.</span></span>  

     <span data-ttu-id="46204-213">На странице **Планирование заказов** обратите внимание на то, что строка планирования для заказа на продажу **1001** больше не существует, а первоначальное требование продажи выполнено.</span><span class="sxs-lookup"><span data-stu-id="46204-213">On the **Order Planning** page, notice that the planning line for sales order **1001** no longer exists and that the initial sales demand has been covered.</span></span>  

6.  <span data-ttu-id="46204-214">Закройте страницу **Планирование заказов**.</span><span class="sxs-lookup"><span data-stu-id="46204-214">Close the **Order Planning** page.</span></span>  

     <span data-ttu-id="46204-215">Теперь при желании можно остаться в этом представлении и выполнить все задачи планирования.</span><span class="sxs-lookup"><span data-stu-id="46204-215">Now, you could choose to stay in this view and complete all the planning tasks.</span></span> <span data-ttu-id="46204-216">Но вместо этого необходимо выполнить роль планировщика производства, перейдя к созданному производственному заказу и открыв страницу **Планирование заказов**.</span><span class="sxs-lookup"><span data-stu-id="46204-216">Instead, you will now take on the Production Planner role by going to the production order that you just created and access the **Order Planning** page.</span></span>  

 <span data-ttu-id="46204-217">В роли планировщика производства вы теперь должны спланировать определенный производственный заказ.</span><span class="sxs-lookup"><span data-stu-id="46204-217">As a production planner you now must plan a specific production order.</span></span>  

### <a name="to-plan-a-specific-production-order"></a><span data-ttu-id="46204-218">Процедура планирования производственного заказа</span><span class="sxs-lookup"><span data-stu-id="46204-218">To plan a specific production order</span></span>  

1.  <span data-ttu-id="46204-219">Откройте производственный заказ **101001** (для десяти велосипедов), который был только что создан с помощью функции **Заказы на изготовление**.</span><span class="sxs-lookup"><span data-stu-id="46204-219">Open the production order **101001**, for ten bicycles, that you just created by using the **Make Orders** function.</span></span>  
2.  <span data-ttu-id="46204-220">Откройте страницу **Компоненты производственного заказа**, чтобы убедиться, что дополнительный колокольчик отражен в производственном заказе.</span><span class="sxs-lookup"><span data-stu-id="46204-220">Open the **Prod. Order Components** page to check that the extra bell is reflected on the production order.</span></span>  
3.  <span data-ttu-id="46204-221">Выберите действие **Планирование**.</span><span class="sxs-lookup"><span data-stu-id="46204-221">Choose the **Planning** action.</span></span>  

     <span data-ttu-id="46204-222">Страница **Планирование заказов** открывается в таком виде, где всегда выполняется фильтрация по определенному производственному спросу.</span><span class="sxs-lookup"><span data-stu-id="46204-222">The **Order Planning** page opens in a view that is always filtered on the specific production demand.</span></span> <span data-ttu-id="46204-223">Требование продаж не отображается.</span><span class="sxs-lookup"><span data-stu-id="46204-223">Sales demand is not displayed.</span></span> <span data-ttu-id="46204-224">Для отображения дополнительных требований необходимо вычислить план.</span><span class="sxs-lookup"><span data-stu-id="46204-224">You must calculate a plan before you can see any additional demand.</span></span>  

4.  <span data-ttu-id="46204-225">Выберите действие **Вычислить план**.</span><span class="sxs-lookup"><span data-stu-id="46204-225">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="46204-226">Обратите внимание, что четыре новых производственных заказа отображаются в виде незапланированного требования производства, производного от заказа **101001**.</span><span class="sxs-lookup"><span data-stu-id="46204-226">Notice that four new production orders appear as unplanned production demand derived from order **101001**.</span></span> <span data-ttu-id="46204-227">Новые строки соответствуют новому требованию производства из сборочных узлов, которые необходимо создать для производства заказа.</span><span class="sxs-lookup"><span data-stu-id="46204-227">The new lines represent new production demand from the subassemblies that must be created to produce the order.</span></span>  

5.  <span data-ttu-id="46204-228">Выберите действие **Раскрыть все**, чтобы просмотреть все производственные требования для производственных заказов.</span><span class="sxs-lookup"><span data-stu-id="46204-228">Choose the **Expand All** action to get an overview of all the production demand for the production orders.</span></span>  

     <span data-ttu-id="46204-229">Чтобы указать дополнительные сведения о строках потребностей, в представление может потребоваться добавить поля **Необходимое количество** и **Доступное требуемое количество**.</span><span class="sxs-lookup"><span data-stu-id="46204-229">To provide additional information about the demand lines, you may want to add the **Demand Quantity** and **Demand Qty. Available** fields to your view.</span></span>  

     <span data-ttu-id="46204-230">Теперь необходимо поставить по десять штук каждого компонента.</span><span class="sxs-lookup"><span data-stu-id="46204-230">Now you must supply ten of each component.</span></span>  

     <span data-ttu-id="46204-231">Обратите внимание, что четыре строки спроса содержат метод пополнения "Произв. заказ".</span><span class="sxs-lookup"><span data-stu-id="46204-231">Note that four of the demand lines have replenishment system Prod. Order.</span></span> <span data-ttu-id="46204-232">Эти четыре сборочных узла соответствуют второму уровню производства велосипеда.</span><span class="sxs-lookup"><span data-stu-id="46204-232">These four subassemblies represent the second product level of the bicycle.</span></span>  

     <span data-ttu-id="46204-233">Настройки пополнения по умолчанию уже указаны, поэтому можно приступать к оформлению заказов.</span><span class="sxs-lookup"><span data-stu-id="46204-233">The default replenishment settings are already filled in and you can proceed to make orders.</span></span>  

6.  <span data-ttu-id="46204-234">Выберите действие **Создать заказы**.</span><span class="sxs-lookup"><span data-stu-id="46204-234">Choose the **Make Orders** action.</span></span>  

     <span data-ttu-id="46204-235">Перед выбором кнопки **ОК** обратите внимание на текст на экспресс-вкладке **Планирование заказов**.</span><span class="sxs-lookup"><span data-stu-id="46204-235">Before you choose the **OK** button, notice the text on the **Order Planning** FastTab.</span></span> <span data-ttu-id="46204-236">Этот текст важен, поскольку в структуре производства велосипеда есть несколько производимых компонентов, сборочных узлов, которые могут требоваться при создании этого производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="46204-236">This text is important because you know that the bicycle has several produced components, subassemblies, in its product structure that might be in demand when you create this production order.</span></span>  

7.  <span data-ttu-id="46204-237">На странице **Создание заказов на поставку** в поле **Заказы на изготовление для** выберите **Все строки**, а затем нажмите кнопку **ОК**, чтобы создать производственные заказы для второго уровня производства заказа.</span><span class="sxs-lookup"><span data-stu-id="46204-237">On the **Make Supply Order** page, in the **Make Orders for** field, choose the **All Lines** option, and then choose the **OK** button to create production orders for the second product level of the order.</span></span>  

     <span data-ttu-id="46204-238">Обратите внимание, что требование производства верхнего уровня для производственного заказа 101001 больше не существует.</span><span class="sxs-lookup"><span data-stu-id="46204-238">Note that the top-level production demand for production order 101001 no longer exists.</span></span> <span data-ttu-id="46204-239">Это означает, что первоначальное требование производства для сборочных узлов уже запланировано.</span><span class="sxs-lookup"><span data-stu-id="46204-239">This means that the initial production demand for subassemblies has been planned for.</span></span>  

     <span data-ttu-id="46204-240">На странице **Планирование заказов** план вычисляется повторно для планирования структуры велосипеда.</span><span class="sxs-lookup"><span data-stu-id="46204-240">On the **Order Planning** page, you calculate a plan again in order to plan the bicycle structure.</span></span>  

8.  <span data-ttu-id="46204-241">Выберите действие **Вычислить план**, чтобы повторно вычислить план, как указано в тексте встроенной справки.</span><span class="sxs-lookup"><span data-stu-id="46204-241">Choose the **Calculate Plan** action to recalculate the plan as instructed by the embedded Help text.</span></span>  

     <span data-ttu-id="46204-242">Две новые строки соответствуют дополнительному требованию производства из сборочных узлов, запланированных на предыдущих шагах.</span><span class="sxs-lookup"><span data-stu-id="46204-242">The two new lines represent additional production demand derived from the subassemblies planned in the previous steps.</span></span> <span data-ttu-id="46204-243">Предлагается сделать два производственных заказа для поставки барабанов (один для 10 втулок переднего колеса и один для 10 втулок заднего колеса).</span><span class="sxs-lookup"><span data-stu-id="46204-243">It is suggested that you make two production orders to supply the wheel hubs, one for 10 front hubs and one for 10 back hubs.</span></span>  

9. <span data-ttu-id="46204-244">Выберите действие **Раскрыть все**, чтобы просмотреть все требования для двух производственных заказов.</span><span class="sxs-lookup"><span data-stu-id="46204-244">Choose the **Expand All** action to get an overview of all the demand for the two production orders.</span></span>  

     <span data-ttu-id="46204-245">Предлагаемый план поставки указывает на то, что для компонентов в общей сложности будет создано четыре заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="46204-245">The suggested supply plan indicates that a total of four purchase orders will be created for the components.</span></span> <span data-ttu-id="46204-246">Решено сделать предлагаемые заказы.</span><span class="sxs-lookup"><span data-stu-id="46204-246">You decide to make the proposed orders.</span></span>  

10. <span data-ttu-id="46204-247">Выберите действие **Создать заказы**.</span><span class="sxs-lookup"><span data-stu-id="46204-247">Choose the **Make Orders** action.</span></span>  
11. <span data-ttu-id="46204-248">В поле **Заказы на изготовление для** выберите параметр **Все строки**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="46204-248">In the **Make Orders for** field, select the **All Lines** option, and then choose the **OK** button.</span></span> <span data-ttu-id="46204-249">Проверьте, есть ли дополнительные требования для производства родительского товара, велосипеда, который продается по заказу на продажу 1001.</span><span class="sxs-lookup"><span data-stu-id="46204-249">Check if additional demand exists for the production of the parent item, the bicycle, which is being sold on sales order 1001.</span></span>  
12. <span data-ttu-id="46204-250">Выберите действие **Вычислить план**.</span><span class="sxs-lookup"><span data-stu-id="46204-250">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="46204-251">В сообщении указывается, что теперь все необходимые товары поставлены.</span><span class="sxs-lookup"><span data-stu-id="46204-251">The message indicates that all required items are now supplied.</span></span> <span data-ttu-id="46204-252">Проверьте запланированные производственные заказы, которые были созданы.</span><span class="sxs-lookup"><span data-stu-id="46204-252">Verify the firm planned production orders that are created.</span></span>  

13. <span data-ttu-id="46204-253">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Утвержд. произв. заказы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="46204-253">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>  

     <span data-ttu-id="46204-254">На странице **Утвержд. произв. заказы** просмотрите, как запланировано время начала и завершения отдельных заказов в соответствии со структурой продукта.</span><span class="sxs-lookup"><span data-stu-id="46204-254">On the **Firm Planned Prod. Orders** page review how start times and end times of individual orders are scheduled according to the product structure.</span></span> <span data-ttu-id="46204-255">Сначала производятся компоненты самого нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="46204-255">The lowest-level components are produced first.</span></span> <span data-ttu-id="46204-256">Поэтому необходимо запланировать многоуровневые заказы так, как описано в этом рабочем процессе планирования.</span><span class="sxs-lookup"><span data-stu-id="46204-256">Therefore, you must plan multilevel orders as demonstrated in this planning workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="46204-257">См. также</span><span class="sxs-lookup"><span data-stu-id="46204-257">See Also</span></span>  
 <span data-ttu-id="46204-258">[Пошаговые руководства по бизнес-процессам](walkthrough-business-process-walkthroughs.md) </span><span class="sxs-lookup"><span data-stu-id="46204-258">[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md) </span></span>  
 [<span data-ttu-id="46204-259">Пошаговое руководство. Автоматическое планирование поставок</span><span class="sxs-lookup"><span data-stu-id="46204-259">Walkthrough: Planning Supplies Automatically</span></span>](walkthrough-planning-supplies-automatically.md)

