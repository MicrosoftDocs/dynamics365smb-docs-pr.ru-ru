---
title: Настройка запасов | Документация Майкрософт
description: Описывается, как настроить процессы запасов, включая маршруты перемещения и склады.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, stock
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: f5b4e07f128551e978dffb2dedeb3e0257eea1ea
ms.sourcegitcommit: 32bfc2acaaf3693afc9aeb86feea505fd328caa1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/19/2021
ms.locfileid: "5024566"
---
# <a name="setting-up-inventory"></a><span data-ttu-id="c3ebb-103">Настройка запасов</span><span class="sxs-lookup"><span data-stu-id="c3ebb-103">Setting Up Inventory</span></span>
<span data-ttu-id="c3ebb-104">Прежде чем приступать к управлению складскими операциями и учетом стоимости товаров, необходимо настроить правила и значения, которые определяют политики запасов в компании.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-104">Before you can manage warehouse activities and inventory costing, you must configure the rules and values that define the company's inventory policies.</span></span>

<span data-ttu-id="c3ebb-105">Вы можете обеспечить лучшее обслуживание клиентов и оптимизировать цепочку поставок, организовав запасы по различным адресам.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-105">You can provide better customer service and optimize your supply chain by organizing your inventory at different addresses.</span></span> <span data-ttu-id="c3ebb-106">После этого вы можете закупать, хранить или продавать товары на различных складах и перемещать их между ними.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-106">You can then buy, store, or sell items at different locations and transfer inventory between them.</span></span>

<span data-ttu-id="c3ebb-107">Если вы настроили запасы, вы можете управлять различными процессами, связанными с товарными транзакциями.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-107">When you have set up your inventory, you can manage various processes related to item transactions.</span></span> <span data-ttu-id="c3ebb-108">Дополнительные сведения см. в разделах [Управление запасами](inventory-manage-inventory.md) и [Управление складом](warehouse-manage-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="c3ebb-108">For more information, see [Manage Inventory](inventory-manage-inventory.md) and [Warehouse Management](warehouse-manage-warehouse.md).</span></span>

