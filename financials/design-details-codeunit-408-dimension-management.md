---
title: "Сведения о проектировании — Codeunit 408 Dimension Management | Microsoft Docs"
description: "Codeunit 408 Dimension Management — это библиотека функций, обрабатывающих общие задачи, связанные с измерениями, такие как копирование из одной таблицы в другую или из одного документа в другой."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 32f67c058570f03d4aa1c84d9bb32289b1f07bec
ms.contentlocale: ru-ru
ms.lasthandoff: 11/10/2017

---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="1b064-103">Сведения о проектировании: Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="1b064-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="1b064-104">Codeunit 408 Dimension Management — это библиотека функций, обрабатывающих общие задачи, связанные с измерениями, такие как копирование из одной таблицы в другую или из одного документа в другой.</span><span class="sxs-lookup"><span data-stu-id="1b064-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="1b064-105">В этом разделе перечислены изменяемые в Microsoft Dynamics NAV 2013 R2 функции и указано, какие изменения внесены в функции.</span><span class="sxs-lookup"><span data-stu-id="1b064-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="1b064-106">Множество функций удалено, поскольку нет необходимости копировать данные между таблицами измерений.</span><span class="sxs-lookup"><span data-stu-id="1b064-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="1b064-107">Измененные функции</span><span class="sxs-lookup"><span data-stu-id="1b064-107">Modified Functions</span></span>  

|<span data-ttu-id="1b064-108">Имя функции</span><span class="sxs-lookup"><span data-stu-id="1b064-108">Function Name</span></span>|<span data-ttu-id="1b064-109">Описание изменения</span><span class="sxs-lookup"><span data-stu-id="1b064-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="1b064-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="1b064-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="1b064-111">Новая функция, которая заменяет собой другие функции проверки и принимает код набора измерений в качестве аргумента вместо таблицы измерений.</span><span class="sxs-lookup"><span data-stu-id="1b064-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="1b064-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="1b064-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="1b064-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="1b064-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="1b064-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="1b064-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="1b064-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="1b064-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="1b064-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="1b064-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="1b064-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="1b064-117">CheckDimValueComb</span></span>|<span data-ttu-id="1b064-118">Удаление.</span><span class="sxs-lookup"><span data-stu-id="1b064-118">Delete.</span></span> <span data-ttu-id="1b064-119">Все потребление должно быть изменено на CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="1b064-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="1b064-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="1b064-120">GetDefaultDim</span></span>|<span data-ttu-id="1b064-121">Изменение для возврата кода набора измерений вместо набора записей.</span><span class="sxs-lookup"><span data-stu-id="1b064-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="1b064-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="1b064-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="1b064-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="1b064-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="1b064-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="1b064-126">Изменение для работы с DimSetID -> ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="1b064-127">Удаленные функции</span><span class="sxs-lookup"><span data-stu-id="1b064-127">Deleted Functions</span></span>  
 <span data-ttu-id="1b064-128">Функции, удаленные из модуля Codeunit 408 в связи с компонентом "Записи набора измерений", перечислены ниже.</span><span class="sxs-lookup"><span data-stu-id="1b064-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="1b064-129">В ходе обновления кода приложения с Microsoft Dynamics NAV 2009 или предыдущих версий до Microsoft Dynamics NAV 2016 следующие функции будут недоступны для Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="1b064-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="1b064-130">Если у вас имеются настройки, использующие какие-либо из этих функций, вам потребуется внести в код соответствующие изменения.</span><span class="sxs-lookup"><span data-stu-id="1b064-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="1b064-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="1b064-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="1b064-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="1b064-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="1b064-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="1b064-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="1b064-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="1b064-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="1b064-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="1b064-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-136">InsertDocDim</span></span>  

 <span data-ttu-id="1b064-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="1b064-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="1b064-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="1b064-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="1b064-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="1b064-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="1b064-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="1b064-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="1b064-141">InsertServContractDim</span></span>  

 <span data-ttu-id="1b064-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="1b064-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="1b064-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="1b064-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="1b064-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-144">GetDocDim</span></span>  

 <span data-ttu-id="1b064-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-145">GetProdDocDim</span></span>  

 <span data-ttu-id="1b064-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="1b064-146">TypeToTableID1</span></span>  

 <span data-ttu-id="1b064-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="1b064-147">TypeToTableID2</span></span>  

 <span data-ttu-id="1b064-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="1b064-148">TypeToTableID3</span></span>  

 <span data-ttu-id="1b064-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="1b064-149">TypeToTableID4</span></span>  

 <span data-ttu-id="1b064-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="1b064-150">TypeToTableID5</span></span>  

 <span data-ttu-id="1b064-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="1b064-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-152">DeleteDocDim</span></span>  

 <span data-ttu-id="1b064-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="1b064-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="1b064-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="1b064-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="1b064-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="1b064-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="1b064-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="1b064-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="1b064-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="1b064-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="1b064-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-160">ShowDocDim</span></span>  

 <span data-ttu-id="1b064-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-161">SaveDocDim</span></span>  

 <span data-ttu-id="1b064-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="1b064-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="1b064-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="1b064-164">ShowTempDim</span></span>  

 <span data-ttu-id="1b064-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="1b064-165">SaveTempDim</span></span>  

 <span data-ttu-id="1b064-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="1b064-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="1b064-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="1b064-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="1b064-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="1b064-168">SaveServContractDim</span></span>  

 <span data-ttu-id="1b064-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="1b064-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="1b064-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="1b064-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="1b064-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="1b064-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="1b064-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="1b064-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="1b064-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="1b064-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="1b064-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="1b064-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="1b064-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="1b064-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="1b064-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="1b064-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="1b064-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="1b064-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="1b064-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="1b064-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="1b064-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="1b064-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="1b064-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="1b064-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="1b064-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="1b064-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="1b064-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="1b064-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="1b064-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="1b064-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="1b064-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="1b064-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="1b064-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="1b064-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="1b064-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="1b064-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="1b064-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="1b064-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="1b064-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="1b064-198">TestDimValue</span></span>  

 <span data-ttu-id="1b064-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="1b064-199">TestNewDimValue</span></span>  

 <span data-ttu-id="1b064-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="1b064-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="1b064-201">(Удалить, поскольку удалена таблица ItemBudgetDim.)</span><span class="sxs-lookup"><span data-stu-id="1b064-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="1b064-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="1b064-202">GetServContractDim</span></span>  

 <span data-ttu-id="1b064-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="1b064-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="1b064-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="1b064-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="1b064-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="1b064-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="1b064-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="1b064-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="1b064-207">См. также</span><span class="sxs-lookup"><span data-stu-id="1b064-207">See Also</span></span>
 <span data-ttu-id="1b064-208">[Сведения о проектировании: операции набора измерений](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="1b064-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="1b064-209">[Сведения о проектировании: обзор операций набора измерений](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="1b064-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="1b064-210">[Сведения о проектировании: поиск комбинаций измерений](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="1b064-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 <span data-ttu-id="1b064-211">[Сведения о проектировании: структура таблицы](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="1b064-211">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 [<span data-ttu-id="1b064-212">Сведения о проектировании: примеры кода измененных шаблонов в модификациях</span><span class="sxs-lookup"><span data-stu-id="1b064-212">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)

