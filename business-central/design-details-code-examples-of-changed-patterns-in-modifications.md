---
title: 'Сведения о проектировании: примеры кода измененных шаблонов в модификациях | Документация Майкрософт'
description: Примеры кода, показывающие измененные шаблоны при модификации и миграции кода измерения для пяти разных сценариев. В нем сравниваются примеры кода в более ранних версиях с примерами кода в Business Central.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: design-details-dimension-set-entries
ms.openlocfilehash: d4ed71c8c196ea6beff49f7a40fc1605fe999abd
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2303728"
---
# <a name="design-details-code-examples-of-changed-patterns-in-modifications"></a><span data-ttu-id="0ccb4-104">Сведения о проектировании: примеры кода измененных шаблонов в модификациях</span><span class="sxs-lookup"><span data-stu-id="0ccb4-104">Design Details: Code Examples of Changed Patterns in Modifications</span></span>
<span data-ttu-id="0ccb4-105">В этом разделе приводятся примеры кода, чтобы отобразить измененные шаблоны при модификации и миграции кода измерения для пяти разных сценариев.</span><span class="sxs-lookup"><span data-stu-id="0ccb4-105">This topic provides code examples to show changed patterns in dimension code modification and migration for five different scenarios.</span></span> <span data-ttu-id="0ccb4-106">В нем сравниваются примеры кода в более ранних версиях с примерами кода в Business Central.</span><span class="sxs-lookup"><span data-stu-id="0ccb4-106">It compares the code examples in earlier versions to the code examples in Business Central.</span></span>

## <a name="posting-a-journal-line"></a><span data-ttu-id="0ccb4-107">Учет строки журнала</span><span class="sxs-lookup"><span data-stu-id="0ccb4-107">Posting a Journal Line</span></span>  
<span data-ttu-id="0ccb4-108">Ключевые изменения перечислены следующим образом:</span><span class="sxs-lookup"><span data-stu-id="0ccb4-108">Key changes are listed as follows:</span></span>  

- <span data-ttu-id="0ccb4-109">Таблицы измерений строки журнала удаляются.</span><span class="sxs-lookup"><span data-stu-id="0ccb4-109">Journal line dimension tables are removed.</span></span>  

- <span data-ttu-id="0ccb4-110">Код набора измерений создается в поле **Код набора измерений**.</span><span class="sxs-lookup"><span data-stu-id="0ccb4-110">A dimension set ID is created in the **Dimension Set ID** field.</span></span>  

<span data-ttu-id="0ccb4-111">**Более ранние версии**</span><span class="sxs-lookup"><span data-stu-id="0ccb4-111">**Earlier Versions**</span></span>  

```  
ResJnlLine."Qty. per Unit of Measure" :=   
  SalesLine."Qty. per Unit of Measure";  

TempJnlLineDim.DELETEALL;  
TempDocDim.RESET;  
TempDocDim.SETRANGE(  
  "Table ID",DATABASE::"Sales Line");  
TempDocDim.SETRANGE(  
  "Line No.",SalesLine."Line No.");  
DimMgt.CopyDocDimToJnlLineDim(  
  TempDocDim,TempJnlLineDim);  
ResJnlPostLine.RunWithCheck(  
  ResJnlLine,TempJnlLineDim);  

```  

 **[!INCLUDE[d365fin](includes/d365fin_md.md)]**  

```  

ResJnlLine."Qty. per Unit of Measure" :=   
  SalesLine."Qty. per Unit of Measure";  

ResJnlLine."Dimension Set ID" :=   
  SalesLine." Dimension Set ID ";  
ResJnlPostLine.Run(ResJnlLine);  

```  

## <a name="posting-a-document"></a><span data-ttu-id="0ccb4-112">Учет документа</span><span class="sxs-lookup"><span data-stu-id="0ccb4-112">Posting a Document</span></span>  
 <span data-ttu-id="0ccb4-113">При учете документа в [!INCLUDE[d365fin](includes/d365fin_md.md)] более не требуется копировать измерения документов.</span><span class="sxs-lookup"><span data-stu-id="0ccb4-113">When you post a document in [!INCLUDE[d365fin](includes/d365fin_md.md)], you no longer have to copy the document dimensions.</span></span>  

 <span data-ttu-id="0ccb4-114">**Более ранние версии**</span><span class="sxs-lookup"><span data-stu-id="0ccb4-114">**Earlier Versions**</span></span>  

```  
DimMgt.MoveOneDocDimToPostedDocDim(  
  TempDocDim,DATABASE::"Sales Line",  
  "Document Type",  
  "No.",  
  SalesShptLine."Line No.",  
  DATABASE::"Sales Shipment Line",  
  SalesShptHeader."No.");  
```  

 **[!INCLUDE[d365fin](includes/d365fin_md.md)]**  

```  
SalesShptLine."Dimension Set ID”  
  := SalesLine."Dimension Set ID”  
```  

## <a name="editing-dimensions-from-a-document"></a><span data-ttu-id="0ccb4-115">Изменение измерений из документа</span><span class="sxs-lookup"><span data-stu-id="0ccb4-115">Editing Dimensions from a Document</span></span>  
 <span data-ttu-id="0ccb4-116">Можно редактировать измерения из документа.</span><span class="sxs-lookup"><span data-stu-id="0ccb4-116">You can edit dimensions from a document.</span></span> <span data-ttu-id="0ccb4-117">Например, можно изменить строку заказа на продажу.</span><span class="sxs-lookup"><span data-stu-id="0ccb4-117">For example, you can edit a sales order line.</span></span>  

 <span data-ttu-id="0ccb4-118">**Более ранние версии**</span><span class="sxs-lookup"><span data-stu-id="0ccb4-118">**Earlier Versions**</span></span>  

