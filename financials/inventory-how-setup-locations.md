---
title: "Практическое руководство. Настройка складов | Документы Майкрософт"
description: "Описывается процедура создания карточки склада для каждого местонахождения или склада, на котором хранятся складские товары, включая правила по перемещению товаров на каждый склад и из него."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 03/28/2017
ms.author: SorenGP
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 9a71dfc20cde7469772d438a0fbb520fbb0bbd9a
ms.contentlocale: ru-ru
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-set-up-locations"></a>Как настроить склады
Если вы покупаете, храните или продаете товары в нескольких местах или складах, вы должны настроить каждый склад с помощью каточки склада и определить маршруты перемещения.

Затем вы сможете создать строки документа для определенного склада, просмотреть доступность по складу и переместить запасы между складами. Дополнительные сведения см. в разделе [Управление запасами](inventory-manage-inventory.md).

**Примечание**. Эта функция требует, чтобы было задано значение **Пакет**. Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).

## <a name="to-create-a-location-card"></a>Создание карточки склада
1. В правом вернем углу щелкните значок **Поиск страницы или отчета** ![Поиск страницы или отчета](media/ui-search/search_small.png "значок "Поиск страницы или отчета""), введите **Склады** и выберите связанную ссылку.
2. Выберите действие **Создать**.
3. В окне **Карточка склада** заполните требуемые поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Повторите шаги 2 и 3 для каждого склада, на котором необходимо хранить запасы.

## <a name="to-create-a-transfer-route"></a>Создание маршрута перемещения
1. В правом вернем углу щелкните значок **Поиск страницы или отчета** ![Поиск страницы или отчета](media/ui-search/search_small.png "значок "Поиск страницы или отчета""), введите **Маршруты перемещения** и выберите связанную ссылку.
2. Либо в любом окне **Карточка склада** выберите действие **Маршруты перемещения**.
3. Выберите действие **Создать**.
4. В окне **Карточка склада** заполните требуемые поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

Теперь вы можете перемещать складские товары между складами. Дополнительные сведения см. в разделе [Практическое руководство. Перемещение запасов между складами](inventory-how-transfer-between-locations.md).    

## <a name="see-also"></a>См. также
[Управление запасами](inventory-manage-inventory.md)  
[Цепочка поставок](madeira-supply-chain.md)  
[Практическое руководство. Перемещение запасов между складами](inventory-how-transfer-between-locations.md)    
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md)  
[Общие бизнес-функции](ui-across-business-areas.md)

