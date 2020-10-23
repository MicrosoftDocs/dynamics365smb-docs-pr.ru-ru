---
title: Сведения о проектировании — обзор строки учета финансового журнала | Документация Майкрософт
description: В этом разделе содержатся подробные сведения о концепциях и принципах, используемых для перегруппировки функции строки учета финансового журнала в Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general journal, posting, codeunit 12
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: aaffac8fe7e10d0155649c960803f65a8136c46d
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3911084"
---
# <a name="design-details-general-journal-post-line"></a><span data-ttu-id="d8fc9-103">Сведения о проектировании: строка учета финансового журнала</span><span class="sxs-lookup"><span data-stu-id="d8fc9-103">Design Details: General Journal Post Line</span></span>
<span data-ttu-id="d8fc9-104">Документация содержит подробные технические сведения о концепциях и принципах, используемых для перегруппировки функции строки учета финансового журнала в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="d8fc9-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="d8fc9-105">В измененном дизайне модуль codeunit 12 проще использовать и поддерживать.</span><span class="sxs-lookup"><span data-stu-id="d8fc9-105">The redesign makes codeunit 12 simpler and more maintainable.</span></span> <span data-ttu-id="d8fc9-106">В начале документа приводится концептуальный обзор переконструирования.</span><span class="sxs-lookup"><span data-stu-id="d8fc9-106">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="d8fc9-107">Затем поясняется техническая архитектура с целью показать изменения, связанные с изменением дизайна.</span><span class="sxs-lookup"><span data-stu-id="d8fc9-107">Then it explains the technical architecture to show the changes that result from the redesign.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="d8fc9-108">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="d8fc9-108">In This Section</span></span>  
[<span data-ttu-id="d8fc9-109">Обзор строки учета финансового журнала</span><span class="sxs-lookup"><span data-stu-id="d8fc9-109">General Journal Post Line Overview</span></span>](design-details-general-journal-post-line-overview.md)  
[<span data-ttu-id="d8fc9-110">Сведения о проектировании: структура интерфейса учета</span><span class="sxs-lookup"><span data-stu-id="d8fc9-110">Design Details: Posting Interface Structure</span></span>](design-details-posting-interface-structure.md)  
[<span data-ttu-id="d8fc9-111">Сведения о проектировании: структура механизма учета</span><span class="sxs-lookup"><span data-stu-id="d8fc9-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)  
[<span data-ttu-id="d8fc9-112">Изменения модуля codeunit 12: сопоставление глобальных переменных для строки учета финансового журнала</span><span class="sxs-lookup"><span data-stu-id="d8fc9-112">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span></span>](design-details-codeunit-12-changes-mapping-global-variables-for-general-journal-post-line.md)  
[<span data-ttu-id="d8fc9-113">Изменения модуля codeunit 12: изменения процедур учета финансовых журналов</span><span class="sxs-lookup"><span data-stu-id="d8fc9-113">Codeunit 12 Changes: Changes in General Journal Post Procedures</span></span>](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)  

## <a name="see-also"></a><span data-ttu-id="d8fc9-114">См. также</span><span class="sxs-lookup"><span data-stu-id="d8fc9-114">See Also</span></span>  
[<span data-ttu-id="d8fc9-115">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="d8fc9-115">Working with General Journals</span></span>](ui-work-general-journals.md)