| <span data-ttu-id="c3ebb-109">По</span><span class="sxs-lookup"><span data-stu-id="c3ebb-109">To</span></span> | <span data-ttu-id="c3ebb-110">Ссылка</span><span class="sxs-lookup"><span data-stu-id="c3ebb-110">See</span></span> |
| --- | --- |
| <span data-ttu-id="c3ebb-111">Определить общую настройку запасов, например серии номеров и использование складов.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-111">Define the general inventory setup, such as number series and how to use locations.</span></span> |[<span data-ttu-id="c3ebb-112">Настройка общей информации по запасам</span><span class="sxs-lookup"><span data-stu-id="c3ebb-112">Set Up General Inventory Information</span></span>](inventory-how-setup-general.md) |
|<span data-ttu-id="c3ebb-113">Настройка эффективной модели распределения с комбинацией различных складов и центров ответственности, присваиваемых бизнес-партнерам или сотрудникам.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-113">Configure an efficient distribution model with a combination of different locations and responsibility centers assigned to business partners or employees.</span></span>|[<span data-ttu-id="c3ebb-114">Работа с центрами ответственности</span><span class="sxs-lookup"><span data-stu-id="c3ebb-114">Work with Responsibility Centers</span></span>](inventory-responsibility-centers.md)|
| <span data-ttu-id="c3ebb-115">Организовать запасы на нескольких складах, включая маршруты перемещения.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-115">Organize your inventory at multiple locations, including transfer routes.</span></span> |[<span data-ttu-id="c3ebb-116">Настройка складов</span><span class="sxs-lookup"><span data-stu-id="c3ebb-116">Set Up Locations</span></span>](inventory-how-register-new-items.md) |
| <span data-ttu-id="c3ebb-117">Создание карточек товара для складируемых, нескладируемых или сервисных товаров, которыми вы торгуете.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-117">Create item cards for inventory, non-inventory, or service items that you trade in.</span></span> |[<span data-ttu-id="c3ebb-118">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="c3ebb-118">Register New Items</span></span>](inventory-how-register-new-items.md) |
|<span data-ttu-id="c3ebb-119">Используйте функцию **Копировать товар** для быстрого создания новой карточки товара на основе существующей.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-119">Use the **Copy Item** function to quickly create a new item card based on an existing one.</span></span>|[<span data-ttu-id="c3ebb-120">Копирование существующих товаров для создания новых товаров</span><span class="sxs-lookup"><span data-stu-id="c3ebb-120">Copy Existing Items to Create New Items</span></span>](inventory-how-copy-items.md)|
|<span data-ttu-id="c3ebb-121">Узнайте, как заполнить поле **Тип** в карточках товара в соответствии с бизнес-целью.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-121">Learn how to fill in the **Type** field on item cards according to the business purpose.</span></span>|[<span data-ttu-id="c3ebb-122">О типах товаров</span><span class="sxs-lookup"><span data-stu-id="c3ebb-122">About Item Types</span></span>](inventory-about-item-types.md)|
|<span data-ttu-id="c3ebb-123">Настроить несколько единиц измерения для товара, которые можно использовать в качестве альтернативных единиц измерения, в транзакциях продажи или покупки либо в производственных транзакциях.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-123">Set up multiple units of measure for an item that you can use as alternate UOMs, for example on sales, purchasing, or production transactions.</span></span>|[<span data-ttu-id="c3ebb-124">Настройка единиц измерения товара</span><span class="sxs-lookup"><span data-stu-id="c3ebb-124">Set Up Item Units of Measure</span></span>](inventory-how-setup-units-of-measure.md)|
|<span data-ttu-id="c3ebb-125">Как дополнение к карточкам товаров, записывайте информацию о товарах на конкретном складе или о конкретном варианте.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-125">As a supplement to item cards, record information about your items in a specific location or of a specific variant.</span></span>|[<span data-ttu-id="c3ebb-126">Настройка единиц хранения</span><span class="sxs-lookup"><span data-stu-id="c3ebb-126">Set Up Stockkeeping Units</span></span>](inventory-how-to-set-up-stockkeeping-units.md)|
| <span data-ttu-id="c3ebb-127">Назначение товаров категориям и задание атрибутов для упрощения поиска товаров для вас и клиентов.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-127">Assign items to categories and give them attributes to help you and customers find items.</span></span> |[<span data-ttu-id="c3ebb-128">Категоризация товаров</span><span class="sxs-lookup"><span data-stu-id="c3ebb-128">Categorize Items</span></span>](inventory-how-categorize-items.md) |
|<span data-ttu-id="c3ebb-129">Одновременный импорт нескольких изображений товаров из ZIP-файла, в котором файлы названы в соответствии с номерами товаров.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-129">Import multiple item pictures in one go from a zip file where the files are named according to item numbers.</span></span>|[<span data-ttu-id="c3ebb-130">Импорт нескольких изображений товаров</span><span class="sxs-lookup"><span data-stu-id="c3ebb-130">Import Multiple Item Pictures</span></span>](inventory-how-import-item-pictures.md)|
|<span data-ttu-id="c3ebb-131">Укажите отчеты по умолчанию, которые будут использоваться для различных типов документов.</span><span class="sxs-lookup"><span data-stu-id="c3ebb-131">Specify default reports to be used for different document types.</span></span>|[<span data-ttu-id="c3ebb-132">Выбор отчета в Business Central</span><span class="sxs-lookup"><span data-stu-id="c3ebb-132">Report Selection in Business Central</span></span>](across-report-selections.md)|

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="c3ebb-133">См. соответствующее обучение на странице [Microsoft Learn](/learn/paths/trade-get-started-dynamics-365-business-central/)</span><span class="sxs-lookup"><span data-stu-id="c3ebb-133">See Related Training at [Microsoft Learn](/learn/paths/trade-get-started-dynamics-365-business-central/)</span></span>

## <a name="see-also"></a><span data-ttu-id="c3ebb-134">См. также</span><span class="sxs-lookup"><span data-stu-id="c3ebb-134">See Also</span></span>

[<span data-ttu-id="c3ebb-135">Управление запасами</span><span class="sxs-lookup"><span data-stu-id="c3ebb-135">Managing Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="c3ebb-136">Управление закупками</span><span class="sxs-lookup"><span data-stu-id="c3ebb-136">Managing Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="c3ebb-137">[Управление продажами](sales-manage-sales.md)  </span><span class="sxs-lookup"><span data-stu-id="c3ebb-137">[Managing Sales](sales-manage-sales.md)  </span></span>  
<span data-ttu-id="c3ebb-138">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c3ebb-138">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="c3ebb-139">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="c3ebb-139">General Business Functionality</span></span>](ui-across-business-areas.md)
