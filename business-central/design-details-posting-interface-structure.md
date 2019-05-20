---
title: Сведения о проектировании — структура интерфейса учета | Документы Майкрософт
description: В этом разделе приведен обзор глобальных процедур в структуре интерфейса учета.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 5905a16341dc487aaf624810d691ac4628ac2e30
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1239525"
---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="bed95-103">Сведения о проектировании: структура интерфейса учета</span><span class="sxs-lookup"><span data-stu-id="bed95-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="bed95-104">В структуре интерфейса учета [!INCLUDE[d365fin](includes/d365fin_md.md)] существует несколько глобальных процедур, использующих одну и ту же структуру:</span><span class="sxs-lookup"><span data-stu-id="bed95-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="bed95-105">RunWithCheck и RunWithoutCheck вызывают код процедуры — универсальный интерфейс учета для строки финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="bed95-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen. Jnl Line.</span></span>  
* <span data-ttu-id="bed95-106">CustPostApplyCustLedgEntry — учет применения клиента, вызываемого из модуля codeunit 226 CustEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="bed95-106">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="bed95-107">VendPostApplyVendLedgEntry — учет применения поставщика, вызываемого из модуля codeunit 227 VendEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="bed95-107">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="bed95-108">UnapplyCustLedgEntry — отмена учета применения клиента, вызываемого из модуля codeunit 226 CustEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="bed95-108">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="bed95-109">UnapplyVendLedgEntry — отмена учета применения поставщика, вызываемого из модуля codeunit 227 VendEntry "Применение учтенных операций".</span><span class="sxs-lookup"><span data-stu-id="bed95-109">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="bed95-110">См. также</span><span class="sxs-lookup"><span data-stu-id="bed95-110">See Also</span></span>  
[<span data-ttu-id="bed95-111">Сведения о проектировании: структура механизма учета</span><span class="sxs-lookup"><span data-stu-id="bed95-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)