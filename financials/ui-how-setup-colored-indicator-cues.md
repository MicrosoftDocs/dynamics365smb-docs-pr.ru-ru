---
title: "Настройка цветных индикаторов, чтобы задать визуальные обозначения действий очереди | Документы Майкрософт"
description: "Настраивайте цветные индикаторы на плитке очереди, чтобы установить индивидуальные обозначения действий очереди."
services: project-madeira
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: personalize, customize
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 0cb10770954f485d9c0a3474615e6c69411de321
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a><span data-ttu-id="63019-103">Практическое руководство. Настройка цветного индикатора в очередях</span><span class="sxs-lookup"><span data-stu-id="63019-103">How to: Set Up a Colored Indicator on Cues</span></span>
<span data-ttu-id="63019-104">Вы можете настроить очереди, отображаемые на странице **Главная**, чтобы включить индикатор, меняющий цвет в зависимости от значений данных в очередях.</span><span class="sxs-lookup"><span data-stu-id="63019-104">You can set up Cues that appear on the **Home** page to include an indicator that changes color based on the data values in the Cues.</span></span>

<span data-ttu-id="63019-105">Индикатор отображается как цветная полоса вдоль верхней границы плитки очереди.</span><span class="sxs-lookup"><span data-stu-id="63019-105">The indicator appears as a colored bar along the top border of the Cue tile.</span></span> <span data-ttu-id="63019-106">Предоставляет визуальный сигнал статуса операций очереди, который может указывать на благоприятные или неблагоприятные условия и необходимость действий пользователя.</span><span class="sxs-lookup"><span data-stu-id="63019-106">It provides a visual signal of the status of the Cue's activity, which can indicate favorable or unfavorable conditions to prompt the user to take action.</span></span> <span data-ttu-id="63019-107">Например, если в очереди отображаются текущие счета продажи, можно настроить, чтобы индикатор отображался зеленым (положительный), если общее число текущих счетов продажи меньше 10, и красным (отрицательный), если это число больше 20.</span><span class="sxs-lookup"><span data-stu-id="63019-107">For example, if a Cue displays ongoing sales invoices, you can set up the indicator to appear green (favorable) when total number of ongoing sales invoices is below 10, and appears red (unfavorable) when the total is greater than 20.</span></span>

<span data-ttu-id="63019-108">В окне **Настройка очереди** можно настроить индикаторы для всех очередей, доступных в базе данных организации.</span><span class="sxs-lookup"><span data-stu-id="63019-108">From the **Cue Setup** window, you set up indicators for all the Cues that are available in the company database.</span></span>

<span data-ttu-id="63019-109">Для настройки индикатора нужно задать до двух пороговых значений, определяющих три диапазона значений данных (низкий, средний и высокий), к которым можно применить другой цвет (или стиль).</span><span class="sxs-lookup"><span data-stu-id="63019-109">To set up the indicator, you specify up to two threshold values that define three ranges of data values (low, middle, and high) to which you can apply a different color (or style).</span></span>

## <a name="to-set-up-colored-indicators-on-cues"></a><span data-ttu-id="63019-110">Настройка цветных индикаторов в очередях</span><span class="sxs-lookup"><span data-stu-id="63019-110">To set up colored indicators on Cues</span></span>
1. <span data-ttu-id="63019-111">В разделе **Действия** на странице **Главная** выберите **Настроить очереди**.</span><span class="sxs-lookup"><span data-stu-id="63019-111">Under **Activities** on your **Home** page, choose **Set Up Cues**.</span></span>  
   <span data-ttu-id="63019-112">Откроется окно **Настройка очереди**.</span><span class="sxs-lookup"><span data-stu-id="63019-112">The **Cue Setup** window appears.</span></span> <span data-ttu-id="63019-113">В окне перечисляются индикаторы, которые в настоящее время настроены в очередях.</span><span class="sxs-lookup"><span data-stu-id="63019-113">The window lists the indicators that are currently setup up on Cues.</span></span>
2. <span data-ttu-id="63019-114">Чтобы изменить индикатор, измените поля и, например, значения различных порогов.</span><span class="sxs-lookup"><span data-stu-id="63019-114">To modify an indicator, edit the fields and modify, for example, the values for the different thresholds.</span></span>  

<span data-ttu-id="63019-115">В следующей таблице перечислены цвета, соответствующие параметрам полей **Стиль низкого диапазона**, **Стиль среднего диапазона** и **Стиль высокого диапазона**.</span><span class="sxs-lookup"><span data-stu-id="63019-115">The following table lists the colors that correspond to the options of the **Low Range Style**, **Middle Range Style**, and **High Range Style** fields.</span></span>

| <span data-ttu-id="63019-116">Параметр</span><span class="sxs-lookup"><span data-stu-id="63019-116">Option</span></span> | <span data-ttu-id="63019-117">Цвет</span><span class="sxs-lookup"><span data-stu-id="63019-117">Color</span></span> |
| --- | --- |
| <span data-ttu-id="63019-118">**Нет**</span><span class="sxs-lookup"><span data-stu-id="63019-118">**None**</span></span> |<span data-ttu-id="63019-119">Без цвета (цвет плитки очереди</span><span class="sxs-lookup"><span data-stu-id="63019-119">No color (same color as the Cue tile</span></span> |
| <span data-ttu-id="63019-120">**Положительный**</span><span class="sxs-lookup"><span data-stu-id="63019-120">**Favorable**</span></span> |<span data-ttu-id="63019-121">Зеленый</span><span class="sxs-lookup"><span data-stu-id="63019-121">Green</span></span> |
| <span data-ttu-id="63019-122">**Отрицательный**</span><span class="sxs-lookup"><span data-stu-id="63019-122">**Unfavorable**</span></span> |<span data-ttu-id="63019-123">Красный</span><span class="sxs-lookup"><span data-stu-id="63019-123">Red</span></span> |
| <span data-ttu-id="63019-124">**Нераспознанные**</span><span class="sxs-lookup"><span data-stu-id="63019-124">**Ambiguous**</span></span> |<span data-ttu-id="63019-125">Желтый</span><span class="sxs-lookup"><span data-stu-id="63019-125">Yellow</span></span> |
| <span data-ttu-id="63019-126">**Подчиненный**</span><span class="sxs-lookup"><span data-stu-id="63019-126">**Subordinate**</span></span> |<span data-ttu-id="63019-127">Серый</span><span class="sxs-lookup"><span data-stu-id="63019-127">Gray</span></span> |

## <a name="see-also"></a><span data-ttu-id="63019-128">См. также</span><span class="sxs-lookup"><span data-stu-id="63019-128">See Also</span></span>
<span data-ttu-id="63019-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="63019-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
