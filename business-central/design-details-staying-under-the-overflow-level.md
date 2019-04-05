---
title: Сведения о проектировании — нахождение ниже уровня допустимого избытка | Документы Майкрософт
description: При использовании максимального количества и фиксированного количества повторного заказа система планирования концентрируется на прогнозируемых складских запасов исключительно в данном горизонте планирования. Это означает, что система планирования может предложить поставку с излишками, если происходят изменения отрицательного спроса или положительного предложения за пределами заданного горизонта планирования.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
redirect_url: design-details-handling-reordering-policies
ms.openlocfilehash: a4a35cec571f1a0c7644fe937553d87007a9567e
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "804664"
---
# <a name="design-details-staying-under-the-overflow-level"></a><span data-ttu-id="c840b-104">Сведения о проектировании: нахождение ниже уровня допустимого избытка</span><span class="sxs-lookup"><span data-stu-id="c840b-104">Design Details: Staying under the Overflow Level</span></span>
<span data-ttu-id="c840b-105">При использовании политик максимального количества и фиксированного количества повторного заказа система планирования концентрируется на прогнозируемых складских запасов исключительно в данном горизонте планирования.</span><span class="sxs-lookup"><span data-stu-id="c840b-105">When using the Maximum Qty. and Fixed Reorder Qty. policies, the planning system focuses on the projected inventory in the given time-bucket only.</span></span> <span data-ttu-id="c840b-106">Это означает, что система планирования может предложить поставку с излишками, если происходят изменения отрицательного спроса или положительного предложения за пределами заданного горизонта планирования.</span><span class="sxs-lookup"><span data-stu-id="c840b-106">This means that the planning system may suggest superfluous supply when negative demand or positive supply changes occur outside of the given time bucket.</span></span> <span data-ttu-id="c840b-107">Если, по этой причине предлагается излишняя поставка, система планирования вычисляет количество, на которое следует уменьшить поставку, чтобы избежать излишней поставки.</span><span class="sxs-lookup"><span data-stu-id="c840b-107">If, for this reason, a superfluous supply is suggested, the planning system calculates which quantity the supply should be decreased to (or deleted) to avoid the superfluous supply.</span></span> <span data-ttu-id="c840b-108">Это количество называется "допустимый избыток".</span><span class="sxs-lookup"><span data-stu-id="c840b-108">This quantity is called the “overflow level.”</span></span> <span data-ttu-id="c840b-109">Он передается как строка планирования с действием **Изменить кол-во (уменьшить)** или **Отмена** и следующим предупреждением.</span><span class="sxs-lookup"><span data-stu-id="c840b-109">The overflow is communicated as a planning line with a **Change Qty. (Decrease)** or **Cancel** action and the following warning message:</span></span>  

<span data-ttu-id="c840b-110">*Внимание! Прогнозируемые запасы [xx] больше, чем допустимый избыток [xx] на срок выполнения [xx].*</span><span class="sxs-lookup"><span data-stu-id="c840b-110">*Attention: The projected inventory [xx] is higher than the overflow level [xx] on the Due Date [xx].*</span></span>  

<span data-ttu-id="c840b-111">![Допустимый избыток запасов](media/supplyplanning_2_overflow1_new.png "Допустимый избыток запасов")</span><span class="sxs-lookup"><span data-stu-id="c840b-111">![Inventory overflow level](media/supplyplanning_2_overflow1_new.png "Inventory overflow level")</span></span>  

##  <a name="calculating-the-overflow-level"></a><span data-ttu-id="c840b-112">Расчет допустимого избытка</span><span class="sxs-lookup"><span data-stu-id="c840b-112">Calculating the Overflow Level</span></span>  
<span data-ttu-id="c840b-113">Допустимый избыток вычисляется разными способами в зависимости от настройки планирования.</span><span class="sxs-lookup"><span data-stu-id="c840b-113">The overflow level is calculated in different ways depending on planning setup.</span></span>  

