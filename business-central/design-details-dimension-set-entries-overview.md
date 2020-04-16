---
title: Обзор записей набора измерений | Документация Майкрософт
description: В этом разделе описывается, как операции набора измерений хранятся и учитываются в Dynamics 365.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dimension
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: f35184a6a69ed0fa1ccd504525a19af6bd9c5955
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3185520"
---
# <a name="dimension-set-entries-overview"></a><span data-ttu-id="90261-103">Обзор записей набора измерений</span><span class="sxs-lookup"><span data-stu-id="90261-103">Dimension Set Entries Overview</span></span>
<span data-ttu-id="90261-104">В этом разделе описывается, как операции набора измерений хранятся и учитываются в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="90261-104">This topic describes how dimension set entries are stored and posted in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="dimension-sets"></a><span data-ttu-id="90261-105">Наборы измерений</span><span class="sxs-lookup"><span data-stu-id="90261-105">Dimension Sets</span></span>  
<span data-ttu-id="90261-106">Набор измерений — это уникальная комбинация значений измерений.</span><span class="sxs-lookup"><span data-stu-id="90261-106">A dimension set is a unique combination of dimension values.</span></span> <span data-ttu-id="90261-107">Это храниться как записи набора измерений в базе данных.</span><span class="sxs-lookup"><span data-stu-id="90261-107">It is stored as dimension set entries in the database.</span></span> <span data-ttu-id="90261-108">Каждая запись набора измерений представляет отдельное значение измерения.</span><span class="sxs-lookup"><span data-stu-id="90261-108">Each dimension set entry represents a single dimension value.</span></span> <span data-ttu-id="90261-109">Набор измерений определяется общим кодом набора измерений, который присваивается каждой операции набора измерений, которая относится к набору измерений.</span><span class="sxs-lookup"><span data-stu-id="90261-109">The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.</span></span>  

<span data-ttu-id="90261-110">В следующем примере представлен набор измерений с тремя операциями набора измерений.</span><span class="sxs-lookup"><span data-stu-id="90261-110">The following example shows a dimension set that has three dimension set entries.</span></span> <span data-ttu-id="90261-111">Набор измерений определяется кодом набора измерений, который равен 108.</span><span class="sxs-lookup"><span data-stu-id="90261-111">The dimension set is identified by a dimension set ID, which is 108.</span></span>  

|<span data-ttu-id="90261-112">Код набора измерений</span><span class="sxs-lookup"><span data-stu-id="90261-112">Dimension Set ID</span></span>|<span data-ttu-id="90261-113">Код Измерения:</span><span class="sxs-lookup"><span data-stu-id="90261-113">Dimension Code</span></span>|<span data-ttu-id="90261-114">Код значения измерения</span><span class="sxs-lookup"><span data-stu-id="90261-114">Dimension Value Code</span></span>|<span data-ttu-id="90261-115">Имя значения измерения</span><span class="sxs-lookup"><span data-stu-id="90261-115">Dimension Value Name</span></span>|  
|----------------------|--------------------|--------------------------|--------------------------|  
|<span data-ttu-id="90261-116">108</span><span class="sxs-lookup"><span data-stu-id="90261-116">108</span></span>|<span data-ttu-id="90261-117">РЕГИОН</span><span class="sxs-lookup"><span data-stu-id="90261-117">AREA</span></span>|<span data-ttu-id="90261-118">70</span><span class="sxs-lookup"><span data-stu-id="90261-118">70</span></span>|<span data-ttu-id="90261-119">Северная Америка</span><span class="sxs-lookup"><span data-stu-id="90261-119">America North</span></span>|  
|<span data-ttu-id="90261-120">108</span><span class="sxs-lookup"><span data-stu-id="90261-120">108</span></span>|<span data-ttu-id="90261-121">БИЗНЕСГРУППА</span><span class="sxs-lookup"><span data-stu-id="90261-121">BUSINESSGROUP</span></span>|<span data-ttu-id="90261-122">HOME</span><span class="sxs-lookup"><span data-stu-id="90261-122">HOME</span></span>|<span data-ttu-id="90261-123">В начало</span><span class="sxs-lookup"><span data-stu-id="90261-123">Home</span></span>|  
|<span data-ttu-id="90261-124">108</span><span class="sxs-lookup"><span data-stu-id="90261-124">108</span></span>|<span data-ttu-id="90261-125">ОТДЕЛ</span><span class="sxs-lookup"><span data-stu-id="90261-125">DEPARTMENT</span></span>|<span data-ttu-id="90261-126">ПРОДАЖИ</span><span class="sxs-lookup"><span data-stu-id="90261-126">SALES</span></span>|<span data-ttu-id="90261-127">Продажи</span><span class="sxs-lookup"><span data-stu-id="90261-127">Sales</span></span>|  

