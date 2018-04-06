---
title: "Сведения о проектировании — структура интерфейса учета | Документы Майкрософт"
description: "В этом разделе приведен обзор глобальных процедур в структуре интерфейса учета."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 97b1bc02f848d583240a1701e41be4b639422a6c
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="21df6-103">Сведения о проектировании: структура интерфейса учета</span><span class="sxs-lookup"><span data-stu-id="21df6-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="21df6-104">В структуре интерфейса учета [!INCLUDE[d365fin](includes/d365fin_md.md)] существует несколько глобальных процедур, использующих одну и ту же структуру:</span><span class="sxs-lookup"><span data-stu-id="21df6-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="21df6-105">RunWithCheck и RunWithoutCheck вызывают код процедуры — универсальный интерфейс учета для строки финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="21df6-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen. Jnl Line.</span></span>  
* <span data-ttu-id="21df6-106">CustPostApplyCustLedgEntry — учет применения клиента, вызываемого из модуля codeunit 226 CustEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="21df6-106">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="21df6-107">VendPostApplyVendLedgEntry — учет применения поставщика, вызываемого из модуля codeunit 227 VendEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="21df6-107">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="21df6-108">UnapplyCustLedgEntry — отмена учета применения клиента, вызываемого из модуля codeunit 226 CustEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="21df6-108">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="21df6-109">UnapplyVendLedgEntry — отмена учета применения поставщика, вызываемого из модуля codeunit 227 VendEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="21df6-109">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="21df6-110">См. также</span><span class="sxs-lookup"><span data-stu-id="21df6-110">See Also</span></span>  
[<span data-ttu-id="21df6-111">Сведения о проектировании: структура механизма учета</span><span class="sxs-lookup"><span data-stu-id="21df6-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)
