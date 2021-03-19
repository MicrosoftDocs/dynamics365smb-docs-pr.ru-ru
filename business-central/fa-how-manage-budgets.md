---
title: Управление бюджетами ОС | Документация Майкрософт
description: Вы можете настраивать информацию о будущих инвестициях, выбытии и амортизации основных средств, чтобы было проще готовить бюджеты и прогнозы.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: forecast
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: acdff4ac5879ee3b9c4237d4bcf6e2d30af72dff
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5380510"
---
# <a name="manage-budgets-for-fixed-assets"></a><span data-ttu-id="f7edb-103">Управление бюджетами основных средств</span><span class="sxs-lookup"><span data-stu-id="f7edb-103">Manage Budgets for Fixed Assets</span></span>
<span data-ttu-id="f7edb-104">Можно настроить бюджетные основные средства.</span><span class="sxs-lookup"><span data-stu-id="f7edb-104">You can set up budgeted fixed assets.</span></span> <span data-ttu-id="f7edb-105">Например, это позволит включать в отчеты ожидаемые приобретения и продажи.</span><span class="sxs-lookup"><span data-stu-id="f7edb-105">For example, this lets you include anticipated acquisitions and sales in reports.</span></span>  

<span data-ttu-id="f7edb-106">Чтобы подготовить отчет о бюджетных прибылях и убытках, бюджетируемый баланс и наличный бюджет, нужны сведения о будущих инвестициях, выбытии и амортизации основных средств.</span><span class="sxs-lookup"><span data-stu-id="f7edb-106">To prepare your budgeted income statement, budgeted balance sheet, and cash budget, you need information about future investments, disposals and depreciation of fixed assets.</span></span> <span data-ttu-id="f7edb-107">Можно получить эти сведения из отчета **ОС - прогнозное значение**.</span><span class="sxs-lookup"><span data-stu-id="f7edb-107">You can get this information from the **Fixed Asset - Projected Value** report.</span></span> <span data-ttu-id="f7edb-108">Прежде чем вывести этот отчет, необходимо подготовить бюджет.</span><span class="sxs-lookup"><span data-stu-id="f7edb-108">Before you print this report, you must prepare the budget.</span></span>  

## <a name="to-budget-the-acquisition-cost-of-a-fixed-asset"></a><span data-ttu-id="f7edb-109">Бюджетирование стоимости приобретения основного средства</span><span class="sxs-lookup"><span data-stu-id="f7edb-109">To budget the acquisition cost of a fixed asset</span></span>
<span data-ttu-id="f7edb-110">Для подготовки бюджета следует настроить карточки основных средств для тех основных средств, которые намечены для приобретения в будущем.</span><span class="sxs-lookup"><span data-stu-id="f7edb-110">To prepare a budget, you have to set up fixed asset cards for fixed assets that you intend to buy in the future.</span></span> <span data-ttu-id="f7edb-111">Бюджетные основные средства настраиваются как обычные основные средства, но их необходимо настроить, чтобы они не учитывались в главной книге.</span><span class="sxs-lookup"><span data-stu-id="f7edb-111">The budget fixed assets are set up as ordinary fixed assets, but it must be set up to not post to the general ledger.</span></span>

<span data-ttu-id="f7edb-112">При учете стоимости приобретения вводится номер бюджетного основного средства в поле **Номер бюджетного ОС**.</span><span class="sxs-lookup"><span data-stu-id="f7edb-112">When you post the acquisition cost, you enter the number of the budgeted fixed asset in the **Budgeted FA No.** field.</span></span> <span data-ttu-id="f7edb-113">Это приведет к учету стоимости приобретения со знаком, противоположным бюджетному средству.</span><span class="sxs-lookup"><span data-stu-id="f7edb-113">This will post an acquisition cost with an opposite sign for the budgeted asset.</span></span> <span data-ttu-id="f7edb-114">Это означает, что общая стоимость приобретения бюджетного основного средства является разницей между бюджетной и действительной стоимостью.</span><span class="sxs-lookup"><span data-stu-id="f7edb-114">This means that the total acquisition cost on the budgeted asset is the difference between the budgeted and the actual acquisition cost.</span></span>

