---
title: Сведения о проектировании — поставка и требования | Документация Майкрософт
description: В этом разделе вводится концепция требования — это общий термин, используемый для любого типа общего требования, такого как заказ на продажу и требуемый компонент в производственном заказе.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, demand, supply, inventory, planning
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 62abcd0e37a9871efd6158a898538b7c18b6b47f
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215332"
---
# <a name="design-details-demand-at-blank-location"></a><span data-ttu-id="ac768-103">Сведения о проектировании: спрос на пустом складе</span><span class="sxs-lookup"><span data-stu-id="ac768-103">Design Details: Demand at Blank Location</span></span>
<span data-ttu-id="ac768-104">Если пользователь создает событие требования, например строку заказа на продажу, программа иногда позволяет пользователю указать код склада, в другие разы — нет, нужно использовать пустой склад.</span><span class="sxs-lookup"><span data-stu-id="ac768-104">When a user creates a demand event, such as a sales order line, the program allows the user to sometimes specify a location code and other times not, that is, use blank location.</span></span>

<span data-ttu-id="ac768-105">Что касается требования с кодом склада или без кода склада, работа системы планирования упрощается при следующих условиях:</span><span class="sxs-lookup"><span data-stu-id="ac768-105">For demand with or without location codes, the planning system operates in a straight forward way when:</span></span>

- <span data-ttu-id="ac768-106">В строках требования всегда содержатся коды склада, а в системе полностью используются единицы хранения, включая соответствующую настройку склада.</span><span class="sxs-lookup"><span data-stu-id="ac768-106">Demand lines always carry location codes and the system fully uses SKUs, including the relevant location setup.</span></span>
- <span data-ttu-id="ac768-107">В строках требования всегда отсутствуют коды склада, а в системе не используются единицы хранения или какие-либо настройки складов (см. последний сценарий в следующем разделе).</span><span class="sxs-lookup"><span data-stu-id="ac768-107">Demand lines never carry location codes, and the system does not use SKUs or any location setup (see the last scenario in the following section).</span></span>

<span data-ttu-id="ac768-108">Но если события требования иногда содержат коды склада, то система планирования будет следовать определенным правилам в зависимости от настройки.</span><span class="sxs-lookup"><span data-stu-id="ac768-108">However, if demand events sometimes have location codes and other times do not, the planning system will follow certain rules depending on setup.</span></span>

## <a name="demand-at-location"></a><span data-ttu-id="ac768-109">Спрос на складе</span><span class="sxs-lookup"><span data-stu-id="ac768-109">Demand at Location</span></span>
<span data-ttu-id="ac768-110">Если система планирования обнаруживает требования на складе, дальнейшие действия определяются тремя важнейшими параметрами настройки.</span><span class="sxs-lookup"><span data-stu-id="ac768-110">When the planning system detects demand at a location, it will behave in different ways depending on three critical setup values.</span></span> <span data-ttu-id="ac768-111">Во время планирования в системе поочередно проверяются три параметра настройки, и планирование проводится в соответствии с их значениями.</span><span class="sxs-lookup"><span data-stu-id="ac768-111">During a planning run, the system checks for three setup values in sequence and plans accordingly.</span></span>

1. <span data-ttu-id="ac768-112">Установлен ли флажок **Склад обязателен**?</span><span class="sxs-lookup"><span data-stu-id="ac768-112">Is there a check mark in the **Location Mandatory** field?</span></span>

    <span data-ttu-id="ac768-113">Если да, то:</span><span class="sxs-lookup"><span data-stu-id="ac768-113">If yes, then:</span></span>

2. <span data-ttu-id="ac768-114">Существует ли для товара единица хранения?</span><span class="sxs-lookup"><span data-stu-id="ac768-114">Does SKU exist for the item?</span></span>

    <span data-ttu-id="ac768-115">Если да, то:</span><span class="sxs-lookup"><span data-stu-id="ac768-115">If yes, then:</span></span>

    <span data-ttu-id="ac768-116">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке единицы хранения.</span><span class="sxs-lookup"><span data-stu-id="ac768-116">The item is planned according to planning parameters on the SKU card.</span></span>

    <span data-ttu-id="ac768-117">Если нет, то:</span><span class="sxs-lookup"><span data-stu-id="ac768-117">If no, then:</span></span>

