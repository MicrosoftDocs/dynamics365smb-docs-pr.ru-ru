---
title: Подбор и отгрузка в основных складских конфигурациях | Документация Майкрософт
description: В Business Central исходящие процессы по подбору и отгрузке могут быть выполнены четырьмя способами при помощи различных функций в зависимости от уровня сложности склада.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/24/2020
ms.author: sgroespe
ms.openlocfilehash: 475f32dbaf9b4b80a61e1cad542fbf6db79cb029
ms.sourcegitcommit: 3e9c89f90db5eaed599630299353300621fe4007
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "3528314"
---
# <a name="walkthrough-picking-and-shipping-in-basic-warehouse-configurations"></a><span data-ttu-id="7f77e-103">Пошаговое руководство. Подбор и отгрузка в основных складских конфигурациях</span><span class="sxs-lookup"><span data-stu-id="7f77e-103">Walkthrough: Picking and Shipping in Basic Warehouse Configurations</span></span>

[!INCLUDE[complete_sample_data](includes/complete_sample_data.md)]

<span data-ttu-id="7f77e-104">В [!INCLUDE[d365fin](includes/d365fin_md.md)] исходящие процессы по подбору и отгрузке могут быть выполнены четырьмя способами при помощи различных функций в зависимости от уровня сложности склада.</span><span class="sxs-lookup"><span data-stu-id="7f77e-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="7f77e-105">Метод</span><span class="sxs-lookup"><span data-stu-id="7f77e-105">Method</span></span>|<span data-ttu-id="7f77e-106">Входящий процесс</span><span class="sxs-lookup"><span data-stu-id="7f77e-106">Inbound process</span></span>|<span data-ttu-id="7f77e-107">Ячейки</span><span class="sxs-lookup"><span data-stu-id="7f77e-107">Bins</span></span>|<span data-ttu-id="7f77e-108">Складской подбор</span><span class="sxs-lookup"><span data-stu-id="7f77e-108">Picks</span></span>|<span data-ttu-id="7f77e-109">Расх. накладные</span><span class="sxs-lookup"><span data-stu-id="7f77e-109">Shipments</span></span>|<span data-ttu-id="7f77e-110">Уровень сложности (см. раздел [Сведения о проектировании: настройка склада](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="7f77e-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|-----------|---------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="7f77e-111">П</span><span class="sxs-lookup"><span data-stu-id="7f77e-111">A</span></span>|<span data-ttu-id="7f77e-112">Выполните учет подбора и отгрузки из строки заказа</span><span class="sxs-lookup"><span data-stu-id="7f77e-112">Post pick and shipment from the order line</span></span>|<span data-ttu-id="7f77e-113">X</span><span class="sxs-lookup"><span data-stu-id="7f77e-113">X</span></span>|||<span data-ttu-id="7f77e-114">2</span><span class="sxs-lookup"><span data-stu-id="7f77e-114">2</span></span>|  
|<span data-ttu-id="7f77e-115">Б</span><span class="sxs-lookup"><span data-stu-id="7f77e-115">B</span></span>|<span data-ttu-id="7f77e-116">Выполните учет подбора и отгрузки из складского документа подбора</span><span class="sxs-lookup"><span data-stu-id="7f77e-116">Post pick and shipment from an inventory pick document</span></span>||<span data-ttu-id="7f77e-117">X</span><span class="sxs-lookup"><span data-stu-id="7f77e-117">X</span></span>||<span data-ttu-id="7f77e-118">3</span><span class="sxs-lookup"><span data-stu-id="7f77e-118">3</span></span>|  
|<span data-ttu-id="7f77e-119">C</span><span class="sxs-lookup"><span data-stu-id="7f77e-119">C</span></span>|<span data-ttu-id="7f77e-120">Выполните учет подбора и отгрузку из документа складской отгрузки</span><span class="sxs-lookup"><span data-stu-id="7f77e-120">Post pick and shipment from a warehouse shipment document</span></span>|||<span data-ttu-id="7f77e-121">X</span><span class="sxs-lookup"><span data-stu-id="7f77e-121">X</span></span>|<span data-ttu-id="7f77e-122">4/5/6</span><span class="sxs-lookup"><span data-stu-id="7f77e-122">4/5/6</span></span>|  
|<span data-ttu-id="7f77e-123">D</span><span class="sxs-lookup"><span data-stu-id="7f77e-123">D</span></span>|<span data-ttu-id="7f77e-124">Выполните учет подбора из складского документа подбора и учет отгрузки из документа складской отгрузки</span><span class="sxs-lookup"><span data-stu-id="7f77e-124">Post pick from a warehouse pick document and post shipment from a warehouse shipment document</span></span>||<span data-ttu-id="7f77e-125">X</span><span class="sxs-lookup"><span data-stu-id="7f77e-125">X</span></span>|<span data-ttu-id="7f77e-126">X</span><span class="sxs-lookup"><span data-stu-id="7f77e-126">X</span></span>|<span data-ttu-id="7f77e-127">4/5/6</span><span class="sxs-lookup"><span data-stu-id="7f77e-127">4/5/6</span></span>|  

