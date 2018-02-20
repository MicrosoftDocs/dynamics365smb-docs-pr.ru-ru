---
title: "Сведения о проектировании — максимальное количество | Документы Майкрософт"
description: "Политика максимального количества — это способ ведения запасов с использованием точки повтора заказа."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 26bed0b8832d5b12ce5d697df8ec6194ac7ae9b2
ms.contentlocale: ru-ru
ms.lasthandoff: 12/14/2017

---
# <a name="design-details-maximum-qty"></a><span data-ttu-id="1ca8b-103">Сведения о проектировании: максимальное количество</span><span class="sxs-lookup"><span data-stu-id="1ca8b-103">Design Details: Maximum Qty.</span></span>
<span data-ttu-id="1ca8b-104">Политика максимального количества — это способ ведения запасов с использованием точки повтора заказа.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-104">The Maximum Quantity policy is a way to maintain inventory using a reorder point.</span></span>  
  
 <span data-ttu-id="1ca8b-105">Все, что имеет отношение к политике "Фикс. кол-во дозаказа", также применяется к этой политике.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-105">Everything regarding the Fixed Reorder Qty. policy also applies to this policy.</span></span> <span data-ttu-id="1ca8b-106">Единственное отличие — в количестве предлагаемой поставки.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-106">The only difference is the quantity of the suggested supply.</span></span> <span data-ttu-id="1ca8b-107">При использовании политики максимального количества, количество повторного заказа определяется динамически с учетом прогнозируемого уровня запасов. Как правило, от заказа к заказу это количество различается.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-107">When using the maximum quantity policy, the reorder quantity will be defined dynamically based on the projected inventory level and will therefore usually differ from order to order.</span></span>  
  
## <a name="calculated-per-time-bucket"></a><span data-ttu-id="1ca8b-108">Расчет на горизонт планирования</span><span class="sxs-lookup"><span data-stu-id="1ca8b-108">Calculated per Time Bucket</span></span>  
 <span data-ttu-id="1ca8b-109">Количество повторного заказа определяется в момент времени (в конце горизонта планирования), когда система планирования обнаружит, что точка повторного заказа пройдена.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-109">The reorder quantity is determined at the point of time (the end of a time bucket) when the planning system detects that the reorder point has been crossed.</span></span> <span data-ttu-id="1ca8b-110">В этот момент система измеряет разницу между текущим прогнозируемым уровнем запасов и указанным максимальным запасом.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-110">At this time, the system measures the gap from the current projected inventory level up to the specified maximum inventory.</span></span> <span data-ttu-id="1ca8b-111">Этот представляет количество, которое подлежит дозаказу.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-111">This constitutes the quantity that should be reordered.</span></span> <span data-ttu-id="1ca8b-112">Система затем проверяет, была ли поставка заказана где-либо еще для получения в течение времени подготовки и если да, то уменьшает количество нового заказа на поставку на уже заказанное количество.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-112">The system then checks if supply has already been ordered elsewhere to be received within the lead time and, if so, reduces the quantity of the new supply order by already ordered quantities.</span></span>  
  
 <span data-ttu-id="1ca8b-113">Система обеспечит, что планированные запасы хотя бы достигнут точки повторного заказа на случай, если пользователь забудет указать максимальное количество запасов.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-113">The system will ensure that the projected inventory at least reaches the reorder point level – in case the user has forgotten to specify a maximum inventory quantity.</span></span>  
  
## <a name="combines-with-order-modifiers"></a><span data-ttu-id="1ca8b-114">Объединение с модификаторами заказа</span><span class="sxs-lookup"><span data-stu-id="1ca8b-114">Combines with Order Modifiers</span></span>  
 <span data-ttu-id="1ca8b-115">В зависимости от настройки может иметь смысл объединить политику максимального количества с модификаторами заказов для обеспечения минимального количества заказа, его округления до целого числа единиц измерения покупки или разделения на несколько партий в соответствии с максимальным количеством заказа.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-115">Depending on the setup, it may be best to combine the Maximum Quantity policy with order modifiers to ensure a minimum order quantity or round it to an integer number of purchase units of measure, or split it into more lots as defined by the maximum order quantity.</span></span>  
  
## <a name="combines-with-calendars"></a><span data-ttu-id="1ca8b-116">Объединение с календарями</span><span class="sxs-lookup"><span data-stu-id="1ca8b-116">Combines with Calendars</span></span>  
 <span data-ttu-id="1ca8b-117">Перед тем как предложить новый заказ на поставку для соответствия точке дозаказа, система планирования проверяет, запланирован ли заказ на нерабочий день, согласно всем календарям, определенным в поле **Код базового календаря** в окнах **Информация об организации** и **Карточка склада**.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-117">Before suggesting a new supply order to meet a reorder point, the planning system checks if the order is scheduled for a non-working day, according to any calendars that are  defined in the **Base Calendar Code** field in the **Company Information** and **Location Card** windows.</span></span>  
  
 <span data-ttu-id="1ca8b-118">Если плановая дата является нерабочим днем, система планирования переместит заказ до ближайшей рабочей даты.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-118">If the scheduled date is a non-working day, the planning system moves the order forward to the nearest working date.</span></span> <span data-ttu-id="1ca8b-119">Это может привести к тому, что заказ достигнет точки повтора заказа, но не удовлетворит определенному спросу.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-119">This may result in an order that meets a reorder point but does not meet some specific demand.</span></span> <span data-ttu-id="1ca8b-120">Если такого несбалансированного спроса система планирования создает дополнительную поставку.</span><span class="sxs-lookup"><span data-stu-id="1ca8b-120">For such unbalanced demand, the planning system creates an extra supply.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="1ca8b-121">См. также</span><span class="sxs-lookup"><span data-stu-id="1ca8b-121">See Also</span></span>  
 <span data-ttu-id="1ca8b-122">[Сведения о проектировании: политики дозаказа](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="1ca8b-122">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="1ca8b-123">[Сведения о проектировании: параметры планирования](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="1ca8b-123">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="1ca8b-124">[Сведения о проектировании: обработка политик дозаказа](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="1ca8b-124">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="1ca8b-125">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="1ca8b-125">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
