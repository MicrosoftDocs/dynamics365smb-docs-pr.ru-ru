---
title: Создание и запуск пакетных заданий | Документы Майкрософт
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
ms.date: 10/01/2018
ms.author: solsen
ms.openlocfilehash: 260cd7761b130bbe3748de3cc109a9f4f56c1384
ms.sourcegitcommit: d09f5ee0e164c7716f4ccb2ed71e2f9732a1f4f9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "853262"
---
# <a name="run-batch-jobs"></a><span data-ttu-id="d5f8a-103">Запуск пакетных заданий</span><span class="sxs-lookup"><span data-stu-id="d5f8a-103">Run Batch Jobs</span></span>
<span data-ttu-id="d5f8a-104">Пакетное задание — это процедура обработки данных в пакетах, например пакетное задание **Коррекция валютных курсов**.</span><span class="sxs-lookup"><span data-stu-id="d5f8a-104">A batch job is a routine that processes data in batches, for example the **Adjust Exchange Rates** batch job.</span></span> <span data-ttu-id="d5f8a-105">В некоторых пакетных заданиях выполняются периодические действия, связанные с учетом, например закрытие отчета о прибыли и убытках в конце финансового года.</span><span class="sxs-lookup"><span data-stu-id="d5f8a-105">There are batch jobs that perform periodic accounting activities, such as closing the income statement at the end of a fiscal year.</span></span> <span data-ttu-id="d5f8a-106">Во многих пакетных заданиях выполняются вычисления, например вычисление финансовых выплат, коррекция валютного курса и вычисление цены единицы.</span><span class="sxs-lookup"><span data-stu-id="d5f8a-106">Many batch jobs do calculation work, such as calculation of finance charges, exchange rate adjustment, and calculation of unit prices.</span></span>

<span data-ttu-id="d5f8a-107">Пакетное задание подобно отчету, за исключением того, что в пакетном задании результаты обработки используются не для печати, а для непосредственного обновления информации.</span><span class="sxs-lookup"><span data-stu-id="d5f8a-107">A batch job is like a report, except the batch job uses the result of its work to update information directly, instead of printing the results.</span></span>

## <a name="to-run-a-batch-job"></a><span data-ttu-id="d5f8a-108">Выполнение пакетного задания</span><span class="sxs-lookup"><span data-stu-id="d5f8a-108">To run a batch job</span></span>
1. <span data-ttu-id="d5f8a-109">Чтобы открыть страницу запроса для соответствующего пакетного задания, выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите название пакетного задания, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d5f8a-109">To open the request page for the relevant batch job, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter the name of the batch job, and then choose the related link.</span></span>
2. <span data-ttu-id="d5f8a-110">Если для этого пакетного задания доступна экспресс-вкладка **Параметры**, заполните поля, определив действия, которые должны в нем выполняться.</span><span class="sxs-lookup"><span data-stu-id="d5f8a-110">If there is an **Options** FastTab for the batch job, fill in the fields to determine what the batch job will do.</span></span>
3. <span data-ttu-id="d5f8a-111">На странице запроса может быть одна или несколько экспресс-вкладок с фильтрами, которые можно использовать для ограничения количества данных, которые будут обрабатываться при выполнении пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="d5f8a-111">The page may contain one or more FastTab with filters, which you can use to limit the data included in the batch job.</span></span> <span data-ttu-id="d5f8a-112">Можно задать критерии в предлагаемых фильтрах или добавить дополнительные фильтры.</span><span class="sxs-lookup"><span data-stu-id="d5f8a-112">You can enter criteria in the suggested filters or add more filters.</span></span>
4. <span data-ttu-id="d5f8a-113">Нажмите кнопку **OK** для запуска пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="d5f8a-113">Choose the **OK** button to start the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="d5f8a-114">См. также</span><span class="sxs-lookup"><span data-stu-id="d5f8a-114">See Also</span></span>
[<span data-ttu-id="d5f8a-115">Сортировка, поиск и фильтрация списков</span><span class="sxs-lookup"><span data-stu-id="d5f8a-115">Sorting, Searching, and Filtering Lists</span></span>](ui-enter-criteria-filters.md)  
<span data-ttu-id="d5f8a-116">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d5f8a-116">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