3. <span data-ttu-id="ac768-118">Содержится ли в поле Компоненты по складам код склада требования?</span><span class="sxs-lookup"><span data-stu-id="ac768-118">Does the Components at Location field contain the demanded location code?</span></span>

  <span data-ttu-id="ac768-119">Если да, то:</span><span class="sxs-lookup"><span data-stu-id="ac768-119">If yes, then:</span></span>

  <span data-ttu-id="ac768-120">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке товара.</span><span class="sxs-lookup"><span data-stu-id="ac768-120">The item is planned according to planning parameters on the item card.</span></span>

  <span data-ttu-id="ac768-121">Если нет, то:</span><span class="sxs-lookup"><span data-stu-id="ac768-121">If no, then:</span></span>

  <span data-ttu-id="ac768-122">Планирование товара производится в соответствии со следующими параметрами: "Политика дозаказа" = "Партия-на-партию, Вкл. товар" = "Да, прочие параметры планирования" = "Пусто" (товары, использующие политику дозаказа "Заказ" продолжают использовать политику "Заказ" так же, как и другие параметры).</span><span class="sxs-lookup"><span data-stu-id="ac768-122">The item is planned according to: Reordering Policy = Lot-for-Lot, Include Inventory = Yes, all other planning parameters = Empty, items using Reordering Policy = Order will remain using Order along with the other settings.</span></span>

> [!NOTE]
> <span data-ttu-id="ac768-123">Исключительная настройка планирования, выдаваемая как последняя реакция в шаге 3 выше, далее в этом документе называется "минимальной альтернативой".</span><span class="sxs-lookup"><span data-stu-id="ac768-123">The exceptional planning setup that is output as the last reaction in step 3 above is referred to in the following as the “minimal alternative”.</span></span> <span data-ttu-id="ac768-124">Эта настройка планирования охватывает только точное требование, все остальные параметры планирования игнорируются.</span><span class="sxs-lookup"><span data-stu-id="ac768-124">This planning setup only covers the exact demand, and all other planning parameters are ignored.</span></span>

<span data-ttu-id="ac768-125">Дополнительные сведения о вариантах данной логики планирования см. в разделе "Сценарии" ниже.</span><span class="sxs-lookup"><span data-stu-id="ac768-125">For information about variations of this planning logic, see the Scenarios section below.</span></span>

## <a name="demand-at-blank-location"></a><span data-ttu-id="ac768-126">Требование на пустом складе</span><span class="sxs-lookup"><span data-stu-id="ac768-126">Demand at Blank Location</span></span>
<span data-ttu-id="ac768-127">Даже если в поле **Склад обязателен** установлен флажок, программа допускает создание строк требования без кода склада — так называемый пустой склад.</span><span class="sxs-lookup"><span data-stu-id="ac768-127">Even if the **Location Mandatory** field is selected, the program will allow demand lines to be created without a location code, also referred to as blank location.</span></span> <span data-ttu-id="ac768-128">Это отклонение для системы, поскольку сюда включены значения различных параметров настройки, касающиеся складов (см. выше), и в результате модуль планирования не создаст строку планирования для такой строки спроса.</span><span class="sxs-lookup"><span data-stu-id="ac768-128">This is a deviation for the system because it has various setup values tuned to dealing with locations (see above) and as a result, the planning engine will not create a planning line for such a demand line.</span></span>

<span data-ttu-id="ac768-129">Если поле **Склад обязателен** не выбрано, но существует какое-либо из значений настройки склада, это также считается отклонением, и в ответ система планирования будет использовать "минимальную альтернативу", то есть планирование товара будет производиться с использованием следующих параметров: "Политика дозаказа" = "Партия-на-партию" (заказ остается заказом), "Вкл. наличие" = "Да", все прочие параметры планирования = "Пусто".</span><span class="sxs-lookup"><span data-stu-id="ac768-129">If the **Location Mandatory** field is not selected but any of the location setup values exist, it is also considered a deviation, and the planning system will react by using the “minimal alternative”: The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

## <a name="scenarios"></a><span data-ttu-id="ac768-130">Сценарии</span><span class="sxs-lookup"><span data-stu-id="ac768-130">Scenarios</span></span>
<span data-ttu-id="ac768-131">В следующем сценарии описываются изменения требования в пустом складе и как система планирования разрешается до "минимальной альтернативы".</span><span class="sxs-lookup"><span data-stu-id="ac768-131">The following scenarios describe variations of demand at blank location and how the planning system resolves to the “minimal alternative.”</span></span>

### <a name="setup-1"></a><span data-ttu-id="ac768-132">Настройка 1:</span><span class="sxs-lookup"><span data-stu-id="ac768-132">Setup 1:</span></span>
<span data-ttu-id="ac768-133">Код склада обязателен = Да</span><span class="sxs-lookup"><span data-stu-id="ac768-133">Location Mandatory = Yes</span></span>

<span data-ttu-id="ac768-134">Настройка единицы хранения — КРАСНЫЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-134">SKU is set up for RED</span></span>

