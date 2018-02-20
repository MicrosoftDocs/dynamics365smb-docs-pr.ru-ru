---
title: "Настройка карточки склада и определение маршрутов перемещения | Документы Майкрософт"
description: "Вы создаете карточку склада для каждого места, где хранятся товары, например для склада или дистрибьюторского центра, а также настраиваете маршруты для перемещения товаров между складами."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 01/25/2018
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 57e16fe7d7dd3edd832fb29773fc2a9c13cba153
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="set-up-locations"></a><span data-ttu-id="2e32c-103">Настройка складов</span><span class="sxs-lookup"><span data-stu-id="2e32c-103">Set Up Locations</span></span>
<span data-ttu-id="2e32c-104">Если вы покупаете, храните или продаете товары в нескольких местах или складах, вы должны настроить каждый склад с помощью каточки склада и определить маршруты перемещения.</span><span class="sxs-lookup"><span data-stu-id="2e32c-104">If you buy, store, or sell items at more than one place or warehouse, you must set each location up with a location card and define transfer routes.</span></span>

<span data-ttu-id="2e32c-105">Затем вы сможете создать строки документа для определенного склада, просмотреть доступность по складу и переместить запасы между складами.</span><span class="sxs-lookup"><span data-stu-id="2e32c-105">You can then create document lines for a specific location, view availability by location, and transfer inventory between locations.</span></span> <span data-ttu-id="2e32c-106">Дополнительные сведения см. в разделе [Управление запасами](inventory-manage-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="2e32c-106">For more information, see [Manage Inventory](inventory-manage-inventory.md).</span></span>

## <a name="to-create-a-location-card"></a><span data-ttu-id="2e32c-107">Создание карточки склада</span><span class="sxs-lookup"><span data-stu-id="2e32c-107">To create a location card</span></span>
1. <span data-ttu-id="2e32c-108">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Склады**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2e32c-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="2e32c-109">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="2e32c-109">Choose the **New** action.</span></span>
3. <span data-ttu-id="2e32c-110">В окне **Карточка склада** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="2e32c-110">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="2e32c-111">Повторите шаги 2 и 3 для каждого склада, на котором необходимо хранить запасы.</span><span class="sxs-lookup"><span data-stu-id="2e32c-111">Repeat steps 2 and 3 for every location where you want to keep inventory.</span></span>

> [!NOTE]  
> <span data-ttu-id="2e32c-112">Многие поля в карточке склада относятся к обработке товаров во входящих и исходящих процессах склада.</span><span class="sxs-lookup"><span data-stu-id="2e32c-112">Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes.</span></span> <span data-ttu-id="2e32c-113">Дополнительные сведения см. в разделе [Настройка управления складом](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="2e32c-113">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

## <a name="to-create-a-transfer-route"></a><span data-ttu-id="2e32c-114">Создание маршрута перемещения</span><span class="sxs-lookup"><span data-stu-id="2e32c-114">To create a transfer route</span></span>
1. <span data-ttu-id="2e32c-115">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Маршруты перемещения**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2e32c-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer Routes**, and then choose the related link.</span></span>
2. <span data-ttu-id="2e32c-116">Либо в любом окне **Карточка склада** выберите действие **Маршруты перемещения**.</span><span class="sxs-lookup"><span data-stu-id="2e32c-116">Alternatively, from any **Location Card** window, choose the **Transfer Routes** action.</span></span>
3. <span data-ttu-id="2e32c-117">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="2e32c-117">Choose the **New** action.</span></span>
4. <span data-ttu-id="2e32c-118">В окне **Карточка склада** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="2e32c-118">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="2e32c-119">Теперь вы можете перемещать складские товары между складами.</span><span class="sxs-lookup"><span data-stu-id="2e32c-119">You can now transfer inventory items between two locations.</span></span> <span data-ttu-id="2e32c-120">Дополнительные сведения см. в разделе [Перемещение запасов между складами](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="2e32c-120">For more information, see [Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>    

## <a name="see-also"></a><span data-ttu-id="2e32c-121">См. также</span><span class="sxs-lookup"><span data-stu-id="2e32c-121">See Also</span></span>
[<span data-ttu-id="2e32c-122">Управление запасами</span><span class="sxs-lookup"><span data-stu-id="2e32c-122">Manage Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="2e32c-123">[Перемещение запасов между складами](inventory-how-transfer-between-locations.md)  </span><span class="sxs-lookup"><span data-stu-id="2e32c-123">[Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)  </span></span>  
<span data-ttu-id="2e32c-124">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2e32c-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="2e32c-125">[Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="2e32c-125">[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)</span></span>  
[<span data-ttu-id="2e32c-126">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="2e32c-126">General Business Functionality</span></span>](ui-across-business-areas.md)

