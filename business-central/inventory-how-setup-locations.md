---
title: Настройка карточки склада и определение маршрутов перемещения | Документация Майкрософт
description: Вы создаете карточку склада для каждого места, где хранятся товары, например для склада или дистрибьюторского центра, а также настраиваете маршруты для перемещения товаров между складами.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 81ee1ad91bd4ec887d85e940152f18e99a6d464c
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3923774"
---
# <a name="set-up-locations"></a>Настройка складов
Если вы покупаете, храните или продаете товары в нескольких местах или складах, вы должны настроить каждый склад с помощью каточки склада и определить маршруты перемещения.

Затем вы сможете создать строки документа для определенного склада, просмотреть доступность по складу и переместить запасы между складами. Дополнительные сведения см. в разделе [Управление запасами](inventory-manage-inventory.md).
<br><br>  
  
> [!Video https://www.microsoft.com/videoplayer/embed/RE4aQvq?rel=0]

## <a name="to-create-a-location-card"></a>Создание карточки склада
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Склады**, затем выберите соответствующую ссылку.
2. Выберите действие **Создать**.
3. На странице **Карточка склада** заполните требуемые поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Повторите шаги 2 и 3 для каждого склада, на котором необходимо хранить запасы.

> [!NOTE]  
> Многие поля в карточке склада относятся к обработке товаров во входящих и исходящих процессах склада. Дополнительные сведения см. в разделе [Настройка управления складом](warehouse-setup-warehouse.md).

## <a name="to-create-a-transfer-route"></a>Создание маршрута перемещения
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Маршруты перемещения**, затем выберите соответствующую ссылку.
2. Либо на любой странице **Карточка склада** выберите действие **Маршруты перемещения**.
3. Выберите действие **Создать**.
4. На странице **Карточка склада** заполните требуемые поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

Теперь вы можете перемещать складские товары между складами. Дополнительные сведения см. в разделе [Перемещение запасов между складами](inventory-how-transfer-between-locations.md).    

## <a name="see-also"></a>См. также
[Управление запасами](inventory-manage-inventory.md)  
[Перемещение запасов между складами](inventory-how-transfer-between-locations.md)    
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Изменение набора отображаемых функций](ui-experiences.md)  
[Общие бизнес-функции](ui-across-business-areas.md)
