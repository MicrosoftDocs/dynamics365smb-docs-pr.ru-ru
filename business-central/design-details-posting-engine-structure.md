---
title: Сведения о проектировании — структура механизма учета | Документация Майкрософт
description: Интерфейс учета и некоторые другие функции модуля codeunit 12 используют функции механизма учета для подготовки и вставки записей операций главной книги и операций НДС. Механизм учета также отвечает за создание регистра главной книги.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: d256a3c752b8f236d1cdb67292ca73dcefb7ab05
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3787400"
---
# <a name="design-details-posting-engine-structure"></a>Сведения о проектировании: структура механизма учета
Интерфейс учета и некоторые другие функции модуля codeunit 12 используют функции механизма учета для подготовки и вставки записей операций главной книги и операций НДС. Механизм учета также отвечает за создание регистра главной книги.  
  
 Функции в следующей таблице обеспечивают стандартную структуру для разработки процедур учета (например, Code, CustPostApplyCustledgEntry, VendPostApplyVendLedgEntry, UnapplyCustLedgEntry, UnapplyVendLedgEntry и Reverse) и предоставляют эксклюзивный доступ к таблице 17 "Операция ГК".  
  
|Маршрут|Описание|  
|-------------|---------------------------------------|  
|StartPosting|Инициализирует буфер учета TempGLEntryBuf, блокирует таблицы "Операция ГК" и "Операция НДС" и инициализирует учетный период, регистр ГК и валютный курс. Следует вызывать только один раз; значение NextEntryNo равно 0.|  
|ContinuePosting|Проверяет и учитывает нереализованный НДС для предыдущего приращения транзакции NextTransactionNo, а также подготавливает учет следующей строки.|  
|FinishPosting|Завершает учет, вставляя операции ГК из временного буфера в таблицу базы данных. Всегда используется вместе с StartPosting. Проверяет несогласованности.|  
|InitGLEntry|Используется для инициализации новой операции ГК для строки финансового журнала. Возвращает GLEntry в качестве параметра.|  
|InitGLEntryVAT|Действует аналогично InitGLEntry, но также назначает номер балансового счета и SummarizeVAT.|  
|InitGLEntryVATCopy|Аналогично InitGLEntryVAT, но также копирует данные учетных групп из операции НДС до SummarizeVAT.|  
|InsertGLEntry|Единственная функция, которая вставляет операцию ГК в глобальную таблицу TempGLEntryBuf. Всегда используйте эту функцию для вставки.|  
|CreateGLEntry|Выполняет InitGLEntry, присваивает сумму в ДОВ, а затем выполняет InsertGLEntry. Заменяет несколько строк кода одним вызовом функции.|  
|CreateGLEntryBalAcc|Действует аналогично CreateGLEntry, но также назначает тип балансового счета и номер балансового счета.|  
|CreateGLEntryVAT|Действует аналогично CreateGLEntry, но с дополнительной обработкой учетных групп и сохранением во временном буфере НДС:<br /><br /> `GLEntry.CopyPostingGroupsFromDtldCVBuf(DtldCVLedgEntryBuf,GenJnlLine."Gen. Posting Type");`<br /><br /> `InsertVATEntriesFromTemp(DtldCVLedgEntryBuf,GLEntry);`|  
|CreateGLEntryVATCollectAdj|Действует аналогично CreateGLEntry, но с дополнительной коллекций коррекций и сохранением во временном буфере НДС:<br /><br /> `CollectAdjustment(AdjAmount,GLEntry.Amount,GLEntry."Additional-Currency Amount",OriginalDateSet);`<br /><br /> `InsertVATEntriesFromTemp(DtldCVLedgEntryBuf,GLEntry);`|  
|CreateGLEntryFromVATEntry|Действует аналогично CreateGLEntry, но также копирует учетные группы из операции НДС.|  
  
## <a name="see-also"></a>См. также  
 [Сведения о проектировании: структура интерфейса учета](design-details-posting-interface-structure.md)