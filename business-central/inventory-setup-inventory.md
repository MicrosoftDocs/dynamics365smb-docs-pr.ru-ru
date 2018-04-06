---
title: "Настройка запасов | Документы Майкрософт"
description: "Описывается, как настроить процессы запасов, включая маршруты перемещения и склады."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, stock
ms.date: 01/12/2018
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 62eee7532e457721430cb31519b5acb23e95bfcb
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="setting-up-inventory"></a><span data-ttu-id="88422-103">Настройка запасов</span><span class="sxs-lookup"><span data-stu-id="88422-103">Setting Up Inventory</span></span>
<span data-ttu-id="88422-104">Прежде чем приступать к управлению складскими операциями и учетом стоимости товаров, необходимо настроить правила и значения, которые определяют политики запасов в компании.</span><span class="sxs-lookup"><span data-stu-id="88422-104">Before you can manage warehouse activities and inventory costing, you must configure the rules and values that define the company's inventory policies.</span></span>

<span data-ttu-id="88422-105">Вы можете обеспечить лучшее обслуживание клиентов и оптимизировать цепочку поставок, организовав запасы по различным адресам.</span><span class="sxs-lookup"><span data-stu-id="88422-105">You can provide better customer service and optimize your supply chain by organizing your inventory at different addresses.</span></span> <span data-ttu-id="88422-106">После этого вы можете закупать, хранить или продавать товары на различных складах и перемещать их между ними.</span><span class="sxs-lookup"><span data-stu-id="88422-106">You can then buy, store, or sell items at different locations and transfer inventory between them.</span></span>

<span data-ttu-id="88422-107">Если вы настроили запасы, вы можете управлять различными процессами, связанными с товарными транзакциями.</span><span class="sxs-lookup"><span data-stu-id="88422-107">When you have set up your inventory, you can manage various processes related to item transactions.</span></span> <span data-ttu-id="88422-108">Дополнительные сведения см. в разделах [Управление запасами](inventory-manage-inventory.md) и [Управление складом](warehouse-manage-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="88422-108">For more information, see [Manage Inventory](inventory-manage-inventory.md) and [Warehouse Management](warehouse-manage-warehouse.md).</span></span>

| <span data-ttu-id="88422-109">По</span><span class="sxs-lookup"><span data-stu-id="88422-109">To</span></span> | <span data-ttu-id="88422-110">Ссылка</span><span class="sxs-lookup"><span data-stu-id="88422-110">See</span></span> |
| --- | --- |
| <span data-ttu-id="88422-111">Определить общую настройку запасов, например серии номеров и использование складов.</span><span class="sxs-lookup"><span data-stu-id="88422-111">Define the general inventory setup, such as number series and how to use locations.</span></span> |[<span data-ttu-id="88422-112">Настройка общей информации по запасам</span><span class="sxs-lookup"><span data-stu-id="88422-112">Set Up General Inventory Information</span></span>](inventory-how-setup-general.md) |
|<span data-ttu-id="88422-113">Настройка эффективной модели распределения с комбинацией различных складов и центров ответственности, присваиваемых бизнес-партнерам или сотрудникам.</span><span class="sxs-lookup"><span data-stu-id="88422-113">Configure an efficient distribution model with a combination of different locations and responsibility centers assigned to business partners or employees.</span></span>|[<span data-ttu-id="88422-114">Работа с центрами ответственности</span><span class="sxs-lookup"><span data-stu-id="88422-114">Work with Responsibility Centers</span></span>](inventory-responsibility-centers.md)|
| <span data-ttu-id="88422-115">Организовать запасы на нескольких складах, включая маршруты перемещения.</span><span class="sxs-lookup"><span data-stu-id="88422-115">Organize your inventory at multiple locations, including transfer routes.</span></span> |[<span data-ttu-id="88422-116">Настройка складов</span><span class="sxs-lookup"><span data-stu-id="88422-116">Set Up Locations</span></span>](inventory-how-register-new-items.md) |
| <span data-ttu-id="88422-117">Создать карточку товара для каждого товара в запасах, которым вы торгуете.</span><span class="sxs-lookup"><span data-stu-id="88422-117">Create item cards for inventory items that you trade in.</span></span> |[<span data-ttu-id="88422-118">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="88422-118">Register New Items</span></span>](inventory-how-register-new-items.md) |
|<span data-ttu-id="88422-119">Настроить несколько единиц измерения для товара, которые можно использовать в качестве альтернативных единиц измерения, в транзакциях продажи или покупки либо в производственных транзакциях.</span><span class="sxs-lookup"><span data-stu-id="88422-119">Set up multiple units of measure for an item that you can use as alternate UOMs, for example on sales, purchasing, or production transactions.</span></span>|[<span data-ttu-id="88422-120">Настройка единиц измерения товара</span><span class="sxs-lookup"><span data-stu-id="88422-120">Set Up Item Units of Measure</span></span>](inventory-how-setup-units-of-measure.md)|
|<span data-ttu-id="88422-121">Как дополнение к карточкам товаров, записывайте информацию о товарах на конкретном складе или о конкретном варианте.</span><span class="sxs-lookup"><span data-stu-id="88422-121">As a supplement to item cards, record information about your items in a specific location or of a specific variant.</span></span>|[<span data-ttu-id="88422-122">Настройка единиц хранения</span><span class="sxs-lookup"><span data-stu-id="88422-122">Set Up Stockkeeping Units</span></span>](inventory-how-to-set-up-stockkeeping-units.md)|
| <span data-ttu-id="88422-123">Назначение товаров категориям и задание атрибутов для упрощения поиска товаров для вас и клиентов.</span><span class="sxs-lookup"><span data-stu-id="88422-123">Assign items to categories and give them attributes to help you and customers find items.</span></span> |[<span data-ttu-id="88422-124">Категоризация товаров</span><span class="sxs-lookup"><span data-stu-id="88422-124">Categorize Items</span></span>](inventory-how-categorize-items.md) |

## <a name="see-also"></a><span data-ttu-id="88422-125">См. также</span><span class="sxs-lookup"><span data-stu-id="88422-125">See Also</span></span>
[<span data-ttu-id="88422-126">Управление запасами</span><span class="sxs-lookup"><span data-stu-id="88422-126">Managing Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="88422-127">Управление закупками</span><span class="sxs-lookup"><span data-stu-id="88422-127">Managing Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="88422-128">[Управление продажами](sales-manage-sales.md)  </span><span class="sxs-lookup"><span data-stu-id="88422-128">[Managing Sales](sales-manage-sales.md)  </span></span>  
<span data-ttu-id="88422-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="88422-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="88422-130">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="88422-130">General Business Functionality</span></span>](ui-across-business-areas.md)

