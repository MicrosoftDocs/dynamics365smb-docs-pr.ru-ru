---
title: "Сведения о проектировании — периоды учета запасов | Документы Майкрософт"
description: "Транзакции или коррекции себестоимости, записанные задним числом, часто влияют на сальдо и количество запасов в учетные периоды, которые могут считаться закрытыми. Это может иметь отрицательный эффект на точность отчетности, особенно в глобальных корпорациях. Функцию периодов инвентаризации можно использовать, чтобы избежать таких проблем, путем открытия или закрытия периодов инвентаризации, чтобы ограничить учет заданным периодом времени."
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
ms.openlocfilehash: 742891cc8037696748b7beb459cc877ea482e2a1
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-inventory-periods"></a>Сведения о проектировании: периоды учета запасов
Транзакции или коррекции себестоимости, записанные задним числом, часто влияют на сальдо и количество запасов в учетные периоды, которые могут считаться закрытыми. Это может иметь отрицательный эффект на точность отчетности, особенно в глобальных корпорациях. Функцию периодов инвентаризации можно использовать, чтобы избежать таких проблем, путем открытия или закрытия периодов инвентаризации, чтобы ограничить учет заданным периодом времени.  

 Учетный период — это период времени, определенный датой окончания, в котором учитываются складские транзакции. После закрытия учетного периода изменения стоимости не могут учитываться в закрытом периоде. Это включает новые операции учета стоимости, ожидаемые операции учета или операции с выставленным счетом, изменение существующих значений и корректировки себестоимости. Однако можно по-прежнему применить к открытой операции книги товаров, которая находится в закрытом периоде. Дополнительные сведения см. в разделе [Сведения о проектировании: применение товара](design-details-item-application.md).  

 Чтобы убедиться, что все транзакционные операции в закрытом периоде являются окончательными, необходимо выполнить следующие условия перед закрытием инвентарного периода.  

-   Все исходящие операции ГК по товарам в этом периоде должны быть закрыты (отрицательные остатки должны отсутствовать).  
-   Все себестоимости товара за период должны быть скорректированы.  
-   Себестоимость всех выпущенных и завершенных производственных заказов за период должна быть скорректирована.  

 При закрытии учетного периода создается операция учетного периода с использованием номера последнего регистра товаров, приходящегося на этот учетный период. Кроме того, дата, время и код пользователя, закрывающего период, записываются в операции учетного периода. Используя эти сведения с последним регистром товара за предыдущий период, можно просмотреть складские транзакции, которые были учтены в учетный период. Также можно снова открыть периоды закрытия склада, если требуется выполнить учет в закрытом периоде. При повторном открытии складского периода создается операция складского периода.  

## <a name="see-also"></a>См. также  
 [Сведения о проектировании: себестоимость запасов](design-details-inventory-costing.md) [Управление себестоимостью товаров](finance-manage-inventory-costs.md) [Финансы](finance.md)  
 [Работа с Financials](ui-work-product.md)