<span data-ttu-id="ac768-135">Компоненты по складам = СИНИЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-135">Components at Location = BLUE</span></span>

#### <a name="case-11-demand-is-at-red-location"></a><span data-ttu-id="ac768-136">Случай 1.1: требование на складе КРАСНЫЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-136">Case 1.1: Demand is at RED location</span></span>
<span data-ttu-id="ac768-137">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке единицы хранения.</span><span class="sxs-lookup"><span data-stu-id="ac768-137">The item is planned according to planning parameters on the SKU card.</span></span>

#### <a name="case-12-demand-is-at-blue-location"></a><span data-ttu-id="ac768-138">Случай 1.2: требование на складе СИНИЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-138">Case 1.2: Demand is at BLUE location</span></span>
<span data-ttu-id="ac768-139">Планирование товара производится в соответствии со следующими параметрами: "Политика повторного заказа" = Партия-на-партию (заказ остается заказом)", Вкл. товар" = "Да, все прочие параметры планирования" = "Пусто".</span><span class="sxs-lookup"><span data-stu-id="ac768-139">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

#### <a name="case-13-demand-is-at-green-location"></a><span data-ttu-id="ac768-140">Случай 1.3: требование на складе ЗЕЛЕНЫЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-140">Case 1.3: Demand is at GREEN location</span></span>
<span data-ttu-id="ac768-141">Планирование товара производится в соответствии со следующими параметрами: "Политика повторного заказа" = Партия-на-партию (заказ остается заказом)", Вкл. товар" = "Да, все прочие параметры планирования" = "Пусто".</span><span class="sxs-lookup"><span data-stu-id="ac768-141">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

#### <a name="case-14-demand-is-at-blank-location"></a><span data-ttu-id="ac768-142">Случай 1.4: требование на ПУСТОМ складе</span><span class="sxs-lookup"><span data-stu-id="ac768-142">Case 1.4: Demand is at BLANK location</span></span>
<span data-ttu-id="ac768-143">Планирование товара не производится, поскольку в строке требования не задан склад.</span><span class="sxs-lookup"><span data-stu-id="ac768-143">The item is not planned because no location is defined on the demand line.</span></span>

### <a name="setup-2"></a><span data-ttu-id="ac768-144">Настройка 2:</span><span class="sxs-lookup"><span data-stu-id="ac768-144">Setup 2:</span></span>
<span data-ttu-id="ac768-145">Код склада обязателен = Да</span><span class="sxs-lookup"><span data-stu-id="ac768-145">Location Mandatory = Yes</span></span>

<span data-ttu-id="ac768-146">Единица хранения не существует</span><span class="sxs-lookup"><span data-stu-id="ac768-146">No SKU exists</span></span>

<span data-ttu-id="ac768-147">Компоненты по складам = СИНИЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-147">Components at Location = BLUE</span></span>

#### <a name="case-21-demand-is-at-red-location"></a><span data-ttu-id="ac768-148">Случай 2.1: требование на складе КРАСНЫЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-148">Case 2.1: Demand is at RED location</span></span>
<span data-ttu-id="ac768-149">Планирование товара производится в соответствии со следующими параметрами: "Политика повторного заказа" = Партия-на-партию (заказ остается заказом)", Вкл. товар" = "Да, все прочие параметры планирования" = "Пусто".</span><span class="sxs-lookup"><span data-stu-id="ac768-149">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

#### <a name="case-22-demand-is-at-blue-location"></a><span data-ttu-id="ac768-150">Случай 2.2: требование на складе СИНИЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-150">Case 2.2: Demand is at BLUE location</span></span>
<span data-ttu-id="ac768-151">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке товара.</span><span class="sxs-lookup"><span data-stu-id="ac768-151">The item is planned according to planning parameters on the item card.</span></span>

### <a name="setup-3"></a><span data-ttu-id="ac768-152">Настройка 3:</span><span class="sxs-lookup"><span data-stu-id="ac768-152">Setup 3:</span></span>
<span data-ttu-id="ac768-153">Код склада обязателен = Нет</span><span class="sxs-lookup"><span data-stu-id="ac768-153">Location Mandatory = No</span></span>

<span data-ttu-id="ac768-154">Единица хранения не существует</span><span class="sxs-lookup"><span data-stu-id="ac768-154">No SKU exists</span></span>

<span data-ttu-id="ac768-155">Компоненты по складам = СИНИЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-155">Components at Location = BLUE</span></span>

