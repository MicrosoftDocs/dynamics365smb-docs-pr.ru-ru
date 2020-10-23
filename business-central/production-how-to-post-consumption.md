---
title: Практическое руководство. Учет потребления в пакетном режиме | Документация Майкрософт
description: Если выбран метод списания **Вручную**, учет компонентов производится вручную с использованием журнала потребления.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: d4b7f90ac533b3071a8c520eefacf98eddd1faba
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3919117"
---
# <a name="batch-post-production-consumption"></a>Учет потребления для производства в пакетном режиме
Если выбран метод списания **Вручную**, учет компонентов производится вручную с использованием журнала потребления.

Можно также настроить систему для автоматического учета (*списания*) компонентов при запуске или завершении производственных заказов. Дополнительные сведения см. в разделе [Включение списания компонентов в соответствии с производственным выпуском](production-how-to-flush-components-according-to-operation-output.md).

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a>Учет потребления для одной или нескольких строк производственного заказа  
1.  Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал потребления**, затем выберите соответствующую ссылку.  
2.  Заполните поля данными производственного заказа и данными о потреблении. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    Если склад, на котором хранятся компоненты, настроен на использование ячеек, но не требует обработки подбора, присвойте код ячейки строке журнала для указания места на складе, откуда должны забираться товары. Дополнительные сведения см. в разделе [Подбор для производства или сборки](warehouse-how-to-pick-for-production.md).  
3.  Выберите действие **Учесть**, чтобы учесть потребление. Соответствующие операции в книге товаров уменьшаются.

## <a name="see-also"></a>См. также  
[Производство](production-manage-manufacturing.md)    
[Настройка производства](production-configure-production-processes.md)  
[Планирование](production-planning.md)      
[Запасы](inventory-manage-inventory.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