### <a name="maximum-qty-reordering-policy"></a><span data-ttu-id="c840b-114">Политика дозаказа "Максимальное кол-во"</span><span class="sxs-lookup"><span data-stu-id="c840b-114">Maximum Qty. reordering policy</span></span>  
<span data-ttu-id="c840b-115">Допустимый избыток = Максимальный запас</span><span class="sxs-lookup"><span data-stu-id="c840b-115">Overflow level = Maximum Inventory</span></span>  

> [!NOTE]  
>  <span data-ttu-id="c840b-116">Если существует минимальное количество заказа, оно будет добавлено следующим образом: допустимый избыток = максимальный запас + минимальное количество заказа.</span><span class="sxs-lookup"><span data-stu-id="c840b-116">If a minimum order quantity exists, then it will be added as follows: Overflow level = Maximum Inventory + Minimum Order Quantity.</span></span>  

### <a name="fixed-reorder-qty-reordering-policy"></a><span data-ttu-id="c840b-117">Политика дозаказа "Фикс. кол-во дозаказа"</span><span class="sxs-lookup"><span data-stu-id="c840b-117">Fixed Reorder Qty. reordering policy</span></span>  
<span data-ttu-id="c840b-118">Допустимый избыток = кол-во для дозаказа + точка дозаказа</span><span class="sxs-lookup"><span data-stu-id="c840b-118">Overflow level = Reorder Quantity + Reorder Point</span></span>  

> [!NOTE]  
>  <span data-ttu-id="c840b-119">Если минимальное количество заказа выше точки дозаказа, оно заменяется следующим образом: допустимый избыток = количество дозаказа + минимальное количество заказа</span><span class="sxs-lookup"><span data-stu-id="c840b-119">If the minimum order quantity is higher than the reorder point, then it will replace as follows: Overflow Level = Reorder Quantity + Minimum Order Quantity</span></span>  

### <a name="order-multiple"></a><span data-ttu-id="c840b-120">Заказать несколько</span><span class="sxs-lookup"><span data-stu-id="c840b-120">Order Multiple</span></span>  
<span data-ttu-id="c840b-121">Если существует множитель заказа, он корректирует допустимый избыток для политик дозаказа "Максимальное кол-во" и "Фикс. кол-во дозаказа".</span><span class="sxs-lookup"><span data-stu-id="c840b-121">If an order multiple exists, then it will adjust the overflow level for both Maximum Qty. and Fixed Reorder Qty. reordering policies.</span></span>  

##  <a name="creating-the-planning-line-with-overflow-warning"></a><span data-ttu-id="c840b-122">Создание строки планирования с предупреждением о переполнении</span><span class="sxs-lookup"><span data-stu-id="c840b-122">Creating the Planning Line with Overflow Warning</span></span>  
<span data-ttu-id="c840b-123">Если из-за существующей поставки прогнозируемые запасы выше допустимого избытка по окончании горизонта планирования, создается строка планирования.</span><span class="sxs-lookup"><span data-stu-id="c840b-123">When an existing supply causes the projected inventory to be higher than the overflow level at the end of a time bucket, a planning line is created.</span></span> <span data-ttu-id="c840b-124">Чтобы предупредить о возможных излишках поставки, строка планирования содержит предупреждение, поле **Принять указание** не выбрано, а указание имеет значение "Отмена" или "Изменить кол-во".</span><span class="sxs-lookup"><span data-stu-id="c840b-124">To warn about the potential superfluous supply, the planning line has a warning message, the **Accept Action Message** field is not selected, and the action message is either Cancel or Change Qty.</span></span>  

### <a name="calculating-the-planning-line-quantity"></a><span data-ttu-id="c840b-125">Расчет количества строки планирования</span><span class="sxs-lookup"><span data-stu-id="c840b-125">Calculating the Planning Line Quantity</span></span>  
<span data-ttu-id="c840b-126">Количество строки планирования = текущее количество поставки - (ожидаемые запасы - допустимый избыток)</span><span class="sxs-lookup"><span data-stu-id="c840b-126">Planning Line Quantity = Current Supply Quantity – (Projected Inventory – Overflow Level)</span></span>  

> [!NOTE]  
>  <span data-ttu-id="c840b-127">Как и во всех строках предупреждений любое максимальное/минимальное количество заказа или множитель заказа будут игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="c840b-127">As with all warning lines, any maximum/minimum order quantity or order multiple will be ignored.</span></span>  

