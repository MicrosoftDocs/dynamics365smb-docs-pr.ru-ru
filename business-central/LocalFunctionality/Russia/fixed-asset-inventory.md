---
title: Инвентаризация основных средств в России
description: Российские улучшения включают инвентаризацию основных средств.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 61e69cb4454b3934e540d4810fa8841d65f1455e
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301177"
---
# <a name="fixed-asset-inventory"></a><span data-ttu-id="7a25d-103">Инвентаризация основных средств</span><span class="sxs-lookup"><span data-stu-id="7a25d-103">Fixed Asset Inventory</span></span>

<span data-ttu-id="7a25d-104">Функция инвентаризации основных средств позволяет:</span><span class="sxs-lookup"><span data-stu-id="7a25d-104">The fixed assets inventory feature enables you to:</span></span> 

- <span data-ttu-id="7a25d-105">выполнять инвентаризацию основных средств в соответствии с требованиями законодательства;</span><span class="sxs-lookup"><span data-stu-id="7a25d-105">Process inventory auditing of fixed assets in accordance with legal requirements.</span></span>
- <span data-ttu-id="7a25d-106">создавать электронные инвентарные списки основных средств, подлежащих инвентаризации, с учетом расчетных количеств и сумм;</span><span class="sxs-lookup"><span data-stu-id="7a25d-106">Generate electronic inventory lists of fixed assets that are to be inventoried with calculated quantities and amounts.</span></span>
- <span data-ttu-id="7a25d-107">разделять инвентарные списки по физическому местоположению основных средств (по коду местоположения основного средства);</span><span class="sxs-lookup"><span data-stu-id="7a25d-107">Divide the inventory lists by the physical locations of fixed assets (by Fixed Asset Location code).</span></span>
- <span data-ttu-id="7a25d-108">фильтровать инвентарные списки по другим аналитикам (например, по подотчетнику);</span><span class="sxs-lookup"><span data-stu-id="7a25d-108">Filter the inventory lists by other analytics (such as responsible employee).</span></span>
- <span data-ttu-id="7a25d-109">печатать формы с инвентарными списками, в которых показаны все основные средства, прошедшие инвентаризацию, а также со списками, в которых перечислены основные средства с разницей только в количестве или сумме;</span><span class="sxs-lookup"><span data-stu-id="7a25d-109">Print the forms with inventory lists that show all inventoried fixed assets, as well as lists that show the fixed assets with differences only in quantities or amounts.</span></span>
- <span data-ttu-id="7a25d-110">печатать стандартные формы основных средств.</span><span class="sxs-lookup"><span data-stu-id="7a25d-110">Print unified fixed asset forms.</span></span>

 

## <a name="inventory-lists-of-fixed-assets"></a><span data-ttu-id="7a25d-111">Инвентарные списки основных средств</span><span class="sxs-lookup"><span data-stu-id="7a25d-111">Inventory Lists of Fixed Assets</span></span> 

<span data-ttu-id="7a25d-112">Для проведения инвентаризации необходимо создать инвентарные списки основных средств с расчетными количествами и суммами.</span><span class="sxs-lookup"><span data-stu-id="7a25d-112">You must create inventory lists of fixed assets with calculated quantities and amounts for inventory auditing.</span></span> <span data-ttu-id="7a25d-113">Такие списки разделены по аналитике: например по физическому местоположению или сотруднику, ответственному за определенные основные средства.</span><span class="sxs-lookup"><span data-stu-id="7a25d-113">The lists are divided by analytics such as physical locations and employees responsible for certain fixed assets.</span></span>

<span data-ttu-id="7a25d-114">Можно создать специальные шаблоны в окне **Журнал учета основных средств**.</span><span class="sxs-lookup"><span data-stu-id="7a25d-114">You can create special templates in the **Fixed Asset Journal** window.</span></span> 

<span data-ttu-id="7a25d-115">Ниже показано, как создать список основных средств, подлежащих инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="7a25d-115">The following procedure shows how to generate a list of fixed assets that are to be inventoried.</span></span> 

1. <span data-ttu-id="7a25d-116">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы ОС**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7a25d-116">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Journals**, and then choose the related link.</span></span>

