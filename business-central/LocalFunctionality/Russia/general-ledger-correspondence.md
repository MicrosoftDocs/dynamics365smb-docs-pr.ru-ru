---
title: Корреспонденция финансовых операций в России
description: Российские улучшения включают корреспонденцию финансовых операций.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: b5217be345dd2217bbb4c566dcbfc218546d81a4
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3921258"
---
# <a name="general-ledger-correspondence"></a><span data-ttu-id="e35a6-103">Корреспонденция финансовых операций</span><span class="sxs-lookup"><span data-stu-id="e35a6-103">General Ledger Correspondence</span></span>

<span data-ttu-id="e35a6-104">Функция корреспонденции финансовых операций позволяет:</span><span class="sxs-lookup"><span data-stu-id="e35a6-104">The general ledger correspondence feature enables you to:</span></span> 

- <span data-ttu-id="e35a6-105">Периодически создавать транзакцию корреспонденции.</span><span class="sxs-lookup"><span data-stu-id="e35a6-105">Create a correspondence transaction periodically.</span></span>
- <span data-ttu-id="e35a6-106">Учитывать операции корреспонденции при учете финансовых транзакций.</span><span class="sxs-lookup"><span data-stu-id="e35a6-106">Post correspondence operations when you post general ledger transactions.</span></span>
- <span data-ttu-id="e35a6-107">Анализировать ряд отчетов для корреспонденции.</span><span class="sxs-lookup"><span data-stu-id="e35a6-107">Analyze a number of reports for correspondence.</span></span>

## <a name="creating-a-general-ledger-correspondence-entry"></a><span data-ttu-id="e35a6-108">Создание операции финансовой корреспонденции</span><span class="sxs-lookup"><span data-stu-id="e35a6-108">Creating a General Ledger Correspondence Entry</span></span>

<span data-ttu-id="e35a6-109">Ниже приводится процедура периодического создания операций финансовой корреспонденции.</span><span class="sxs-lookup"><span data-stu-id="e35a6-109">The following procedure shows how to periodically create general ledger correspondence entries.</span></span>

1. <span data-ttu-id="e35a6-110">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Создать корреспонденцию счетов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e35a6-110">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Create G/L Correspondence**, and then choose the related link.</span></span>
2. <span data-ttu-id="e35a6-111">Введите в поле **Номер транзакции**</span><span class="sxs-lookup"><span data-stu-id="e35a6-111">Enter the **Transaction No.**</span></span> <span data-ttu-id="e35a6-112">номер транзакции, если финансовая корреспонденция должна быть создана только для выбранной транзакции.</span><span class="sxs-lookup"><span data-stu-id="e35a6-112">field with the transaction number if general ledger correspondence is to be created only for the selected transaction.</span></span> <span data-ttu-id="e35a6-113">В противном случае оставьте поле пустым.</span><span class="sxs-lookup"><span data-stu-id="e35a6-113">Otherwise, leave it blank.</span></span>

<span data-ttu-id="e35a6-114">Чтобы настроить автоматическую финансовую корреспонденцию:</span><span class="sxs-lookup"><span data-stu-id="e35a6-114">To set up automatic general ledger correspondence:</span></span>

1. <span data-ttu-id="e35a6-115">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка ГК**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e35a6-115">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="e35a6-116">Установите флажок **Авт. корреспонденция**.</span><span class="sxs-lookup"><span data-stu-id="e35a6-116">Select the **Automatic G/L Correspondence** check box.</span></span>

## <a name="reports"></a><span data-ttu-id="e35a6-117">Отчеты</span><span class="sxs-lookup"><span data-stu-id="e35a6-117">Reports</span></span>

<span data-ttu-id="e35a6-118">Следующие отчеты были добавлены для анализа данных из транзакций корреспонденции:</span><span class="sxs-lookup"><span data-stu-id="e35a6-118">The following reports have been added for the analysis of data from correspondence transactions:</span></span>

- <span data-ttu-id="e35a6-119">Фин. Корресп. Главная Книга (страница 12403; отчет 12431)</span><span class="sxs-lookup"><span data-stu-id="e35a6-119">General Ledger - Correspondence (page 12403; report 12431)</span></span>
- <span data-ttu-id="e35a6-120">Операции корреспонденции (страница 12401)</span><span class="sxs-lookup"><span data-stu-id="e35a6-120">G/L Correspondence Entries (page 12401)</span></span>
- <span data-ttu-id="e35a6-121">Отчет Фин. Корресп. Журнал-Ордер (отчет 12432)</span><span class="sxs-lookup"><span data-stu-id="e35a6-121">G/L Corresp. Journal Order (report 12432)</span></span>
- <span data-ttu-id="e35a6-122">Отчет Фин. Корресп. Анализ Операций (отчет 12435)</span><span class="sxs-lookup"><span data-stu-id="e35a6-122">G/L Corresp Entries Analysis (report 12435)</span></span>

### <a name="general-ledger---correspondence-window"></a><span data-ttu-id="e35a6-123">Окно "Фин. Корресп. Главная Книга"</span><span class="sxs-lookup"><span data-stu-id="e35a6-123">General Ledger - Correspondence Window</span></span>

<span data-ttu-id="e35a6-124">Окно **Фин. Корресп. Главная Книга** отображает обороты по корреспонденции счетов за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="e35a6-124">The **General Ledger - Correspondence** window shows turnovers in the chosen period in correspondence.</span></span>

