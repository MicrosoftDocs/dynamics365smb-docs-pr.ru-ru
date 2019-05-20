---
title: Настройка визуальных обозначений действий очереди | Документы Майкрософт
description: Настраивайте цветные индикаторы на плитке очереди, чтобы установить индивидуальные обозначения действий очереди.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: personalize, customize
ms.date: 04/01/2019
ms.author: solsen
redirect_url: admin-how-set-up-colored-indicator-on-cues
ms.openlocfilehash: f79f1a65ee17d8ca46a8ecf1cd9d49c5246bef63
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1248115"
---
# <a name="set-up-a-colored-indicator-on-cues"></a><span data-ttu-id="5e7f6-103">Настройка цветного индикатора в очередях</span><span class="sxs-lookup"><span data-stu-id="5e7f6-103">Set Up a Colored Indicator on Cues</span></span>
<span data-ttu-id="5e7f6-104">Можно настроить очереди, отображаемые в ролевом центре, чтобы включить индикатор, меняющий цвет в зависимости от значений данных в очереди.</span><span class="sxs-lookup"><span data-stu-id="5e7f6-104">You can set up Cues that appear on the Role Center to include an indicator that changes color based on the data values in the Cues.</span></span>

<span data-ttu-id="5e7f6-105">Индикатор отображается как цветная полоса вдоль верхней границы плитки очереди.</span><span class="sxs-lookup"><span data-stu-id="5e7f6-105">The indicator appears as a colored bar along the top border of the Cue tile.</span></span> <span data-ttu-id="5e7f6-106">Предоставляет визуальный сигнал статуса операций очереди, который может указывать на благоприятные или неблагоприятные условия и необходимость действий пользователя.</span><span class="sxs-lookup"><span data-stu-id="5e7f6-106">It provides a visual signal of the status of the Cue's activity, which can indicate favorable or unfavorable conditions to prompt the user to take action.</span></span> <span data-ttu-id="5e7f6-107">Например, если в очереди отображаются текущие счета продажи, можно настроить, чтобы индикатор отображался зеленым (положительный), если общее число текущих счетов продажи меньше 10, и красным (отрицательный), если это число больше 20.</span><span class="sxs-lookup"><span data-stu-id="5e7f6-107">For example, if a Cue displays ongoing sales invoices, you can set up the indicator to appear green (favorable) when total number of ongoing sales invoices is below 10, and appears red (unfavorable) when the total is greater than 20.</span></span>

<span data-ttu-id="5e7f6-108">На странице **Настройка очереди** можно настроить индикаторы для всех очередей, доступных в базе данных организации.</span><span class="sxs-lookup"><span data-stu-id="5e7f6-108">From the **Cue Setup** page, you set up indicators for all the Cues that are available in the company database.</span></span>

<span data-ttu-id="5e7f6-109">Для настройки индикатора нужно задать до двух пороговых значений, определяющих три диапазона значений данных (низкий, средний и высокий), к которым можно применить другой цвет (или стиль).</span><span class="sxs-lookup"><span data-stu-id="5e7f6-109">To set up the indicator, you specify up to two threshold values that define three ranges of data values (low, middle, and high) to which you can apply a different color (or style).</span></span>

## <a name="to-set-up-colored-indicators-on-cues"></a><span data-ttu-id="5e7f6-110">Настройка цветных индикаторов в очередях</span><span class="sxs-lookup"><span data-stu-id="5e7f6-110">To set up colored indicators on Cues</span></span>
1. <span data-ttu-id="5e7f6-111">В разделе **Действия** в ролевом центре выберите **Настроить очереди**.</span><span class="sxs-lookup"><span data-stu-id="5e7f6-111">Under **Activities** on your Role Center, choose **Set Up Cues**.</span></span>  
   <span data-ttu-id="5e7f6-112">Откроется страница **Настройка очереди**.</span><span class="sxs-lookup"><span data-stu-id="5e7f6-112">The **Cue Setup** page appears.</span></span> <span data-ttu-id="5e7f6-113">На странице перечисляются индикаторы, которые в настоящее время настроены в очередях.</span><span class="sxs-lookup"><span data-stu-id="5e7f6-113">The page lists the indicators that are currently setup up on Cues.</span></span>
2. <span data-ttu-id="5e7f6-114">Чтобы изменить индикатор, измените поля и, например, значения различных порогов.</span><span class="sxs-lookup"><span data-stu-id="5e7f6-114">To modify an indicator, edit the fields and modify, for example, the values for the different thresholds.</span></span>  

<span data-ttu-id="5e7f6-115">В следующей таблице перечислены цвета, соответствующие параметрам полей **Стиль низкого диапазона**, **Стиль среднего диапазона** и **Стиль высокого диапазона**.</span><span class="sxs-lookup"><span data-stu-id="5e7f6-115">The following table lists the colors that correspond to the options of the **Low Range Style**, **Middle Range Style**, and **High Range Style** fields.</span></span>

| <span data-ttu-id="5e7f6-116">Параметр</span><span class="sxs-lookup"><span data-stu-id="5e7f6-116">Option</span></span> | <span data-ttu-id="5e7f6-117">Цвет</span><span class="sxs-lookup"><span data-stu-id="5e7f6-117">Color</span></span> |
| --- | --- |
| <span data-ttu-id="5e7f6-118">**Нет**</span><span class="sxs-lookup"><span data-stu-id="5e7f6-118">**None**</span></span> |<span data-ttu-id="5e7f6-119">Без цвета (цвет очереди)</span><span class="sxs-lookup"><span data-stu-id="5e7f6-119">No color (same color as the Cue tile)</span></span>|
| <span data-ttu-id="5e7f6-120">**Положительный**</span><span class="sxs-lookup"><span data-stu-id="5e7f6-120">**Favorable**</span></span> |<span data-ttu-id="5e7f6-121">Зеленый</span><span class="sxs-lookup"><span data-stu-id="5e7f6-121">Green</span></span> |
| <span data-ttu-id="5e7f6-122">**Отрицательный**</span><span class="sxs-lookup"><span data-stu-id="5e7f6-122">**Unfavorable**</span></span> |<span data-ttu-id="5e7f6-123">Красный</span><span class="sxs-lookup"><span data-stu-id="5e7f6-123">Red</span></span> |
| <span data-ttu-id="5e7f6-124">**Нераспознанные**</span><span class="sxs-lookup"><span data-stu-id="5e7f6-124">**Ambiguous**</span></span> |<span data-ttu-id="5e7f6-125">Желтый</span><span class="sxs-lookup"><span data-stu-id="5e7f6-125">Yellow</span></span> |
| <span data-ttu-id="5e7f6-126">**Подчиненный**</span><span class="sxs-lookup"><span data-stu-id="5e7f6-126">**Subordinate**</span></span> |<span data-ttu-id="5e7f6-127">Серый</span><span class="sxs-lookup"><span data-stu-id="5e7f6-127">Gray</span></span> |

## <a name="see-also"></a><span data-ttu-id="5e7f6-128">См. также</span><span class="sxs-lookup"><span data-stu-id="5e7f6-128">See Also</span></span>
<span data-ttu-id="5e7f6-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5e7f6-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
