---
title: Сведения о проектировании — Codeunit 408 Dimension Management | Microsoft Docs
description: Codeunit 408 Dimension Management — это библиотека функций, обрабатывающих общие задачи, связанные с измерениями, такие как копирование из одной таблицы в другую или из одного документа в другой.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 95d4afc18b0be620df2f4b2067a093237c7c4df2
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "803861"
---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="53709-103">Сведения о проектировании: Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="53709-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="53709-104">Codeunit 408 Dimension Management — это библиотека функций, обрабатывающих общие задачи, связанные с измерениями, такие как копирование из одной таблицы в другую или из одного документа в другой.</span><span class="sxs-lookup"><span data-stu-id="53709-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="53709-105">В этом разделе перечислены изменяемые в Microsoft Dynamics NAV 2013 R2 функции и указано, какие изменения внесены в функции.</span><span class="sxs-lookup"><span data-stu-id="53709-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="53709-106">Множество функций удалено, поскольку нет необходимости копировать данные между таблицами измерений.</span><span class="sxs-lookup"><span data-stu-id="53709-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="53709-107">Измененные функции</span><span class="sxs-lookup"><span data-stu-id="53709-107">Modified Functions</span></span>  

|<span data-ttu-id="53709-108">Имя функции</span><span class="sxs-lookup"><span data-stu-id="53709-108">Function Name</span></span>|<span data-ttu-id="53709-109">Описание изменения</span><span class="sxs-lookup"><span data-stu-id="53709-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="53709-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="53709-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="53709-111">Новая функция, которая заменяет собой другие функции проверки и принимает код набора измерений в качестве аргумента вместо таблицы измерений.</span><span class="sxs-lookup"><span data-stu-id="53709-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="53709-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="53709-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="53709-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="53709-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="53709-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="53709-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="53709-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="53709-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="53709-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="53709-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="53709-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="53709-117">CheckDimValueComb</span></span>|<span data-ttu-id="53709-118">Удаление.</span><span class="sxs-lookup"><span data-stu-id="53709-118">Delete.</span></span> <span data-ttu-id="53709-119">Все потребление должно быть изменено на CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="53709-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="53709-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="53709-120">GetDefaultDim</span></span>|<span data-ttu-id="53709-121">Изменение для возврата кода набора измерений вместо набора записей.</span><span class="sxs-lookup"><span data-stu-id="53709-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="53709-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="53709-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="53709-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="53709-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="53709-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="53709-126">Изменение для работы с DimSetID -> ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="53709-127">Удаленные функции</span><span class="sxs-lookup"><span data-stu-id="53709-127">Deleted Functions</span></span>  
 <span data-ttu-id="53709-128">Функции, удаленные из модуля Codeunit 408 в связи с компонентом "Записи набора измерений", перечислены ниже.</span><span class="sxs-lookup"><span data-stu-id="53709-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="53709-129">В ходе обновления кода приложения с Microsoft Dynamics NAV 2009 или предыдущих версий до Microsoft Dynamics NAV 2016 следующие функции будут недоступны для Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="53709-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="53709-130">Если у вас имеются настройки, использующие какие-либо из этих функций, вам потребуется внести в код соответствующие изменения.</span><span class="sxs-lookup"><span data-stu-id="53709-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="53709-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="53709-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="53709-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="53709-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="53709-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="53709-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="53709-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="53709-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="53709-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="53709-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-136">InsertDocDim</span></span>  

 <span data-ttu-id="53709-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="53709-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="53709-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="53709-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="53709-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="53709-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="53709-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="53709-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="53709-141">InsertServContractDim</span></span>  

 <span data-ttu-id="53709-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="53709-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="53709-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="53709-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="53709-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-144">GetDocDim</span></span>  

 <span data-ttu-id="53709-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-145">GetProdDocDim</span></span>  

 <span data-ttu-id="53709-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="53709-146">TypeToTableID1</span></span>  

 <span data-ttu-id="53709-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="53709-147">TypeToTableID2</span></span>  

 <span data-ttu-id="53709-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="53709-148">TypeToTableID3</span></span>  

 <span data-ttu-id="53709-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="53709-149">TypeToTableID4</span></span>  

 <span data-ttu-id="53709-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="53709-150">TypeToTableID5</span></span>  

 <span data-ttu-id="53709-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="53709-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-152">DeleteDocDim</span></span>  

 <span data-ttu-id="53709-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="53709-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="53709-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="53709-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="53709-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="53709-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="53709-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="53709-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="53709-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="53709-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="53709-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-160">ShowDocDim</span></span>  

 <span data-ttu-id="53709-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-161">SaveDocDim</span></span>  

 <span data-ttu-id="53709-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="53709-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="53709-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="53709-164">ShowTempDim</span></span>  

 <span data-ttu-id="53709-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="53709-165">SaveTempDim</span></span>  

 <span data-ttu-id="53709-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="53709-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="53709-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="53709-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="53709-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="53709-168">SaveServContractDim</span></span>  

 <span data-ttu-id="53709-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="53709-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="53709-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="53709-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="53709-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="53709-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="53709-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="53709-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="53709-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="53709-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="53709-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="53709-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="53709-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="53709-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="53709-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="53709-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="53709-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="53709-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="53709-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="53709-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="53709-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="53709-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="53709-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="53709-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="53709-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="53709-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="53709-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="53709-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="53709-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="53709-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="53709-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="53709-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="53709-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="53709-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="53709-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="53709-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="53709-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="53709-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="53709-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="53709-198">TestDimValue</span></span>  

 <span data-ttu-id="53709-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="53709-199">TestNewDimValue</span></span>  

 <span data-ttu-id="53709-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="53709-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="53709-201">(Удалить, поскольку удалена таблица ItemBudgetDim.)</span><span class="sxs-lookup"><span data-stu-id="53709-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="53709-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="53709-202">GetServContractDim</span></span>  

 <span data-ttu-id="53709-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="53709-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="53709-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="53709-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="53709-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="53709-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="53709-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="53709-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="53709-207">См. также</span><span class="sxs-lookup"><span data-stu-id="53709-207">See Also</span></span>
 <span data-ttu-id="53709-208">[Сведения о проектировании: операции набора измерений](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="53709-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="53709-209">[Сведения о проектировании: обзор операций набора измерений](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="53709-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="53709-210">[Сведения о проектировании: поиск комбинаций измерений](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="53709-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 <span data-ttu-id="53709-211">[Сведения о проектировании: структура таблицы](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="53709-211">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 [<span data-ttu-id="53709-212">Сведения о проектировании: примеры кода измененных шаблонов в модификациях</span><span class="sxs-lookup"><span data-stu-id="53709-212">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)
