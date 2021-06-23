---
title: Сведения о проектировании — поиск комбинаций измерений | Документация Майкрософт
description: Если страница закрывается после редактирования набора измерений Business Central определяет, существует ли отредактированный набор измерений. Если набор не существует, создается новый набор и возвращается код комбинации измерений.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 544cb3a1844aaf85ab937031a23d6d00506ffa74
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215757"
---
# <a name="design-details-searching-for-dimension-combinations"></a><span data-ttu-id="a8a23-104">Сведения о проектировании: поиск комбинаций измерений</span><span class="sxs-lookup"><span data-stu-id="a8a23-104">Design Details: Searching for Dimension Combinations</span></span>
<span data-ttu-id="a8a23-105">Если страница закрывается после редактирования набора измерений [!INCLUDE[prod_short](includes/prod_short.md)] определяет, существует ли отредактированный набор измерений.</span><span class="sxs-lookup"><span data-stu-id="a8a23-105">When you close a page after you edit a set of dimensions, [!INCLUDE[prod_short](includes/prod_short.md)] evaluates whether the edited set of dimensions exists.</span></span> <span data-ttu-id="a8a23-106">Если набор не существует, создается новый набор и возвращается код комбинации измерений.</span><span class="sxs-lookup"><span data-stu-id="a8a23-106">If the set does not exist, a new set is created and the dimension combination ID is returned.</span></span>  

## <a name="building-search-tree"></a><span data-ttu-id="a8a23-107">Создание дерева поиска</span><span class="sxs-lookup"><span data-stu-id="a8a23-107">Building Search Tree</span></span>  
 <span data-ttu-id="a8a23-108">Таблица 481 **Узел дерева набора измерений** используется, когда [!INCLUDE[prod_short](includes/prod_short.md)] выполняет оценку того, существует ли набор измерений в таблице 480 **Операция набора измерений**.</span><span class="sxs-lookup"><span data-stu-id="a8a23-108">Table 481 **Dimension Set Tree Node** is used when [!INCLUDE[prod_short](includes/prod_short.md)] evaluates whether a set of dimensions already exists in table 480 **Dimension Set Entry** table.</span></span> <span data-ttu-id="a8a23-109">Оценка выполняется путем рекурсивного обхода дерева поиска начиная с верхнего уровня (0).</span><span class="sxs-lookup"><span data-stu-id="a8a23-109">The evaluation is performed by recursively traversing the search tree starting at the top level numbered 0.</span></span> <span data-ttu-id="a8a23-110">Верхний уровень 0 представляет набор измерений без операций набора измерений.</span><span class="sxs-lookup"><span data-stu-id="a8a23-110">The top level 0 represents a dimension set with no dimension set entries.</span></span> <span data-ttu-id="a8a23-111">Дочерние элементы этого набора измерений представляют наборы измерений только с одной операцией набора измерений.</span><span class="sxs-lookup"><span data-stu-id="a8a23-111">The children of this dimension set represent dimension sets with only one dimension set entry.</span></span> <span data-ttu-id="a8a23-112">Дочерние элементы этих наборов измерений представляют наборы измерений с двумя дочерними элементами и т. д.</span><span class="sxs-lookup"><span data-stu-id="a8a23-112">The children of these dimension sets represent dimension sets with two children, and so on.</span></span>  

### <a name="example-1"></a><span data-ttu-id="a8a23-113">Пример 1</span><span class="sxs-lookup"><span data-stu-id="a8a23-113">Example 1</span></span>  
 <span data-ttu-id="a8a23-114">На следующей схеме представлено дерево поиска с шестью наборами измерений.</span><span class="sxs-lookup"><span data-stu-id="a8a23-114">The following diagram represents a search tree with six dimension sets.</span></span> <span data-ttu-id="a8a23-115">На схеме отображается только идентификационная операция набора измерений.</span><span class="sxs-lookup"><span data-stu-id="a8a23-115">Only the distinguishing dimension set entry is displayed in the diagram.</span></span>  

 <span data-ttu-id="a8a23-116">![Пример древовидной структуры измерений](media/nav2013_dimension_tree.png "Пример древовидной структуры измерений")</span><span class="sxs-lookup"><span data-stu-id="a8a23-116">![Example of dimension tree structure](media/nav2013_dimension_tree.png "Example of dimension tree structure")</span></span>  

 <span data-ttu-id="a8a23-117">В следующей таблице описан полный список операций набора измерений, формирующих каждый набор измерений.</span><span class="sxs-lookup"><span data-stu-id="a8a23-117">The following table describes a complete list of dimension set entries that make up each dimension set.</span></span>  

