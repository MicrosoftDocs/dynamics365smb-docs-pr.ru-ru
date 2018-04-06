---
title: "Как перемещать товары в расширенных конфигурациях склада | Документы Майкрософт"
description: "В расширенных настройках складов, в которых используются расширенный подбор и размещение, складские перемещения между ячейками выполняются мастером склада, который подготавливает перемещения в журнале передвижений, а затем создает складские передвижения, которые должны выполнить сотрудники склада."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/232017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 4caa041c6b3acef5d0cbf6c037f0ec535cd3176e
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="move-items-in-advanced-warehouse-configurations"></a><span data-ttu-id="0dc4b-103">Перемещение товаров в расширенных конфигурациях склада</span><span class="sxs-lookup"><span data-stu-id="0dc4b-103">Move Items in Advanced Warehouse Configurations</span></span>
<span data-ttu-id="0dc4b-104">В расширенных настройках складов, в которых используются расширенный подбор и размещение, складские перемещения между ячейками выполняются мастером склада, который подготавливает перемещения в журнале передвижений, а затем создает складские передвижения, которые должны выполнить сотрудники склада.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-104">In advanced warehouse configurations, that is, locations with directed put-away and pick, warehouse movements between bins are performed by a senior employee preparing warehouse movements in the movement worksheet and then creating the warehouse movements for warehouse employees to perform.</span></span>  

## <a name="to-move-items-with-the-warehouse-movement-worksheet"></a><span data-ttu-id="0dc4b-105">Перемещение товаров с помощью журнала складских передвижений</span><span class="sxs-lookup"><span data-stu-id="0dc4b-105">To move items with the warehouse movement worksheet</span></span>
<span data-ttu-id="0dc4b-106">Окно **Журнал перемещения** имеет две функции, которые обеспечивают поддержку автоматического заполнения строк.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-106">The **Movement Worksheet** window has two functions that can assist in automatically filling in the lines.</span></span> <span data-ttu-id="0dc4b-107">Первая функция называется **Расчет пополнения ячеек**.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-107">The first is the **Calculate Bin Replenishment** function.</span></span> <span data-ttu-id="0dc4b-108">Эта функция, используя рейтинги ячеек, предлагает пополнить ячейки с высоким рейтингом за счет ячеек с низким рейтингом. Вторая функция называется **Получить содержимое ячейки**, она вводит в строки журнала все содержимое указанной ячейки или ячеек.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-108">This function uses the bin rankings to suggest replenishment for high-ranking bins from low-ranking bins. The second is the **Get Bin Content** function, which fills in the worksheet lines with the entire bin contents of the bin or bins you specify.</span></span>

1.  <span data-ttu-id="0dc4b-109">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журнал перемещения**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Movement Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0dc4b-110">Введите в строки журнала необходимую информацию о перемещениях.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-110">Enter the warehouse movement information on the worksheet lines as appropriate.</span></span>  
3. <span data-ttu-id="0dc4b-111">Выберите действие **Создать передвижение**, чтобы создать документ складского перемещения, который будет зарегистрирован по завершении складского перемещения.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-111">Choose the **Create Movement** action to create a warehouse movement document which can then be registered when the warehouse movement is completed.</span></span>  

### <a name="to-register-the-warehouse-movement"></a><span data-ttu-id="0dc4b-112">Регистрация складского передвижения</span><span class="sxs-lookup"><span data-stu-id="0dc4b-112">To register the warehouse movement</span></span>  
1.  <span data-ttu-id="0dc4b-113">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Перемещения**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Movements**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0dc4b-114">Откройте складское передвижение, которое необходимо обработать.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-114">Open the warehouse movement that you want to process.</span></span>  
3.  <span data-ttu-id="0dc4b-115">В строках типа действия **Поместить** укажите место, время и единицу товара, который нужно переместить путем изменения полей **Код зоны**, **Код ячейки**, **Кол-во для обработки** или **Дата завершения**.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-115">On lines of action type **Place**, specify where, which, and when to move the item in question by editing the **Zone Code**, **Bin Code**, **Qty. to Handle**, or **Due Date** fields.</span></span>  

    <span data-ttu-id="0dc4b-116">Еcли склад настроен таким образом, что коды ячейки соответствуют физическому плану склада, какие-либо количества нескольких товаров отбираются из идущих подряд ячеек, а затем помещаются в ячейки подбора, которые также могут располагаться подряд.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-116">If your warehouse has been set up so the bin codes follow the physical structure of the warehouse, you can take quantities of several items from successive bulk bins and then place them in forward picking bins, which also might be close to one another.</span></span>  
