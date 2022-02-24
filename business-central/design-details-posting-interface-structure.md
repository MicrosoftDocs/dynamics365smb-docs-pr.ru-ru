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
# <a name="design-details-posting-interface-structure"></a>Сведения о проектировании: структура интерфейса учета
В структуре интерфейса учета [!INCLUDE[d365fin](includes/d365fin_md.md)] существует несколько глобальных процедур, использующих одну и ту же структуру:  
  
* RunWithCheck и RunWithoutCheck вызывают код процедуры — универсальный интерфейс учета для строки финансового журнала.  
* CustPostApplyCustLedgEntry — учет применения клиента, вызываемого из модуля codeunit 226 CustEntry "Применение учтенных операций".  
* VendPostApplyVendLedgEntry — учет применения поставщика, вызываемого из модуля codeunit 227 VendEntry "Применение учтенных операций".  
* UnapplyCustLedgEntry — отмена учета применения клиента, вызываемого из модуля codeunit 226 CustEntry "Применение учтенных операций".  
* UnapplyVendLedgEntry — отмена учета применения поставщика, вызываемого из модуля codeunit 227 VendEntry "Применение учтенных операций".  
  
## <a name="see-also"></a>См. также  
[Сведения о проектировании: структура механизма учета](design-details-posting-engine-structure.md)