#### <a name="case-31-demand-is-at-red-location"></a><span data-ttu-id="ac768-156">Случай 3.1: требование на складе КРАСНЫЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-156">Case 3.1: Demand is at RED location</span></span>
<span data-ttu-id="ac768-157">Планирование товара производится в соответствии со следующими параметрами: "Политика повторного заказа" = Партия-на-партию (заказ остается заказом)", Вкл. товар" = "Да, все прочие параметры планирования" = "Пусто".</span><span class="sxs-lookup"><span data-stu-id="ac768-157">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

#### <a name="case-32-demand-is-at-blue-location"></a><span data-ttu-id="ac768-158">Случай 3.2: требование на складе СИНИЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-158">Case 3.2: Demand is at BLUE location</span></span>
<span data-ttu-id="ac768-159">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке товара.</span><span class="sxs-lookup"><span data-stu-id="ac768-159">The item is planned according to planning parameters on the item card.</span></span>

#### <a name="case-33-demand-is-at-blank-location"></a><span data-ttu-id="ac768-160">Случай 3.3: требование на ПУСТОМ складе</span><span class="sxs-lookup"><span data-stu-id="ac768-160">Case 3.3: Demand is at BLANK location</span></span>
<span data-ttu-id="ac768-161">Планирование товара производится в соответствии со следующими параметрами: "Политика повторного заказа" = Партия-на-партию (заказ остается заказом)", Вкл. товар" = "Да, все прочие параметры планирования" = "Пусто".</span><span class="sxs-lookup"><span data-stu-id="ac768-161">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

### <a name="setup-4"></a><span data-ttu-id="ac768-162">Настройка 4:</span><span class="sxs-lookup"><span data-stu-id="ac768-162">Setup 4:</span></span>
<span data-ttu-id="ac768-163">Код склада обязателен = Нет</span><span class="sxs-lookup"><span data-stu-id="ac768-163">Location Mandatory = No</span></span>

<span data-ttu-id="ac768-164">Единица хранения не существует</span><span class="sxs-lookup"><span data-stu-id="ac768-164">No SKU exists</span></span>

<span data-ttu-id="ac768-165">Компоненты по складам = ПУСТОЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-165">Components at Location = BLANK</span></span>

#### <a name="case-41-demand-is-at-blue-location"></a><span data-ttu-id="ac768-166">Случай 4.1: требование на складе СИНИЙ</span><span class="sxs-lookup"><span data-stu-id="ac768-166">Case 4.1: Demand is at BLUE location</span></span>
<span data-ttu-id="ac768-167">Планирование товара производится в соответствии со следующими параметрами: "Политика повторного заказа" = Партия-на-партию (заказ остается заказом)", Вкл. товар" = "Да, все прочие параметры планирования" = "Пусто".</span><span class="sxs-lookup"><span data-stu-id="ac768-167">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

#### <a name="case-42-demand-is-at-blank-location"></a><span data-ttu-id="ac768-168">Случай 4.2: требование на ПУСТОМ складе</span><span class="sxs-lookup"><span data-stu-id="ac768-168">Case 4.2: Demand is at BLANK location</span></span>
<span data-ttu-id="ac768-169">Планирование товара производится в соответствии с параметрами планирования, указанными в карточке товара.</span><span class="sxs-lookup"><span data-stu-id="ac768-169">The item is planned according to planning parameters on the item card.</span></span>

<span data-ttu-id="ac768-170">Как показано в последнем сценарии, единственный способ получить правильный результат для строки требования без кода склада — это отключить все значения настройки, относящиеся к складам.</span><span class="sxs-lookup"><span data-stu-id="ac768-170">As illustrated in the last scenario, the only way to get a correct result for a demand line without a location code is to disable all setup values relating to locations.</span></span> <span data-ttu-id="ac768-171">Кроме того, единственным способом получить стабильные результаты планирования для требований на складах является использование единиц хранения.</span><span class="sxs-lookup"><span data-stu-id="ac768-171">Similarly, the only way to get stable planning results for demand at locations is to use SKUs.</span></span> <span data-ttu-id="ac768-172">Следовательно, если организации часто проводят планирование требований на складах, рекомендуется использовать область "Единицы хранения".</span><span class="sxs-lookup"><span data-stu-id="ac768-172">Therefore, if companies often plan for demand at locations, they are strongly advised to use the Stockkeeping Units granule.</span></span>

## <a name="see-also"></a><span data-ttu-id="ac768-173">См. также</span><span class="sxs-lookup"><span data-stu-id="ac768-173">See Also</span></span>  
<span data-ttu-id="ac768-174">[Сведения о проектировании: балансировка спроса и поставки](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="ac768-174">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="ac768-175">[Сведения о проектировании: основные понятия системы планирования](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="ac768-175">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="ac768-176">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="ac768-176">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]