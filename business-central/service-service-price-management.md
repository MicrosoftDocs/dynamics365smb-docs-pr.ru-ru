---
title: "Управление сервисной ценой | Документы Майкрософт"
description: "В этом разделе описывается, как использовать лучшие цены в сервисных заказах, создавать для клиентов персонализированные соглашения по сервисным ценам, повышать эффективность работы обслуживающего персонала и ускорять процесс выставления счетов."
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/28/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 75c50a7044e3494df5aadb90caa1c008a6ac101c
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="service-price-management"></a>Управление сервисной ценой
Функциональные возможности управления сервисной ценой позволяют использовать лучшие цены в сервисных заказах, создавать для клиентов персонализированные соглашения по сервисным ценам, повышать эффективность работы обслуживающего персонала и ускорять процесс выставления счетов.  
  
Управление сервисной ценой позволяет создавать различные группы сервисных цен, чтобы учитывать сервисный товар или группу сервисных товаров, а также тип неисправности, с которой связана сервисная задача. Подобные группы можно настраивать на ограниченный срок или для определенного клиента или валюты. Можно использовать схемы расчета цен как шаблоны, чтобы соотносить каждую отдельную цену с определенным сервисным заданием.  
  
Например, можно назначить определенные товары, которые будут соотноситься с данной сервисной ценой, а также тип необходимых работ. Аналогично можно использовать различные суммы НДС и суммы скидок для разных ценовых групп сервисного обслуживания. Чтобы избежать ошибок при применении цен, можно назначить фиксированную, минимальную или максимальную цену в зависимости от соглашений, заключенных с клиентами.  
  
Перед корректировкой цены для какого-либо сервисного товара по сервисному заказу вам предлагается обзор последствий такой корректировки цены. Можно согласиться с этими результатами или же внести дополнительные изменения, если необходимо получить другой результат. Полная коррекция осуществляется построчно, то есть новые строки при этом не создаются.  
  
И, наконец, стандартный отчет и статистика группы сервисных цен позволяют следить за прибылью по каждой ценовой группе сервисного обслуживания.  
  
## <a name="service-price-adjustment-groups"></a>Группы коррекции цен на сервисное обслуживание  
Группы коррекции цены обслуживания используются для настройки различных типов коррекции цен. Например, можно создать одну группу коррекции сервисной цены, чтобы корректировать цены на запасные части, другую — чтобы корректировать цены на труд, третью — чтобы корректировать цены для себестоимости, и т. д. Можно также указать, относится ли корректировка сервисных цен только к какому-то одному товару или ресурсу, или ко всем товарам и ресурсам.  
  
Каждая группа коррекции сервисной цены содержит информацию об изменениях, которые надо внести в строки сервиса.  
  
Функция коррекции сервисной цены не применяется к сервисным товарам, относящимся к сервисным контрактам. Можно корректировать только сервисные цены на товары, относящиеся к определенному сервисному заказу. Невозможно корректировать цену сервисного товара, находящегося на гарантии. Невозможно корректировать цену сервисного товара из сервисного заказа, если связанная с ним сервисная строка была полностью или частично учтена в составе счета.  
  
При выполнении функции корректировки сервисной цены все скидки в заказе меняются на значения корректировки сервисной цены.  
  
## <a name="service-price-groups"></a>Ценовые группы сервисного обслуживания  
Можно настроить сервисные ценовые группы, чтобы создавать группы сервисных товаров, получающие определенные сервисные цены. После настройки сервисных ценовых групп можно присваивать их сервисным товарам в строках сервисных товаров. Группам сервисных товаров можно также присвоить ценовые группы сервиса.  
  
Прежде чем приписывать сервисную группу цен какому-либо сервисному товару, необходимо определить, к какой сфере проблем, к какой валюте или группе корректировки сервисной цены относится данная ценовая группа сервисного обслуживания. Необходимо указать, до какой суммы можно корректировать сервисную цену, и включает ли эта сумма НДС и скидки. Также следует определить, относится ли эта корректировка к фиксированной сумме или применяется только в определенных условиях.  
  
Когда ценовая группа сервисного обслуживания присвоена некоторому сервисному товару, все специализированные сервисные цены, установленные в этой группе, автоматически применяются к данному сервисному товару.  
  
## <a name="service-pricing"></a>Сервисные цены  
Фактические типы сервисных цен (тип корректировки цены и цена) устанавливаются для комбинации ценовых групп сервиса и ценовых групп клиентов. Для каждого типа сервисной цены выбирается группа корректировки сервисной цены. Также определяется тип коррекции сервисной цены: фиксированная, максимальная или минимальная и фактическая цена.  
  
Например, можно установить типы сервисных цен для ценовой группы радиосервиса. Для клиентов без ценовой группы можно применить сервисные цены с максимальной ценой работы (группа коррекции цены работы). Для клиентов с отдельной ценовой группой можно применить сервисные цены с фиксированной ценой работы (та же группа коррекции цены работы).  
  
## <a name="service-price-adjustment"></a>Коррекции цен на сервисное обслуживание  
Коррекция сервисной цены позволяет корректировать цены для товаров, ресурсов, счета Главной книги или себестоимости по сервисному заказу.  
  
После ввода товара в строку сервисного товара нужно ввести все данные о стоимости данного товара по строкам сервиса. При выполнении функции коррекции сервисной цены следует предварительно просмотреть корректировки цен. При необходимости можно внести дополнительные изменения. Когда все изменения приняты, значения коррекции вычисляются и переводятся в сервисные строки. После этого можно производить учет сервисного заказа.  
  
В зависимости от типа коррекции сервисной цены общая сумма коррекции вычисляется следующим образом:  
  
В следующей таблице приводится описание расчетов.  
  
|Параметр | Описанием |  
|----------------------------------|---------------------------------------|  
|**Фиксированная цена**|Это означает, что для сервисного товара, ресурса, счета главной книги или себестоимости запрашивается фиксированная цена, которая не зависит от реальной себестоимости или стандартной оплаты. Если выбран этот параметр, коррекция сервисной цены не выйдет за пределы суммы, определенной ценовой группы сервиса.|  
|**Максимум**|Это означает, что для клиента устанавливается верхняя граница издержек, независимо от реальной себестоимости или стандартной оплаты. Если выбран этот параметр, коррекция сервисной цены производится только тогда, когда общая цена превышает сумму, указанную для ценовой группы сервиса.|  
|**Минимум**|Это означает, что для клиента устанавливается нижняя граница издержек, независимо от реальной себестоимости или стандартной оплаты. Если выбран этот параметр, коррекция сервисной цены производится только тогда, когда общая сумма оказывается ниже суммы, указанной для ценовой группы сервиса.|  
  
## <a name="see-also"></a>См. также  
[Настройка цен и дополнительных издержек для сервисов](service-how-setup-service-costs-pricing.md)  
[Настройка управления сервисным обслуживанием](service-setup-service.md)  
