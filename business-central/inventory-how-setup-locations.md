---
title: Настройка карточки склада и определение маршрутов перемещения
description: Вы создаете карточку склада для каждого места, где хранятся товары, например для склада или дистрибьюторского центра, а также настраиваете маршруты для перемещения товаров между складами.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 06/01/2021
ms.author: edupont
ms.openlocfilehash: 0319f0c64dd46610aa82705257091bd9478ac14f
ms.sourcegitcommit: 1aab52477956bf1aa7376fc7fb984644bc398c61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "6184328"
---
# <a name="set-up-locations"></a><span data-ttu-id="650a8-103">Настройка складов</span><span class="sxs-lookup"><span data-stu-id="650a8-103">Set Up Locations</span></span>

<span data-ttu-id="650a8-104">Если вы покупаете, храните или продаете товары в нескольких местах или складах, вы должны настроить каждый склад с помощью каточки склада и определить маршруты перемещения.</span><span class="sxs-lookup"><span data-stu-id="650a8-104">If you buy, store, or sell items at more than one place or warehouse, you must set up each location with a location card and define transfer routes.</span></span> <span data-ttu-id="650a8-105">[!INCLUDE [prod_short](includes/prod_short.md)] использует местоположения, чтобы отслеживать запасы как в более простых случаях, так и в более сложных складских процессах.</span><span class="sxs-lookup"><span data-stu-id="650a8-105">[!INCLUDE [prod_short](includes/prod_short.md)] uses locations to help keep track of inventory in both simpler cases and the more complex warehouse processes.</span></span>

