---
title: "Сведения о проектировании — обработка политик дозаказа | Документы Майкрософт"
description: "Обзор задач для определения политики повтора заказа при планировании поставок."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 2a6658508f8e12a11989d54da6d6c8e3a36631cc
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-handling-reordering-policies"></a>Сведения о проектировании: обработка политик дозаказа
Чтобы товар мог участвовать в планировании поставок, должна быть определена политика дозаказа. Существует четыре следующих политики повторного заказа.  
  
* Фикс. кол-во повтора заказа  
* Максимальное кол-во  
* Заказ  
* Партия на партию  
  
Политики "Фикс. кол-во дозаказа" и "Максимальное кол-во" относятся к планированию запасов. Хотя планирование запасов технически проще процедуры балансировки, эти политики должны сосуществовать с поэтапной балансировкой поставок и трассировкой заказов. Для контроля интеграции между этими двумя сущностями и обеспечения обзорности соответствующей логики планирования, строгие принципы регулируют работу с политиками повторных заказов.  
  
## <a name="in-this-section"></a>В этом разделе  
[Сведения о проектировании: роль точки дозаказа](design-details-the-role-of-the-reorder-point.md)  
[Сведения о проектировании: отслеживание уровня прогнозируемых запасов и точки дозаказа](design-details-monitoring-the-projected-inventory-level-and-the-reorder-point.md)  
[Сведения о проектировании: роль горизонта планирования](design-details-the-role-of-the-time-bucket.md)  
[Сведения о проектировании: нахождение ниже уровня допустимого избытка](design-details-staying-under-the-overflow-level.md)  
[Сведения о проектировании: обработка прогнозируемых отрицательных остатков](design-details-handling-projected-negative-inventory.md)  
[Сведения о проектировании: политики дозаказа](design-details-reordering-policies.md)  
  
## <a name="see-also"></a>См. также  
[Сведения о проектировании: параметры планирования](design-details-planning-parameters.md)   
[Сведения о проектировании: таблица "Назначение произ. плана"](design-details-planning-assignment-table.md)   
[Сведения о проектировании: основные понятия системы планирования](design-details-central-concepts-of-the-planning-system.md)   
[Сведения о проектировании: балансировка спроса и поставки](design-details-balancing-demand-and-supply.md)   
[Сведения о проектировании: планирование поставок](design-details-supply-planning.md)