### <a name="defining-the-action-message-type"></a><span data-ttu-id="c840b-128">Определение типа сообщения о действии</span><span class="sxs-lookup"><span data-stu-id="c840b-128">Defining the Action Message Type</span></span>  

-   <span data-ttu-id="c840b-129">Если количество в строке планирования выше или равно 0, отображается сообщение о действии "Изменить кол-во".</span><span class="sxs-lookup"><span data-stu-id="c840b-129">If the planning line quantity is higher than 0, then the action message is Change Qty.</span></span>  
-   <span data-ttu-id="c840b-130">Если количество в строке планирования ниже или равно 0, отображается сообщение о действии "Отмена".</span><span class="sxs-lookup"><span data-stu-id="c840b-130">If the planning line quantity is equal to or lower than 0, then the action message is Cancel</span></span>  

### <a name="composing-the-warning-message"></a><span data-ttu-id="c840b-131">Создание предупреждающего сообщения</span><span class="sxs-lookup"><span data-stu-id="c840b-131">Composing the Warning Message</span></span>  
<span data-ttu-id="c840b-132">В случае избытка на странице **Нетрассируемые элементы планирования** отображается предупреждающее сообщение со следующими сведениями:</span><span class="sxs-lookup"><span data-stu-id="c840b-132">In case of overflow, the **Untracked Planning Elements** page displays a warning message with the following information:</span></span>  

-   <span data-ttu-id="c840b-133">Прогнозируемый уровень запасов, инициировавший предупреждение</span><span class="sxs-lookup"><span data-stu-id="c840b-133">The projected inventory level that triggered the warning</span></span>  
-   <span data-ttu-id="c840b-134">Вычисленный допустимый избыток</span><span class="sxs-lookup"><span data-stu-id="c840b-134">The calculated overflow level</span></span>  
-   <span data-ttu-id="c840b-135">Дата оплаты события предложения.</span><span class="sxs-lookup"><span data-stu-id="c840b-135">The due date of the supply event.</span></span>  

<span data-ttu-id="c840b-136">Пример. Прогнозируемые запасы 120 больше, чем допустимый избыток 60 в 28-01-11</span><span class="sxs-lookup"><span data-stu-id="c840b-136">Example: “The projected inventory 120 is higher than the overflow level 60 on 28-01-11”</span></span>  

## <a name="scenario"></a><span data-ttu-id="c840b-137">Сценарий</span><span class="sxs-lookup"><span data-stu-id="c840b-137">Scenario</span></span>  
<span data-ttu-id="c840b-138">В этом сценарии клиент меняет количество заказа на продажу с 70 на 40 штук в период между двумя процессами планирования.</span><span class="sxs-lookup"><span data-stu-id="c840b-138">In this scenario, a customer changes a sales order from 70 to 40 pieces between two planning runs.</span></span> <span data-ttu-id="c840b-139">Функция переполнения устанавливается для уменьшения покупки, которая была предложена для первоначального количества продаж.</span><span class="sxs-lookup"><span data-stu-id="c840b-139">The overflow feature sets in to reduce the purchase that was suggested for the initial sales quantity.</span></span>  

### <a name="item-setup"></a><span data-ttu-id="c840b-140">Настройка товара</span><span class="sxs-lookup"><span data-stu-id="c840b-140">Item setup</span></span>  

|<span data-ttu-id="c840b-141">Политика повтора заказа</span><span class="sxs-lookup"><span data-stu-id="c840b-141">Reordering Policy</span></span>|<span data-ttu-id="c840b-142">Максимальное кол-во</span><span class="sxs-lookup"><span data-stu-id="c840b-142">Maximum Qty.</span></span>|  
|-----------------------|------------------|  
|<span data-ttu-id="c840b-143">Максимальное количество заказа</span><span class="sxs-lookup"><span data-stu-id="c840b-143">Maximum Order Quantity</span></span>|<span data-ttu-id="c840b-144">100</span><span class="sxs-lookup"><span data-stu-id="c840b-144">100</span></span>|  
|<span data-ttu-id="c840b-145">Точка повтора заказа</span><span class="sxs-lookup"><span data-stu-id="c840b-145">Reorder Point</span></span>|<span data-ttu-id="c840b-146">50</span><span class="sxs-lookup"><span data-stu-id="c840b-146">50</span></span>|  
|<span data-ttu-id="c840b-147">Запасы</span><span class="sxs-lookup"><span data-stu-id="c840b-147">Inventory</span></span>|<span data-ttu-id="c840b-148">80</span><span class="sxs-lookup"><span data-stu-id="c840b-148">80</span></span>|  