<span data-ttu-id="650a8-106">Затем вы сможете создать строки документа для определенного склада, просмотреть доступность по складу и переместить запасы между складами.</span><span class="sxs-lookup"><span data-stu-id="650a8-106">You can then create document lines for a specific location, view availability by location, and transfer inventory between locations.</span></span> <span data-ttu-id="650a8-107">Дополнительные сведения см. в разделе [Управление запасами](inventory-manage-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="650a8-107">For more information, see [Manage Inventory](inventory-manage-inventory.md).</span></span>
<br><br>  
  
> [!Video https://www.microsoft.com/videoplayer/embed/RE4aQvq?rel=0]

## <a name="location-cards"></a><span data-ttu-id="650a8-108">Карточки склада</span><span class="sxs-lookup"><span data-stu-id="650a8-108">Location cards</span></span>

<span data-ttu-id="650a8-109">В карточке местоположения указывается информация о местоположении, например о складе или распределительном центре.</span><span class="sxs-lookup"><span data-stu-id="650a8-109">The location card specifies information about a location, such as a warehouse or distribution center.</span></span> <span data-ttu-id="650a8-110">Каждому местоположению присваивается имя и код.</span><span class="sxs-lookup"><span data-stu-id="650a8-110">You give each location a name and a code that represents the location.</span></span> <span data-ttu-id="650a8-111">Затем, если требуется зарегистрировать транзакции для данного склада, можно указать код склада в других частях программы.</span><span class="sxs-lookup"><span data-stu-id="650a8-111">You can then enter the location code in other parts of the program when you want to record transactions for a given location.</span></span>  

<span data-ttu-id="650a8-112">Здесь можно ввести информацию о ячейках и политиках склада.</span><span class="sxs-lookup"><span data-stu-id="650a8-112">You can enter information about bins and warehouse policies for each location.</span></span> <span data-ttu-id="650a8-113">В зависимости от выбранных политик склада с помощью параметров на экспресс-вкладке **Ячейки** можно определить ячейки, которые будут использоваться по умолчанию при выполнении транзакций.</span><span class="sxs-lookup"><span data-stu-id="650a8-113">Based on the warehouse policies you select, you can use the options on the **Bins** FastTab to define the bins that will be used as default bins when you are performing transactions.</span></span> <span data-ttu-id="650a8-114">При использовании расширенного подбора и размещения с помощью параметров на экспресс-вкладке **Политики в отношении ячеек** можно определить способ использования дополнительных складских функций.</span><span class="sxs-lookup"><span data-stu-id="650a8-114">If you are using directed put-away and pick, you use most of the options on the **Bin Policies** FastTab to define how you would like to use the various advanced warehousing features.</span></span>  

<span data-ttu-id="650a8-115">Некоторые поля параметров выделены серым и отключены другими настройками на странице **Карточка склада**, чтобы ограничить неподдерживаемые комбинаций настроек.</span><span class="sxs-lookup"><span data-stu-id="650a8-115">Some option fields are grayed and disabled by other settings in the **Location Card** page to restrict unsupported setup combinations.</span></span>  

<span data-ttu-id="650a8-116">Выберите действие **Зоны** или **Ячейки**, чтобы просмотреть сведения о зонах и ячейках, которые могут быть определены для склада.</span><span class="sxs-lookup"><span data-stu-id="650a8-116">Choose the **Zones** or **Bins** action to view information about zones and bins that may be defined for the location.</span></span>

### <a name="to-create-a-location-card"></a><span data-ttu-id="650a8-117">Создание карточки склада</span><span class="sxs-lookup"><span data-stu-id="650a8-117">To create a location card</span></span>

1. <span data-ttu-id="650a8-118">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Склады**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="650a8-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="650a8-119">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="650a8-119">Choose the **New** action.</span></span>
3. <span data-ttu-id="650a8-120">На странице **Карточка склада** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="650a8-120">On the **Location Card** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="650a8-121">Повторите шаги 2 и 3 для каждого склада, на котором необходимо хранить запасы.</span><span class="sxs-lookup"><span data-stu-id="650a8-121">Repeat steps 2 and 3 for every location where you want to keep inventory.</span></span>

> [!NOTE]  
> <span data-ttu-id="650a8-122">Многие поля в карточке склада относятся к обработке товаров во входящих и исходящих процессах склада.</span><span class="sxs-lookup"><span data-stu-id="650a8-122">Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes.</span></span> <span data-ttu-id="650a8-123">Поля не актуальны для компаний, которым не требуется более сложная функциональность склада.</span><span class="sxs-lookup"><span data-stu-id="650a8-123">The fields are not relevant for companies that do not require the more complex warehouse functionality.</span></span> <span data-ttu-id="650a8-124">Дополнительные сведения см. в разделе [Настройка управления складом](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="650a8-124">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

<span data-ttu-id="650a8-125">Вы можете изменить конфигурацию местоположения позже, но вы не можете редактировать настройку местоположений, в которых есть записи книги товаров.</span><span class="sxs-lookup"><span data-stu-id="650a8-125">You can change the configuration of a location later, but you cannot edit the setup of locations that have item ledger entries.</span></span>  

<span data-ttu-id="650a8-126">Затем, если у вас есть несколько местоположений, вы можете определить маршруты передачи между местоположениями.</span><span class="sxs-lookup"><span data-stu-id="650a8-126">Next, if you have multiple locations, you can define transfer routes between locations.</span></span>  

### <a name="to-create-a-transfer-route"></a><span data-ttu-id="650a8-127">Создание маршрута перемещения</span><span class="sxs-lookup"><span data-stu-id="650a8-127">To create a transfer route</span></span>

1. <span data-ttu-id="650a8-128">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Маршруты перемещения**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="650a8-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer Routes**, and then choose the related link.</span></span>
2. <span data-ttu-id="650a8-129">Либо на любой странице **Карточка склада** выберите действие **Маршруты перемещения**.</span><span class="sxs-lookup"><span data-stu-id="650a8-129">Alternatively, from any **Location Card** page, choose the **Transfer Routes** action.</span></span>
3. <span data-ttu-id="650a8-130">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="650a8-130">Choose the **New** action.</span></span>
4. <span data-ttu-id="650a8-131">На странице **Карточка склада** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="650a8-131">On the **Location Card** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="650a8-132">Теперь вы можете перемещать складские товары между складами.</span><span class="sxs-lookup"><span data-stu-id="650a8-132">You can now transfer inventory items between two locations.</span></span> <span data-ttu-id="650a8-133">Дополнительные сведения см. в разделе [Перемещение запасов между складами](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="650a8-133">For more information, see [Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>    

## <a name="bins"></a><span data-ttu-id="650a8-134">Ячейки</span><span class="sxs-lookup"><span data-stu-id="650a8-134">Bins</span></span>

<span data-ttu-id="650a8-135">Ячейки являются базовой складской структурой и используются для формирования предложений по размещению товаров.</span><span class="sxs-lookup"><span data-stu-id="650a8-135">Bins represent the basic warehouse structure and are used to make suggestions about the placement of items.</span></span> <span data-ttu-id="650a8-136">После создания ячеек можно точно определить содержимое для помещения в каждую ячейку; ячейка может также функционировать в качестве плавающей ячейки без определенного содержимого.</span><span class="sxs-lookup"><span data-stu-id="650a8-136">When you have created your bins, you can define precisely the contents that you want to place in each bin, or the bin can function as a floating bin without specified contents.</span></span> <span data-ttu-id="650a8-137">Ячейки преимущественно используются при основных и дополнительных складских операциях.</span><span class="sxs-lookup"><span data-stu-id="650a8-137">Bins are predominantly used in basic and advance warehouse operations.</span></span> <span data-ttu-id="650a8-138">Если вы управляете запасами в более простой настройке, вам, вероятно, не понадобятся ячейки.</span><span class="sxs-lookup"><span data-stu-id="650a8-138">If you manage inventory in a more simple setup, you probably do not need bins.</span></span>

<span data-ttu-id="650a8-139">Чтобы использовать функцию ячеек в каком-либо местоположении, сначала активируйте функцию на карточке **Местоположение**, выбрав поле **Ячейка обязательна** на экспресс-вкладке **Склад**.</span><span class="sxs-lookup"><span data-stu-id="650a8-139">To use the bin functionality at a location, you first activate the functionality on the **Location** card by selecting the **Bins Mandatory** field on the **Warehouse** FastTab.</span></span> <span data-ttu-id="650a8-140">Затем разрабатывается поток товаров на складе путем указания кодов ячеек в полях настройки, представляющих различные потоки.</span><span class="sxs-lookup"><span data-stu-id="650a8-140">Then you design the item flow at the location by specifying bin codes in setup fields that represent the different flows.</span></span>

> [!NOTE]
> <span data-ttu-id="650a8-141">Прежде чем можно будет указать коды ячеек в карточке склада, эти коды ячеек необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="650a8-141">Before you can specify bin codes on the location card, the bin codes must be created.</span></span>

<span data-ttu-id="650a8-142">Дополнительные сведения см. в разделах [Создание ячеек](warehouse-how-to-create-individual-bins.md) и [Настройка типов ячеек](warehouse-how-to-set-up-bin-types.md).</span><span class="sxs-lookup"><span data-stu-id="650a8-142">For more information, see [Create Bins](warehouse-how-to-create-individual-bins.md) and [Set Up Bin Types](warehouse-how-to-set-up-bin-types.md).</span></span>  

## <a name="zones"></a><span data-ttu-id="650a8-143">Зоны</span><span class="sxs-lookup"><span data-stu-id="650a8-143">Zones</span></span>

<span data-ttu-id="650a8-144">Если вы хотите структурировать свои ячейки по зонам, вы можете сделать это на странице **Зоны**.</span><span class="sxs-lookup"><span data-stu-id="650a8-144">If you want to structure your bins under zones, you can do that in the **Zones** page.</span></span>

<span data-ttu-id="650a8-145">[!INCLUDE [prod_short](includes/prod_short.md)] копирует поля, настроенные для конкретной зоны, в ячейки данной зоны.</span><span class="sxs-lookup"><span data-stu-id="650a8-145">[!INCLUDE [prod_short](includes/prod_short.md)] copies the fields that you set for any particular zone to the bins within it.</span></span> <span data-ttu-id="650a8-146">Таким образом, можно воспользоваться функцией присвоения зоны ячейке или шаблону ячейки (фильтр создания ячейки), и несколько оставшихся полей будут заполнены автоматически.</span><span class="sxs-lookup"><span data-stu-id="650a8-146">This way, you can assign a zone to a bin or a bin template (bin creation filter), and several other fields are then filled in automatically.</span></span>

<span data-ttu-id="650a8-147">Однако можно также настроить только одну зону и организовать деятельность склада только при помощи ячеек.</span><span class="sxs-lookup"><span data-stu-id="650a8-147">However, you can choose to set up just one zone and to organize your warehouse according to bins alone.</span></span> <span data-ttu-id="650a8-148">Дополнительные сведения см. в разделе [Настройка управления складом](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="650a8-148">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="650a8-149">См. также</span><span class="sxs-lookup"><span data-stu-id="650a8-149">See Also</span></span>

[<span data-ttu-id="650a8-150">Управление запасами</span><span class="sxs-lookup"><span data-stu-id="650a8-150">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="650a8-151">Перемещение запасов между складами</span><span class="sxs-lookup"><span data-stu-id="650a8-151">Transfer Inventory Between Locations</span></span>](inventory-how-transfer-between-locations.md)  
[<span data-ttu-id="650a8-152">Создание ячеек</span><span class="sxs-lookup"><span data-stu-id="650a8-152">Create Bins</span></span>](warehouse-how-to-create-individual-bins.md)  
[<span data-ttu-id="650a8-153">Настройка типов ячеек</span><span class="sxs-lookup"><span data-stu-id="650a8-153">Set Up Bin Types</span></span>](warehouse-how-to-set-up-bin-types.md)  
[<span data-ttu-id="650a8-154">Настройка управления складом</span><span class="sxs-lookup"><span data-stu-id="650a8-154">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
<span data-ttu-id="650a8-155">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="650a8-155">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="650a8-156">Изменение набора отображаемых функций</span><span class="sxs-lookup"><span data-stu-id="650a8-156">Change Which Features are Displayed</span></span>](ui-experiences.md)  
[<span data-ttu-id="650a8-157">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="650a8-157">General Business Functionality</span></span>](ui-across-business-areas.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]