---
title: "Настройка плана счетов | Документы Майкрософт"
description: "Описывает процедуру изменения плана счетов."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: COA, cha of acc
ms.date: 03/28/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 48202a9e9a763dcb22bed9975aa9c4a39d2dc4ae
ms.contentlocale: ru-ru
ms.lasthandoff: 05/04/2017


---
# <a name="setting-up-or-changing-the-chart-of-accounts"></a>Настройка или изменение плана счетов
В плане счетов отображаются счета главной книги, на которых хранятся финансовые данные. [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] включает стандартный план счетов, готовый к использованию в вашей организации.
Однако вы можете изменить счета по умолчанию и добавить новые счета.  

## <a name="adding-or-changing-accounts"></a>Добавление или изменение счетов
В плане счетов вы можете открыть каждый счет ГК и добавить или изменить параметры.

**Примечание**. Вы можете удалить счет главной книги. Однако прежде чем удалять его, должно быть соблюдено следующее:  

* Сальдо счета должно быть нулевым.  
* В окне **Настройка Главной книги** должно быть задано поле **Разрешить удаление счета ГК до**, а на счете не должно быть операций книги в эту дату и после нее.  
* Если в окне **Настройка Главной книги** установлен флажок **Проверка использования счета ГК**, то счет не должен использоваться ни в одной из учетных групп или настроек учета.  

[!INCLUDE[d365fin](includes/d365fin_md.md)] не допускает удаления счета главной книги, на котором хранятся данные, необходимые для плана счетов.  

## <a name="see-also"></a>См. также
[Главная книга и план счетов](finance-general-ledger.md)  
[Управление банковскими счетами](bank-manage-bank-accounts.md)  
[Измерения](finance-dimensions.md)  
[Импорт из других финансовых систем](upload-data.md)  
[Практическое руководство. Работа с кодами GIFI в Канаде](ca-finance-work-gifi-codes.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]
