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
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 146fc08f389a5c068044358c59b7d8911f0b3343
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-set-up-locations"></a><span data-ttu-id="c896f-103">Практическое руководство. Настройка складов</span><span class="sxs-lookup"><span data-stu-id="c896f-103">How to: Set Up Locations</span></span>
<span data-ttu-id="c896f-104">Если вы покупаете, храните или продаете товары в нескольких местах или складах, вы должны настроить каждый склад с помощью каточки склада и определить маршруты перемещения.</span><span class="sxs-lookup"><span data-stu-id="c896f-104">If you buy, store, or sell items at more than one place or warehouse, you must set each location up with a location card and define transfer routes.</span></span>

<span data-ttu-id="c896f-105">Затем вы сможете создать строки документа для определенного склада, просмотреть доступность по складу и переместить запасы между складами.</span><span class="sxs-lookup"><span data-stu-id="c896f-105">You can then create document lines for a specific location, view availability by location, and transfer inventory between locations.</span></span> <span data-ttu-id="c896f-106">Дополнительные сведения см. в разделе [Управление запасами](inventory-manage-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="c896f-106">For more information, see [Manage Inventory](inventory-manage-inventory.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="c896f-107">Эта функция требует, чтобы было задано значение **Пакет**.</span><span class="sxs-lookup"><span data-stu-id="c896f-107">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="c896f-108">Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="c896f-108">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-create-a-location-card"></a><span data-ttu-id="c896f-109">Создание карточки склада</span><span class="sxs-lookup"><span data-stu-id="c896f-109">To create a location card</span></span>
1. <span data-ttu-id="c896f-110">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Склады**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="c896f-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="c896f-111">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="c896f-111">Choose the **New** action.</span></span>
3. <span data-ttu-id="c896f-112">В окне **Карточка склада** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="c896f-112">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="c896f-113">Повторите шаги 2 и 3 для каждого склада, на котором необходимо хранить запасы.</span><span class="sxs-lookup"><span data-stu-id="c896f-113">Repeat steps 2 and 3 for every location where you want to keep inventory.</span></span>

## <a name="to-create-a-transfer-route"></a><span data-ttu-id="c896f-114">Создание маршрута перемещения</span><span class="sxs-lookup"><span data-stu-id="c896f-114">To create a transfer route</span></span>
1. <span data-ttu-id="c896f-115">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Маршруты перемещения**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="c896f-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer Routes**, and then choose the related link.</span></span>
2. <span data-ttu-id="c896f-116">Либо в любом окне **Карточка склада** выберите действие **Маршруты перемещения**.</span><span class="sxs-lookup"><span data-stu-id="c896f-116">Alternatively, from any **Location Card** window, choose the **Transfer Routes** action.</span></span>
3. <span data-ttu-id="c896f-117">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="c896f-117">Choose the **New** action.</span></span>
4. <span data-ttu-id="c896f-118">В окне **Карточка склада** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="c896f-118">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="c896f-119">Теперь вы можете перемещать складские товары между складами.</span><span class="sxs-lookup"><span data-stu-id="c896f-119">You can now transfer inventory items between two locations.</span></span> <span data-ttu-id="c896f-120">Дополнительные сведения см. в разделе [Практическое руководство. Перемещение запасов между складами](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="c896f-120">For more information, see [How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>    

## <a name="see-also"></a><span data-ttu-id="c896f-121">См. также</span><span class="sxs-lookup"><span data-stu-id="c896f-121">See Also</span></span>
[<span data-ttu-id="c896f-122">Управление запасами</span><span class="sxs-lookup"><span data-stu-id="c896f-122">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="c896f-123">Цепочка поставок</span><span class="sxs-lookup"><span data-stu-id="c896f-123">Supply Chain</span></span>](madeira-supply-chain.md)  
<span data-ttu-id="c896f-124">[Практическое руководство. Перемещение запасов между складами](inventory-how-transfer-between-locations.md)  </span><span class="sxs-lookup"><span data-stu-id="c896f-124">[How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)  </span></span>  
<span data-ttu-id="c896f-125">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c896f-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="c896f-126">[Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="c896f-126">[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)</span></span>  
[<span data-ttu-id="c896f-127">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="c896f-127">General Business Functionality</span></span>](ui-across-business-areas.md)

