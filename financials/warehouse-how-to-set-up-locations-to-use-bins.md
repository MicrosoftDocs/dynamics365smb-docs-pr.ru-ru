---
title: "Как настраивать склады для использования ячеек | Документы Майкрософт"
description: "Ячейки являются базовой складской структурой и используются для формирования предложений по размещению товаров. После создания ячеек можно четко определить содержимое для помещения в каждую ячейку; ячейка может также функционировать в качестве плавающей ячейки без определенного содержимого."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 2d84f1222dccca86f5906af1c82fc0e6192173d6
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="set-up-locations-to-use-bins"></a><span data-ttu-id="844bb-104">Настройка складов для использования ячеек</span><span class="sxs-lookup"><span data-stu-id="844bb-104">Set Up Locations to Use Bins</span></span>
<span data-ttu-id="844bb-105">Ячейки являются базовой складской структурой и используются для формирования предложений по размещению товаров.</span><span class="sxs-lookup"><span data-stu-id="844bb-105">Bins represent the basic warehouse structure and are used to make suggestions about the placement of items.</span></span> <span data-ttu-id="844bb-106">После создания ячеек можно четко определить содержимое для помещения в каждую ячейку; ячейка может также функционировать в качестве плавающей ячейки без определенного содержимого.</span><span class="sxs-lookup"><span data-stu-id="844bb-106">When you have created your bins, you can define very specifically the contents that you want to place in each bin, or the bin can function as a floating bin without specified contents.</span></span>  

<span data-ttu-id="844bb-107">Чтобы воспользоваться функциями ячейки на складе, их нужно сначала активировать в карточке **Склад**.</span><span class="sxs-lookup"><span data-stu-id="844bb-107">To use the bin functionality at a location, you first activate the functionality on the **Location** card.</span></span> <span data-ttu-id="844bb-108">Затем разрабатывается поток товаров на складе путем указания кодов ячеек в полях настройки, представляющих различные потоки.</span><span class="sxs-lookup"><span data-stu-id="844bb-108">Then you design the item flow at the location by specifying bin codes in setup fields that represent the different flows.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="844bb-109">Прежде чем можно будет указать коды ячеек в карточке склада, эти коды ячеек необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="844bb-109">Before you can specify bin codes on the location card, the bin codes must be created.</span></span> <span data-ttu-id="844bb-110">Дополнительные сведения см. в разделе [Создание ячеек](warehouse-how-to-create-individual-bins.md).</span><span class="sxs-lookup"><span data-stu-id="844bb-110">For more information, see [Create Bins](warehouse-how-to-create-individual-bins.md).</span></span>  