2. <span data-ttu-id="7a25d-117">Выберите действие **Расчет ОС**.</span><span class="sxs-lookup"><span data-stu-id="7a25d-117">Choose the **Calculate FA** action.</span></span> <span data-ttu-id="7a25d-118">Откроется форма запроса отчета для создания инвентарных списков основных средств.</span><span class="sxs-lookup"><span data-stu-id="7a25d-118">The request form of a report that makes fixed asset inventory lists is displayed.</span></span>

3. <span data-ttu-id="7a25d-119">На экспресс-вкладке **Основные средства** отфильтруйте основные средства.</span><span class="sxs-lookup"><span data-stu-id="7a25d-119">On the **Fixed Asset** FastTab, filter the fixed assets.</span></span>

   > :speech_balloon: <span data-ttu-id="7a25d-120">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="7a25d-120">**Note**</span></span>
   >
   > <span data-ttu-id="7a25d-121">Фильтрацию можно выполнять по любому параметру из карточки основного средства, например по местоположению основного средства или по подотчетнику.</span><span class="sxs-lookup"><span data-stu-id="7a25d-121">They can be filtered by any parameter from the Fixed Asset card, such fixed asset location or responsible employee.</span></span> 

<span data-ttu-id="7a25d-122">Параметры, перечисленные в таблице ниже, можно найти на экспресс-вкладке **Параметры**.</span><span class="sxs-lookup"><span data-stu-id="7a25d-122">The parameters listed in the following table are on the **Options** FastTab.</span></span>

| <span data-ttu-id="7a25d-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="7a25d-123">Parameter</span></span>                                | <span data-ttu-id="7a25d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7a25d-124">Description</span></span>                                                  |
| :--------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="7a25d-125">**ОС Журнал Шаблон**</span><span class="sxs-lookup"><span data-stu-id="7a25d-125">**Fixed Asset Journal Template**</span></span>         | <span data-ttu-id="7a25d-126">Выберите шаблон журнала основных средств, который будет использоваться для работы со списком основных средств в ходе инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="7a25d-126">Select the fixed asset journal template to work with the fixed assets list during the inventory auditing process.</span></span> <span data-ttu-id="7a25d-127">По умолчанию указывается шаблон журнала основных средств.</span><span class="sxs-lookup"><span data-stu-id="7a25d-127">It is filled by default with the fixed asset journal template.</span></span> |
| <span data-ttu-id="7a25d-128">**Код книги амортизации**</span><span class="sxs-lookup"><span data-stu-id="7a25d-128">**Depreciation Book Code**</span></span>               | <span data-ttu-id="7a25d-129">Выберите книгу амортизации с записями, для которых будет выполнен расчет по количеству и сумме.</span><span class="sxs-lookup"><span data-stu-id="7a25d-129">Select the depreciation book with the records, which will be calculated by quantities and amounts.</span></span> |
| <span data-ttu-id="7a25d-130">**Начальный Документ Номер**</span><span class="sxs-lookup"><span data-stu-id="7a25d-130">**Starting Document No.**</span></span>                | <span data-ttu-id="7a25d-131">Укажите номер документа, применявшийся при создании строк в журнале основных средств.</span><span class="sxs-lookup"><span data-stu-id="7a25d-131">Specify the document number used to make lines in the fixed asset journal.</span></span> |
| <span data-ttu-id="7a25d-132">**Дата Документа**</span><span class="sxs-lookup"><span data-stu-id="7a25d-132">**Document Date**</span></span>                        | <span data-ttu-id="7a25d-133">Укажите дату документа.</span><span class="sxs-lookup"><span data-stu-id="7a25d-133">Specify the document date.</span></span>                                   |
| <span data-ttu-id="7a25d-134">**Дата учета**</span><span class="sxs-lookup"><span data-stu-id="7a25d-134">**Posting Date**</span></span>                         | <span data-ttu-id="7a25d-135">Укажите дату учета.</span><span class="sxs-lookup"><span data-stu-id="7a25d-135">Specify the posting date.</span></span> <span data-ttu-id="7a25d-136">Количества и суммы рассчитываются на эту дату.</span><span class="sxs-lookup"><span data-stu-id="7a25d-136">The quantities and amounts are calculated on this date.</span></span> <span data-ttu-id="7a25d-137">В поле **Дата учета** тоже заносится это значение.</span><span class="sxs-lookup"><span data-stu-id="7a25d-137">The **Posting Date** field is also filled with this value.</span></span> |
| <span data-ttu-id="7a25d-138">**Показывать ОС с Остаточной Стоимостью = 0**</span><span class="sxs-lookup"><span data-stu-id="7a25d-138">**Show Fixed Asset with Book Value = 0**</span></span> | <span data-ttu-id="7a25d-139">Установите этот флажок, чтобы создать в журнале основных средств строки для ОС с нулевой остаточной стоимостью.</span><span class="sxs-lookup"><span data-stu-id="7a25d-139">Select this field to create fixed asset journal lines for fixed assets which have a book value of zero.</span></span> |

