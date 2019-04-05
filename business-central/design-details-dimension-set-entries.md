---
title: Сведения о проектировании — записи набора измерений | Документы Майкрософт
description: Документация содержит подробные технические сведения о концепциях и принципах, используемых для перегруппировки функции хранения и учета операций измерения.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, dimensions, codeunit
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 5563241784aaf8bfa1a29f8568411be657647cf7
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "804644"
---
# <a name="design-details-dimension-set-entries"></a><span data-ttu-id="3b1cc-103">Сведения о проектировании: операции набора измерений</span><span class="sxs-lookup"><span data-stu-id="3b1cc-103">Design Details: Dimension Set Entries</span></span>
<span data-ttu-id="3b1cc-104">Документация содержит подробные технические сведения о концепциях и принципах, используемых для перегруппировки функции хранения и учета операций измерения в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3b1cc-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the dimension entry storing and posting feature in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="3b1cc-105">В начале документа приводится концептуальный обзор переконструирования.</span><span class="sxs-lookup"><span data-stu-id="3b1cc-105">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="3b1cc-106">Затем поясняется техническая архитектура с целью понять, как осуществляется перегруппировка.</span><span class="sxs-lookup"><span data-stu-id="3b1cc-106">Then it explains the technical architecture to show how the redesign is made.</span></span> <span data-ttu-id="3b1cc-107">Наконец, в ней приводятся примеры кода для подготовки к миграции и обновлению кодов измерений.</span><span class="sxs-lookup"><span data-stu-id="3b1cc-107">Finally, it provides code examples to prepare you for dimension code migration and upgrade.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="3b1cc-108">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="3b1cc-108">In This Section</span></span>  
[<span data-ttu-id="3b1cc-109">Обзор записей набора измерений</span><span class="sxs-lookup"><span data-stu-id="3b1cc-109">Dimension Set Entries Overview</span></span>](design-details-dimension-set-entries-overview.md)  
[<span data-ttu-id="3b1cc-110">Сведения о проектировании: поиск комбинаций измерений</span><span class="sxs-lookup"><span data-stu-id="3b1cc-110">Design Details: Searching for Dimension Combinations</span></span>](design-details-searching-for-dimension-combinations.md)  
[<span data-ttu-id="3b1cc-111">Сведения о проектировании: структура таблицы</span><span class="sxs-lookup"><span data-stu-id="3b1cc-111">Design Details: Table Structure</span></span>](design-details-table-structure.md)  
[<span data-ttu-id="3b1cc-112">Сведения о проектировании: Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="3b1cc-112">Design Details: Codeunit 408 Dimension Management</span></span>](design-details-codeunit-408-dimension-management.md)  
[<span data-ttu-id="3b1cc-113">Сведения о проектировании: примеры кода измененных шаблонов в модификациях</span><span class="sxs-lookup"><span data-stu-id="3b1cc-113">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)
