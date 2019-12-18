---
title: Как присвоить товарам стандартные ячейки | Документация Майкрософт
description: Если на складе используются ячейки, присвоение товарам стандартных ячеек может значительно облегчить процесс отгрузки, приемки и перемещения товаров. Когда товару присваивается стандартная ячейка, она будет предлагаться в начале каждой транзакции для этого товара.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: d9a6efce014d3332a5dbb2f92a50c591c0c82eac
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881850"
---
# <a name="assign-default-bins-to-items"></a><span data-ttu-id="84caa-104">Присвоение товарам стандартных ячеек</span><span class="sxs-lookup"><span data-stu-id="84caa-104">Assign Default Bins to Items</span></span>
<span data-ttu-id="84caa-105">Если на складе используются ячейки, присвоение товарам стандартных ячеек может значительно облегчить процесс отгрузки, приемки и перемещения товаров.</span><span class="sxs-lookup"><span data-stu-id="84caa-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span></span> <span data-ttu-id="84caa-106">Когда товару присваивается стандартная ячейка, она будет предлагаться в начале каждой транзакции для этого товара.</span><span class="sxs-lookup"><span data-stu-id="84caa-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span></span> <span data-ttu-id="84caa-107">Стандартные ячейки задаются на странице **Содержимое ячейки**.</span><span class="sxs-lookup"><span data-stu-id="84caa-107">Default bins are defined on the **Bin Content** page.</span></span>  

## <a name="to-assign-a-default-bin-to-an-item"></a><span data-ttu-id="84caa-108">Присвоение товару ячейки по умолчанию</span><span class="sxs-lookup"><span data-stu-id="84caa-108">To assign a default bin to an item</span></span>
1.  <span data-ttu-id="84caa-109">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал создания содержимого ячеек**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="84caa-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Content Creation Worksheet**, and choose the related link.</span></span>  
2.  <span data-ttu-id="84caa-110">Введите код ячейки и сведения о товаре для каждой ячейки, которую предполагается задать в качестве стандартной для товара.</span><span class="sxs-lookup"><span data-stu-id="84caa-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span></span> <span data-ttu-id="84caa-111">Убедитесь, что выбрано поле **По умолчанию**.</span><span class="sxs-lookup"><span data-stu-id="84caa-111">Make sure to select the **Default** field.</span></span>  
3.  <span data-ttu-id="84caa-112">Выберите действие **Создать содержимое ячеек**.</span><span class="sxs-lookup"><span data-stu-id="84caa-112">Choose the **Create Bin Content** action.</span></span> <span data-ttu-id="84caa-113">Теперь товару присвоены стандартные ячейки.</span><span class="sxs-lookup"><span data-stu-id="84caa-113">Default bins are now assigned for your item.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="84caa-114">При размещении товара, которому не присвоена стандартная ячейка, ему будет приписана в качестве ячейки по умолчанию та ячейка, в которой этот товар размещен.</span><span class="sxs-lookup"><span data-stu-id="84caa-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span></span>  

## <a name="to-change-the-default-bin-for-an-item"></a><span data-ttu-id="84caa-115">Изменение стандартной ячейки для товара</span><span class="sxs-lookup"><span data-stu-id="84caa-115">To change the default bin for an item</span></span>  
<span data-ttu-id="84caa-116">Может возникать необходимость изменить стандартную ячейку для товара или присвоить стандартную ячейку новому товару.</span><span class="sxs-lookup"><span data-stu-id="84caa-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span></span>    
1.  <span data-ttu-id="84caa-117">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Содержимое ячейки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="84caa-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Contents**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="84caa-118">В поле **Фильтр по складу** выберите нужный код склада.</span><span class="sxs-lookup"><span data-stu-id="84caa-118">In the **Location Filter** field, select the appropriate location code.</span></span>  
3.  <span data-ttu-id="84caa-119">Найдите запись о текущей стандартной ячейке данного товара и снимите флажок **Станд. ячейка**.</span><span class="sxs-lookup"><span data-stu-id="84caa-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span></span>  
4.  <span data-ttu-id="84caa-120">Найдите строку "Содержимое ячейки" для той ячейки, которая должна стать новой стандартной ячейкой.</span><span class="sxs-lookup"><span data-stu-id="84caa-120">Find the bin content line for the bin that you would like as the new default bin.</span></span> <span data-ttu-id="84caa-121">Установите флажок **Станд. ячейка**.</span><span class="sxs-lookup"><span data-stu-id="84caa-121">Select the **Default Bin** check box.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="84caa-122">При первом размещении товара, у которого еще нет стандартной ячейки, ему в качестве стандартной будет приписана системой та ячейка, куда этот товар размещен.</span><span class="sxs-lookup"><span data-stu-id="84caa-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span></span>  

## <a name="see-also"></a><span data-ttu-id="84caa-123">См. также</span><span class="sxs-lookup"><span data-stu-id="84caa-123">See Also</span></span>  
[<span data-ttu-id="84caa-124">Управление складом</span><span class="sxs-lookup"><span data-stu-id="84caa-124">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="84caa-125">Наличие</span><span class="sxs-lookup"><span data-stu-id="84caa-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="84caa-126">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="84caa-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="84caa-127">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="84caa-127">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="84caa-128">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="84caa-128">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="84caa-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="84caa-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