4.  <span data-ttu-id="0dc4b-117">В строках типа действия **Взять** укажите в поле **Кол-во для обработки** часть содержимого ячейки, которую необходимо переместить.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-117">On lines of action type **Take**, specify in the **Qty. to Handle** field a part quantity of the bin content that you want to move.</span></span> <span data-ttu-id="0dc4b-118">Все остальные поля в строках с типом действия **Взять** доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-118">All other fields on lines of action type **Take** are read-only.</span></span>  
5.  <span data-ttu-id="0dc4b-119">Чтобы переместить все предложенные значения количества в поле **Кол-во**, выберите действие **Автозаполнение кол-ва для обработки**.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-119">To move all suggested quantities as specified in the **Quantity** field, choose the **Autofill Qty. to Handle** action.</span></span>  
6. <span data-ttu-id="0dc4b-120">Выберите действие **Регистр**.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-120">Choose the **Register** action.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0dc4b-121">Если на складе используются расширенный подбор и размещение, и используются типы ячеек, то товары нельзя вручную перемещать в ячейки или из них, если они имеют тип ПОЛУЧЕНИЕ, потому что товары, находящиеся в ячейке этого типа, должны быть зарегистрированы как размещенные до того, как они станут частью доступных складских запасов.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-121">If the location uses directed put-away and pick, then you cannot manually move items in or out of bins of bin type RECEIVE, because items in such bins must be registered as being put away before they are part of available inventory.</span></span>

## <a name="to-register-the-movement-of-an-item-that-has-already-occurred"></a><span data-ttu-id="0dc4b-122">Регистрация уже выполненных передвижений товара</span><span class="sxs-lookup"><span data-stu-id="0dc4b-122">To register the movement of an item that has already occurred</span></span>  
<span data-ttu-id="0dc4b-123">Если на складе, для которого настроены расширенный подбор и размещение, нужно переместить товары в другие ячейки без предшествовавшего складского размещения, подбора или передвижения, можно зарегистрировать правильное местоположение товаров на складе, используя **Склад - журнал реклассификаций**.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-123">If your location uses directed put-away and pick, and you need to move items to other bins without a pre-existing warehouse put-away, pick, or movement, you can register the correct placement of the items in the warehouse using the **Whse. Reclassification Journal**.</span></span>

1.  <span data-ttu-id="0dc4b-124">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Складской журнал реклассифик.**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Whse. Reclassification Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0dc4b-125">Заполните поля **Номер товара**, **Из кода зоны**, **Из кода ячейки**, **В код зоны** и **В код ячейки**.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-125">Fill in the **Item No.**, **From Zone Code**, **From Bin Code**, **To Zone Code**, and **To Bin Code** fields.</span></span>  
3.  <span data-ttu-id="0dc4b-126">Выберите действие **Регистр**.</span><span class="sxs-lookup"><span data-stu-id="0dc4b-126">Choose the **Register** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0dc4b-127">См. также</span><span class="sxs-lookup"><span data-stu-id="0dc4b-127">See Also</span></span>  
[<span data-ttu-id="0dc4b-128">Управление складом</span><span class="sxs-lookup"><span data-stu-id="0dc4b-128">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="0dc4b-129">Наличие</span><span class="sxs-lookup"><span data-stu-id="0dc4b-129">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="0dc4b-130">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="0dc4b-130">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="0dc4b-131">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="0dc4b-131">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="0dc4b-132">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="0dc4b-132">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="0dc4b-133">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0dc4b-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