### <a name="situation-before-sales-decrease"></a><span data-ttu-id="c840b-149">Ситуация до снижения продаж</span><span class="sxs-lookup"><span data-stu-id="c840b-149">Situation before sales decrease</span></span>  

|<span data-ttu-id="c840b-150">Событие</span><span class="sxs-lookup"><span data-stu-id="c840b-150">Event</span></span>|<span data-ttu-id="c840b-151">Изменить кол-во</span><span class="sxs-lookup"><span data-stu-id="c840b-151">Change Qty.</span></span>|<span data-ttu-id="c840b-152">Ожидаемые запасы</span><span class="sxs-lookup"><span data-stu-id="c840b-152">Projected Inventory</span></span>|  
|-----------|-----------------|-------------------------|  
|<span data-ttu-id="c840b-153">День первый</span><span class="sxs-lookup"><span data-stu-id="c840b-153">Day one</span></span>|<span data-ttu-id="c840b-154">Нет</span><span class="sxs-lookup"><span data-stu-id="c840b-154">None</span></span>|<span data-ttu-id="c840b-155">80</span><span class="sxs-lookup"><span data-stu-id="c840b-155">80</span></span>|  
|<span data-ttu-id="c840b-156">Продажа</span><span class="sxs-lookup"><span data-stu-id="c840b-156">Sale</span></span>|<span data-ttu-id="c840b-157">-70</span><span class="sxs-lookup"><span data-stu-id="c840b-157">-70</span></span>|<span data-ttu-id="c840b-158">10</span><span class="sxs-lookup"><span data-stu-id="c840b-158">10</span></span>|  
|<span data-ttu-id="c840b-159">Конец горизонта планирования</span><span class="sxs-lookup"><span data-stu-id="c840b-159">End of time bucket</span></span>|<span data-ttu-id="c840b-160">Нет</span><span class="sxs-lookup"><span data-stu-id="c840b-160">None</span></span>|<span data-ttu-id="c840b-161">10</span><span class="sxs-lookup"><span data-stu-id="c840b-161">10</span></span>|  
|<span data-ttu-id="c840b-162">Предложение нового возврата покупки</span><span class="sxs-lookup"><span data-stu-id="c840b-162">Suggest new purchase order</span></span>|<span data-ttu-id="c840b-163">+90</span><span class="sxs-lookup"><span data-stu-id="c840b-163">+90</span></span>|<span data-ttu-id="c840b-164">100</span><span class="sxs-lookup"><span data-stu-id="c840b-164">100</span></span>|  

### <a name="situation-after-sales-decrease"></a><span data-ttu-id="c840b-165">Ситуация после снижения продаж</span><span class="sxs-lookup"><span data-stu-id="c840b-165">Situation after sales decrease</span></span>  

