---
title: Планирование со складами или без складов | Документация Майкрософт
description: Важно понимать планирование с кодом склада или без кода склада в строках требования.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: dd86568c87a9cbb66214ae88b75fcdae8e85b59d
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5383179"
---
# <a name="planning-with-or-without-locations"></a><span data-ttu-id="7f8c9-103">Планирование со складами и без складов</span><span class="sxs-lookup"><span data-stu-id="7f8c9-103">Planning With or Without Locations</span></span>
<span data-ttu-id="7f8c9-104">Что касается планирования с кодом склада или без кода склада в строке требования, работа системы планирования упрощается при следующих условиях:</span><span class="sxs-lookup"><span data-stu-id="7f8c9-104">Concerning planning with or without location codes on demand lines, the planning system operates in a straight forward way when:</span></span>  

-   <span data-ttu-id="7f8c9-105">в строках требования всегда имеются коды склада, а в системе полностью используются единицы хранения, включая соответствующую настройку склада.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-105">demand lines always carry location codes and the system fully uses stockkeeping units, including the relevant location setup.</span></span>  
-   <span data-ttu-id="7f8c9-106">в строках требования всегда отсутствуют коды склада, а в системе не используются единицы хранения или какие-либо настройки складов (см. последний из сценариев, приведенных ниже).</span><span class="sxs-lookup"><span data-stu-id="7f8c9-106">demand lines never carry location codes and the system does not use SKUs or any location setup (see last scenario below).</span></span>  

<span data-ttu-id="7f8c9-107">Но если строки требований то содержат коды склада, то нет, система планирования, в зависимости от настройки, будет следовать определенным правилам.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-107">However, if demand lines sometimes have location codes and other times do not, the planning system will follow certain rules depending on setup.</span></span>  

## <a name="demand-at-location"></a><span data-ttu-id="7f8c9-108">Спрос на складе</span><span class="sxs-lookup"><span data-stu-id="7f8c9-108">Demand at Location</span></span>  
<span data-ttu-id="7f8c9-109">Если система планирования обнаруживает спрос на складе (строку с кодом склада), дальнейшие действия определяются 3 важнейшими параметрами настройки.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-109">When the planning system detects demand at a location (a line with a location code), it will behave in different ways depending on 3 critical setup values.</span></span>  

<span data-ttu-id="7f8c9-110">Во время исполнения планирования в системе поочередно проверяются 3 параметра настройки, и планирование проводится в соответствии с их значениями.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-110">During a planning run, the system checks for the 3 setup values in sequence and plans accordingly:</span></span>  

1.  <span data-ttu-id="7f8c9-111">Установлен ли флажок **Склад обязателен**?</span><span class="sxs-lookup"><span data-stu-id="7f8c9-111">Is there a check mark in the **Location Mandatory** field?</span></span>  

    <span data-ttu-id="7f8c9-112">Если да, то:</span><span class="sxs-lookup"><span data-stu-id="7f8c9-112">If yes, then:</span></span>  

2.  <span data-ttu-id="7f8c9-113">Существует ли для товара единица хранения?</span><span class="sxs-lookup"><span data-stu-id="7f8c9-113">Does SKU exist for the item?</span></span>  

    <span data-ttu-id="7f8c9-114">Если да, то:</span><span class="sxs-lookup"><span data-stu-id="7f8c9-114">If yes, then:</span></span>  

    <span data-ttu-id="7f8c9-115">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке единицы хранения.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-115">The item is planned according to planning parameters on the SKU card.</span></span>  

    <span data-ttu-id="7f8c9-116">Если нет, то:</span><span class="sxs-lookup"><span data-stu-id="7f8c9-116">If no, then:</span></span>  

