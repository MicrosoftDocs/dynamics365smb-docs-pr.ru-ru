---
title: Анализ движения денежных средств | Документация Майкрософт
description: Описывается, как использовать диаграммы цикла кассы, дохода и расхода, движения денежных средств и прогноза движения денежных средств для анализа и будущего переноса кассы в организацию и из нее.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: money flow, expense and income, liquidity, cash receipts minus cash payments, Cartera
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 7bc87f8fc096241e7f77efb0eb4e7bceb1d28aef
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5391178"
---
# <a name="analyzing-cash-flow-in-your-company"></a><span data-ttu-id="e7b5f-103">Анализ движения денежных средств в организации</span><span class="sxs-lookup"><span data-stu-id="e7b5f-103">Analyzing Cash Flow in Your Company</span></span>
<span data-ttu-id="e7b5f-104">Диаграммы в ролевом центре бухгалтера предоставляют аналитики, которые помогут принимать обоснованные решения относительно того, что сделать с кассой.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-104">The charts on the Accountant Role Center provide insights that can help you make solid decisions about what to do with your cash.</span></span>  

| <span data-ttu-id="e7b5f-105">Чтобы на эти вопросы</span><span class="sxs-lookup"><span data-stu-id="e7b5f-105">To answer questions like these</span></span> | <span data-ttu-id="e7b5f-106">Используйте эту диаграмму</span><span class="sxs-lookup"><span data-stu-id="e7b5f-106">Use this chart</span></span> |
| --- | --- |
| <span data-ttu-id="e7b5f-107">Как долго касса занята в процессе продаж?</span><span class="sxs-lookup"><span data-stu-id="e7b5f-107">How long does the sales process tie up my cash?</span></span></br> <span data-ttu-id="e7b5f-108">Следует ли мне увеличить или уменьшить уровень запасов?</span><span class="sxs-lookup"><span data-stu-id="e7b5f-108">Should I increase or reduce inventory levels?</span></span> |<span data-ttu-id="e7b5f-109">Цикл кассы</span><span class="sxs-lookup"><span data-stu-id="e7b5f-109">Cash Cycle</span></span> |
| <span data-ttu-id="e7b5f-110">Когда касса была перенесена из моей организации или в нее?</span><span class="sxs-lookup"><span data-stu-id="e7b5f-110">When did cash move in and out of my company?</span></span></br> <span data-ttu-id="e7b5f-111">Одни периоды лучше других?</span><span class="sxs-lookup"><span data-stu-id="e7b5f-111">Are some periods better than others?</span></span> |<span data-ttu-id="e7b5f-112">Движение денежных средств</span><span class="sxs-lookup"><span data-stu-id="e7b5f-112">Cash Flow</span></span> |
| <span data-ttu-id="e7b5f-113">Цифры не сходятся за период?</span><span class="sxs-lookup"><span data-stu-id="e7b5f-113">Do the numbers seem off for a period?</span></span></br> <span data-ttu-id="e7b5f-114">Следует ли мне провести расследование?</span><span class="sxs-lookup"><span data-stu-id="e7b5f-114">Should I investigate?</span></span> |<span data-ttu-id="e7b5f-115">Доходы и расходы</span><span class="sxs-lookup"><span data-stu-id="e7b5f-115">Income & Expense</span></span> |
| <span data-ttu-id="e7b5f-116">Когда могут возникнуть кассовые излишки или дефицит?</span><span class="sxs-lookup"><span data-stu-id="e7b5f-116">When might a cash surplus or deficit happen?</span></span></br> <span data-ttu-id="e7b5f-117">Следует ли выплатить долг или занять для удовлетворения предстоящих расходов?</span><span class="sxs-lookup"><span data-stu-id="e7b5f-117">Should I pay down debt, or borrow to meet upcoming expenses?</span></span> |<span data-ttu-id="e7b5f-118">Прогнозы движения денежных средств</span><span class="sxs-lookup"><span data-stu-id="e7b5f-118">Cash Flow Forecasts</span></span> |

<span data-ttu-id="e7b5f-119">В ролевом центре бухгалтера в разделе **Финансовое исполнение** диаграммы **Цикл кассы**, **Движение денежных средств** и **Доходы и расходы** предлагают способы анализа движения денежных средств:</span><span class="sxs-lookup"><span data-stu-id="e7b5f-119">On the Accountant Role Center, under **Finance Performance**, the **Cash Cycle**, **Cash Flow**, and **Income & Expense** charts offer ways to analyze cash flow:</span></span>  