|<span data-ttu-id="a8a23-118">Наборы измерений</span><span class="sxs-lookup"><span data-stu-id="a8a23-118">Dimension Sets</span></span>|<span data-ttu-id="a8a23-119">Записи набора измерений</span><span class="sxs-lookup"><span data-stu-id="a8a23-119">Dimension Set Entries</span></span>|  
|--------------------|---------------------------|  
|<span data-ttu-id="a8a23-120">Комплект 0</span><span class="sxs-lookup"><span data-stu-id="a8a23-120">Set 0</span></span>|<span data-ttu-id="a8a23-121">Нет</span><span class="sxs-lookup"><span data-stu-id="a8a23-121">None</span></span>|  
|<span data-ttu-id="a8a23-122">Комплект 1</span><span class="sxs-lookup"><span data-stu-id="a8a23-122">Set 1</span></span>|<span data-ttu-id="a8a23-123">AREA 30</span><span class="sxs-lookup"><span data-stu-id="a8a23-123">AREA 30</span></span>|  
|<span data-ttu-id="a8a23-124">Комплект 2</span><span class="sxs-lookup"><span data-stu-id="a8a23-124">Set 2</span></span>|<span data-ttu-id="a8a23-125">AREA 30, DEPT ADM</span><span class="sxs-lookup"><span data-stu-id="a8a23-125">AREA 30, DEPT ADM</span></span>|  
|<span data-ttu-id="a8a23-126">Комплект 3</span><span class="sxs-lookup"><span data-stu-id="a8a23-126">Set 3</span></span>|<span data-ttu-id="a8a23-127">AREA 30, DEPT PROD</span><span class="sxs-lookup"><span data-stu-id="a8a23-127">AREA 30, DEPT PROD</span></span>|  
|<span data-ttu-id="a8a23-128">Комплект 4</span><span class="sxs-lookup"><span data-stu-id="a8a23-128">Set 4</span></span>|<span data-ttu-id="a8a23-129">AREA 30, DEPT ADM, PROJ VW</span><span class="sxs-lookup"><span data-stu-id="a8a23-129">AREA 30, DEPT ADM, PROJ VW</span></span>|  
|<span data-ttu-id="a8a23-130">Комплект 5</span><span class="sxs-lookup"><span data-stu-id="a8a23-130">Set 5</span></span>|<span data-ttu-id="a8a23-131">AREA 40</span><span class="sxs-lookup"><span data-stu-id="a8a23-131">AREA 40</span></span>|  
|<span data-ttu-id="a8a23-132">Комплект 6</span><span class="sxs-lookup"><span data-stu-id="a8a23-132">Set 6</span></span>|<span data-ttu-id="a8a23-133">AREA 40, PROJ VW</span><span class="sxs-lookup"><span data-stu-id="a8a23-133">AREA 40, PROJ VW</span></span>|  

### <a name="example-2"></a><span data-ttu-id="a8a23-134">Пример 2</span><span class="sxs-lookup"><span data-stu-id="a8a23-134">Example 2</span></span>  
 <span data-ttu-id="a8a23-135">Этот пример показывает, как [!INCLUDE[prod_short](includes/prod_short.md)] оценивает, существует ли набор измерений, состоящий из операций набора измерений AREA 40, DEPT PROD.</span><span class="sxs-lookup"><span data-stu-id="a8a23-135">This example shows how [!INCLUDE[prod_short](includes/prod_short.md)] evaluates whether a dimension set that consists of the dimension set entries AREA 40, DEPT PROD exists.</span></span>  

 <span data-ttu-id="a8a23-136">Сначала [!INCLUDE[prod_short](includes/prod_short.md)] также обновляет таблицу **Узел дерева набора измерений**, чтобы гарантировать, что дерево поиска будет выглядеть так, как на следующей схеме.</span><span class="sxs-lookup"><span data-stu-id="a8a23-136">First, [!INCLUDE[prod_short](includes/prod_short.md)] also updates the **Dimension Set Tree Node** table to make sure that the search tree looks like the following diagram.</span></span> <span data-ttu-id="a8a23-137">Таким образом, набор измерений 7 становится дочерним набором набора измерений 5.</span><span class="sxs-lookup"><span data-stu-id="a8a23-137">Thus dimension set 7 becomes a child of the dimension set 5.</span></span>  

 <span data-ttu-id="a8a23-138">![Пример древовидной структуры измерений в NAV 2013](media/nav2013_dimension_tree_example2.png "Пример древовидной структуры измерений в NAV 2013")</span><span class="sxs-lookup"><span data-stu-id="a8a23-138">![Example of dimension tree structure in NAV 2013](media/nav2013_dimension_tree_example2.png "Example of dimension tree structure in NAV 2013")</span></span>  

