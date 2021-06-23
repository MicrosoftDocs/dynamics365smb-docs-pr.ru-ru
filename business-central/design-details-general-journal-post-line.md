---
title: Сведения о проектировании — обзор строки учета финансового журнала | Документация Майкрософт
description: В этом разделе содержатся подробные сведения о концепциях и принципах, используемых для перегруппировки функции строки учета финансового журнала в Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general journal, posting, codeunit 12
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 8492c83437be4cd850bafdaaa5dc70d00a075674
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215232"
---
# <a name="design-details-general-journal-post-line"></a><span data-ttu-id="18c91-103">Сведения о проектировании: строка учета финансового журнала</span><span class="sxs-lookup"><span data-stu-id="18c91-103">Design Details: General Journal Post Line</span></span>

<span data-ttu-id="18c91-104">Документация содержит подробные технические сведения о концепциях и принципах, используемых для перегруппировки функции строки учета финансового журнала в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="18c91-104">This documentation provides detailed technical insight into the concepts and principles that were used to redesign the general journal posting line feature in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="18c91-105">В измененном дизайне модуль codeunit 12 проще использовать и поддерживать.</span><span class="sxs-lookup"><span data-stu-id="18c91-105">The redesign made codeunit 12 simpler and more maintainable.</span></span> <span data-ttu-id="18c91-106">В начале документа приводится концептуальный обзор переконструирования.</span><span class="sxs-lookup"><span data-stu-id="18c91-106">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="18c91-107">Затем поясняется техническая архитектура с целью показать изменения, связанные с изменением дизайна.</span><span class="sxs-lookup"><span data-stu-id="18c91-107">Then it explains the technical architecture to show the changes that result from the redesign.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="18c91-108">Информация в этом разделе относится к переработке в более ранней версии продукта, Microsoft Dynamics NAV 2013 R2.</span><span class="sxs-lookup"><span data-stu-id="18c91-108">The information in this section applies to the redesign in an earlier version of the product, Microsoft Dynamics NAV 2013 R2.</span></span>

## <a name="in-this-section"></a><span data-ttu-id="18c91-109">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="18c91-109">In This Section</span></span>

[<span data-ttu-id="18c91-110">Обзор строки учета финансового журнала</span><span class="sxs-lookup"><span data-stu-id="18c91-110">General Journal Post Line Overview</span></span>](design-details-general-journal-post-line-overview.md)  
[<span data-ttu-id="18c91-111">Сведения о проектировании: структура интерфейса учета</span><span class="sxs-lookup"><span data-stu-id="18c91-111">Design Details: Posting Interface Structure</span></span>](design-details-posting-interface-structure.md)  
[<span data-ttu-id="18c91-112">Сведения о проектировании: структура механизма учета</span><span class="sxs-lookup"><span data-stu-id="18c91-112">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)  

## <a name="see-also"></a><span data-ttu-id="18c91-113">См. также</span><span class="sxs-lookup"><span data-stu-id="18c91-113">See Also</span></span>

<span data-ttu-id="18c91-114">[Работа с финансовыми журналами](ui-work-general-journals.md)
[Сведения о проектировании: строка учета финансового журнала (Dynamics NAV)](/dynamics-nav-app/design-details-general-journal-post-line)</span><span class="sxs-lookup"><span data-stu-id="18c91-114">[Working with General Journals](ui-work-general-journals.md)
[Design Details: General Journal Post Line (Dynamics NAV)](/dynamics-nav-app/design-details-general-journal-post-line)</span></span>  

[!INCLUDE[footer-include](includes/footer-banner.md)]