1. <span data-ttu-id="f7edb-115">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Основные средства**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f7edb-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="f7edb-116">Выберите действие **Создать**, чтобы создать новую карточку основного средства для бюджетируемого основного средства.</span><span class="sxs-lookup"><span data-stu-id="f7edb-116">Choose the **New** action to create a new fixed asset card for the budgeted fixed asset.</span></span>
3. <span data-ttu-id="f7edb-117">Установите флажок **Бюджетируемое ОС** для предотвращения учета в главной книге.</span><span class="sxs-lookup"><span data-stu-id="f7edb-117">Select the **Budgeted Asset** check box to prevent posting to the general ledger.</span></span>
4. <span data-ttu-id="f7edb-118">Заполните оставшиеся поля, назначьте книгу амортизации, затем учтите первую стоимость приобретения с бюджетированным основным средством, введенным в поле **Номер бюджетного ОС** в строке журнала.</span><span class="sxs-lookup"><span data-stu-id="f7edb-118">Fill in the remaining fields, assign a depreciation book, and then post the first acquisition cost with the budgeted fixed asset entered in the **Budgeted FA No.** field on the journal line.</span></span> <span data-ttu-id="f7edb-119">Дополнительные сведения см. в разделе [Приобретение основных средств](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="f7edb-119">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span></span>

## <a name="to-budget-the-disposal-of-a-fixed-asset"></a><span data-ttu-id="f7edb-120">Бюджетирование реализации основного средства</span><span class="sxs-lookup"><span data-stu-id="f7edb-120">To budget the disposal of a fixed asset</span></span>
<span data-ttu-id="f7edb-121">Если планируется продажа основных средств в пределах бюджетного периода, то можно ввести информацию о ценах продажи и дате продажи.</span><span class="sxs-lookup"><span data-stu-id="f7edb-121">If you plan to sell assets within the budget period, you can enter information about sales price and sales date.</span></span>

1. <span data-ttu-id="f7edb-122">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Основные средства**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f7edb-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="f7edb-123">Выберите списываемое основное средство, затем выберите действие **Книги амортизации**.</span><span class="sxs-lookup"><span data-stu-id="f7edb-123">Select the fixed asset to be disposed of, and then choose the **Depreciation Books** action.</span></span>
3. <span data-ttu-id="f7edb-124">На странице **ОС - книги амортизации** заполните поля **Прогнозная дата выбытия** и **Прогнозные поступления от выбытия**.</span><span class="sxs-lookup"><span data-stu-id="f7edb-124">On the **FA Depreciation Books** page, fill in the **Projected Disposal Date** and **Projected Proceeds on Disposal** fields.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-view-projected-disposal-values"></a><span data-ttu-id="f7edb-125">Просмотр стоимости планируемой реализации</span><span class="sxs-lookup"><span data-stu-id="f7edb-125">To view projected disposal values</span></span>
<span data-ttu-id="f7edb-126">Для просмотра планируемых значений стоимости реализации и расчета прибылей и убытков можно использовать отчет **ОС - прогнозное значение**.</span><span class="sxs-lookup"><span data-stu-id="f7edb-126">To see the projected disposal values and have the gain and loss calculated, you can use the **FA Projected Value** report.</span></span>

1. <span data-ttu-id="f7edb-127">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **ОС - прогнозируемое значение**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f7edb-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Projected Value**, and then choose the related link.</span></span>
2. <span data-ttu-id="f7edb-128">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="f7edb-128">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="f7edb-129">Нажмите кнопку **Печать** или **Просмотр**.</span><span class="sxs-lookup"><span data-stu-id="f7edb-129">Choose the **Print** or **Preview** button.</span></span>

## <a name="to-budget-depreciation"></a><span data-ttu-id="f7edb-130">Составление бюджета амортизации</span><span class="sxs-lookup"><span data-stu-id="f7edb-130">To budget depreciation</span></span>
<span data-ttu-id="f7edb-131">Отчет **ОС - прогнозное значение** можно использовать для расчета будущей амортизации.</span><span class="sxs-lookup"><span data-stu-id="f7edb-131">You can use the **Fixed Asset - Projected Value** report to calculate future depreciation.</span></span> <span data-ttu-id="f7edb-132">В отчете будет показана учетная стоимость и накопленная амортизация на начало выбранного периода, изменения в течение данного периода, учтенная стоимость и накопленная амортизация на конец выбранного периода.</span><span class="sxs-lookup"><span data-stu-id="f7edb-132">The report shows the book value and accumulated depreciation at the start of the selected period, changes during the period, and the book value and accumulated depreciation at the end of the selected period.</span></span>

1. <span data-ttu-id="f7edb-133">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **ОС — прогнозное значение**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f7edb-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Asset Projected Value**, and then choose the related link.</span></span>
2. <span data-ttu-id="f7edb-134">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="f7edb-134">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="f7edb-135">Для просмотра общих значений стоимости для всех основных средств снимите флажок **Новая страница для ОС**.</span><span class="sxs-lookup"><span data-stu-id="f7edb-135">To see total values for all assets, clear the **Print per Fixed Asset** check box.</span></span>
4. <span data-ttu-id="f7edb-136">Оставьте экспресс-вкладку **Основное средство** пустой, если нужно включить все основные средства.</span><span class="sxs-lookup"><span data-stu-id="f7edb-136">Leave the **Fixed Asset** FastTab blank to have all assets included.</span></span> <span data-ttu-id="f7edb-137">В поле **Бюджетируемое ОС** можно ввести **Нет** для исключения бюджетируемых основных средств или **Да** для просмотра только бюджетируемых основных средств.</span><span class="sxs-lookup"><span data-stu-id="f7edb-137">In the **Budgeted Asset** field, enter **No** to exclude budgeted assets or **Yes** to see budgeted assets only.</span></span>
5. <span data-ttu-id="f7edb-138">Нажмите кнопку **Печать** или **Просмотр**.</span><span class="sxs-lookup"><span data-stu-id="f7edb-138">Choose the **Print** or **Preview** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="f7edb-139">См. также</span><span class="sxs-lookup"><span data-stu-id="f7edb-139">See Also</span></span>
[<span data-ttu-id="f7edb-140">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="f7edb-140">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="f7edb-141">Настройка основных средств</span><span class="sxs-lookup"><span data-stu-id="f7edb-141">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="f7edb-142">Финансы</span><span class="sxs-lookup"><span data-stu-id="f7edb-142">Finance</span></span>](finance.md)  
[<span data-ttu-id="f7edb-143">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="f7edb-143">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="f7edb-144">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f7edb-144">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]