* <span data-ttu-id="e7b5f-120">См. цифры за период с помощью слайдера временной шкалы.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-120">See figures for a period by using the timeline slider.</span></span>  
* <span data-ttu-id="e7b5f-121">Отфильтруйте диаграмму, выбрав источник в легенде.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-121">Filter the chart by choosing the source in the legend.</span></span>  
* <span data-ttu-id="e7b5f-122">Измените продолжительность периода или перейдите к предыдущему либо следующему периоду, выбрав параметры в раскрывающемся меню **Финансовое исполнение**.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-122">Change the length of the period, or go to the previous or next period, by choosing options on the **Finance Performance** drop down.</span></span>  
* <span data-ttu-id="e7b5f-123">Просмотрите операции, выбрав точку на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-123">View the entries by choosing a point in the chart.</span></span> <span data-ttu-id="e7b5f-124">Например, точка на временной шкале или сегмент столбца.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-124">For example, a point on the timeline or a column segment.</span></span> <span data-ttu-id="e7b5f-125">Если номера не совпадают, здесь можно внести корректировки.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-125">If the numbers seem off, this is where you can make adjustments.</span></span>  

<span data-ttu-id="e7b5f-126">Хотя диаграмма **Прогноз движения денежных средств** отдельная, она устроена аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-126">Although it's separate, the **Cash Flow Forecast** chart is similar.</span></span> <span data-ttu-id="e7b5f-127">Можно просмотреть сведения, отфильтровать результаты и изменить отображаемую информацию аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-127">You view details, filter results, and change what is displayed in the same ways.</span></span> <span data-ttu-id="e7b5f-128">При изменении настройки можно обновить прогноз, выбрав **Прогноз движения денежных средств** и щелкнув **Пересчитать прогноз**.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-128">If you change a setting, you can refresh the forecast by choosing **Cash Flow Forecast**, and then **Recalculate Forecast**.</span></span>

<span data-ttu-id="e7b5f-129">Если требуется проверить прогноз в дополнение к операциям прогноза, можно также просмотреть журнал движения денежных средств.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-129">If you want to examine the forecast, in addition to forecast entries, you can also look at the cash flow worksheet.</span></span> <span data-ttu-id="e7b5f-130">Например, можно посмотреть, как в прогнозе:</span><span class="sxs-lookup"><span data-stu-id="e7b5f-130">For example, you can see how the forecast:</span></span>

* <span data-ttu-id="e7b5f-131">Обрабатываются подтвержденные продажи и покупки.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-131">Handles confirmed sales and purchases.</span></span>  
* <span data-ttu-id="e7b5f-132">Вычитается кредиторская задолженность и добавляется дебиторская задолженность.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-132">Subtracts payables and adds receivables.</span></span>  
* <span data-ttu-id="e7b5f-133">Пропускаются дублирующие заказы на продажу и заказы на покупку.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-133">Skips duplicate sales orders and purchase orders.</span></span>  

## <a name="to-view-a-cash-flow-worksheet"></a><span data-ttu-id="e7b5f-134">Просмотр журнала движения денежных средств</span><span class="sxs-lookup"><span data-stu-id="e7b5f-134">To view a cash flow worksheet</span></span>
1. <span data-ttu-id="e7b5f-135">Выполните поиск по **Прогнозы движения денежных средств**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-135">Search for **Cash Flow Forecasts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e7b5f-136">Выберите прогноз движения денежных средств, а затем щелкните действие **Журнал движения денежных средств**.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-136">Choose a cash flow forecast, and then choose the **Cash Flow Worksheet** action.</span></span>  
3. <span data-ttu-id="e7b5f-137">На странице **Журнал движения денежных средств** выберите действие **Предложить строки журнала**.</span><span class="sxs-lookup"><span data-stu-id="e7b5f-137">On the **Cash Flow Worksheet** page, choose the **Suggest Worksheet Lines** action.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="e7b5f-138">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/forecast-cash-flow-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="e7b5f-138">See Related Training at [Microsoft Learn](/learn/modules/forecast-cash-flow-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="e7b5f-139">См. также</span><span class="sxs-lookup"><span data-stu-id="e7b5f-139">See Also</span></span>
[<span data-ttu-id="e7b5f-140">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="e7b5f-140">Setting Up Finance</span></span>](finance-setup-finance.md)  
<span data-ttu-id="e7b5f-141">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e7b5f-141">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="e7b5f-142">Настройка анализа движения денежных средств</span><span class="sxs-lookup"><span data-stu-id="e7b5f-142">Setting Up Cash Flow Analysis</span></span>](finance-setup-cash-flow-analyses.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]