3.  <span data-ttu-id="7f8c9-117">Содержится ли в поле **Компоненты по складам** код склада требования?</span><span class="sxs-lookup"><span data-stu-id="7f8c9-117">Does the **Components at Location** field contain the demanded location code?</span></span>  

    <span data-ttu-id="7f8c9-118">Если да, то:</span><span class="sxs-lookup"><span data-stu-id="7f8c9-118">If yes, then:</span></span>  

    <span data-ttu-id="7f8c9-119">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке товара.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-119">The item is planned according to planning parameters on the item card.</span></span>  

    <span data-ttu-id="7f8c9-120">Если нет, то:</span><span class="sxs-lookup"><span data-stu-id="7f8c9-120">If no, then:</span></span>  

    <span data-ttu-id="7f8c9-121">Планирование товара производится в соответствии со следующими параметрами: Политика повторного заказа =  *Партия-на-партию*, Вкл. товар =  *Да*, прочие параметры планирования = Пусто.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-121">The item is planned according to: Reordering Policy =  *Lot-for-Lot*, Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span> <span data-ttu-id="7f8c9-122">(Товары, использующие политику повторного заказа  *Заказ*, продолжают использовать политику  *Заказ* так же, как и другие параметры.)</span><span class="sxs-lookup"><span data-stu-id="7f8c9-122">(Items using reordering policy  *Order* remain using  *Order* as well as the other settings.)</span></span>  

> [!NOTE]  
>  <span data-ttu-id="7f8c9-123">Эта минимальная альтернатива касается только конкретного спроса.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-123">This minimal alternative only covers the exact demand.</span></span> <span data-ttu-id="7f8c9-124">Все определенные параметры планирования игнорируются.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-124">Any planning parameters defined are ignored.</span></span>  

<span data-ttu-id="7f8c9-125">См. варианты в сценариях, приведенные ниже.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-125">See variations in the scenarios below.</span></span>  

## <a name="demand-at-blank-location"></a><span data-ttu-id="7f8c9-126">Спрос на складе "Пустой"</span><span class="sxs-lookup"><span data-stu-id="7f8c9-126">Demand at "Blank Location"</span></span>  
<span data-ttu-id="7f8c9-127">Даже если установлен флажок **Код склада обязателен**, система допускает создание строк требования без кода склада — так называемый *ПУСТОЙ* склад.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-127">Even if the **Location Mandatory** check box is selected, the system will allow demand lines to be created without a location code – also referred to as *BLANK* location.</span></span> <span data-ttu-id="7f8c9-128">Это отклонение для системы, поскольку сюда включены значения различных параметров настройки, касающиеся складов (см. выше), и в результате модуль планирования не создаст строку планирования для такой строки спроса.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-128">This is a deviation for the system because it has various setup values tuned to dealing with locations (see above) and as a result, the planning engine will not create a planning line for such a demand line.</span></span> <span data-ttu-id="7f8c9-129">Если флажок в поле **Склад обязателен** не установлен, а значения настройки склада существуют, то это также считается отклонением, и система планирования прореагируют, выдав "минимальную альтернативу":</span><span class="sxs-lookup"><span data-stu-id="7f8c9-129">If the **Location Mandatory** field is not selected but any of the location setup values exist, then that is also considered a deviation and the planning system will react by outputting the "minimal alternative":</span></span>   
<span data-ttu-id="7f8c9-130">Планирование товара в этом случае производится в соответствии со следующими параметрами: Политика повторного заказа = *Партия-на-партию* (политика *Заказ* остается равной *Заказ)*, Вкл. товар = *Да*, прочие параметры планирования = Пусто.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-130">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains *Order)*, Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

<span data-ttu-id="7f8c9-131">См. варианты в сценариях настройки, приведенных ниже.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-131">See variations in the setup scenarios below.</span></span>  

### <a name="setup-1"></a><span data-ttu-id="7f8c9-132">Настройка 1:</span><span class="sxs-lookup"><span data-stu-id="7f8c9-132">Setup 1:</span></span>  

-   <span data-ttu-id="7f8c9-133">Код склада обязателен = *Да*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-133">Location Mandatory = *Yes*</span></span>  
-   <span data-ttu-id="7f8c9-134">Настройка единицы хранения —  *КРАСНЫЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-134">SKU is set up for  *RED*</span></span>  
-   <span data-ttu-id="7f8c9-135">Компоненты по складам =  *СИНИЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-135">Component at Location =  *BLUE*</span></span>  

#### <a name="case-11-demand-is-at--red-location"></a><span data-ttu-id="7f8c9-136">Случай 1.1: спрос на складе *КРАСНЫЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-136">Case 1.1: Demand is at  *RED* location</span></span>  

<span data-ttu-id="7f8c9-137">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке единицы хранения (включая возможное перемещение).</span><span class="sxs-lookup"><span data-stu-id="7f8c9-137">The item is planned according to planning parameters on the SKU card (including possible transfer).</span></span>  

