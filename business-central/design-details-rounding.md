---
title: Сведения о проектировании — округление | Документация Майкрософт
description: Округление остатков может быть выполнено при переоценке себестоимости расхода склада, измеренного при количестве, отличном от соответствующего прихода склада. Округление остатков рассчитываются для всех методов учета себестоимости при выполнении пакетного задания **Коррекция себест. запасов**.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: d8fac07df8d83b46a6ab8ed4d20a50a81c0731d5
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "6214857"
---
# <a name="design-details-rounding"></a>Сведения о проектировании: округление
Округление остатков может быть выполнено при переоценке себестоимости расхода склада, измеренного при количестве, отличном от соответствующего прихода склада. Округление остатков рассчитываются для всех методов учета себестоимости при выполнении пакетного задания **Коррекция себест. запасов**.  

 При использовании метода средней стоимости округление остатка вычисляется и записывается в накопительном режиме, по отдельным операциям.  

 При использовании метода учета затрат, отличного от метода средней стоимости округление остатка рассчитывается, когда приход склада полностью применен, то есть когда остающееся количество для складского прихода равно нулю. Затем создается отдельная операция для округления остатка, и датой учета этой операции округления является дата учета последней операции стоимости, за которую выставлен счет, прихода склада.  

## <a name="example"></a>Пример  
 В следующем примере показано, как разные остатки округления обрабатываются в методе учета средней себестоимости и методе учета себестоимости без среднего соответственно. В обоих случаях было выполнено пакетное задание **Коррекция себест. запасов**.  

 В следующей таблице показаны операции журнала товаров, используемые в этих примерах.  

|Дата учета|Количество|Номер операции|  
|------------------|--------------|---------------|  
|01-01-20|3|1|  
|02-01-20|-1|2|  
|03-01-20|-1|3|  
|04-01-20|-1|4|  

 Для товара, использующего метод учета себестоимости "По средней", округление остатка (1/300) рассчитывается с первоначальным уменьшением (операция номер 2) и переносится в операцию номер 3. Следовательно, операция номер 3 оценивается как 3,34.  

 В следующей таблице показаны результирующие операции стоимости.  

|Дата учета|Количество|Сумма себестоимости (факт.)|Номер товарной операции|Номер операции|  
|------------------|--------------|----------------------------|---------------------------|---------------|  
|01-01-20|3|10|1|1|  
|02-01-20|-1|-3,33|2|2|  
|03-01-20|-1|-3,34|3|3|  
|04-01-20|-1|-3,33|4|4|  

 Для товара, использующего метод учета себестоимости, отличный от "По средней", округление остатка (0,01) рассчитывается, если оставшееся количество для прихода склада равно нулю. Округление остатка имеет отдельную операцию (номер 5).  

 В следующей таблице показаны результирующие операции стоимости.  

|Дата учета|Количество|Сумма себестоимости (факт.)|Номер товарной операции|Номер операции|  
|------------------|--------------|----------------------------|---------------------------|---------------|  
|01-01-20|3|10|1|1|  
|02-01-20|-1|-3,33|2|2|  
|03-01-20|-1|-3,33|3|3|  
|04-01-20|-1|-3,33|4|4|  
|01-01-20|0|-0,01|1|5|  

## <a name="see-also"></a>См. также  
 [Сведения о проектировании: себестоимость запасов](design-details-inventory-costing.md)   
 [Сведения о проектировании: коррекция себестоимости](design-details-cost-adjustment.md)   
 [Сведения о проектировании: методы учета себестоимости](design-details-costing-methods.md) [Управление себестоимостью товаров](finance-manage-inventory-costs.md)  
 [Финансы](finance.md)  
 [Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]