## <a name="dimension-set-entries"></a><span data-ttu-id="90261-128">Записи набора измерений</span><span class="sxs-lookup"><span data-stu-id="90261-128">Dimension Set Entries</span></span>  
<span data-ttu-id="90261-129">Наборы измерений сохраняются в таблице **Запись набора измерений** в виде записей набора измерений с одинаковым кодом набора измерений.</span><span class="sxs-lookup"><span data-stu-id="90261-129">Dimension sets are stored in the **Dimension Set Entry** table as dimension set entries with the same dimension set ID.</span></span>  

<span data-ttu-id="90261-130">![Поток записей набора измерений](media/dimensionentrynav7.png "Поток записей набора измерений")</span><span class="sxs-lookup"><span data-stu-id="90261-130">![Flow of dimension set entries](media/dimensionentrynav7.png "Flow of dimension set entries")</span></span>  

<span data-ttu-id="90261-131">При создании новой строки журнала, заголовка документа или строки документа можно указать комбинации значений измерений.</span><span class="sxs-lookup"><span data-stu-id="90261-131">When you create a new journal line, document header, or document line, you can specify a combination of dimension values.</span></span> <span data-ttu-id="90261-132">Вместо явного сохранения значения каждого измерения в базе данных, код набора измерений присваивается строке журнала, заголовку документа или строке документа для определения набора измерений.</span><span class="sxs-lookup"><span data-stu-id="90261-132">Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.</span></span>  

<span data-ttu-id="90261-133">При редактировании и закрытии страницы **Изменить записи набора измерений** проверяется существование комбинации значений измерений как набора измерений в таблице.</span><span class="sxs-lookup"><span data-stu-id="90261-133">When you edit and close the **Edit Dimension Set Entries** page, a check is performed to see whether the combination of dimension values exists as a dimension set in the table.</span></span> <span data-ttu-id="90261-134">Если в таблице встречается комбинация, соответствующий КОД набора измерений присваивается заголовку документа, строке журнала, либо строке документа.</span><span class="sxs-lookup"><span data-stu-id="90261-134">If the combination occurs in the table, then the corresponding dimension set ID is assigned to the journal line, document header, or document line.</span></span> <span data-ttu-id="90261-135">В противном случае новый набор измерений добавляется к таблице, а идентификатор нового набора измерений присваивается заголовку документа, строке журнала либо строке документа.</span><span class="sxs-lookup"><span data-stu-id="90261-135">Otherwise, a new dimension set is added to the table, and the new dimension set ID is assigned to the journal line, document header, or document line.</span></span>

## <a name="codeunit-408-dimension-management"></a><span data-ttu-id="90261-136">Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="90261-136">Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="90261-137">Codeunit 408, Dimension Management, — это библиотека функций, обрабатывающих общие задачи, связанные с измерениями, такие как копирование из одной таблицы в другую или из одного документа в другой.</span><span class="sxs-lookup"><span data-stu-id="90261-137">Codeunit 408, Dimension Management, is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span>

## <a name="performance-improvement"></a><span data-ttu-id="90261-138">Повышение производительности</span><span class="sxs-lookup"><span data-stu-id="90261-138">Performance Improvement</span></span>  
<span data-ttu-id="90261-139">При сохранении наборов измерений один раз в базе данных экономится пространство БД и улучшается общая производительность.</span><span class="sxs-lookup"><span data-stu-id="90261-139">By storing dimension sets once in the database, database space is preserved and overall performance is improved.</span></span>  

## <a name="see-also"></a><span data-ttu-id="90261-140">См. также</span><span class="sxs-lookup"><span data-stu-id="90261-140">See Also</span></span>  
<span data-ttu-id="90261-141">[Сведения о проектировании: поиск комбинаций измерений](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="90261-141">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
<span data-ttu-id="90261-142">[Сведения о проектировании: структура таблицы](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="90261-142">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
[<span data-ttu-id="90261-143">Сведения о проектировании: операции набора измерений</span><span class="sxs-lookup"><span data-stu-id="90261-143">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)   