#### <a name="case-12-demand-is-at--blue-location"></a><span data-ttu-id="7f8c9-138">Случай 1.2: спрос на складе *СИНИЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-138">Case 1.2: Demand is at  *BLUE* location</span></span>  

<span data-ttu-id="7f8c9-139">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке товара.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-139">The item is planned according to planning parameters on the item card.</span></span>  

#### <a name="case-13-demand-is-at--green-location"></a><span data-ttu-id="7f8c9-140">Случай 1.3: спрос на складе  *ЗЕЛЕНЫЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-140">Case 1.3: Demand is at  *GREEN* location</span></span>  

<span data-ttu-id="7f8c9-141">Планирование товара производится в соответствии со следующими параметрами: Политика повторного заказа = *Партия-на-партию* (политика *Заказ* остается равной *Заказ*), Вкл. товар = *Да*, все прочие параметры планирования = Пусто.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-141">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

#### <a name="case-14-demand-is-at--blank-location"></a><span data-ttu-id="7f8c9-142">Случай 1.4: спрос на складе  *ПУСТОЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-142">Case 1.4: Demand is at  *BLANK* location</span></span>  

<span data-ttu-id="7f8c9-143">Планирование товара не производится, поскольку в строке требования не задан склад.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-143">The item is not planned because no location is defined on the demand line.</span></span>  

### <a name="setup-2"></a><span data-ttu-id="7f8c9-144">Настройка 2:</span><span class="sxs-lookup"><span data-stu-id="7f8c9-144">Setup 2:</span></span>  

-   <span data-ttu-id="7f8c9-145">Код склада обязателен = *Да*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-145">Location Mandatory = *Yes*</span></span>  
-   <span data-ttu-id="7f8c9-146">Единица хранения не существует</span><span class="sxs-lookup"><span data-stu-id="7f8c9-146">No SKU exists</span></span>  
-   <span data-ttu-id="7f8c9-147">Компоненты по складам =  *СИНИЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-147">Component at Location =  *BLUE*</span></span>  

#### <a name="case-21-demand-is-at--red-location"></a><span data-ttu-id="7f8c9-148">Случай 2.1: спрос на складе  *КРАСНЫЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-148">Case 2.1: Demand is at  *RED* location</span></span>  

<span data-ttu-id="7f8c9-149">Планирование товара производится в соответствии со следующими параметрами: Политика повторного заказа = *Партия-на-партию* (политика *Заказ* остается равной *Заказ*), Вкл. товар = *Да*, все прочие параметры планирования = Пусто.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-149">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

#### <a name="case-22-demand-is-at--blue-location"></a><span data-ttu-id="7f8c9-150">Случай 2.2: спрос на складе *СИНИЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-150">Case 2.2: Demand is at  *BLUE* location</span></span>  

<span data-ttu-id="7f8c9-151">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке товара.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-151">The item is planned according to planning parameters on the item card.</span></span>  

### <a name="setup-3"></a><span data-ttu-id="7f8c9-152">Настройка 3:</span><span class="sxs-lookup"><span data-stu-id="7f8c9-152">Setup 3:</span></span>  

-   <span data-ttu-id="7f8c9-153">Код склада обязателен = *Нет*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-153">Location Mandatory = *No*</span></span>  
-   <span data-ttu-id="7f8c9-154">Единица хранения не существует</span><span class="sxs-lookup"><span data-stu-id="7f8c9-154">No SKU exists</span></span>  
-   <span data-ttu-id="7f8c9-155">Компоненты по складам =  *СИНИЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-155">Component at Location =  *BLUE*</span></span>  

#### <a name="case-31-demand-is-at--red-location"></a><span data-ttu-id="7f8c9-156">Случай 3.1: спрос на складе  *КРАСНЫЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-156">Case 3.1: Demand is at  *RED* location</span></span>  

<span data-ttu-id="7f8c9-157">Планирование товара производится в соответствии со следующими параметрами: Политика повторного заказа = *Партия-на-партию* (политика *Заказ* остается равной *Заказ*), Вкл. товар = *Да*, все прочие параметры планирования = Пусто.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-157">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

#### <a name="case-32-demand-is-at--blue-location"></a><span data-ttu-id="7f8c9-158">Случай 3.2: спрос на складе *СИНИЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-158">Case 3.2: Demand is at  *BLUE* location</span></span>  

