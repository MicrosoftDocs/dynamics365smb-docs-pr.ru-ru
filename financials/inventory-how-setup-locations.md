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
ms.date: 01/25/2018
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 57e16fe7d7dd3edd832fb29773fc2a9c13cba153
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="set-up-locations"></a>Настройка складов
Если вы покупаете, храните или продаете товары в нескольких местах или складах, вы должны настроить каждый склад с помощью каточки склада и определить маршруты перемещения.

Затем вы сможете создать строки документа для определенного склада, просмотреть доступность по складу и переместить запасы между складами. Дополнительные сведения см. в разделе [Управление запасами](inventory-manage-inventory.md).

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

Теперь вы можете перемещать складские товары между складами. Дополнительные сведения см. в разделе [Перемещение запасов между складами](inventory-how-transfer-between-locations.md).    

## <a name="see-also"></a>См. также
[Управление запасами](inventory-manage-inventory.md)  
[Перемещение запасов между складами](inventory-how-transfer-between-locations.md)    
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md)  
[Общие бизнес-функции](ui-across-business-areas.md)