### <a name="finding-dimension-set-id"></a><span data-ttu-id="a8a23-139">Поиск кода набора измерений</span><span class="sxs-lookup"><span data-stu-id="a8a23-139">Finding Dimension Set ID</span></span>  
 <span data-ttu-id="a8a23-140">На концептуальном уровне **Родительский код**, **Измерение** и **Значение измерения** в дереве поиска объединяются и используются как первичный ключ, поскольку [!INCLUDE[prod_short](includes/prod_short.md)] перемещается по дереву в том же порядке, что и операции измерений.</span><span class="sxs-lookup"><span data-stu-id="a8a23-140">At a conceptual level, **Parent ID**, **Dimension**, and **Dimension Value**, in the search tree, are combined and used as the primary key because [!INCLUDE[prod_short](includes/prod_short.md)] traverses the tree in the same order as the dimension entries.</span></span> <span data-ttu-id="a8a23-141">Функция GET (запись) используется для поиска ИД набора измерений.</span><span class="sxs-lookup"><span data-stu-id="a8a23-141">The GET function (record) is used to search for dimension set ID.</span></span> <span data-ttu-id="a8a23-142">В следующем примере кода показано, как найти ИД набора измерений с тремя значениями измерений.</span><span class="sxs-lookup"><span data-stu-id="a8a23-142">The following code example shows how to find the dimension set ID when there are three dimension values.</span></span>  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet."Parent ID",UserDim.DimCode,UserDim.DimValueCode);  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

<span data-ttu-id="a8a23-143">Однако чтобы сохранить возможность [!INCLUDE[prod_short](includes/prod_short.md)] переименовывать как измерение, так и значение измерения, в таблицу 349 **Значение измерения** добавлено целочисленное поле **ИД значения измерения**.</span><span class="sxs-lookup"><span data-stu-id="a8a23-143">However, to preserve the ability of [!INCLUDE[prod_short](includes/prod_short.md)] to rename both a dimension and a dimension value, table 349, **Dimension Value**, is extended with an integer field, **Dimension Value ID**.</span></span> <span data-ttu-id="a8a23-144">Эта таблица преобразует пару полей **Измерение** и **Значение измерения** в целочисленное значение.</span><span class="sxs-lookup"><span data-stu-id="a8a23-144">This table converts the field pair, **Dimension** and **Dimension Value**, to an integer value.</span></span> <span data-ttu-id="a8a23-145">Переименовав измерение и значение измерения, целое значение не меняется.</span><span class="sxs-lookup"><span data-stu-id="a8a23-145">When you rename the dimension and dimension value, the integer value is not changed.</span></span>  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet.ParentID,UserDim."Dimension Value ID");  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

## <a name="see-also"></a><span data-ttu-id="a8a23-146">См. также</span><span class="sxs-lookup"><span data-stu-id="a8a23-146">See Also</span></span>
    
 <span data-ttu-id="a8a23-147">[Сведения о проектировании: операции набора измерений](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="a8a23-147">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="a8a23-148">[Обзор записей набора измерений](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="a8a23-148">[Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 [<span data-ttu-id="a8a23-149">Сведения о проектировании: структура таблицы</span><span class="sxs-lookup"><span data-stu-id="a8a23-149">Design Details: Table Structure</span></span>](design-details-table-structure.md)   
 


[!INCLUDE[footer-include](includes/footer-banner.md)]
