---
title: Сведения о проектировании — обработка прогнозируемых отрицательных остатков | Документы Майкрософт
description: Точка повторного заказа выражает предполагаемый спрос во время подготовки товара. Когда точка дозаказа пройдена, нужно заказывать еще. Однако прогнозируемые запасы должны быть достаточно большими для того, чтобы удовлетворить спрос до получения нового заказа. В то же время страховой запас должен устранить колебания в спросе и увеличить количество до целевого уровня обслуживания.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: design-details-handling-reordering-policies
ms.openlocfilehash: a0ecfe62e70c434ecfd6d698424e20119be13554
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1246436"
---
# <a name="design-details-handling-projected-negative-inventory"></a><span data-ttu-id="a85f2-106">Сведения о проектировании: обработка прогнозируемых отрицательных остатков</span><span class="sxs-lookup"><span data-stu-id="a85f2-106">Design Details: Handling Projected Negative Inventory</span></span>
<span data-ttu-id="a85f2-107">Точка повторного заказа выражает предполагаемый спрос во время подготовки товара.</span><span class="sxs-lookup"><span data-stu-id="a85f2-107">The reorder point expresses the anticipated demand during the lead time of the item.</span></span> <span data-ttu-id="a85f2-108">Когда точка дозаказа пройдена, нужно заказывать еще.</span><span class="sxs-lookup"><span data-stu-id="a85f2-108">When the reorder point is passed, it is time to order more.</span></span> <span data-ttu-id="a85f2-109">Однако прогнозируемые запасы должны быть достаточно большими для того, чтобы удовлетворить спрос до получения нового заказа.</span><span class="sxs-lookup"><span data-stu-id="a85f2-109">But the projected inventory must be large enough to cover the demand until the new order is received.</span></span> <span data-ttu-id="a85f2-110">В то же время страховой запас должен устранить колебания в спросе и увеличить количество до целевого уровня обслуживания.</span><span class="sxs-lookup"><span data-stu-id="a85f2-110">Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.</span></span>  

 <span data-ttu-id="a85f2-111">Следовательно, система планирования считает, что возникла чрезвычайная ситуация, если будущий спрос невозможно удовлетворить из прогнозируемых запасов, или, иными словами, если прогнозируемые запасы становятся отрицательными.</span><span class="sxs-lookup"><span data-stu-id="a85f2-111">Consequently, the planning system considers it an emergency if a future demand cannot be served from the projected inventory, or expressed in another way, that the projected inventory goes negative.</span></span> <span data-ttu-id="a85f2-112">Система обрабатывает такое исключение, предлагая новый заказ на поставку, чтобы покрыть часть спроса, который не может быть покрыт поставкой со склада или другой поставкой.</span><span class="sxs-lookup"><span data-stu-id="a85f2-112">The system deals with such an exception by suggesting a new supply order to meet the part of the demand that cannot be met by inventory or other supply.</span></span> <span data-ttu-id="a85f2-113">Размер нового заказа на поставку не учитывает максимальные запасы или количество повторного запаса, а также модификаторы заказа, такие как "максимальное кол-во заказа", "минимальное кол-во заказа" и "заказать несколько".</span><span class="sxs-lookup"><span data-stu-id="a85f2-113">The order size of the new supply order will not take the maximum inventory or the reorder quantity into consideration, nor will it take into consideration the order modifiers Maximum Order Quantity, Minimum Order Quantity, and Order Multiple.</span></span> <span data-ttu-id="a85f2-114">Вместо этого будет отражен точный дефицит.</span><span class="sxs-lookup"><span data-stu-id="a85f2-114">Instead, it will reflect the exact deficiency.</span></span>  

 <span data-ttu-id="a85f2-115">Строка планирования для этого типа заказов на поставку отобразит предупреждающий значок аварийной ситуации с возможностью просмотра пользователем дополнительных сведений для прояснения ситуации.</span><span class="sxs-lookup"><span data-stu-id="a85f2-115">The planning line for this type of supply order will display an Emergency warning icon, and additional information will be provided upon lookup to inform the user of the situation.</span></span>  

 <span data-ttu-id="a85f2-116">На следующем рисунке поставка D представляет экстренный заказ для коррекции отрицательных остатков.</span><span class="sxs-lookup"><span data-stu-id="a85f2-116">In the following illustration, supply D represents an emergency order to adjust for negative inventory.</span></span>  

 <span data-ttu-id="a85f2-117">![Предложение экстренного планирования для предотвращения отрицательных остатков](media/nav_app_supply_planning_2_negative_inventory.png "Предложение экстренного планирования для предотвращения отрицательных остатков")</span><span class="sxs-lookup"><span data-stu-id="a85f2-117">![Emergency planning suggestion to avoid negative inventory](media/nav_app_supply_planning_2_negative_inventory.png "Emergency planning suggestion to avoid negative inventory")</span></span>  