<span data-ttu-id="7a25d-140">Отчет создает один раздел в шаблоне журнала основных средств для каждого местоположения основных средств, отфильтрованного в форме запроса.</span><span class="sxs-lookup"><span data-stu-id="7a25d-140">The report creates one batch in the fixed asset journal template for every fixed asset location that is filtered in the request form.</span></span> <span data-ttu-id="7a25d-141">Для каждого отфильтрованного основного средства создается одна строка журнала в разделе, соответствующем местоположению этого ОС.</span><span class="sxs-lookup"><span data-stu-id="7a25d-141">For every fixed asset that is filtered, one journal line is created in the batch according to its location.</span></span> <span data-ttu-id="7a25d-142">Раздел журнала создается для основных средств в каждом местоположении ОС.</span><span class="sxs-lookup"><span data-stu-id="7a25d-142">A journal batch is created for fixed assets in each fixed asset location.</span></span> 

<span data-ttu-id="7a25d-143">Ниже показано, как начать инвентаризацию по местоположению основных средств.</span><span class="sxs-lookup"><span data-stu-id="7a25d-143">The following procedure shows how to begin inventory auditing by fixed asset locations.</span></span> 

1. <span data-ttu-id="7a25d-144">Выберите раздел, соответствующий местоположению основных средств, а затем выберите **ОК**.</span><span class="sxs-lookup"><span data-stu-id="7a25d-144">Select the batch according to the fixed asset location, and choose **ОК**.</span></span>

   > :speech_balloon: <span data-ttu-id="7a25d-145">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="7a25d-145">**Note**</span></span>
   >
   > <span data-ttu-id="7a25d-146">Можно просмотреть строки основных средств, отфильтрованные в отчете, и строки для данного местоположения ОС.</span><span class="sxs-lookup"><span data-stu-id="7a25d-146">You can view the fixed assets lines that are filtered in the report and the lines that are in this fixed asset location.</span></span>

2. <span data-ttu-id="7a25d-147">Расположите столбцы журнала основных средств таким образом, чтобы можно было просматривать расчетные и фактические количества и суммы.</span><span class="sxs-lookup"><span data-stu-id="7a25d-147">Place the columns of the fixed asset journal so that you can view calculated and actual quantities and amounts.</span></span> <span data-ttu-id="7a25d-148">Они указаны в следующих полях:</span><span class="sxs-lookup"><span data-stu-id="7a25d-148">They are reflected in the following fields:</span></span>

   - <span data-ttu-id="7a25d-149">**Фактическое количество**</span><span class="sxs-lookup"><span data-stu-id="7a25d-149">**Actual Quantity**</span></span>
   - <span data-ttu-id="7a25d-150">**Расчетное количество**</span><span class="sxs-lookup"><span data-stu-id="7a25d-150">**Calc. Quantity**</span></span>
   - <span data-ttu-id="7a25d-151">**Фактическая сумма**</span><span class="sxs-lookup"><span data-stu-id="7a25d-151">**Actual Amount**</span></span>
   - <span data-ttu-id="7a25d-152">**Расчетная сумма**</span><span class="sxs-lookup"><span data-stu-id="7a25d-152">**Calc. Amount**</span></span>

 

> :speech_balloon: <span data-ttu-id="7a25d-153">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="7a25d-153">**Note**</span></span>
>
> <span data-ttu-id="7a25d-154">Значение суммы — это остаточная стоимость основного средства.</span><span class="sxs-lookup"><span data-stu-id="7a25d-154">The amount value is the book value of the fixed asset.</span></span>



 

## <a name="see-also"></a><span data-ttu-id="7a25d-155">См. также</span><span class="sxs-lookup"><span data-stu-id="7a25d-155">See Also</span></span>

[<span data-ttu-id="7a25d-156">ОС: местоположения и ответственные сотрудники</span><span class="sxs-lookup"><span data-stu-id="7a25d-156">Fixed Asset Locations and Employees</span></span>](Fixed-Asset-Locations-and-Employees.md)
