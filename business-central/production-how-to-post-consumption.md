---
title: "Практическое руководство. Учет потребления в пакетном режиме | Документы Майкрософт"
description: "Если выбран метод списания **Вручную**, учет компонентов производится вручную с использованием журнала потребления."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 4058d16ee3bdfc10933e1f3a01c84fbc5d0b0ebb
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="batch-post-production-consumption"></a>Учет потребления для производства в пакетном режиме
Если выбран метод списания **Вручную**, учет компонентов производится вручную с использованием журнала потребления.

Можно также настроить систему для автоматического учета (*списания*) компонентов при запуске или завершении производственных заказов. Дополнительные сведения см. в разделе [Включение списания компонентов в соответствии с производственным выпуском](production-how-to-flush-components-according-to-operation-output.md).

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a>Учет потребления для одной или нескольких строк производственного заказа  
1.  Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журнал потребления**, затем выберите связанную ссылку.  
2.  Заполните поля данными производственного заказа и данными о потреблении. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    Если склад, на котором хранятся компоненты, настроен на использование ячеек, но не требует обработки подбора, присвойте код ячейки строке журнала для указания места на складе, откуда должны забираться товары. Дополнительные сведения см. в разделе [Подбор для производства или сборки](warehouse-how-to-pick-for-production.md).  
3.  Выберите действие **Учесть**, чтобы учесть потребление. Соответствующие операции в книге товаров уменьшаются.

## <a name="see-also"></a>См. также  
[Производство](production-manage-manufacturing.md)    
[Настройка производства](production-configure-production-processes.md)  
[Планирование](production-planning.md)      
[Наличие](inventory-manage-inventory.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