|<span data-ttu-id="c840b-166">Изменение</span><span class="sxs-lookup"><span data-stu-id="c840b-166">Change</span></span>|<span data-ttu-id="c840b-167">Изменить кол-во</span><span class="sxs-lookup"><span data-stu-id="c840b-167">Change Qty.</span></span>|<span data-ttu-id="c840b-168">Ожидаемые запасы</span><span class="sxs-lookup"><span data-stu-id="c840b-168">Projected Inventory</span></span>|  
|------------|-----------------|-------------------------|  
|<span data-ttu-id="c840b-169">День первый</span><span class="sxs-lookup"><span data-stu-id="c840b-169">Day one</span></span>|<span data-ttu-id="c840b-170">Нет</span><span class="sxs-lookup"><span data-stu-id="c840b-170">None</span></span>|<span data-ttu-id="c840b-171">80</span><span class="sxs-lookup"><span data-stu-id="c840b-171">80</span></span>|  
|<span data-ttu-id="c840b-172">Продажа</span><span class="sxs-lookup"><span data-stu-id="c840b-172">Sale</span></span>|<span data-ttu-id="c840b-173">-40</span><span class="sxs-lookup"><span data-stu-id="c840b-173">-40</span></span>|<span data-ttu-id="c840b-174">40</span><span class="sxs-lookup"><span data-stu-id="c840b-174">40</span></span>|  
|<span data-ttu-id="c840b-175">Покупка</span><span class="sxs-lookup"><span data-stu-id="c840b-175">Purchase</span></span>|<span data-ttu-id="c840b-176">+90</span><span class="sxs-lookup"><span data-stu-id="c840b-176">+90</span></span>|<span data-ttu-id="c840b-177">130</span><span class="sxs-lookup"><span data-stu-id="c840b-177">130</span></span>|  
|<span data-ttu-id="c840b-178">Конец горизонта планирования</span><span class="sxs-lookup"><span data-stu-id="c840b-178">End of time bucket</span></span>|<span data-ttu-id="c840b-179">Нет</span><span class="sxs-lookup"><span data-stu-id="c840b-179">None</span></span>|<span data-ttu-id="c840b-180">130</span><span class="sxs-lookup"><span data-stu-id="c840b-180">130</span></span>|  
|<span data-ttu-id="c840b-181">Предложение по уменьшению количества покупки</span><span class="sxs-lookup"><span data-stu-id="c840b-181">Suggest to decrease purchase</span></span><br /><br /> <span data-ttu-id="c840b-182">заказ с 90 до 60</span><span class="sxs-lookup"><span data-stu-id="c840b-182">order from 90 to 60</span></span>|<span data-ttu-id="c840b-183">-30</span><span class="sxs-lookup"><span data-stu-id="c840b-183">-30</span></span>|<span data-ttu-id="c840b-184">100</span><span class="sxs-lookup"><span data-stu-id="c840b-184">100</span></span>|  

### <a name="resulting-planning-lines"></a><span data-ttu-id="c840b-185">Результирующие строки планирования</span><span class="sxs-lookup"><span data-stu-id="c840b-185">Resulting Planning Lines</span></span>  
 <span data-ttu-id="c840b-186">Создается одна строка планирования (предупреждение) для уменьшения количества покупки 30 с 90 до 60 для соответствия прогнозируемых запасов 100 допустимому избытку.</span><span class="sxs-lookup"><span data-stu-id="c840b-186">One planning line (warning) is created to reduce the purchase with 30 from 90 to 60 to keep the projected inventory on 100 according to the overflow level.</span></span>  

<span data-ttu-id="c840b-187">![Планирование в соответствии с допустимым избытком](media/nav_app_supply_planning_2_overflow2.png "Планирование в соответствии с допустимым избытком")</span><span class="sxs-lookup"><span data-stu-id="c840b-187">![Plan according to overflow level](media/nav_app_supply_planning_2_overflow2.png "Plan according to overflow level")</span></span>  

> [!NOTE]  
>  <span data-ttu-id="c840b-188">Без функции допустимого избытка никаких предупреждений не создается, если прогнозируемый уровень склада выше максимальных запасов.</span><span class="sxs-lookup"><span data-stu-id="c840b-188">Without the Overflow feature, no warning is created if the projected inventory level is above maximum inventory.</span></span> <span data-ttu-id="c840b-189">Это может вызвать поставку с излишками в количестве 30.</span><span class="sxs-lookup"><span data-stu-id="c840b-189">This could cause a superfluous supply of 30.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c840b-190">См. также</span><span class="sxs-lookup"><span data-stu-id="c840b-190">See Also</span></span>  
<span data-ttu-id="c840b-191">[Сведения о проектировании: политики дозаказа](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="c840b-191">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="c840b-192">[Сведения о проектировании: параметры планирования](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="c840b-192">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="c840b-193">[Сведения о проектировании: обработка политик дозаказа](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="c840b-193">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="c840b-194">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="c840b-194">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
