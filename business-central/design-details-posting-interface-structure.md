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
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 236cbcc45ccca23905dcb79a491236c80b2bdebf
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "804534"
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