<span data-ttu-id="7f77e-128">Дополнительные сведения см. в разделе [Сведения о проектировании: исходящий складской поток](design-details-outbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="7f77e-128">For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="7f77e-129">В следующем пошаговом руководстве показан метод B в предыдущей таблице.</span><span class="sxs-lookup"><span data-stu-id="7f77e-129">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="7f77e-130">Об этом пошаговом руководстве</span><span class="sxs-lookup"><span data-stu-id="7f77e-130">About This Walkthrough</span></span>

<span data-ttu-id="7f77e-131">В основных складских конфигурациях, если настройки склада требуют обработки подбора, но не обработки отгрузки, то для регистрации и учета информации о подборе и отгрузке для исходящих документов-источников следует использовать страницу **Подбор запасов**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-131">In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Inventory Pick** page to record and post pick and ship information for your outbound source documents.</span></span> <span data-ttu-id="7f77e-132">Исходящий документ-источник может быть заказом на продажу, возвратом покупки, исходящим заказом перемещения или производственным заказом, для которого необходимы компоненты.</span><span class="sxs-lookup"><span data-stu-id="7f77e-132">The outbound source document can be a sales order, purchase return order, outbound transfer order, or a production order with component need.</span></span>  

<span data-ttu-id="7f77e-133">В этом пошаговом руководстве демонстрируются следующие задачи:</span><span class="sxs-lookup"><span data-stu-id="7f77e-133">This walkthrough demonstrates the following tasks:</span></span>  

- <span data-ttu-id="7f77e-134">Настройка склада "СЕРЕБРЯНЫЙ" для складских подборов.</span><span class="sxs-lookup"><span data-stu-id="7f77e-134">Setting up SILVER location for inventory picks.</span></span>  
- <span data-ttu-id="7f77e-135">Создание заказа на продажу для клиента 10000 на 30 громкоговорителей.</span><span class="sxs-lookup"><span data-stu-id="7f77e-135">Creating a sales order for customer 10000 for 30 loudspeakers.</span></span>  
- <span data-ttu-id="7f77e-136">Выпуск заказа на продажу для обработки на складе.</span><span class="sxs-lookup"><span data-stu-id="7f77e-136">Releasing the sales order for warehouse handling.</span></span>  
- <span data-ttu-id="7f77e-137">Создание складского подбора на основании выпущенного документа-источника.</span><span class="sxs-lookup"><span data-stu-id="7f77e-137">Creating an inventory pick based on a released source document.</span></span>  
- <span data-ttu-id="7f77e-138">Регистрация складского перемещения из склада с одновременным учетом расходной накладной продажи для исходного заказа на продажу.</span><span class="sxs-lookup"><span data-stu-id="7f77e-138">Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.</span></span>  

## <a name="roles"></a><span data-ttu-id="7f77e-139">Роли</span><span class="sxs-lookup"><span data-stu-id="7f77e-139">Roles</span></span>

<span data-ttu-id="7f77e-140">В этом пошаговом руководстве демонстрируются задачи, выполняемые исполнителями следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="7f77e-140">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

- <span data-ttu-id="7f77e-141">Заведующий складом</span><span class="sxs-lookup"><span data-stu-id="7f77e-141">Warehouse Manager</span></span>  
- <span data-ttu-id="7f77e-142">Обработчик заказов</span><span class="sxs-lookup"><span data-stu-id="7f77e-142">Order Processor</span></span>  
- <span data-ttu-id="7f77e-143">Работник склада</span><span class="sxs-lookup"><span data-stu-id="7f77e-143">Warehouse Worker</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="7f77e-144">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="7f77e-144">Prerequisites</span></span>

<span data-ttu-id="7f77e-145">Для выполнения данного пошагового руководства необходимо выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="7f77e-145">To complete this walkthrough, you will need:</span></span>  

- <span data-ttu-id="7f77e-146">Для интернет-версии [!INCLUDE[prodshort](includes/prodshort.md)], компания, основанная на параметре **Расширенный ознакомительный выпуск — полные демонстрационные данные** в среде песочницы.</span><span class="sxs-lookup"><span data-stu-id="7f77e-146">For [!INCLUDE[prodshort](includes/prodshort.md)] online, a company based on the **Advanced Evaluation - Complete Sample Data** option in a sandbox environment.</span></span> <span data-ttu-id="7f77e-147">Для [!INCLUDE[prodshort](includes/prodshort.md)] локальная версия, CRONUS International Ltd. установлена.</span><span class="sxs-lookup"><span data-stu-id="7f77e-147">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, CRONUS International Ltd. installed.</span></span>  
- <span data-ttu-id="7f77e-148">Чтобы назначить себя работником склада SILVER, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="7f77e-148">To make yourself a warehouse employee at the location SILVER by following these steps:</span></span>  

  1. <span data-ttu-id="7f77e-149">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сотрудники склада**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7f77e-149">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
  2. <span data-ttu-id="7f77e-150">Выберите поле **ИД пользователя** и укажите свою учетную запись пользователя на странице **Пользователи**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-150">Choose the **User ID** field, and select your own user account on the **Users** page.</span></span>  
  3. <span data-ttu-id="7f77e-151">В поле **Код склада** введите "СЕРЕБР".</span><span class="sxs-lookup"><span data-stu-id="7f77e-151">In the **Location Code** field, enter SILVER.</span></span>  
  4. <span data-ttu-id="7f77e-152">Выберите поле **По умолчанию**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-152">Select the **Default** field.</span></span>  

- <span data-ttu-id="7f77e-153">Сделайте товар LS-81 доступным на складе "СЕРЕБРЯНЫЙ" при помощи следующих шагов:</span><span class="sxs-lookup"><span data-stu-id="7f77e-153">Make item LS-81 available at SILVER location by following these steps:</span></span>  

  1. <span data-ttu-id="7f77e-154">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы товаров**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7f77e-154">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Journals**, and then choose the related link.</span></span>  
  2. <span data-ttu-id="7f77e-155">Откройте журнал по умолчанию, а затем создайте две строки журнала товаров со следующими сведениями о рабочей дате (23 января).</span><span class="sxs-lookup"><span data-stu-id="7f77e-155">Open the default journal, and then create two item journal lines with the following information about the work date (January 23).</span></span>  

        |<span data-ttu-id="7f77e-156">Тип операции</span><span class="sxs-lookup"><span data-stu-id="7f77e-156">Entry Type</span></span>|<span data-ttu-id="7f77e-157">Код товара</span><span class="sxs-lookup"><span data-stu-id="7f77e-157">Item Number</span></span>|<span data-ttu-id="7f77e-158">Код Склада</span><span class="sxs-lookup"><span data-stu-id="7f77e-158">Location Code</span></span>|<span data-ttu-id="7f77e-159">Код ячейки</span><span class="sxs-lookup"><span data-stu-id="7f77e-159">Bin Code</span></span>|<span data-ttu-id="7f77e-160">количество;</span><span class="sxs-lookup"><span data-stu-id="7f77e-160">Quantity</span></span>|  
        |----------------|-----------------|-------------------|--------------|--------------|  
        |<span data-ttu-id="7f77e-161">Приход</span><span class="sxs-lookup"><span data-stu-id="7f77e-161">Positive Adjmt.</span></span>|<span data-ttu-id="7f77e-162">LS-81</span><span class="sxs-lookup"><span data-stu-id="7f77e-162">LS-81</span></span>|<span data-ttu-id="7f77e-163">СЕРЕБР.</span><span class="sxs-lookup"><span data-stu-id="7f77e-163">SILVER</span></span>|<span data-ttu-id="7f77e-164">С-01-0001</span><span class="sxs-lookup"><span data-stu-id="7f77e-164">S-01-0001</span></span>|<span data-ttu-id="7f77e-165">20</span><span class="sxs-lookup"><span data-stu-id="7f77e-165">20</span></span>|  
        |<span data-ttu-id="7f77e-166">Приход</span><span class="sxs-lookup"><span data-stu-id="7f77e-166">Positive Adjmt.</span></span>|<span data-ttu-id="7f77e-167">LS-81</span><span class="sxs-lookup"><span data-stu-id="7f77e-167">LS-81</span></span>|<span data-ttu-id="7f77e-168">СЕРЕБР.</span><span class="sxs-lookup"><span data-stu-id="7f77e-168">SILVER</span></span>|<span data-ttu-id="7f77e-169">С-01-0002</span><span class="sxs-lookup"><span data-stu-id="7f77e-169">S-01-0002</span></span>|<span data-ttu-id="7f77e-170">20</span><span class="sxs-lookup"><span data-stu-id="7f77e-170">20</span></span>|  

  3. <span data-ttu-id="7f77e-171">Выберите действие **Учет**, затем выберите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-171">Choose the **Post** action, and then select the **Yes** button.</span></span>  

## <a name="story"></a><span data-ttu-id="7f77e-172">Сюжет</span><span class="sxs-lookup"><span data-stu-id="7f77e-172">Story</span></span>

<span data-ttu-id="7f77e-173">Элен, менеджер склада в CRONUS, настроила "СЕРЕБРЯНЫЙ" склад для базовой обработки подбора, где работники склада обрабатывают исходящие заказы по отдельности.</span><span class="sxs-lookup"><span data-stu-id="7f77e-173">Ellen, the warehouse manager at CRONUS, sets up SILVER warehouse for basic pick handling where warehouse workers process outbound orders individually.</span></span> <span data-ttu-id="7f77e-174">Светлана, обработчик заказов, создает заказ на продажу 30 единиц товара LS-81, которые должны быть поставлены клиенту 10000 из СЕРЕБРЯНОГО склада.</span><span class="sxs-lookup"><span data-stu-id="7f77e-174">Susan, the order processor, creates a sales order for 30 units of item LS-81 to be shipped to customer 10000 from the SILVER Warehouse.</span></span> <span data-ttu-id="7f77e-175">Вадим, работник склада, должен убедиться, что отгружаемый товар подготовлен и поставлен клиенту.</span><span class="sxs-lookup"><span data-stu-id="7f77e-175">John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer.</span></span> <span data-ttu-id="7f77e-176">Вадим управляет всеми включенными задачами на странице **Подбор запасов**, которое автоматически указывает на ячейки, где сохраняется LS-81.</span><span class="sxs-lookup"><span data-stu-id="7f77e-176">John manages all involved tasks on the **Inventory Pick** page, which automatically points to the bins where LS-81 is stored.</span></span>  

## <a name="setting-up-the-location"></a><span data-ttu-id="7f77e-177">Настройка склада</span><span class="sxs-lookup"><span data-stu-id="7f77e-177">Setting Up the Location</span></span>

<span data-ttu-id="7f77e-178">Настройка страницы **Карточка склада** определяет потоки склада организации.</span><span class="sxs-lookup"><span data-stu-id="7f77e-178">The setup of the **Location Card** page defines the company’s warehouse flows.</span></span>  

### <a name="to-set-up-the-location"></a><span data-ttu-id="7f77e-179">Настройка склада</span><span class="sxs-lookup"><span data-stu-id="7f77e-179">To set up the location</span></span>

1. <span data-ttu-id="7f77e-180">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Склады**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7f77e-180">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>  
2. <span data-ttu-id="7f77e-181">Откройте карточку склада СЕРЕБРЯНЫЙ.</span><span class="sxs-lookup"><span data-stu-id="7f77e-181">Open the SILVER location card.</span></span>  
3. <span data-ttu-id="7f77e-182">На экспресс-вкладке **Склад** установите флажок **Требуется подбор**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-182">On the **Warehouse** FastTab, choose the **Require Pick** check box.</span></span>  

## <a name="creating-the-sales-order"></a><span data-ttu-id="7f77e-183">Создание заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="7f77e-183">Creating the Sales Order</span></span>

<span data-ttu-id="7f77e-184">Заказы на продажу — это наиболее распространенный тип исходного исходящего документа.</span><span class="sxs-lookup"><span data-stu-id="7f77e-184">Sales orders are the most common type of outbound source document.</span></span>  

### <a name="to-create-the-sales-order"></a><span data-ttu-id="7f77e-185">Создание заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="7f77e-185">To create the sales order</span></span>

1. <span data-ttu-id="7f77e-186">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7f77e-186">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="7f77e-187">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-187">Choose the **New** action.</span></span>  
3. <span data-ttu-id="7f77e-188">Создайте заказ на продажу для клиента 10000 на рабочую дату (23 января) со следующей строкой заказа на продажу.</span><span class="sxs-lookup"><span data-stu-id="7f77e-188">Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.</span></span>  

    |<span data-ttu-id="7f77e-189">Товар</span><span class="sxs-lookup"><span data-stu-id="7f77e-189">Item</span></span>|<span data-ttu-id="7f77e-190">Код Склада</span><span class="sxs-lookup"><span data-stu-id="7f77e-190">Location Code</span></span>|<span data-ttu-id="7f77e-191">Количество</span><span class="sxs-lookup"><span data-stu-id="7f77e-191">Quantity</span></span>|  
    |----|-------------|--------|  
    |<span data-ttu-id="7f77e-192">LS_81</span><span class="sxs-lookup"><span data-stu-id="7f77e-192">LS_81</span></span>|<span data-ttu-id="7f77e-193">СЕРЕБР.</span><span class="sxs-lookup"><span data-stu-id="7f77e-193">SILVER</span></span>|<span data-ttu-id="7f77e-194">30</span><span class="sxs-lookup"><span data-stu-id="7f77e-194">30</span></span>|  

     <span data-ttu-id="7f77e-195">Перейти к уведомлению склада, что заказ на продажу готов для обработки на складе.</span><span class="sxs-lookup"><span data-stu-id="7f77e-195">Proceed to notify the warehouse that the sales order is ready for warehouse handling.</span></span>  

4. <span data-ttu-id="7f77e-196">Выберите действие **Выпустить**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-196">Choose the **Release** action.</span></span>  

    <span data-ttu-id="7f77e-197">Вадим переходит к подбору и отгрузке проданных товаров.</span><span class="sxs-lookup"><span data-stu-id="7f77e-197">John proceeds to pick and ship the sold items.</span></span>  

## <a name="picking-and-shipping-items"></a><span data-ttu-id="7f77e-198">Товары по подбору и отгрузке</span><span class="sxs-lookup"><span data-stu-id="7f77e-198">Picking and Shipping Items</span></span>

<span data-ttu-id="7f77e-199">На странице **Подбор запасов** можно управлять всеми исходящими складскими операциями для конкретного документа\-источника, такого как заказ на покупку.</span><span class="sxs-lookup"><span data-stu-id="7f77e-199">On the **Inventory Pick** page, you can manage all outbound warehouse activities for a specific source document, such as a sales order.</span></span> [!INCLUDE[tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

### <a name="to-pick-and-ship-items"></a><span data-ttu-id="7f77e-200">Подбор и отгрузка товаров</span><span class="sxs-lookup"><span data-stu-id="7f77e-200">To pick and ship items</span></span>

1. <span data-ttu-id="7f77e-201">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Подбор запасов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7f77e-201">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Picks**, and then choose the related link.</span></span>  
2. <span data-ttu-id="7f77e-202">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-202">Choose the **New** action.</span></span>  

    <span data-ttu-id="7f77e-203">Убедитесь, что поле **Нет.**</span><span class="sxs-lookup"><span data-stu-id="7f77e-203">Make sure that the **No.**</span></span> <span data-ttu-id="7f77e-204">на экспресс-вкладке **Общие** заполнено.</span><span class="sxs-lookup"><span data-stu-id="7f77e-204">field on the **General** FastTab is filled in.</span></span>
3. <span data-ttu-id="7f77e-205">Выберите поле **Документ\-источник**, а затем выберите **Заказ на продажу**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-205">Select the **Source Document** field, and then select **Sales Order**.</span></span>  
4. <span data-ttu-id="7f77e-206">Выберите поле **Номер источника**, выберите строку для продажи клиенту 10000, а затем выберите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-206">Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="7f77e-207">В качестве альтернативы выберите действие **Получить источник документа**, а затем выберите заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="7f77e-207">Alternatively, choose the **Get Source Document** action, and then select the sales order.</span></span>  
5. <span data-ttu-id="7f77e-208">Выберите действие **Автозаполнение кол-ва для обработки**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-208">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="7f77e-209">В качестве альтернативы в поле **Кол-во для обработки** введите 10 и 20 соответственно в двух строках складского подбора.</span><span class="sxs-lookup"><span data-stu-id="7f77e-209">Alternatively, in the **Qty. to Handle** field, enter 10 and 20 respectively on the two inventory pick lines.</span></span>  
6. <span data-ttu-id="7f77e-210">Выберите действие **Учет**, выберите **Отгрузить**, затем выберите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="7f77e-210">Choose the **Post** action, select **Ship**, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="7f77e-211">Теперь 30 громкоговорителей зарегистрированы как подобранные из ячеек С-01-0001 и С-01-0002, и создана отрицательная операция товарной книги, отражающая учтенную расходную накладную продажи.</span><span class="sxs-lookup"><span data-stu-id="7f77e-211">The 30 loudspeakers are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7f77e-212">См. также</span><span class="sxs-lookup"><span data-stu-id="7f77e-212">See Also</span></span>

[<span data-ttu-id="7f77e-213">Подбор товаров с помощью подбора запасов</span><span class="sxs-lookup"><span data-stu-id="7f77e-213">Pick Items with Inventory Picks</span></span>](warehouse-how-to-pick-items-with-inventory-picks.md)  
[<span data-ttu-id="7f77e-214">Подбор товаров для складской отгрузки</span><span class="sxs-lookup"><span data-stu-id="7f77e-214">Pick Items for Warehouse Shipment</span></span>](warehouse-how-to-pick-items-for-warehouse-shipment.md)  
[<span data-ttu-id="7f77e-215">Настройка базовых складов с помощью зон операций</span><span class="sxs-lookup"><span data-stu-id="7f77e-215">Set Up Basic Warehouses with Operations Areas</span></span>](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)  
[<span data-ttu-id="7f77e-216">Перемещение компонентов в производственную зону в базовых конфигурациях склада</span><span class="sxs-lookup"><span data-stu-id="7f77e-216">Move Components to an Operation Area in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)  
[<span data-ttu-id="7f77e-217">Подбор для производства или сборки</span><span class="sxs-lookup"><span data-stu-id="7f77e-217">Pick for Production or Assembly</span></span>](warehouse-how-to-pick-for-production.md)  
[<span data-ttu-id="7f77e-218">Перемещение специальных товаров в базовых конфигурациях склада</span><span class="sxs-lookup"><span data-stu-id="7f77e-218">Move Items Ad Hoc in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)  
[<span data-ttu-id="7f77e-219">Сведения о проектировании: исходящий складской поток</span><span class="sxs-lookup"><span data-stu-id="7f77e-219">Design Details: Outbound Warehouse Flow</span></span>](design-details-outbound-warehouse-flow.md)  
[<span data-ttu-id="7f77e-220">Пошаговые описания бизнес-процессов</span><span class="sxs-lookup"><span data-stu-id="7f77e-220">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
<span data-ttu-id="7f77e-221">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7f77e-221">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
