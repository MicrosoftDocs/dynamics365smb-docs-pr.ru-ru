---
title: Подбор и отгрузка в основных складских конфигурациях
description: В Business Central исходящие процессы по подбору и отгрузке могут быть выполнены четырьмя способами при помощи различных функций в зависимости от уровня сложности склада.
author: jill-kotel-andersson
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 05/27/2021
ms.author: edupont
ms.openlocfilehash: e1763e6288c8b8218955049ba7ef4c461ee5164e
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "6214657"
---
# <a name="walkthrough-picking-and-shipping-in-basic-warehouse-configurations"></a><span data-ttu-id="993f6-103">Пошаговое руководство. Подбор и отгрузка в основных складских конфигурациях</span><span class="sxs-lookup"><span data-stu-id="993f6-103">Walkthrough: Picking and Shipping in Basic Warehouse Configurations</span></span>

<!-- [!INCLUDE[complete_sample_data](includes/complete_sample_data.md)] -->

<span data-ttu-id="993f6-104">В [!INCLUDE[prod_short](includes/prod_short.md)] исходящие процессы по подбору и отгрузке могут быть выполнены четырьмя способами при помощи различных функций в зависимости от уровня сложности склада.</span><span class="sxs-lookup"><span data-stu-id="993f6-104">In [!INCLUDE[prod_short](includes/prod_short.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="993f6-105">Метод</span><span class="sxs-lookup"><span data-stu-id="993f6-105">Method</span></span>|<span data-ttu-id="993f6-106">Входящий процесс</span><span class="sxs-lookup"><span data-stu-id="993f6-106">Inbound process</span></span>|<span data-ttu-id="993f6-107">Ячейки</span><span class="sxs-lookup"><span data-stu-id="993f6-107">Bins</span></span>|<span data-ttu-id="993f6-108">Складской подбор</span><span class="sxs-lookup"><span data-stu-id="993f6-108">Picks</span></span>|<span data-ttu-id="993f6-109">Расх. накладные</span><span class="sxs-lookup"><span data-stu-id="993f6-109">Shipments</span></span>|<span data-ttu-id="993f6-110">Уровень сложности (см. раздел [Сведения о проектировании: настройка склада](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="993f6-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|-----------|---------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="993f6-111">П</span><span class="sxs-lookup"><span data-stu-id="993f6-111">A</span></span>|<span data-ttu-id="993f6-112">Выполните учет подбора и отгрузки из строки заказа</span><span class="sxs-lookup"><span data-stu-id="993f6-112">Post pick and shipment from the order line</span></span>|<span data-ttu-id="993f6-113">X</span><span class="sxs-lookup"><span data-stu-id="993f6-113">X</span></span>|||<span data-ttu-id="993f6-114">2</span><span class="sxs-lookup"><span data-stu-id="993f6-114">2</span></span>|  
|<span data-ttu-id="993f6-115">Б</span><span class="sxs-lookup"><span data-stu-id="993f6-115">B</span></span>|<span data-ttu-id="993f6-116">Выполните учет подбора и отгрузки из складского документа подбора</span><span class="sxs-lookup"><span data-stu-id="993f6-116">Post pick and shipment from an inventory pick document</span></span>||<span data-ttu-id="993f6-117">X</span><span class="sxs-lookup"><span data-stu-id="993f6-117">X</span></span>||<span data-ttu-id="993f6-118">3</span><span class="sxs-lookup"><span data-stu-id="993f6-118">3</span></span>|  
|<span data-ttu-id="993f6-119">C</span><span class="sxs-lookup"><span data-stu-id="993f6-119">C</span></span>|<span data-ttu-id="993f6-120">Выполните учет подбора и отгрузку из документа складской отгрузки</span><span class="sxs-lookup"><span data-stu-id="993f6-120">Post pick and shipment from a warehouse shipment document</span></span>|||<span data-ttu-id="993f6-121">X</span><span class="sxs-lookup"><span data-stu-id="993f6-121">X</span></span>|<span data-ttu-id="993f6-122">4/5/6</span><span class="sxs-lookup"><span data-stu-id="993f6-122">4/5/6</span></span>|  
|<span data-ttu-id="993f6-123">D</span><span class="sxs-lookup"><span data-stu-id="993f6-123">D</span></span>|<span data-ttu-id="993f6-124">Выполните учет подбора из складского документа подбора и учет отгрузки из документа складской отгрузки</span><span class="sxs-lookup"><span data-stu-id="993f6-124">Post pick from a warehouse pick document and post shipment from a warehouse shipment document</span></span>||<span data-ttu-id="993f6-125">X</span><span class="sxs-lookup"><span data-stu-id="993f6-125">X</span></span>|<span data-ttu-id="993f6-126">X</span><span class="sxs-lookup"><span data-stu-id="993f6-126">X</span></span>|<span data-ttu-id="993f6-127">4/5/6</span><span class="sxs-lookup"><span data-stu-id="993f6-127">4/5/6</span></span>|  

<span data-ttu-id="993f6-128">Дополнительные сведения см. в разделе [Сведения о проектировании: исходящий складской поток](design-details-outbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="993f6-128">For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="993f6-129">В следующем пошаговом руководстве показан метод B в предыдущей таблице.</span><span class="sxs-lookup"><span data-stu-id="993f6-129">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="993f6-130">Об этом пошаговом руководстве</span><span class="sxs-lookup"><span data-stu-id="993f6-130">About This Walkthrough</span></span>

<span data-ttu-id="993f6-131">В основных складских конфигурациях, если настройки склада требуют обработки подбора, но не обработки отгрузки, то для регистрации и учета информации о подборе и отгрузке для исходящих документов-источников следует использовать страницу **Подбор запасов**.</span><span class="sxs-lookup"><span data-stu-id="993f6-131">In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Inventory Pick** page to record and post pick and ship information for your outbound source documents.</span></span> <span data-ttu-id="993f6-132">Исходящий документ-источник может быть заказом на продажу, возвратом покупки, исходящим заказом перемещения или производственным заказом, для которого необходимы компоненты.</span><span class="sxs-lookup"><span data-stu-id="993f6-132">The outbound source document can be a sales order, purchase return order, outbound transfer order, or a production order with component need.</span></span>  

<span data-ttu-id="993f6-133">В этом пошаговом руководстве демонстрируются следующие задачи:</span><span class="sxs-lookup"><span data-stu-id="993f6-133">This walkthrough demonstrates the following tasks:</span></span>  

- <span data-ttu-id="993f6-134">Настройка склада "ЮГ" для складских подборов.</span><span class="sxs-lookup"><span data-stu-id="993f6-134">Setting up SOUTH location for inventory picks.</span></span>  
- <span data-ttu-id="993f6-135">Создание заказа на продажу для клиента 10000 на 30 ламп Амстердам.</span><span class="sxs-lookup"><span data-stu-id="993f6-135">Creating a sales order for customer 10000 for 30 Amsterdam Lamps.</span></span>  
- <span data-ttu-id="993f6-136">Выпуск заказа на продажу для обработки на складе.</span><span class="sxs-lookup"><span data-stu-id="993f6-136">Releasing the sales order for warehouse handling.</span></span>  
- <span data-ttu-id="993f6-137">Создание складского подбора на основании выпущенного документа-источника.</span><span class="sxs-lookup"><span data-stu-id="993f6-137">Creating an inventory pick based on a released source document.</span></span>  
- <span data-ttu-id="993f6-138">Регистрация складского перемещения из склада с одновременным учетом расходной накладной продажи для исходного заказа на продажу.</span><span class="sxs-lookup"><span data-stu-id="993f6-138">Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.</span></span>  

## <a name="roles"></a><span data-ttu-id="993f6-139">Роли</span><span class="sxs-lookup"><span data-stu-id="993f6-139">Roles</span></span>

<span data-ttu-id="993f6-140">В этом пошаговом руководстве демонстрируются задачи, выполняемые исполнителями следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="993f6-140">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

- <span data-ttu-id="993f6-141">Заведующий складом</span><span class="sxs-lookup"><span data-stu-id="993f6-141">Warehouse Manager</span></span>  
- <span data-ttu-id="993f6-142">Обработчик заказов</span><span class="sxs-lookup"><span data-stu-id="993f6-142">Order Processor</span></span>  
- <span data-ttu-id="993f6-143">Работник склада</span><span class="sxs-lookup"><span data-stu-id="993f6-143">Warehouse Worker</span></span>  

<!-- ## Prerequisites

To complete this walkthrough, you will need:  

- For [!INCLUDE[prod_short](includes/prod_short.md)] online, a company based on the **Advanced Evaluation - Complete Sample Data** option in a sandbox environment. For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, CRONUS installed.
 -->

## <a name="story"></a><span data-ttu-id="993f6-144">Сюжет</span><span class="sxs-lookup"><span data-stu-id="993f6-144">Story</span></span>

<span data-ttu-id="993f6-145">Элен, менеджер склада в CRONUS, настроила "ЮГ" склад для базовой обработки подбора, где работники склада обрабатывают исходящие заказы по отдельности.</span><span class="sxs-lookup"><span data-stu-id="993f6-145">Ellen, the warehouse manager at CRONUS, sets up SOUTH warehouse for basic pick handling where warehouse workers process outbound orders individually.</span></span> <span data-ttu-id="993f6-146">Светлана, обработчик заказов, создает заказ на продажу 30 единиц товара 1928-S, которые должны быть поставлены клиенту 10000 из склада "ЮГ".</span><span class="sxs-lookup"><span data-stu-id="993f6-146">Susan, the order processor, creates a sales order for 30 units of item 1928-S to be shipped to customer 10000 from the SOUTH Warehouse.</span></span> <span data-ttu-id="993f6-147">Вадим, работник склада, должен убедиться, что отгружаемый товар подготовлен и поставлен клиенту.</span><span class="sxs-lookup"><span data-stu-id="993f6-147">John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer.</span></span> <span data-ttu-id="993f6-148">Вадим управляет всеми включенными задачами на странице **Подбор запасов**, которое автоматически указывает на ячейки, где сохраняется 1928-S.</span><span class="sxs-lookup"><span data-stu-id="993f6-148">John manages all involved tasks on the **Inventory Pick** page, which automatically points to the bins where 1928-S is stored.</span></span>

[!INCLUDE[set_up_location.md](includes/set_up_location.md)]

### <a name="setting-up-the-bin-codes"></a><span data-ttu-id="993f6-149">Настройка кодов ячеек</span><span class="sxs-lookup"><span data-stu-id="993f6-149">Setting Up the Bin Codes</span></span>
<span data-ttu-id="993f6-150">После того, как вы настроили склад, вы должны добавить две ячейки.</span><span class="sxs-lookup"><span data-stu-id="993f6-150">Once you have the location set up, you must add two bins.</span></span>

#### <a name="to-setup-the-bin-codes"></a><span data-ttu-id="993f6-151">Настройка кодов ячеек</span><span class="sxs-lookup"><span data-stu-id="993f6-151">To setup the bin codes</span></span>

1. <span data-ttu-id="993f6-152">Выберите действие **Ячейки**.</span><span class="sxs-lookup"><span data-stu-id="993f6-152">Select the **Bins** action.</span></span>
2. <span data-ttu-id="993f6-153">Создайте две ячейки с кодами *S-01-0001* и *S-01-0002*.</span><span class="sxs-lookup"><span data-stu-id="993f6-153">Create two bins, with the codes *S-01-0001* and *S-01-0002*.</span></span>

### <a name="making-yourself-a-warehouse-employee-at-location-south"></a><span data-ttu-id="993f6-154">Назначения себя сотрудником склада "ЮГ"</span><span class="sxs-lookup"><span data-stu-id="993f6-154">Making Yourself a Warehouse Employee at Location SOUTH</span></span>

<span data-ttu-id="993f6-155">Чтобы использовать эту функцию, вы должны добавить себя на склад в качестве складского работника.</span><span class="sxs-lookup"><span data-stu-id="993f6-155">In order to use this functionality, you must add yourself to the location as a warehouse worker.</span></span> 

#### <a name="to-make-yourself-a-warehouse-employee"></a><span data-ttu-id="993f6-156">Чтобы назначить себя работником склада</span><span class="sxs-lookup"><span data-stu-id="993f6-156">To make yourself a warehouse employee</span></span>

  1. <span data-ttu-id="993f6-157">Выберите первый значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сотрудники склада**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="993f6-157">Choose the ![Lightbulb that opens the Tell Me feature first](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
  2. <span data-ttu-id="993f6-158">Выберите поле **ИД пользователя** и укажите свою учетную запись пользователя на странице **Работники склада**.</span><span class="sxs-lookup"><span data-stu-id="993f6-158">Choose the **User ID** field, and select your own user account on the **Warehouse Employees** page.</span></span>
  3. <span data-ttu-id="993f6-159">В поле **Код склада** выберите "ЮГ".</span><span class="sxs-lookup"><span data-stu-id="993f6-159">In the **Location Code** field, choose SOUTH.</span></span>  
  4. <span data-ttu-id="993f6-160">Выберите поле **По умолчанию**, затем выберите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="993f6-160">Select the **Default** field, and then select the **Yes** button.</span></span>  

### <a name="making-item-1928-s-available"></a><span data-ttu-id="993f6-161">Делаем товар 1928-S доступным</span><span class="sxs-lookup"><span data-stu-id="993f6-161">Making Item 1928-S Available</span></span>

<span data-ttu-id="993f6-162">Чтобы сделать товар 1928-S доступным на складе "ЮГ", выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="993f6-162">To make item 1928-S available at the SOUTH location follow these steps:</span></span>  

  1. <span data-ttu-id="993f6-163">Выберите второй значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы товаров**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="993f6-163">Choose the ![Lightbulb that opens the Tell Me feature second](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Journals**, and then choose the related link.</span></span>  
  2. <span data-ttu-id="993f6-164">Откройте журнал по умолчанию, а затем создайте две строки журнала товаров со следующими сведениями о рабочей дате (23 января).</span><span class="sxs-lookup"><span data-stu-id="993f6-164">Open the default journal, and then create two item journal lines with the following information about the work date (January 23).</span></span>  

        |<span data-ttu-id="993f6-165">Тип операции</span><span class="sxs-lookup"><span data-stu-id="993f6-165">Entry Type</span></span>|<span data-ttu-id="993f6-166">Код товара</span><span class="sxs-lookup"><span data-stu-id="993f6-166">Item Number</span></span>|<span data-ttu-id="993f6-167">Код Склада</span><span class="sxs-lookup"><span data-stu-id="993f6-167">Location Code</span></span>|<span data-ttu-id="993f6-168">Код ячейки</span><span class="sxs-lookup"><span data-stu-id="993f6-168">Bin Code</span></span>|<span data-ttu-id="993f6-169">количество;</span><span class="sxs-lookup"><span data-stu-id="993f6-169">Quantity</span></span>|  
        |----------------|-----------------|-------------------|--------------|--------------|  
        |<span data-ttu-id="993f6-170">Приход</span><span class="sxs-lookup"><span data-stu-id="993f6-170">Positive Adjmt.</span></span>|<span data-ttu-id="993f6-171">1928-S</span><span class="sxs-lookup"><span data-stu-id="993f6-171">1928-S</span></span>|<span data-ttu-id="993f6-172">ЮГ</span><span class="sxs-lookup"><span data-stu-id="993f6-172">SOUTH</span></span>|<span data-ttu-id="993f6-173">С-01-0001</span><span class="sxs-lookup"><span data-stu-id="993f6-173">S-01-0001</span></span>|<span data-ttu-id="993f6-174">20</span><span class="sxs-lookup"><span data-stu-id="993f6-174">20</span></span>|  
        |<span data-ttu-id="993f6-175">Приход</span><span class="sxs-lookup"><span data-stu-id="993f6-175">Positive Adjmt.</span></span>|<span data-ttu-id="993f6-176">1928-S</span><span class="sxs-lookup"><span data-stu-id="993f6-176">1928-S</span></span>|<span data-ttu-id="993f6-177">ЮГ</span><span class="sxs-lookup"><span data-stu-id="993f6-177">SOUTH</span></span>|<span data-ttu-id="993f6-178">С-01-0002</span><span class="sxs-lookup"><span data-stu-id="993f6-178">S-01-0002</span></span>|<span data-ttu-id="993f6-179">20</span><span class="sxs-lookup"><span data-stu-id="993f6-179">20</span></span>|  

        <span data-ttu-id="993f6-180">По умолчанию поле **Код ячейки** в строках продаж скрыто, поэтому необходимо включить его отображение.</span><span class="sxs-lookup"><span data-stu-id="993f6-180">By default, the **Bin Code** field on the sales lines are hidden, so you must display it.</span></span> <span data-ttu-id="993f6-181">Для этого вам необходимо персонализировать страницу.</span><span class="sxs-lookup"><span data-stu-id="993f6-181">To do this you need to personalize the page.</span></span> <span data-ttu-id="993f6-182">Дополнительные сведения см. в разделе [Чтобы начать персонализацию страницы с помощью баннера персонализации](ui-personalization-user.md#to-start-personalizing-a-page-through-the-personalizing-banner).</span><span class="sxs-lookup"><span data-stu-id="993f6-182">For more information, see [To start personalizing a page through the Personalizing banner](ui-personalization-user.md#to-start-personalizing-a-page-through-the-personalizing-banner).</span></span>

  3. <span data-ttu-id="993f6-183">Выберите **Действия**, выберите **Учет** а затем выберите **Учет**.</span><span class="sxs-lookup"><span data-stu-id="993f6-183">Choose **Actions**, then **Posting**, and then choose **Post**.</span></span>  
  4. <span data-ttu-id="993f6-184">Нажмите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="993f6-184">Select the **Yes** button.</span></span>  

## <a name="creating-the-sales-order"></a><span data-ttu-id="993f6-185">Создание заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="993f6-185">Creating the Sales Order</span></span>

<span data-ttu-id="993f6-186">Заказы на продажу — это наиболее распространенный тип исходного исходящего документа.</span><span class="sxs-lookup"><span data-stu-id="993f6-186">Sales orders are the most common type of outbound source document.</span></span>  

### <a name="to-create-the-sales-order"></a><span data-ttu-id="993f6-187">Создание заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="993f6-187">To create the sales order</span></span>

1. <span data-ttu-id="993f6-188">Выберите третий значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="993f6-188">Choose the ![Lightbulb that opens the Tell Me feature third](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="993f6-189">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="993f6-189">Choose the **New** action.</span></span>  
3. <span data-ttu-id="993f6-190">Создайте заказ на продажу для клиента 10000 на рабочую дату (23 января) со следующей строкой заказа на продажу.</span><span class="sxs-lookup"><span data-stu-id="993f6-190">Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.</span></span>  

    |<span data-ttu-id="993f6-191">Товар</span><span class="sxs-lookup"><span data-stu-id="993f6-191">Item</span></span>|<span data-ttu-id="993f6-192">Код Склада</span><span class="sxs-lookup"><span data-stu-id="993f6-192">Location Code</span></span>|<span data-ttu-id="993f6-193">количество;</span><span class="sxs-lookup"><span data-stu-id="993f6-193">Quantity</span></span>|  
    |----|-------------|--------|  
    |<span data-ttu-id="993f6-194">1928-S</span><span class="sxs-lookup"><span data-stu-id="993f6-194">1928-S</span></span>|<span data-ttu-id="993f6-195">ЮГ</span><span class="sxs-lookup"><span data-stu-id="993f6-195">SOUTH</span></span>|<span data-ttu-id="993f6-196">30</span><span class="sxs-lookup"><span data-stu-id="993f6-196">30</span></span>|  

     <span data-ttu-id="993f6-197">Перейти к уведомлению склада, что заказ на продажу готов для обработки на складе.</span><span class="sxs-lookup"><span data-stu-id="993f6-197">Proceed to notify the warehouse that the sales order is ready for warehouse handling.</span></span>  

4. <span data-ttu-id="993f6-198">Выберите действие **Выпустить**.</span><span class="sxs-lookup"><span data-stu-id="993f6-198">Choose the **Release** action.</span></span>  

    <span data-ttu-id="993f6-199">Вадим переходит к подбору и отгрузке проданных товаров.</span><span class="sxs-lookup"><span data-stu-id="993f6-199">John proceeds to pick and ship the sold items.</span></span>  

## <a name="picking-and-shipping-items"></a><span data-ttu-id="993f6-200">Товары по подбору и отгрузке</span><span class="sxs-lookup"><span data-stu-id="993f6-200">Picking and Shipping Items</span></span>

<span data-ttu-id="993f6-201">На странице **Подбор запасов** можно управлять всеми исходящими складскими операциями для конкретного документа\-источника, такого как заказ на покупку.</span><span class="sxs-lookup"><span data-stu-id="993f6-201">On the **Inventory Pick** page, you can manage all outbound warehouse activities for a specific source document, such as a sales order.</span></span> [!INCLUDE[tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

### <a name="to-pick-and-ship-items"></a><span data-ttu-id="993f6-202">Подбор и отгрузка товаров</span><span class="sxs-lookup"><span data-stu-id="993f6-202">To pick and ship items</span></span>

1. <span data-ttu-id="993f6-203">Выберите четвертый значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Подбор запасов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="993f6-203">Choose the ![Lightbulb that opens the Tell Me feature fourth](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Picks**, and then choose the related link.</span></span>  
2. <span data-ttu-id="993f6-204">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="993f6-204">Choose the **New** action.</span></span>  

    <span data-ttu-id="993f6-205">Убедитесь, что поле **Нет.**</span><span class="sxs-lookup"><span data-stu-id="993f6-205">Make sure that the **No.**</span></span> <span data-ttu-id="993f6-206">на экспресс-вкладке **Общие** заполнено.</span><span class="sxs-lookup"><span data-stu-id="993f6-206">field on the **General** FastTab is filled in.</span></span>
3. <span data-ttu-id="993f6-207">Выберите поле **Документ\-источник**, а затем выберите **Заказ на продажу**.</span><span class="sxs-lookup"><span data-stu-id="993f6-207">Select the **Source Document** field, and then select **Sales Order**.</span></span>  
4. <span data-ttu-id="993f6-208">Выберите поле **Номер источника**, выберите строку для продажи клиенту 10000, а затем выберите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="993f6-208">Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="993f6-209">В качестве альтернативы выберите действие **Получить источник документа**, а затем выберите заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="993f6-209">Alternatively, choose the **Get Source Document** action, and then select the sales order.</span></span>  
5. <span data-ttu-id="993f6-210">Выберите действие **Автозаполнение кол-ва для обработки**.</span><span class="sxs-lookup"><span data-stu-id="993f6-210">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="993f6-211">В качестве альтернативы в поле **Кол-во для обработки** введите 10 и 20 соответственно в двух строках складского подбора.</span><span class="sxs-lookup"><span data-stu-id="993f6-211">Alternatively, in the **Qty. to Handle** field, enter 10 and 20 respectively on the two inventory pick lines.</span></span>  
6. <span data-ttu-id="993f6-212">Выберите действие **Учет**, выберите **Отгрузить**, затем выберите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="993f6-212">Choose the **Post** action, select **Ship**, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="993f6-213">Теперь 30 фонарей Амстердам зарегистрированы как подобранные из ячеек С-01-0001 и С-01-0002, и создана отрицательная операция товарной книги, отражающая учтенную расходную накладную продажи.</span><span class="sxs-lookup"><span data-stu-id="993f6-213">The 30 Amsterdam Lamps are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="993f6-214">См. также</span><span class="sxs-lookup"><span data-stu-id="993f6-214">See Also</span></span>

[<span data-ttu-id="993f6-215">Подбор товаров с помощью подбора запасов</span><span class="sxs-lookup"><span data-stu-id="993f6-215">Pick Items with Inventory Picks</span></span>](warehouse-how-to-pick-items-with-inventory-picks.md)  
[<span data-ttu-id="993f6-216">Подбор товаров для складской отгрузки</span><span class="sxs-lookup"><span data-stu-id="993f6-216">Pick Items for Warehouse Shipment</span></span>](warehouse-how-to-pick-items-for-warehouse-shipment.md)  
[<span data-ttu-id="993f6-217">Настройка базовых складов с помощью зон операций</span><span class="sxs-lookup"><span data-stu-id="993f6-217">Set Up Basic Warehouses with Operations Areas</span></span>](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)  
[<span data-ttu-id="993f6-218">Перемещение компонентов в производственную зону в базовых конфигурациях склада</span><span class="sxs-lookup"><span data-stu-id="993f6-218">Move Components to an Operation Area in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)  
[<span data-ttu-id="993f6-219">Подбор для производства или сборки</span><span class="sxs-lookup"><span data-stu-id="993f6-219">Pick for Production or Assembly</span></span>](warehouse-how-to-pick-for-production.md)  
[<span data-ttu-id="993f6-220">Перемещение специальных товаров в базовых конфигурациях склада</span><span class="sxs-lookup"><span data-stu-id="993f6-220">Move Items Ad Hoc in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)  
[<span data-ttu-id="993f6-221">Сведения о проектировании: исходящий складской поток</span><span class="sxs-lookup"><span data-stu-id="993f6-221">Design Details: Outbound Warehouse Flow</span></span>](design-details-outbound-warehouse-flow.md)  
[<span data-ttu-id="993f6-222">Пошаговые описания бизнес-процессов</span><span class="sxs-lookup"><span data-stu-id="993f6-222">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
<span data-ttu-id="993f6-223">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="993f6-223">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]