## <a name="to-set-up-a-location-to-use-bins"></a><span data-ttu-id="844bb-111">Настройка склада для использования ячеек</span><span class="sxs-lookup"><span data-stu-id="844bb-111">To set up a location to use bins</span></span>  
1.  <span data-ttu-id="844bb-112">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Склады**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="844bb-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="844bb-113">Выберите расположение, где необходимо использовать ячейки.</span><span class="sxs-lookup"><span data-stu-id="844bb-113">Select the location where you want to use bins.</span></span>  
3.  <span data-ttu-id="844bb-114">Выберите действие **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="844bb-114">Choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="844bb-115">На экспресс-вкладке **Склад** установите флажок **Ячейка обязательна**.</span><span class="sxs-lookup"><span data-stu-id="844bb-115">On the **Warehouse** FastTab, select the **Bin Mandatory** check box.</span></span>  
5.  <span data-ttu-id="844bb-116">Если на складе не используется расширенный подбор и размещение, введите в поле **Выбор ячейки по умолчанию** метод, который должен использоваться системой при присвоении товару стандартной ячейки.</span><span class="sxs-lookup"><span data-stu-id="844bb-116">If you are not using directed put-away and pick for the location, fill in the **Default Bin Selection** field with the method the system should use when assigning a default bin to an item.</span></span>  
6.  <span data-ttu-id="844bb-117">Откройте карточку склада, для которого требуется настроить ячейки.</span><span class="sxs-lookup"><span data-stu-id="844bb-117">Open the card for the location that you want to set up bins for.</span></span>
7.  <span data-ttu-id="844bb-118">На экспресс-вкладке **Ячейки** выберите ячейки, которые требуется использовать по умолчанию для приемки и отгрузки, а также в качестве входящих, исходящих и ячеек сборки.</span><span class="sxs-lookup"><span data-stu-id="844bb-118">On the **Bins** FastTab, select the bins that you want to use as the default for receipts, shipments, inbound, outbound, and open shop floor bins.</span></span>  
8.  <span data-ttu-id="844bb-119">Введенные сюда коды ячеек автоматически появятся в заголовках и в строках различных складских документов.</span><span class="sxs-lookup"><span data-stu-id="844bb-119">The bin codes you fill in here will appear automatically on the headers and on the lines of various warehouse documents.</span></span> <span data-ttu-id="844bb-120">Стандартные ячейки определяют все начальные и конечные размещения товаров на складе.</span><span class="sxs-lookup"><span data-stu-id="844bb-120">The default bins define all starting or ending placements of items in the warehouse.</span></span>  
9.  <span data-ttu-id="844bb-121">Если используется расширенный подбор и размещение, выберите ячейку для коррекций склада.</span><span class="sxs-lookup"><span data-stu-id="844bb-121">If you are using directed put-away and pick, select a bin for your warehouse adjustments.</span></span> <span data-ttu-id="844bb-122">Код ячейки в поле **Код ячейки коррекции** определяет виртуальную ячейку, в которую следует записывать расхождения в складском запасе при регистрации наблюдаемых расхождений, зарегистрированных в журнале товаров на складе, или расхождений, вычисленных при регистрации складской инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="844bb-122">The bin code in the **Adjustment Bin Code** field defines the virtual bin in which to record discrepancies in inventory when you register either observed differences registered in the warehouse item journal, or differences calculated when you register a warehouse physical inventory.</span></span>  
10. <span data-ttu-id="844bb-123">Заполните поля на экспресс-вкладке **Политики ячеек**, если они относятся к данному складу.</span><span class="sxs-lookup"><span data-stu-id="844bb-123">Fill in the fields on the **Bin Policies** FastTab if they are relevant to your warehouse.</span></span> <span data-ttu-id="844bb-124">Наиболее важными являются поля **Политика заполнения ячеек**, **Разрешить разбивку** и **Код шаблона размещения**.</span><span class="sxs-lookup"><span data-stu-id="844bb-124">The most important fields are **Bin Capacity Policy**, **Allow Breakbulk**, and **Put-away Template Code** fields.</span></span>  
11. <span data-ttu-id="844bb-125">На экспресс-вкладке **Склад** заполните поля **Исходящие - время обработки склада**, **Входящие - время обработки склада** и **Код базового календаря**.</span><span class="sxs-lookup"><span data-stu-id="844bb-125">On the **Warehouse** FastTab, fill in the **Outbound Whse. Handling Time**, **Inbound Whse. Handling Time**, and the **Base Calendar Code** fields.</span></span> <span data-ttu-id="844bb-126">Дополнительные сведения см. в разделе [Настройка базовых календарей](across-how-to-assign-base-calendars.md).</span><span class="sxs-lookup"><span data-stu-id="844bb-126">For more information, see [Set Up Base Calendars](across-how-to-assign-base-calendars.md).</span></span>

## <a name="filling-the-consumption-bin"></a><span data-ttu-id="844bb-127">Заполнение ячейки потребления</span><span class="sxs-lookup"><span data-stu-id="844bb-127">Filling the Consumption Bin</span></span>
<span data-ttu-id="844bb-128">Эта блок-схема показывает, как поле **Код ячейки** в строках компонентов производственного заказа заполняется в соответствии с настройкой склада.</span><span class="sxs-lookup"><span data-stu-id="844bb-128">This flow chart shows how the **Bin Code** field on production order component lines is filled according to your location setup.</span></span>

<span data-ttu-id="844bb-129">![Диаграмма ячейки](media/binflow.png "BinFlow")</span><span class="sxs-lookup"><span data-stu-id="844bb-129">![Bin flow chart](media/binflow.png "BinFlow")</span></span>  

## <a name="see-also"></a><span data-ttu-id="844bb-130">См. также</span><span class="sxs-lookup"><span data-stu-id="844bb-130">See Also</span></span>
[<span data-ttu-id="844bb-131">Управление складом</span><span class="sxs-lookup"><span data-stu-id="844bb-131">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="844bb-132">Наличие</span><span class="sxs-lookup"><span data-stu-id="844bb-132">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="844bb-133">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="844bb-133">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="844bb-134">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="844bb-134">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="844bb-135">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="844bb-135">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="844bb-136">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="844bb-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