```  
Table 37, function ShowDimensions:  
TESTFIELD("Document No.");  
TESTFIELD("Line No.");  
DocDim.SETRANGE("Table ID",DATABASE::"Sales Line");  
DocDim.SETRANGE("Document Type","Document Type");  
DocDim.SETRANGE("Document No.","Document No.");  
DocDim.SETRANGE("Line No.","Line No.");  
DocDimensions.SETTABLEVIEW(DocDim);  
DocDimensions.RUNMODAL;  
```  

 **[!INCLUDE[d365fin](includes/d365fin_md.md)]**  

```  
Table 37, function ShowDimensions:  
"Dimension ID" :=   
  DimSetEntry.EditDimensionSet(  
    "Dimension ID");  
```  

## <a name="showing-dimensions-from-posted-entries"></a><span data-ttu-id="0ccb4-119">Отображение измерений из учтенных операций</span><span class="sxs-lookup"><span data-stu-id="0ccb4-119">Showing Dimensions from Posted Entries</span></span>  
 <span data-ttu-id="0ccb4-120">Можно отобразить измерения из учтенных операций, например строки расходной накладной.</span><span class="sxs-lookup"><span data-stu-id="0ccb4-120">You can show dimensions from posted entries, such as sales shipment lines.</span></span>  

 <span data-ttu-id="0ccb4-121">**Более ранние версии**</span><span class="sxs-lookup"><span data-stu-id="0ccb4-121">**Earlier Versions**</span></span>  

```  
Table 111, function ShowDimensions:  
TESTFIELD("No.");  
TESTFIELD("Line No.");  
PostedDocDim.SETRANGE(  
  "Table ID",DATABASE::"Sales Shipment Line");  
PostedDocDim.SETRANGE(  
  "Document No.","Document No.");  
PostedDocDim.SETRANGE("Line No.","Line No.");  
PostedDocDimensions.SETTABLEVIEW(PostedDocDim);  
PostedDocDimensions.RUNMODAL;  
```  

 **[!INCLUDE[d365fin](includes/d365fin_md.md)]**  

```  
Table 111, function ShowDimensions:  
DimSetEntry.ShowDimensionSet(  
  "Dimension ID");  
```  

## <a name="getting-default-dimensions-for-a-document"></a><span data-ttu-id="0ccb4-122">Получение измерений по умолчанию для документа</span><span class="sxs-lookup"><span data-stu-id="0ccb4-122">Getting Default Dimensions for a Document</span></span>  
 <span data-ttu-id="0ccb4-123">Можно получить измерения по умолчанию для документа, например строку заказа на продажу.</span><span class="sxs-lookup"><span data-stu-id="0ccb4-123">You can get default dimensions for a document, such as a sales order line.</span></span>  

 <span data-ttu-id="0ccb4-124">**Более ранние версии**</span><span class="sxs-lookup"><span data-stu-id="0ccb4-124">**Earlier Versions**</span></span>  

```  
Table 37, function CreateDim()  
SourceCodeSetup.GET;  
TableID[1] := Type1;  
No[1] := No1;  
TableID[2] := Type2;  
No[2] := No2;  
TableID[3] := Type3;  
No[3] := No3;  
"Shortcut Dimension 1 Code" := '';  
"Shortcut Dimension 2 Code" := '';  
DimMgt.GetPreviousDocDefaultDim(  
  DATABASE::"Sales Header","Document Type",  
  "Document No.",0,  
  DATABASE::Customer,  
  "Shortcut Dimension 1 Code",  
  "Shortcut Dimension 2 Code");  
DimMgt.GetDefaultDim(  
  TableID,No,SourceCodeSetup.Sales,  
  "Shortcut Dimension 1 Code",  
  "Shortcut Dimension 2 Code");  
IF "Line No." <> 0 THEN  
  DimMgt.UpdateDocDefaultDim(  
    DATABASE::"Sales Line","Document Type",  
    "Document No.","Line No.",  
    "Shortcut Dimension 1 Code",  
    "Shortcut Dimension 2 Code");  
```  

 **[!INCLUDE[d365fin](includes/d365fin_md.md)]**  

```  
Table 37, function CreateDim()  
SourceCodeSetup.GET;  
TableID[1] := Type1;  
No[1] := No1;  
TableID[2] := Type2;  
No[2] := No2;  
TableID[3] := Type3;  
No[3] := No3;  
"Shortcut Dimension 1 Code" := '';  
"Shortcut Dimension 2 Code" := '';  
GetSalesHeader;  
"Dimension ID" :=  
  DimMgt.GetDefaultDimID(  
    TableID,No,SourceCodeSetup.Sales,  
    "Shortcut Dimension 1 Code",  
    "Shortcut Dimension 2 Code",  
    SalesHeader."Dimension ID",  
    DATABASE::"Sales Header");

```  

## <a name="see-also"></a><span data-ttu-id="0ccb4-125">См. также</span><span class="sxs-lookup"><span data-stu-id="0ccb4-125">See Also</span></span>  
<span data-ttu-id="0ccb4-126">[Сведения о проектировании: операции набора измерений](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="0ccb4-126">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
[<span data-ttu-id="0ccb4-127">Сведения о проектировании: структура таблицы</span><span class="sxs-lookup"><span data-stu-id="0ccb4-127">Design Details: Table Structure</span></span>](design-details-table-structure.md)   