<span data-ttu-id="7f8c9-159">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке товара.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-159">The item is planned according to planning parameters on the item card.</span></span>  

#### <a name="case-33-demand-is-at--blank-location"></a><span data-ttu-id="7f8c9-160">Случай 3.3: спрос на складе  *ПУСТОЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-160">Case 3.3: Demand is at  *BLANK* location</span></span>  

<span data-ttu-id="7f8c9-161">Планирование товара производится в соответствии со следующими параметрами: Политика повторного заказа = *Партия-на-партию* (политика *Заказ* остается равной *Заказ*), Вкл. товар = *Да*, все прочие параметры планирования = Пусто.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-161">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

### <a name="setup-4"></a><span data-ttu-id="7f8c9-162">Настройка 4:</span><span class="sxs-lookup"><span data-stu-id="7f8c9-162">Setup 4:</span></span>  

-   <span data-ttu-id="7f8c9-163">Код склада обязателен = *Нет*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-163">Location Mandatory = *No*</span></span>  
-   <span data-ttu-id="7f8c9-164">Единица хранения не существует</span><span class="sxs-lookup"><span data-stu-id="7f8c9-164">No SKU exists</span></span>  
-   <span data-ttu-id="7f8c9-165">Компоненты по складам =  *ПУСТОЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-165">Component at Location =  *BLANK*</span></span>  

#### <a name="case-41-demand-is-at--blue-location"></a><span data-ttu-id="7f8c9-166">Случай 4.1: спрос на складе  *СИНИЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-166">Case 4.1: Demand is at  *BLUE* location</span></span>  

<span data-ttu-id="7f8c9-167">Планирование товара производится в соответствии со следующими параметрами: Политика повторного заказа = *Партия-на-партию* (политика *Заказ* остается равной *Заказ*), Вкл. товар = *Да*, все прочие параметры планирования = Пусто.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-167">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

#### <a name="case-42-demand-is-at--blank-location"></a><span data-ttu-id="7f8c9-168">Случай 4.2: спрос на складе  *ПУСТОЙ*</span><span class="sxs-lookup"><span data-stu-id="7f8c9-168">Case 4.2: Demand is at  *BLANK* location</span></span>  

<span data-ttu-id="7f8c9-169">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке товара.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-169">The item is planned according to planning parameters on the item card.</span></span>  

<span data-ttu-id="7f8c9-170">Как показывает последний сценарий, единственный способ получить правильный результат для строки требования без кода склада - это отключить все значения настройки, относящиеся к складам.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-170">As you can see from the last scenario, the only way to get a correct result for a demand line without a location code is to disable all setup values relating to locations.</span></span> <span data-ttu-id="7f8c9-171">Кроме того, единственным способом получить стабильные результаты планирования для требований на складе - является использование складских единиц учета.</span><span class="sxs-lookup"><span data-stu-id="7f8c9-171">Similarly, the only way to get stable planning results for demand at locations is to use stockkeeping units.</span></span>  

<span data-ttu-id="7f8c9-172">Следовательно, при частом проведении планирования с учетом требований на складах рекомендуется использовать функцию «Единицы хранения».</span><span class="sxs-lookup"><span data-stu-id="7f8c9-172">Therefore, if you often plan for demand at locations, it is strongly advised to use the Stockkeeping Units feature.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7f8c9-173">См. также</span><span class="sxs-lookup"><span data-stu-id="7f8c9-173">See Also</span></span>
<span data-ttu-id="7f8c9-174">[Планирование](production-planning.md)  </span><span class="sxs-lookup"><span data-stu-id="7f8c9-174">[Planning](production-planning.md)  </span></span>  
[<span data-ttu-id="7f8c9-175">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="7f8c9-175">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="7f8c9-176">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="7f8c9-176">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="7f8c9-177">Наличие</span><span class="sxs-lookup"><span data-stu-id="7f8c9-177">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="7f8c9-178">Покупки</span><span class="sxs-lookup"><span data-stu-id="7f8c9-178">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="7f8c9-179">[Сведения о проектировании: планирование поставок](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="7f8c9-179">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="7f8c9-180">Рекомендации по настройке. Планирование поставок</span><span class="sxs-lookup"><span data-stu-id="7f8c9-180">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="7f8c9-181">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7f8c9-181">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]