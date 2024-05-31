---
title: Сведения о проектировании — структура интерфейса учета
description: В этом разделе приведен обзор глобальных процедур и сведения о дизайне в структуре интерфейса учета.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'posting, interface, design'
ms.date: 06/15/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# Сведения о проектировании: структура интерфейса учета
В структуре интерфейса учета [!INCLUDE[prod_short](includes/prod_short.md)] существует несколько глобальных процедур, использующих одну и ту же структуру:  
  
* RunWithCheck и RunWithoutCheck вызывают код процедуры — универсальный интерфейс учета для строки финансового журнала.  
* CustPostApplyCustLedgEntry — учет применения клиента, вызываемого из модуля codeunit 226 CustEntry "Применение учтенных операций".  
* VendPostApplyVendLedgEntry — учет применения поставщика, вызываемого из модуля codeunit 227 VendEntry "Применение учтенных операций".  
* UnapplyCustLedgEntry — отмена учета применения клиента, вызываемого из модуля codeunit 226 CustEntry "Применение учтенных операций".  
* UnapplyVendLedgEntry — отмена учета применения поставщика, вызываемого из модуля codeunit 227 VendEntry "Применение учтенных операций".  
  
## См. также  
[Сведения о проектировании: структура механизма учета](design-details-posting-engine-structure.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]