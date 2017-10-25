---
title: "Сведения о проектировании — определение приоритета заказов | Документы Майкрософт"
description: "Узнайте, как задавать приоритеты для удовлетворения требований как спроса, так и предложения."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, priority, prioritize, order, sku, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7af645f5a9dd7f34619d05cb2d4f0f7f8ad1921d
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-prioritizing-orders"></a>Сведения о проектировании: определение приоритета заказов
В пределах заданной единицы хранения запрошенная или доступная дата представляет наивысший приоритет; спрос сегодняшнего дня необходимо удовлетворить перед спросом следующей недели. Но в дополнение к этому общему приоритету система планирования предложит тип спроса, который требуется удовлетворить до удовлетворения другого спроса. Аналогично она укажет, какой источник поставки следует применить до применения других источников поставки. Это осуществляется в соответствии с приоритетами заказов.  
  
Загруженный спрос и поставка влияют на профиль для прогнозируемых запасов в соответствии со следующими приоритетами:  
  
## <a name="priorities-on-the-demand-side"></a>Приоритеты на стороне спроса  
1. Уже отгружено: операция книги товаров  
2. Возврат покупки  
3. Заказ на продажу  
4. Сервисный заказ  
5. Требуемый производственный компонент  
6. Строка заказа на сборку  
7. Заказ на исходящее перемещение  
8. Общий заказ (еще не использованный в связанных заказах на продажу)  
9. Прогноз (еще не использованный в других заказах на продажу)  
  
> [!NOTE]  
>  Возвраты покупок обычно не включаются в планирование поставок; они всегда должны резервироваться из партии, которая будет возвращена. Если возвраты покупок не зарезервированы, они играют роль в наличии и имеют высокий приоритет, чтобы система планирования не предлагала заказ на поставку лишь для того, чтобы обслужить возврат покупки.  
  
## <a name="priorities-on-the-supply-side"></a>Приоритеты на стороне поставки  
1. Уже существует на складе: операция книги товаров ("Гибкость планирования" = "Нет")  
2. Возврат продажи ("Гибкость планирования" = "Нет")  
3. Заказ на входящее перемещение  
4. Производственный заказ  
5. Сборочный заказ  
6. Заказ на покупку  
  
## <a name="priority-related-to-the-state-of-demand-and-supply"></a>Приоритет, связанный с состоянием спрос и поставки  
Помимо приоритетов, определяемых типом спроса и поставки, текущее состояние заказов в процессе выполнения также определяет приоритет. Например, складские операции оказывают влияние, и учитывается статус заказов на продажу, покупку, перемещение и сборку:  
  
1. Частично скорректировано ("Гибкость планирования" = "Нет")  
2. Уже обрабатывается на складе ("Гибкость планирования" = "Нет")  
3. Выпущено — все типы заказов ("Гибкость планирования" = "Неограниченно")  
4. Утвержденный производственный заказ ("Гибкость планирования" = "Неограниченно")  
5. Запланировано/открыто — все типы заказов ("Гибкость планирования" = "Неограниченно")  
  
## <a name="see-also"></a>См. также  
[Сведения о проектировании: балансировка спроса и поставки](design-details-balancing-demand-and-supply.md)   
[Сведения о проектировании: основные понятия системы планирования](design-details-central-concepts-of-the-planning-system.md)   
[Сведения о проектировании: планирование поставок](design-details-supply-planning.md)