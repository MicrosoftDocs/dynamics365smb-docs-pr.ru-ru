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
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: c6b66ecee87e1fd128733f541d46b97f44af0453
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "935663"
---
# <a name="design-details-dimension-set-entries"></a><span data-ttu-id="3b7b0-103">Сведения о проектировании: операции набора измерений</span><span class="sxs-lookup"><span data-stu-id="3b7b0-103">Design Details: Dimension Set Entries</span></span>
<span data-ttu-id="3b7b0-104">Документация содержит подробные технические сведения о концепциях и принципах функции хранения и учета операций измерения в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3b7b0-104">This documentation provides detailed technical insight into the concepts and principles of the dimension-entry storing and posting functionality in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="3b7b0-105">В начале документа приводится концептуальный обзор.</span><span class="sxs-lookup"><span data-stu-id="3b7b0-105">The documentation starts by describing conceptual overviews.</span></span> <span data-ttu-id="3b7b0-106">Затем рассматривается техническая архитектура.</span><span class="sxs-lookup"><span data-stu-id="3b7b0-106">Then it explains the technical architecture.</span></span> <span data-ttu-id="3b7b0-107">Наконец, в ней приводятся примеры кода для подготовки к миграции и обновлению кодов измерений из версий до Dynamics NAV 2013R2.</span><span class="sxs-lookup"><span data-stu-id="3b7b0-107">Finally, it provides code examples to prepare you for dimension code migration and upgrade from versions earlier than Dynamics NAV 2013R2.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="3b7b0-108">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="3b7b0-108">In This Section</span></span>  
[<span data-ttu-id="3b7b0-109">Обзор записей набора измерений</span><span class="sxs-lookup"><span data-stu-id="3b7b0-109">Dimension Set Entries Overview</span></span>](design-details-dimension-set-entries-overview.md)  
[<span data-ttu-id="3b7b0-110">Сведения о проектировании: поиск комбинаций измерений</span><span class="sxs-lookup"><span data-stu-id="3b7b0-110">Design Details: Searching for Dimension Combinations</span></span>](design-details-searching-for-dimension-combinations.md)  
[<span data-ttu-id="3b7b0-111">Сведения о проектировании: структура таблицы</span><span class="sxs-lookup"><span data-stu-id="3b7b0-111">Design Details: Table Structure</span></span>](design-details-table-structure.md)  
[<span data-ttu-id="3b7b0-112">Сведения о проектировании: Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="3b7b0-112">Design Details: Codeunit 408 Dimension Management</span></span>](design-details-codeunit-408-dimension-management.md)  
[<span data-ttu-id="3b7b0-113">Сведения о проектировании: примеры кода измененных шаблонов в модификациях</span><span class="sxs-lookup"><span data-stu-id="3b7b0-113">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)
