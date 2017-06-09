---
title: "Закрытие периодов | Документы Майкрософт"
description: "Содержит описание процессов закрытия периодов."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, aging, creditor payments, vendor payments
ms.date: 03/21/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 1d0af3dbc94c32447facfbd24747ddc140cc1691
ms.contentlocale: ru-ru
ms.lasthandoff: 05/04/2017


---
# <a name="closing-periods"></a>Закрытие периодов
[!INCLUDE[d365fin](includes/d365fin_md.md)] не требует принудительного закрытия периодов, однако предусмотрено множество действий на конец периода (месяца), которые можно выполнить. В этом разделе представлен обзор дополнительных процессов и действий для закрытия периодов.  

## <a name="general-ledger"></a>Главная книга
* Укажите системные и пользовательские периоды учета.  

    Они определяют даты, между которыми возможен учет. В зависимости от бизнеса можно разрешить учет в начале процесса или ближе к концу. Дополнительные сведения см. в разделе [Практическое руководство. Определение периодов учета](finance-how-specify-posting-periods.md).  
* Внесите все необходимые корректировки в ГК.  
* Обновите и учтите типовые журналы.  
  <!--* Process Consolidations-->
* Создайте финансовые отчеты следующим образом:  
  * Откройте окно **Финансовый отчет** и выберите действие **Печать**.  

## <a name="sales-and-receivables"></a>Продажи и дебиторская задолженность
* Учтите все заказы на продажу, счета, кредит-ноты и заказы на возврат.  
* Выполните учет всех журналов кассовых поступлений.  
* Выполните обновление и учет типовых журналов, относящихся к продажам и расчетам с дебиторами.  
* Выполните выверку дебиторской задолженности с главной книгой.  
* Выполните пакетное задание **Удаление заказов на продажу, по которым выставлены счета**.  

## <a name="purchases-and-payables"></a>Покупки и кредиторская задолженность
* Выполните учет всех заказов на покупку, счетов, кредит-нот и заказов на возврат.  
* Выполните учет всех журналов оплат.  
* Выполните обновление и учет типовых журналов, относящихся к покупкам и расчетам с кредиторами.  
* Выполните отчет **Кредиторская задолженность по срокам давности** и проведите выверку кредиторской задолженности с главной книгой.  
* Выполните пакетное задание **Удалить заказы на покупку, по которым выставлены счета**.  

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a>Расчет и обработка налога с продаж
* Завершите отчеты по НДС.  

## <a name="see-also"></a>См. также
[Закрытие года и периодов](year-close-years-periods.md)  
[Закрытие книг](year-close-books.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

