---
title: Сведения о проектировании — поиск комбинаций измерений | Документы Майкрософт
description: Если страница закрывается после редактирования набора измерений Business Central определяет, существует ли отредактированный набор измерений. Если набор не существует, создается новый набор и возвращается код комбинации измерений.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: cde720526fdad4c9e4352f08f649d6bd3fc51540
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1240957"
---
# <a name="design-details-searching-for-dimension-combinations"></a><span data-ttu-id="91521-104">Сведения о проектировании: поиск комбинаций измерений</span><span class="sxs-lookup"><span data-stu-id="91521-104">Design Details: Searching for Dimension Combinations</span></span>
<span data-ttu-id="91521-105">Если страница закрывается после редактирования набора измерений [!INCLUDE[d365fin](includes/d365fin_md.md)] определяет, существует ли отредактированный набор измерений.</span><span class="sxs-lookup"><span data-stu-id="91521-105">When you close a page after you edit a set of dimensions, [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether the edited set of dimensions exists.</span></span> <span data-ttu-id="91521-106">Если набор не существует, создается новый набор и возвращается код комбинации измерений.</span><span class="sxs-lookup"><span data-stu-id="91521-106">If the set does not exist, a new set is created and the dimension combination ID is returned.</span></span>  

## <a name="building-search-tree"></a><span data-ttu-id="91521-107">Создание дерева поиска</span><span class="sxs-lookup"><span data-stu-id="91521-107">Building Search Tree</span></span>  
 <span data-ttu-id="91521-108">Таблица 481 **Узел дерева набора измерений** используется, когда [!INCLUDE[d365fin](includes/d365fin_md.md)] выполняет оценку того, существует ли набор измерений в таблице 480 **Операция набора измерений**.</span><span class="sxs-lookup"><span data-stu-id="91521-108">Table 481 **Dimension Set Tree Node** is used when [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether a set of dimensions already exists in table 480 **Dimension Set Entry** table.</span></span> <span data-ttu-id="91521-109">Оценка выполняется путем рекурсивного обхода дерева поиска начиная с верхнего уровня (0).</span><span class="sxs-lookup"><span data-stu-id="91521-109">The evaluation is performed by recursively traversing the search tree starting at the top level numbered 0.</span></span> <span data-ttu-id="91521-110">Верхний уровень 0 представляет набор измерений без операций набора измерений.</span><span class="sxs-lookup"><span data-stu-id="91521-110">The top level 0 represents a dimension set with no dimension set entries.</span></span> <span data-ttu-id="91521-111">Дочерние элементы этого набора измерений представляют наборы измерений только с одной операцией набора измерений.</span><span class="sxs-lookup"><span data-stu-id="91521-111">The children of this dimension set represent dimension sets with only one dimension set entry.</span></span> <span data-ttu-id="91521-112">Дочерние элементы этих наборов измерений представляют наборы измерений с двумя дочерними элементами и т. д.</span><span class="sxs-lookup"><span data-stu-id="91521-112">The children of these dimension sets represent dimension sets with two children, and so on.</span></span>  

### <a name="example-1"></a><span data-ttu-id="91521-113">Пример 1</span><span class="sxs-lookup"><span data-stu-id="91521-113">Example 1</span></span>  
 <span data-ttu-id="91521-114">На следующей схеме представлено дерево поиска с шестью наборами измерений.</span><span class="sxs-lookup"><span data-stu-id="91521-114">The following diagram represents a search tree with six dimension sets.</span></span> <span data-ttu-id="91521-115">На схеме отображается только идентификационная операция набора измерений.</span><span class="sxs-lookup"><span data-stu-id="91521-115">Only the distinguishing dimension set entry is displayed in the diagram.</span></span>  

 <span data-ttu-id="91521-116">![Пример древовидной структуры измерений](media/nav2013_dimension_tree.png "Пример древовидной структуры измерений")</span><span class="sxs-lookup"><span data-stu-id="91521-116">![Example of dimension tree structure](media/nav2013_dimension_tree.png "Example of dimension tree structure")</span></span>  

 <span data-ttu-id="91521-117">В следующей таблице описан полный список операций набора измерений, формирующих каждый набор измерений.</span><span class="sxs-lookup"><span data-stu-id="91521-117">The following table describes a complete list of dimension set entries that make up each dimension set.</span></span>  

|<span data-ttu-id="91521-118">Наборы измерений</span><span class="sxs-lookup"><span data-stu-id="91521-118">Dimension Sets</span></span>|<span data-ttu-id="91521-119">Записи набора измерений</span><span class="sxs-lookup"><span data-stu-id="91521-119">Dimension Set Entries</span></span>|  
|--------------------|---------------------------|  
|<span data-ttu-id="91521-120">Комплект 0</span><span class="sxs-lookup"><span data-stu-id="91521-120">Set 0</span></span>|<span data-ttu-id="91521-121">Нет</span><span class="sxs-lookup"><span data-stu-id="91521-121">None</span></span>|  
|<span data-ttu-id="91521-122">Комплект 1</span><span class="sxs-lookup"><span data-stu-id="91521-122">Set 1</span></span>|<span data-ttu-id="91521-123">AREA 30</span><span class="sxs-lookup"><span data-stu-id="91521-123">AREA 30</span></span>|  
|<span data-ttu-id="91521-124">Комплект 2</span><span class="sxs-lookup"><span data-stu-id="91521-124">Set 2</span></span>|<span data-ttu-id="91521-125">AREA 30, DEPT ADM</span><span class="sxs-lookup"><span data-stu-id="91521-125">AREA 30, DEPT ADM</span></span>|  
|<span data-ttu-id="91521-126">Комплект 3</span><span class="sxs-lookup"><span data-stu-id="91521-126">Set 3</span></span>|<span data-ttu-id="91521-127">AREA 30, DEPT PROD</span><span class="sxs-lookup"><span data-stu-id="91521-127">AREA 30, DEPT PROD</span></span>|  
|<span data-ttu-id="91521-128">Комплект 4</span><span class="sxs-lookup"><span data-stu-id="91521-128">Set 4</span></span>|<span data-ttu-id="91521-129">AREA 30, DEPT ADM, PROJ VW</span><span class="sxs-lookup"><span data-stu-id="91521-129">AREA 30, DEPT ADM, PROJ VW</span></span>|  
|<span data-ttu-id="91521-130">Комплект 5</span><span class="sxs-lookup"><span data-stu-id="91521-130">Set 5</span></span>|<span data-ttu-id="91521-131">AREA 40</span><span class="sxs-lookup"><span data-stu-id="91521-131">AREA 40</span></span>|  
|<span data-ttu-id="91521-132">Комплект 6</span><span class="sxs-lookup"><span data-stu-id="91521-132">Set 6</span></span>|<span data-ttu-id="91521-133">AREA 40, PROJ VW</span><span class="sxs-lookup"><span data-stu-id="91521-133">AREA 40, PROJ VW</span></span>|  

### <a name="example-2"></a><span data-ttu-id="91521-134">Пример 2</span><span class="sxs-lookup"><span data-stu-id="91521-134">Example 2</span></span>  
 <span data-ttu-id="91521-135">Этот пример показывает, как [!INCLUDE[d365fin](includes/d365fin_md.md)] оценивает, существует ли набор измерений, состоящий из операций набора измерений AREA 40, DEPT PROD.</span><span class="sxs-lookup"><span data-stu-id="91521-135">This example shows how [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether a dimension set that consists of the dimension set entries AREA 40, DEPT PROD exists.</span></span>  

 <span data-ttu-id="91521-136">Сначала [!INCLUDE[d365fin](includes/d365fin_md.md)] также обновляет таблицу **Узел дерева набора измерений**, чтобы гарантировать, что дерево поиска будет выглядеть так, как на следующей схеме.</span><span class="sxs-lookup"><span data-stu-id="91521-136">First, [!INCLUDE[d365fin](includes/d365fin_md.md)] also updates the **Dimension Set Tree Node** table to make sure that the search tree looks like the following diagram.</span></span> <span data-ttu-id="91521-137">Таким образом, набор измерений 7 становится дочерним набором набора измерений 5.</span><span class="sxs-lookup"><span data-stu-id="91521-137">Thus dimension set 7 becomes a child of the dimension set 5.</span></span>  

 <span data-ttu-id="91521-138">![Пример древовидной структуры измерений в NAV 2013](media/nav2013_dimension_tree_example2.png "Пример древовидной структуры измерений в NAV 2013")</span><span class="sxs-lookup"><span data-stu-id="91521-138">![Example of dimension tree structure in NAV 2013](media/nav2013_dimension_tree_example2.png "Example of dimension tree structure in NAV 2013")</span></span>  

### <a name="finding-dimension-set-id"></a><span data-ttu-id="91521-139">Поиск кода набора измерений</span><span class="sxs-lookup"><span data-stu-id="91521-139">Finding Dimension Set ID</span></span>  
 <span data-ttu-id="91521-140">На концептуальном уровне **Родительский код**, **Измерение** и **Значение измерения** в дереве поиска объединяются и используются как первичный ключ, поскольку [!INCLUDE[d365fin](includes/d365fin_md.md)] перемещается по дереву в том же порядке, что и операции измерений.</span><span class="sxs-lookup"><span data-stu-id="91521-140">At a conceptual level, **Parent ID**, **Dimension**, and **Dimension Value**, in the search tree, are combined and used as the primary key because [!INCLUDE[d365fin](includes/d365fin_md.md)] traverses the tree in the same order as the dimension entries.</span></span> <span data-ttu-id="91521-141">Функция GET (запись) используется для поиска ИД набора измерений.</span><span class="sxs-lookup"><span data-stu-id="91521-141">The GET function (record) is used to search for dimension set ID.</span></span> <span data-ttu-id="91521-142">В следующем примере кода показано, как найти ИД набора измерений с тремя значениями измерений.</span><span class="sxs-lookup"><span data-stu-id="91521-142">The following code example shows how to find the dimension set ID when there are three dimension values.</span></span>  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet."Parent ID",UserDim.DimCode,UserDim.DimValueCode);  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

<span data-ttu-id="91521-143">Однако чтобы сохранить возможность [!INCLUDE[d365fin](includes/d365fin_md.md)] переименовывать как измерение, так и значение измерения, в таблицу 349 **Значение измерения** добавлено целочисленное поле **ИД значения измерения**.</span><span class="sxs-lookup"><span data-stu-id="91521-143">However, to preserve the ability of [!INCLUDE[d365fin](includes/d365fin_md.md)] to rename both a dimension and a dimension value, table 349, **Dimension Value**, is extended with an integer field, **Dimension Value ID**.</span></span> <span data-ttu-id="91521-144">Эта таблица преобразует пару полей **Измерение** и **Значение измерения** в целочисленное значение.</span><span class="sxs-lookup"><span data-stu-id="91521-144">This table converts the field pair, **Dimension** and **Dimension Value**, to an integer value.</span></span> <span data-ttu-id="91521-145">Переименовав измерение и значение измерения, целое значение не меняется.</span><span class="sxs-lookup"><span data-stu-id="91521-145">When you rename the dimension and dimension value, the integer value is not changed.</span></span>  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet.ParentID,UserDim."Dimension Value ID");  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

## <a name="see-also"></a><span data-ttu-id="91521-146">См. также</span><span class="sxs-lookup"><span data-stu-id="91521-146">See Also</span></span>  
 <span data-ttu-id="91521-147">[Функция GET (запись)](/dynamics-nav/GET-Function--Record-)  </span><span class="sxs-lookup"><span data-stu-id="91521-147">[GET Function (Record)](/dynamics-nav/GET-Function--Record-)  </span></span>  
 <span data-ttu-id="91521-148">[Сведения о проектировании: операции набора измерений](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="91521-148">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="91521-149">[Обзор записей набора измерений](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="91521-149">[Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="91521-150">[Сведения о проектировании: структура таблицы](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="91521-150">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 <span data-ttu-id="91521-151">[Сведения о проектировании: Codeunit 408 Dimension Management](design-details-codeunit-408-dimension-management.md) </span><span class="sxs-lookup"><span data-stu-id="91521-151">[Design Details: Codeunit 408 Dimension Management](design-details-codeunit-408-dimension-management.md) </span></span>  
 [<span data-ttu-id="91521-152">Сведения о проектировании: примеры кода измененных шаблонов в модификациях</span><span class="sxs-lookup"><span data-stu-id="91521-152">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)
