---
title: "Настройка карточки склада и определение маршрутов перемещения | Документы Майкрософт"
description: "Вы создаете карточку склада для каждого места, где хранятся товары, например для склада или дистрибьюторского центра, а также настраиваете маршруты для перемещения товаров между складами."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7d82b1c63bb1da367736f8dd044640b583493af8
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-locations"></a>Практическое руководство. Настройка складов
Если вы покупаете, храните или продаете товары в нескольких местах или складах, вы должны настроить каждый склад с помощью каточки склада и определить маршруты перемещения.

Затем вы сможете создать строки документа для определенного склада, просмотреть доступность по складу и переместить запасы между складами. Дополнительные сведения см. в разделе [Управление запасами](inventory-manage-inventory.md).

> [!NOTE]  
>   Эта функция требует, чтобы было задано значение **Suite**. Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).

## <a name="to-create-a-location-card"></a>Создание карточки склада
1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Склады**, а затем выберите связанную ссылку.
2. Выберите действие **Создать**.
3. В окне **Карточка склада** заполните требуемые поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Повторите шаги 2 и 3 для каждого склада, на котором необходимо хранить запасы.

> [!NOTE]  
> Многие поля в карточке склада относятся к обработке товаров во входящих и исходящих процессах склада. Дополнительные сведения см. в разделе [Настройка управления складом](warehouse-setup-warehouse.md). 

## <a name="to-create-a-transfer-route"></a>Создание маршрута перемещения
1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Маршруты перемещения**, а затем выберите связанную ссылку.
2. Либо в любом окне **Карточка склада** выберите действие **Маршруты перемещения**.
3. Выберите действие **Создать**.
4. В окне **Карточка склада** заполните требуемые поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

Теперь вы можете перемещать складские товары между складами. Дополнительные сведения см. в разделе [Практическое руководство. Перемещение запасов между складами](inventory-how-transfer-between-locations.md).    

## <a name="see-also"></a>См. также
[Управление запасами](inventory-manage-inventory.md)  
[Практическое руководство. Перемещение запасов между складами](inventory-how-transfer-between-locations.md)    
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md)  
[Общие бизнес-функции](ui-across-business-areas.md)

