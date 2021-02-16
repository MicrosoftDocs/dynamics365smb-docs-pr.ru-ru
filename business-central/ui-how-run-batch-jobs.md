---
title: Создание и запуск пакетных заданий | Документация Майкрософт
description: Пакетные задания запускаются для обработки данных и обновления информации, например для выполнения периодических действий и других расчетов.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, process
ms.date: 10/01/2020
ms.author: solsen
ms.openlocfilehash: 04ae13561f44d544d38b04e3a881a0e707b441b4
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4760521"
---
# <a name="run-batch-jobs-and-xmlports"></a><span data-ttu-id="229c4-103">Запуск пакетных заданий и XMLport</span><span class="sxs-lookup"><span data-stu-id="229c4-103">Run Batch Jobs and XMLports</span></span>
<span data-ttu-id="229c4-104">Пакетное задание — это процедура обработки данных в пакетах, например пакетное задание **Коррекция валютных курсов**.</span><span class="sxs-lookup"><span data-stu-id="229c4-104">A batch job is a routine that processes data in batches, for example the **Adjust Exchange Rates** batch job.</span></span> <span data-ttu-id="229c4-105">В некоторых пакетных заданиях выполняются периодические действия, связанные с учетом, например закрытие отчета о прибыли и убытках в конце финансового года.</span><span class="sxs-lookup"><span data-stu-id="229c4-105">There are batch jobs that perform periodic accounting activities, such as closing the income statement at the end of a fiscal year.</span></span> <span data-ttu-id="229c4-106">Во многих пакетных заданиях выполняются вычисления, например вычисление финансовых выплат, коррекция валютного курса и вычисление цены единицы.</span><span class="sxs-lookup"><span data-stu-id="229c4-106">Many batch jobs do calculation work, such as calculation of finance charges, exchange rate adjustment, and calculation of unit prices.</span></span>

<span data-ttu-id="229c4-107">Пакетное задание подобно отчету, за исключением того, что в пакетном задании результаты обработки используются не для печати, а для непосредственного обновления информации.</span><span class="sxs-lookup"><span data-stu-id="229c4-107">A batch job is like a report, except the batch job uses the result of its work to update information directly, instead of printing the results.</span></span>

<span data-ttu-id="229c4-108">Вы можете запланировать, когда должно запускаться пакетное задание.</span><span class="sxs-lookup"><span data-stu-id="229c4-108">You can schedule when a batch job runs.</span></span> <span data-ttu-id="229c4-109">Дополнительные сведения см. в разделе [Использование очередей работ для планирования задач](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="229c4-109">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>

## <a name="to-run-a-batch-job"></a><span data-ttu-id="229c4-110">Выполнение пакетного задания</span><span class="sxs-lookup"><span data-stu-id="229c4-110">To run a batch job</span></span>
1. <span data-ttu-id="229c4-111">Чтобы открыть страницу запроса для соответствующего пакетного задания, выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите название пакетного задания, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="229c4-111">To open the request page for the relevant batch job, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter the name of the batch job, and then choose the related link.</span></span>
2. <span data-ttu-id="229c4-112">Если для этого пакетного задания доступна экспресс-вкладка **Параметры**, заполните поля, определив действия, которые должны в нем выполняться.</span><span class="sxs-lookup"><span data-stu-id="229c4-112">If there is an **Options** FastTab for the batch job, fill in the fields to determine what the batch job will do.</span></span>
3. <span data-ttu-id="229c4-113">На странице запроса может быть одна или несколько экспресс-вкладок с фильтрами, которые можно использовать для ограничения количества данных, которые будут обрабатываться при выполнении пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="229c4-113">The page may contain one or more FastTab with filters, which you can use to limit the data included in the batch job.</span></span> <span data-ttu-id="229c4-114">Можно задать критерии в предлагаемых фильтрах или добавить дополнительные фильтры.</span><span class="sxs-lookup"><span data-stu-id="229c4-114">You can enter criteria in the suggested filters or add more filters.</span></span>
4. <span data-ttu-id="229c4-115">Нажмите кнопку **OK** для запуска пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="229c4-115">Choose the **OK** button to start the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="229c4-116">См. также</span><span class="sxs-lookup"><span data-stu-id="229c4-116">See Also</span></span>
[<span data-ttu-id="229c4-117">Сортировка, поиск и фильтрация списков</span><span class="sxs-lookup"><span data-stu-id="229c4-117">Sorting, Searching, and Filtering Lists</span></span>](ui-enter-criteria-filters.md)  
[<span data-ttu-id="229c4-118">Использование очередей работ для планирования задач</span><span class="sxs-lookup"><span data-stu-id="229c4-118">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)  
<span data-ttu-id="229c4-119">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="229c4-119">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>
