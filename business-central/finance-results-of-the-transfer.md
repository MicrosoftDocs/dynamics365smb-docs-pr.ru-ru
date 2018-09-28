---
title: "Результаты перемещения | Документы Майкрософт"
description: "В этом разделе описывается, что происходит после перемещения операций главной книги в операции затрат."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: general ledger, transfer, cost entries
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: d171c7764042cd59fe9ca6e0bbce2b4d3d30f050
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="results-of-transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="3ed7d-103">Результаты переноса операций главной книги в операции затрат</span><span class="sxs-lookup"><span data-stu-id="3ed7d-103">Results of Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="3ed7d-104">Во время перемещения операций Главной книги в операции затрат [!INCLUDE[d365fin](includes/d365fin_md.md)] создает связи в записях таблиц **Операция ГК**, **Операция затрат** и **Регистр затрат**, чтобы сделать возможным трассировку подключений между операциями затрат и операциями Главной книги.</span><span class="sxs-lookup"><span data-stu-id="3ed7d-104">During the transfer of general ledger entries to cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates connections in the entries in the **G/L Entry** table, the **Cost Entry** table, and the **Cost Register** table to make it possible to trace the connections between cost entries and general ledger entries.</span></span>  

## <a name="general-ledger-entries"></a><span data-ttu-id="3ed7d-105">Операции главной книги</span><span class="sxs-lookup"><span data-stu-id="3ed7d-105">General Ledger Entries</span></span>  
<span data-ttu-id="3ed7d-106">Для каждой операции Главной книги, которая перемещается в модель учета затрат, [!INCLUDE[d365fin](includes/d365fin_md.md)] заполняет поле **Номер операции** затрат.</span><span class="sxs-lookup"><span data-stu-id="3ed7d-106">For each general ledger entry that is transferred to cost accounting, [!INCLUDE[d365fin](includes/d365fin_md.md)] fills the cost **Entry No.** field.</span></span>  

## <a name="cost-entries"></a><span data-ttu-id="3ed7d-107">Записи затрат</span><span class="sxs-lookup"><span data-stu-id="3ed7d-107">Cost Entries</span></span>  
<span data-ttu-id="3ed7d-108">Для каждой записи затрат [!INCLUDE[d365fin](includes/d365fin_md.md)] сохраняет номер соответствующей операции Главной книги в поле **Номер операции ГК** в таблице **Операция затрат**.</span><span class="sxs-lookup"><span data-stu-id="3ed7d-108">For each cost entry, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the corresponding general ledger entry in the **G/L Entry No.** field in the **Cost Entry** table.</span></span>  

<span data-ttu-id="3ed7d-109">Для совмещенных записей затрат [!INCLUDE[d365fin](includes/d365fin_md.md)] сохраняет номер последней операции Главной книги, которой является операция с наибольшим номером.</span><span class="sxs-lookup"><span data-stu-id="3ed7d-109">For combined cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the last general ledger entry, which is the entry with the highest entry number.</span></span>  

<span data-ttu-id="3ed7d-110">Поле **Счет ГК** в таблице **Операция затрат** содержит номер счета главной книги, из которого происходит операция затрат.</span><span class="sxs-lookup"><span data-stu-id="3ed7d-110">The **G/L Account** field in the **Cost Entry** table contains the number of the general ledger account that the cost entry came from.</span></span>  

<span data-ttu-id="3ed7d-111">Для единых записей затрат [!INCLUDE[d365fin](includes/d365fin_md.md)] переносит учетный текст из Главной книги в текстовое поле **Описание**.</span><span class="sxs-lookup"><span data-stu-id="3ed7d-111">For single cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] transfers the posting text from the general ledger entry to the **Description** text field.</span></span> <span data-ttu-id="3ed7d-112">Для совмещенных операций в текстовом поле отображается, что эти операции перенесены как совмещенные.</span><span class="sxs-lookup"><span data-stu-id="3ed7d-112">For combined entries, the text field shows these entries are transferred as combined entries.</span></span> <span data-ttu-id="3ed7d-113">Например, для совокупной месячной записи за октябрь 2013 текст может быть **совокупными записями за октябрь 2013**.</span><span class="sxs-lookup"><span data-stu-id="3ed7d-113">For example, for a combined entry for the month of October in 2013, the text can be **Combined Entries, October 2013**.</span></span>  

## <a name="cost-register"></a><span data-ttu-id="3ed7d-114">Регистр затрат</span><span class="sxs-lookup"><span data-stu-id="3ed7d-114">Cost Register</span></span>  
<span data-ttu-id="3ed7d-115">В таблице **Регистр затрат** [!INCLUDE[d365fin](includes/d365fin_md.md)] создает запись с перемещением источника из Главной книги.</span><span class="sxs-lookup"><span data-stu-id="3ed7d-115">In the **Cost Register** table, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates an entry with the source transfer from general ledger.</span></span> <span data-ttu-id="3ed7d-116">Записи операций записи с номерами первой и последней операции, которые перенесены, в дополнение к номерам первой и последней операции затрат, которые созданы.</span><span class="sxs-lookup"><span data-stu-id="3ed7d-116">The entry records the first and last entry numbers of the general ledger entries that are transferred, in addition to the first and last entry numbers of the cost entries that are created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3ed7d-117">См. также</span><span class="sxs-lookup"><span data-stu-id="3ed7d-117">See Also</span></span>  
<span data-ttu-id="3ed7d-118">[Перенос операций ГК в операции затрат](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="3ed7d-118">[Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
<span data-ttu-id="3ed7d-119">[Критерии для переноса операций главной книги в операции затрат](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="3ed7d-119">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
<span data-ttu-id="3ed7d-120">[Автоматическое перемещение и объединенные операции](finance-automatic-transfer-combined-entries.md) </span><span class="sxs-lookup"><span data-stu-id="3ed7d-120">[Automatic Transfer and Combined Entries](finance-automatic-transfer-combined-entries.md) </span></span>  
[<span data-ttu-id="3ed7d-121">Перемещение и операции учета затрат</span><span class="sxs-lookup"><span data-stu-id="3ed7d-121">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  

