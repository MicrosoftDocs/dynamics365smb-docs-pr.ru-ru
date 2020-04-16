---
title: Сведения о проектировании — структура интерфейса учета | Документация Майкрософт
description: В этом разделе приведен обзор глобальных процедур в структуре интерфейса учета.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: c50f045cf1a379d4fb908e0c17d7b9775fd1a9ee
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3184872"
---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="7c84d-103">Сведения о проектировании: структура интерфейса учета</span><span class="sxs-lookup"><span data-stu-id="7c84d-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="7c84d-104">В структуре интерфейса учета [!INCLUDE[d365fin](includes/d365fin_md.md)] существует несколько глобальных процедур, использующих одну и ту же структуру:</span><span class="sxs-lookup"><span data-stu-id="7c84d-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="7c84d-105">RunWithCheck и RunWithoutCheck вызывают код процедуры — универсальный интерфейс учета для строки финансового</span><span class="sxs-lookup"><span data-stu-id="7c84d-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen.</span></span> <span data-ttu-id="7c84d-106">журнала.</span><span class="sxs-lookup"><span data-stu-id="7c84d-106">Jnl Line.</span></span>  
* <span data-ttu-id="7c84d-107">CustPostApplyCustLedgEntry — учет применения клиента, вызываемого из модуля codeunit 226 CustEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="7c84d-107">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="7c84d-108">VendPostApplyVendLedgEntry — учет применения поставщика, вызываемого из модуля codeunit 227 VendEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="7c84d-108">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="7c84d-109">UnapplyCustLedgEntry — отмена учета применения клиента, вызываемого из модуля codeunit 226 CustEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="7c84d-109">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="7c84d-110">UnapplyVendLedgEntry — отмена учета применения поставщика, вызываемого из модуля codeunit 227 VendEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="7c84d-110">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="7c84d-111">См. также</span><span class="sxs-lookup"><span data-stu-id="7c84d-111">See Also</span></span>  
[<span data-ttu-id="7c84d-112">Сведения о проектировании: структура механизма учета</span><span class="sxs-lookup"><span data-stu-id="7c84d-112">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)