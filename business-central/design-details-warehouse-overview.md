---
title: Сведения о проектировании — обзор склада | Документация Майкрософт
description: Для обеспечения поддержки физической обработки товаров на уровне зон и ячеек все сведения должны отслеживаться для каждой транзакции или перемещения на складе. Управление этим осуществляется в таблице **Складская операция**. Каждая транзакция хранится в складском регистре.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 8842bd23f6d2d470599afe9b4382b35cec3d9251
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4749547"
---
# <a name="design-details-warehouse-overview"></a><span data-ttu-id="0ccee-105">Сведения о проектировании: обзор склада</span><span class="sxs-lookup"><span data-stu-id="0ccee-105">Design Details: Warehouse Overview</span></span>
<span data-ttu-id="0ccee-106">Для обеспечения поддержки физической обработки товаров на уровне зон и ячеек все сведения должны отслеживаться для каждой транзакции или перемещения на складе.</span><span class="sxs-lookup"><span data-stu-id="0ccee-106">To support the physical handling of items on the zone and bin level, all information must be traced for each transaction or movement in the warehouse.</span></span> <span data-ttu-id="0ccee-107">Управление этим осуществляется в таблице **Складская операция**.</span><span class="sxs-lookup"><span data-stu-id="0ccee-107">This is managed in the **Warehouse Entry** table.</span></span> <span data-ttu-id="0ccee-108">Каждая транзакция хранится в складском регистре.</span><span class="sxs-lookup"><span data-stu-id="0ccee-108">Each transaction is stored in a warehouse register.</span></span>  

<span data-ttu-id="0ccee-109">Складские документы и складской журнал используются для регистрации перемещений товаров на складе.</span><span class="sxs-lookup"><span data-stu-id="0ccee-109">Warehouse documents and a warehouse journal are used to register item movements in the warehouse.</span></span> <span data-ttu-id="0ccee-110">При каждом перемещении, получении, размещении, подборе, отгрузке или коррекции товара на складе регистрируются складские операции для хранения физической информации о зоне, ячейке и количестве.</span><span class="sxs-lookup"><span data-stu-id="0ccee-110">Every time that an item in the warehouse is moved, received, put away, picked, shipped, or adjusted, warehouse entries are registered to store the physical information about zone, bin, and quantity.</span></span>

