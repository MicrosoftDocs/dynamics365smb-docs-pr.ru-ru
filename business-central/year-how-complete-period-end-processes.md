---
title: Необязательные действия для закрытия периодов
description: В этом разделе описываются необязательные процессы и действия по закрытию учетных периодов в Business Central.
author: jswymer
ms.topic: overview
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'year closing, close accounting period, close fiscal year, aging, creditor payments, vendor payments'
ms.date: 08/29/2022
ms.author: jswymer
---
# <a name="overview-of-tasks-to-close-accounting-periods"></a><a name="overview-of-tasks-to-close-accounting-periods"></a>Обзор задач по закрытию учетных периодов

[!INCLUDE[prod_short](includes/prod_short.md)] не требует принудительного закрытия периодов, однако предусмотрено множество действий на конец периода (месяца), которые можно выполнить. В этом разделе представлен обзор дополнительных процессов и действий для закрытия периодов.  

## <a name="general-ledger"></a><a name="general-ledger"></a>Главная книга

* Укажите системные и пользовательские периоды учета.  

    Они определяют даты, между которыми возможен учет. В зависимости от бизнеса можно разрешить учет в начале процесса или ближе к концу. Узнайте больше в разделе [Указание периодов учета](finance-how-specify-posting-periods.md).  
* Внесите все необходимые корректировки в главную книгу (ГК).  
* Обновите и учтите типовые журналы.  
  <!--* Process Consolidations-->
* Выполните финансовые отчеты следующим образом:  
  * Откройте страницу **Финансовые отчеты** и выберите действие **Печать**.  

## <a name="sales-and-receivables"></a><a name="sales-and-receivables"></a>Продажи и дебиторская задолженность

* Учтите все заказы на продажу, счета, кредит-ноты и заказы на возврат.  
* Выполните учет всех журналов кассовых поступлений.  
* Обновление и учет типовых журналов, относящихся к продажам и дебиторской задолженности.  
* Выполните выверку дебиторской задолженности с главной книгой.  
* Выполните пакетное задание **Удаление заказов на продажу, по которым выставлены счета**.  

## <a name="purchases-and-payables"></a><a name="purchases-and-payables"></a>Покупки и кредиторская задолженность

* Выполните учет всех заказов на покупку, счетов, кредит-нот и заказов на возврат.  
* Выполните учет всех журналов оплат.  
* Обновление и учет типовых журналов, относящихся к покупкам и кредиторской задолженности.  
* Выполните отчет **Кредиторская задолженность по срокам давности** и проведите выверку кредиторской задолженности с главной книгой.  
* Выполните пакетное задание **Удалить заказы на покупку, по которым выставлены счета**.  

## <a name="fixed-assets"></a><a name="fixed-assets"></a>Основные средства

* Учет всех затрат на обслуживание, учтенных через журналы ОС или счета.
* Учет корректировок.
* Учет повышения стоимости.
* Учет амортизации.
* Обновление и учет типового журнала основных средств.

## <a name="intercompany"></a><a name="intercompany"></a>Межфирменный

* Обработка межфирменных транзакций.

## <a name="calculate-and-process-sales-tax"></a><a name="calculate-and-process-sales-tax"></a>Расчет и обработка налога с продаж

* Заполнение налоговых выписок.  

## <a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/close-fiscal-year-dynamics-365-business-central/)

## <a name="see-also"></a><a name="see-also"></a>См. также

[Закрытие года и периодов](year-close-years-periods.md)  
[Закрытие книг](year-close-books.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
