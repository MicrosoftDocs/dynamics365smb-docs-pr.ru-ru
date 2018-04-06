---
title: "Результаты перемещения | Документы Майкрософт"
description: "В этом разделе описывается, что происходит после перемещения операций главной книги в операции затрат."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: general ledger, transfer, cost entries
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: d479727b8d0cbb4b4ec9f127136f4e0578b8afb7
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="results-of-transferring-general-ledger-entries-to-cost-entries"></a>Результаты переноса операций главной книги в операции затрат
Во время перемещения операций Главной книги в операции затрат [!INCLUDE[d365fin](includes/d365fin_md.md)] создает связи в записях таблиц **Операция ГК**, **Операция затрат** и **Регистр затрат**, чтобы сделать возможным трассировку подключений между операциями затрат и операциями Главной книги.  

## <a name="general-ledger-entries"></a>Операции главной книги  
Для каждой операции Главной книги, которая перемещается в модель учета затрат, [!INCLUDE[d365fin](includes/d365fin_md.md)] заполняет поле **Номер операции** затрат.  

## <a name="cost-entries"></a>Записи затрат  
Для каждой записи затрат [!INCLUDE[d365fin](includes/d365fin_md.md)] сохраняет номер соответствующей операции Главной книги в поле **Номер операции ГК** в таблице **Операция затрат**.  

Для совмещенных записей затрат [!INCLUDE[d365fin](includes/d365fin_md.md)] сохраняет номер последней операции Главной книги, которой является операция с наибольшим номером.  

Поле **Счет ГК** в таблице **Операция затрат** содержит номер счета главной книги, из которого происходит операция затрат.  

Для единых записей затрат [!INCLUDE[d365fin](includes/d365fin_md.md)] переносит учетный текст из Главной книги в текстовое поле **Описание**. Для совмещенных операций в текстовом поле отображается, что эти операции перенесены как совмещенные. Например, для совокупной месячной записи за октябрь 2013 текст может быть **совокупными записями за октябрь 2013**.  

## <a name="cost-register"></a>Регистр затрат  
В таблице **Регистр затрат** [!INCLUDE[d365fin](includes/d365fin_md.md)] создает запись с перемещением источника из Главной книги. Записи операций записи с номерами первой и последней операции, которые перенесены, в дополнение к номерам первой и последней операции затрат, которые созданы.  

## <a name="see-also"></a>См. также  
[Перенос операций ГК в операции затрат](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md)   
[Критерии для переноса операций главной книги в операции затрат](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md)   
[Автоматическое перемещение и объединенные операции](finance-automatic-transfer-combined-entries.md)   
[Перемещение и операции учета затрат](finance-transfer-and-post-cost-entries.md)  

