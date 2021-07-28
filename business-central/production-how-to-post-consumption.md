---
title: Учет потребления в пакетном режиме
description: Если выбран метод списания "Вручную", учет компонентов производится вручную с использованием журнала потребления.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 2f31c7f48e88a44eb3f437827b6b24f255180d9a
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "6440432"
---
# <a name="batch-post-production-consumption"></a>Учет потребления для производства в пакетном режиме

Если выбран метод списания **Вручную**, учет компонентов производится вручную с использованием журнала потребления.  

>[!NOTE]
> Если в поле **Требуется подбор** в карточке товара установлен флажок для указания необходимости для данного склада обработки подбора запасов, это пакетное задание использовать не нужно. [!INCLUDE[prod_short](includes/prod_short.md)] будет обрабатывать потребление при учете подбора запасов. Дополнительные сведения см. в разделе [Подбор для производства в базовых конфигурациях склада](warehouse-how-to-pick-for-production.md#pick-for-production-in-basic-warehouse-configurations).  

Можно также настроить [!INCLUDE[prod_short](includes/prod_short.md)] для автоматического учета (*списания*) компонентов при запуске или завершении производственных заказов. Дополнительные сведения см. в разделе [Включение списания компонентов в соответствии с производственным выпуском](production-how-to-flush-components-according-to-operation-output.md).

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a>Учет потребления для одной или нескольких строк производственного заказа

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Журнал потребления**, а затем выберите связанную ссылку.  
2. Заполните поля данными производственного заказа и данными о потреблении. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    Используйте действие **Расчет потребления** для создания строк журнала из производственных заказов на основе фактического (учтенное количество готовой продукции) или ожидаемого выпуска продукции (расчетное количество готовой продукции).

    > [!NOTE]
    > Если вы настроили карточку местоположения так, чтобы она требовала обработки комплектования склада, то в поле **Количество** на странице **Журнал потребления** можно ввести только уже скомплектованные количества через действие склада, а не какое-либо рассчитанное количество. Дополнительные сведения см. в разделе [Подбор для производства или сборки в расширенных конфигурациях склада](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md)

3. Выберите действие **Учесть**, чтобы учесть потребление. Соответствующие запасы уменьшаются.

## <a name="see-also"></a>См. также

[Производство](production-manage-manufacturing.md)  
[Настройка производства](production-configure-production-processes.md)  
[Планирование](production-planning.md)  
[Запасы](inventory-manage-inventory.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