1. <span data-ttu-id="e35a6-125">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Корреспонденция**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e35a6-125">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Correspondence**, and then choose the related link.</span></span>
2. <span data-ttu-id="e35a6-126">Выберите действие **Фин. Корресп. Главная Книга**.</span><span class="sxs-lookup"><span data-stu-id="e35a6-126">Choose the **General Ledger - Correspondence** action.</span></span>

<span data-ttu-id="e35a6-127">Заголовок окна **Фин. Корресп. Главная Книга** содержит следующие фильтры:</span><span class="sxs-lookup"><span data-stu-id="e35a6-127">The header of the **General Ledger - Correspondence** window contains the following filters:</span></span>

- <span data-ttu-id="e35a6-128">Фильтр по дате</span><span class="sxs-lookup"><span data-stu-id="e35a6-128">Date Filter</span></span>
- <span data-ttu-id="e35a6-129">Фильтр по филиалу</span><span class="sxs-lookup"><span data-stu-id="e35a6-129">Business unit Filter</span></span>
- <span data-ttu-id="e35a6-130">Фильтр по глобальному измерению 1</span><span class="sxs-lookup"><span data-stu-id="e35a6-130">Global Dimension 1 Filter</span></span>
- <span data-ttu-id="e35a6-131">Фильтр по глобальному измерению 2</span><span class="sxs-lookup"><span data-stu-id="e35a6-131">Global Dimension 2 Filter</span></span>

<span data-ttu-id="e35a6-132">В подформе отчета показан оборот в корреспонденции с другими счетами:</span><span class="sxs-lookup"><span data-stu-id="e35a6-132">In the subform, the report shows the turnover in correspondence with other accounts:</span></span>

:::image type="content" source="../../media/ru/General-Ledger-Correspondence.png" alt-text="Корреспонденция финансовых операций":::

### <a name="gl-corresp-entries-analysis-report"></a><span data-ttu-id="e35a6-134">Отчет Фин. Корресп. Анализ Операций</span><span class="sxs-lookup"><span data-stu-id="e35a6-134">G/L Corresp Entries Analysis Report</span></span>

<span data-ttu-id="e35a6-135">**Отчет Фин. Корресп. Анализ Операций** отображает записи корреспонденции для каждого счета.</span><span class="sxs-lookup"><span data-stu-id="e35a6-135">The **G/L Corresp Entries Analysis** report shows the correspondence entries for each account.</span></span> <span data-ttu-id="e35a6-136">Отчет может использоваться для обзора операций по счету главной книги с корреспондированием и итоговыми суммами.</span><span class="sxs-lookup"><span data-stu-id="e35a6-136">The report can be used to get an overview of general ledger account entries with correspondence and totals.</span></span>

1. <span data-ttu-id="e35a6-137">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Корреспонденция**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e35a6-137">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Correspondence**, and then choose the related link.</span></span>
2. <span data-ttu-id="e35a6-138">Выберите действие **Фин. Корресп. Анализ Операций**.</span><span class="sxs-lookup"><span data-stu-id="e35a6-138">Choose the **G/L Corresp Entries Analysis** action.</span></span>

<span data-ttu-id="e35a6-139">На вкладке **Параметры** формы запроса имеется возможность задать параметры, заполнив поля сведениями, описанными в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e35a6-139">On the **Options** tab of the request form, you can set parameters by filling in the fields with the information listed in the following table.</span></span>

| <span data-ttu-id="e35a6-140">Поле</span><span class="sxs-lookup"><span data-stu-id="e35a6-140">Field</span></span>                  | <span data-ttu-id="e35a6-141">Описание</span><span class="sxs-lookup"><span data-stu-id="e35a6-141">Description</span></span>                                                  |
| ---------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="e35a6-142">**Начало периода**</span><span class="sxs-lookup"><span data-stu-id="e35a6-142">**Period Beginning**</span></span>   | <span data-ttu-id="e35a6-143">Введите дату начала периода для операций, которые нужно включить в отчет.</span><span class="sxs-lookup"><span data-stu-id="e35a6-143">Enter the starting date of the period, for the entries that you want to include in the report.</span></span> |
| <span data-ttu-id="e35a6-144">**Окончание периода**</span><span class="sxs-lookup"><span data-stu-id="e35a6-144">**Ending of Period**</span></span>   | <span data-ttu-id="e35a6-145">Введите дату окончания периода для операций, которые нужно включить в отчет.</span><span class="sxs-lookup"><span data-stu-id="e35a6-145">Enter the ending date of the period, for the entries that you want to include in the report.</span></span> |
| <span data-ttu-id="e35a6-146">**Другие параметры**:</span><span class="sxs-lookup"><span data-stu-id="e35a6-146">**Other parameters**:</span></span><br /><span data-ttu-id="e35a6-147">**Без нулевых оборотов**, **Без нулевых строк**, **Дебет и кредит раздельно**, **Новая страница для счета ГК**</span><span class="sxs-lookup"><span data-stu-id="e35a6-147">**Without Zero Net Changes**, **Without Zero Lines**, **Debit Credit Separately**, **New Page for GL Acc**</span></span> | <span data-ttu-id="e35a6-148">Указание представления отчета, например, нужно ли выводить сведения для каждого счета без нулевых строк или нулевых оборотов.</span><span class="sxs-lookup"><span data-stu-id="e35a6-148">Specify the view of the report, such as whether the information for each account should be written without zero lines or net changes.</span></span> |

## <a name="see-also"></a><span data-ttu-id="e35a6-149">См. также</span><span class="sxs-lookup"><span data-stu-id="e35a6-149">See Also</span></span>

[<span data-ttu-id="e35a6-150">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="e35a6-150">Russia Local Functionality</span></span>](russia-local-functionality.md)