<span data-ttu-id="0ccee-111">Таблица **Содержимое ячейки** используется для обработки разнообразных измерений содержимого ячейки для товара, например единицы измерения, максимального количества и минимального количества.</span><span class="sxs-lookup"><span data-stu-id="0ccee-111">The **Bin Content** table is used to handle all the different dimensions of the contents of a bin per item, such as unit of measure, maximum quantity, and minimum quantity.</span></span> <span data-ttu-id="0ccee-112">Таблица **Содержимое ячейки** также содержит поля FlowField для складских операций, инструкций склада и строк складского журнала, что обеспечивает возможность быстрого вычисления доступности товара по ячейкам и ячеек для товаров.</span><span class="sxs-lookup"><span data-stu-id="0ccee-112">The **Bin Content** table also contains flow fields to the warehouse entries, warehouse instructions, and warehouse journal lines, which ensures that the availability of an item per bin and a bin for an item can be calculated quickly.</span></span> <span data-ttu-id="0ccee-113">Дополнительные сведения см. в разделе [Сведения о проектировании: наличие на складе](design-details-availability-in-the-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="0ccee-113">For more information, see [Design Details: Availability in the Warehouse](design-details-availability-in-the-warehouse.md).</span></span>  

<span data-ttu-id="0ccee-114">Если учет товаров осуществляется за пределами складского модуля, ячейка корректировки по умолчанию для конкретного склада используется для синхронизации складских операций с операциями инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="0ccee-114">When item postings occur outside the warehouse module, a default adjustment bin per location is used to synchronize warehouse entries with inventory entries.</span></span> <span data-ttu-id="0ccee-115">Во время инвентаризации склада любые расхождения между расчетными и подсчитанными количествами регистрируются в ячейке для коррекций, а затем учитываются как корректирующие операции книги товаров.</span><span class="sxs-lookup"><span data-stu-id="0ccee-115">During physical inventory of the warehouse, any differences between the calculated and counted quantities are recorded in the adjustment bin and then posted as correcting item ledger entries.</span></span> <span data-ttu-id="0ccee-116">Дополнительные сведения см. в разделе [Сведения о проектировании: интеграция с запасом](design-details-integration-with-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="0ccee-116">For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).</span></span>  

<span data-ttu-id="0ccee-117">На следующей иллюстрации показаны типичные складские потоки.</span><span class="sxs-lookup"><span data-stu-id="0ccee-117">The following illustration outlines typical warehouse flows.</span></span>  

<span data-ttu-id="0ccee-118">![Обзор складских процессов](media/design_details_warehouse_management_overview.png "Обзор складских процессов")</span><span class="sxs-lookup"><span data-stu-id="0ccee-118">![Overview of warehouse processes](media/design_details_warehouse_management_overview.png "Overview of warehouse processes")</span></span>  

## <a name="basic-or-advanced-warehousing"></a><span data-ttu-id="0ccee-119">Базовые или расширенные функции склада</span><span class="sxs-lookup"><span data-stu-id="0ccee-119">Basic or Advanced Warehousing</span></span>  
<span data-ttu-id="0ccee-120">Складская функциональность в [!INCLUDE[prod_short](includes/prod_short.md)] может быть реализована на разных уровнях сложности в зависимости от процессов и объема заказов компании.</span><span class="sxs-lookup"><span data-stu-id="0ccee-120">Warehouse functionality in [!INCLUDE[prod_short](includes/prod_short.md)] can be implemented in different complexity levels, depending on a company’s processes and order volume.</span></span> <span data-ttu-id="0ccee-121">Основное различие в том, что действия выполняются на уровне отдельных заказов в базовом складировании, когда они консолидируются для нескольких заказов в расширенном складировании.</span><span class="sxs-lookup"><span data-stu-id="0ccee-121">The main difference is that activities are performed order-by-order in basic warehousing when they are consolidated for multiple orders in advanced warehousing.</span></span>  

 <span data-ttu-id="0ccee-122">Чтобы различить разные уровни сложности, в этой документации используется два общих понятия — базовое и расширенное складирование.</span><span class="sxs-lookup"><span data-stu-id="0ccee-122">To differentiate between the different complexity levels, this documentation refers to two general denominations, Basic and Advanced Warehousing.</span></span> <span data-ttu-id="0ccee-123">Эта простая дифференциация охватывает несколько разных уровней сложности, как определено областями продукции и настройками склада, каждый из которых поддерживается разными документами ИП.</span><span class="sxs-lookup"><span data-stu-id="0ccee-123">This simple differentiation covers several different complexity levels as defined by product granules and location setup, each supported by different UI documents.</span></span> <span data-ttu-id="0ccee-124">Дополнительные сведения см. в разделе [Сведения о проектировании: настройка склада](design-details-warehouse-setup.md).</span><span class="sxs-lookup"><span data-stu-id="0ccee-124">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0ccee-125">Самый расширенный уровень складирования — установки WMS в этой документации, поскольку этот уровень требует самой широкой функциональности, системы управления складом.</span><span class="sxs-lookup"><span data-stu-id="0ccee-125">The most advanced level of warehousing is referred to as “WMS installations” in this documentation, since this level requires the most advanced granule, Warehouse Management Systems.</span></span>  

 <span data-ttu-id="0ccee-126">Следующие документы ИП используются в основном и расширенном складировании.</span><span class="sxs-lookup"><span data-stu-id="0ccee-126">The following different UI documents are used in basic and advanced warehousing.</span></span>  

## <a name="basic-ui-documents"></a><span data-ttu-id="0ccee-127">Основные документы пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="0ccee-127">Basic UI Documents</span></span>  

-   <span data-ttu-id="0ccee-128">**Размещение запасов**</span><span class="sxs-lookup"><span data-stu-id="0ccee-128">**Inventory Put-away**</span></span>  
-   <span data-ttu-id="0ccee-129">**Подбор запасов**</span><span class="sxs-lookup"><span data-stu-id="0ccee-129">**Inventory Pick**</span></span>  
-   <span data-ttu-id="0ccee-130">**Перемещение запасов**</span><span class="sxs-lookup"><span data-stu-id="0ccee-130">**Inventory Movement**</span></span>  
-   <span data-ttu-id="0ccee-131">**Журнал товаров**</span><span class="sxs-lookup"><span data-stu-id="0ccee-131">**Item Journal**</span></span>  
-   <span data-ttu-id="0ccee-132">**Журнал реклассификации товаров**</span><span class="sxs-lookup"><span data-stu-id="0ccee-132">**Item Reclassification Journal**</span></span>  
-   <span data-ttu-id="0ccee-133">(Различные отчеты)</span><span class="sxs-lookup"><span data-stu-id="0ccee-133">(Various reports)</span></span>  

## <a name="advanced-ui-documents"></a><span data-ttu-id="0ccee-134">Документы по расширенному пользовательскому интерфейсу</span><span class="sxs-lookup"><span data-stu-id="0ccee-134">Advanced UI Documents</span></span>  

-   <span data-ttu-id="0ccee-135">**Складская приемка**</span><span class="sxs-lookup"><span data-stu-id="0ccee-135">**Warehouse Receipt**</span></span>  
-   <span data-ttu-id="0ccee-136">**Журнал размещения**</span><span class="sxs-lookup"><span data-stu-id="0ccee-136">**Put-away Worksheet**</span></span>  
-   <span data-ttu-id="0ccee-137">**Складское размещение**</span><span class="sxs-lookup"><span data-stu-id="0ccee-137">**Warehouse Put-away**</span></span>  
-   <span data-ttu-id="0ccee-138">**Журнал подбора**</span><span class="sxs-lookup"><span data-stu-id="0ccee-138">**Pick Worksheet**</span></span>  
-   <span data-ttu-id="0ccee-139">**Складской подбор**</span><span class="sxs-lookup"><span data-stu-id="0ccee-139">**Warehouse Pick**</span></span>  
-   <span data-ttu-id="0ccee-140">**Журнал перемещения**</span><span class="sxs-lookup"><span data-stu-id="0ccee-140">**Movement Worksheet**</span></span>  
-   <span data-ttu-id="0ccee-141">**Складское перемещение**</span><span class="sxs-lookup"><span data-stu-id="0ccee-141">**Warehouse Movement**</span></span>  
-   <span data-ttu-id="0ccee-142">**Внутренний подбор склада**</span><span class="sxs-lookup"><span data-stu-id="0ccee-142">**Internal Whse. Pick**</span></span>  
-   <span data-ttu-id="0ccee-143">**Внутреннее размещение склада**</span><span class="sxs-lookup"><span data-stu-id="0ccee-143">**Internal Whse. Put-away**</span></span>  
-   <span data-ttu-id="0ccee-144">**Журнал создания ячеек**</span><span class="sxs-lookup"><span data-stu-id="0ccee-144">**Bin Creation Worksheet**</span></span>  
-   <span data-ttu-id="0ccee-145">**Журнал создания содержимого ячеек**</span><span class="sxs-lookup"><span data-stu-id="0ccee-145">**Bin Content Creation Worksheet**</span></span>  
-   <span data-ttu-id="0ccee-146">**Журнал товаров склада**</span><span class="sxs-lookup"><span data-stu-id="0ccee-146">**Whse. Item Journal**</span></span>  
-   <span data-ttu-id="0ccee-147">**Журнал реклассификации складских товаров**</span><span class="sxs-lookup"><span data-stu-id="0ccee-147">**Whse. Item Reclass. Journal**</span></span>  
-   <span data-ttu-id="0ccee-148">(Различные отчеты)</span><span class="sxs-lookup"><span data-stu-id="0ccee-148">(Various reports)</span></span>  

<span data-ttu-id="0ccee-149">Дополнительные сведения о каждом документе см. в соответствующих разделах страниц.</span><span class="sxs-lookup"><span data-stu-id="0ccee-149">For more information about each document, see the respective page topics.</span></span>  

### <a name="terminology"></a><span data-ttu-id="0ccee-150">Терминология</span><span class="sxs-lookup"><span data-stu-id="0ccee-150">Terminology</span></span>  
<span data-ttu-id="0ccee-151">Для того чтобы скоординировать с финансовыми понятиями покупки и продажи, складская документация [!INCLUDE[prod_short](includes/prod_short.md)] использует следующие термины для обозначения потока товаров на складе.</span><span class="sxs-lookup"><span data-stu-id="0ccee-151">To align with the financial concepts of purchases and sales, [!INCLUDE[prod_short](includes/prod_short.md)] warehouse documentation refers to the following terms for item flow in the warehouse.</span></span>  

|<span data-ttu-id="0ccee-152">Термин</span><span class="sxs-lookup"><span data-stu-id="0ccee-152">Term</span></span>|<span data-ttu-id="0ccee-153">Описание</span><span class="sxs-lookup"><span data-stu-id="0ccee-153">Description</span></span>|  
|----------|---------------------------------------|  
|<span data-ttu-id="0ccee-154">Входящий поток</span><span class="sxs-lookup"><span data-stu-id="0ccee-154">Inbound flow</span></span>|<span data-ttu-id="0ccee-155">Товары, перемещаемые на склад, например покупки и входящие перемещения.</span><span class="sxs-lookup"><span data-stu-id="0ccee-155">Items moving into the warehouse location, such as purchases and inbound transfers.</span></span>|  
|<span data-ttu-id="0ccee-156">Внутренний поток</span><span class="sxs-lookup"><span data-stu-id="0ccee-156">Internal flow</span></span>|<span data-ttu-id="0ccee-157">Товары, перемещаемые в пределах склада, например производственные компоненты и выход.</span><span class="sxs-lookup"><span data-stu-id="0ccee-157">Items moving inside the warehouse location, such as production components and output.</span></span>|  
|<span data-ttu-id="0ccee-158">Исходящий поток</span><span class="sxs-lookup"><span data-stu-id="0ccee-158">Outbound flow</span></span>|<span data-ttu-id="0ccee-159">Товары, перемещаемые со склада, например продажи и исходящие перемещения.</span><span class="sxs-lookup"><span data-stu-id="0ccee-159">Items moving out of the warehouse location, such as sales and outbound transfers.</span></span>|  

## <a name="see-also"></a><span data-ttu-id="0ccee-160">См. также</span><span class="sxs-lookup"><span data-stu-id="0ccee-160">See Also</span></span>  
 [<span data-ttu-id="0ccee-161">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="0ccee-161">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)