1.  <span data-ttu-id="a85f2-118">Поставка **A** (изначально прогнозируемые запасы) ниже точки дозаказа.</span><span class="sxs-lookup"><span data-stu-id="a85f2-118">Supply **A**, initial projected inventory, is below reorder point.</span></span>  
2.  <span data-ttu-id="a85f2-119">Создана новая поставка с прямым планированием (**C**).</span><span class="sxs-lookup"><span data-stu-id="a85f2-119">A new forward-scheduled supply is created (**C**).</span></span>  

     <span data-ttu-id="a85f2-120">(Количество = максимальный запас - уровень прогнозируемых запасов)</span><span class="sxs-lookup"><span data-stu-id="a85f2-120">(Quantity = Maximum Inventory – Projected Inventory Level)</span></span>  
3.  <span data-ttu-id="a85f2-121">Поставка **A** закрыта спросом **B**, который удовлетворен в полном размере.</span><span class="sxs-lookup"><span data-stu-id="a85f2-121">Supply **A** is closed by demand **B**, which is not fully covered.</span></span>  

     <span data-ttu-id="a85f2-122">(В соответствии со спросом **B** можно попытаться запланировать поставку C, однако это будет невозможно согласно понятию "горизонт планирования".)</span><span class="sxs-lookup"><span data-stu-id="a85f2-122">(Demand **B** could try to schedule Supply C in but that will not happen according to the time-bucket concept.)</span></span>  
4.  <span data-ttu-id="a85f2-123">Создается новая поставка (**D**) для покрытия оставшегося количества в спросе **B**.</span><span class="sxs-lookup"><span data-stu-id="a85f2-123">New supply (**D**) is created to cover the remaining quantity on Demand **B**.</span></span>  
5.  <span data-ttu-id="a85f2-124">Спрос **B** закрыт (создание напоминания для прогнозируемых запасов).</span><span class="sxs-lookup"><span data-stu-id="a85f2-124">Demand **B** is closed (creating a reminder to the projected inventory).</span></span>  
6.  <span data-ttu-id="a85f2-125">Новая заявка **D** закрыта.</span><span class="sxs-lookup"><span data-stu-id="a85f2-125">The new supply **D** is closed.</span></span>  
7.  <span data-ttu-id="a85f2-126">Ожидаемые запасы проверены; точка дозаказа не пересечена.</span><span class="sxs-lookup"><span data-stu-id="a85f2-126">Projected Inventory is checked; reorder point has not been crossed.</span></span>  
8.  <span data-ttu-id="a85f2-127">Поставка **C** закрыта (спрос больше не существует).</span><span class="sxs-lookup"><span data-stu-id="a85f2-127">Supply **C** is closed (no more demand exists).</span></span>  
9. <span data-ttu-id="a85f2-128">Окончательная проверка: необработанных напоминаний об уровне запасов не существует.</span><span class="sxs-lookup"><span data-stu-id="a85f2-128">Final check: No outstanding inventory level reminders exist.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="a85f2-129">Шаг 4 демонстрирует поведение системы в версиях до Microsoft Dynamics NAV 2009 SP1.</span><span class="sxs-lookup"><span data-stu-id="a85f2-129">Step 4 reflects how the system reacts in versions earlier than Microsoft Dynamics NAV 2009 SP1.</span></span>  

 <span data-ttu-id="a85f2-130">Это завершает описание основных принципов, связанных с планированием запасов на основе политик повторных заказов.</span><span class="sxs-lookup"><span data-stu-id="a85f2-130">This concludes the description of central principles relating to inventory planning based on reordering policies.</span></span> <span data-ttu-id="a85f2-131">В следующем разделе описываются характеристики четырех поддерживаемых политик повторного заказа.</span><span class="sxs-lookup"><span data-stu-id="a85f2-131">The following section describes the characteristics of the four supported reordering policies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a85f2-132">См. также</span><span class="sxs-lookup"><span data-stu-id="a85f2-132">See Also</span></span>  
 <span data-ttu-id="a85f2-133">[Сведения о проектировании: политики дозаказа](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="a85f2-133">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="a85f2-134">[Сведения о проектировании: параметры планирования](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="a85f2-134">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="a85f2-135">[Сведения о проектировании: обработка политик дозаказа](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="a85f2-135">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="a85f2-136">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="a85f2-136">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
