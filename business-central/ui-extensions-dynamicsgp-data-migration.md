---
title: "Миграция данных из Dynamics GP с помощью расширения для миграции данных | Microsoft Docs"
description: "Используйте расширение для миграции данных Dynamics GP, чтобы перенести клиентов, поставщиков, товары и счета из Dynamics GP в Business Central."
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: ad1b888d475c0523c5a905e804a3f89ab4531b28
ms.openlocfilehash: 3761bdb0d6b9a51ed309ac4189ff263de76f4679
ms.contentlocale: ru-ru
ms.lasthandoff: 05/17/2018

---
# <a name="the-dynamics-gp-data-migration-extension-for-business-central"></a>Расширение "Миграция данных Dynamics GP" для Business Central 
Это расширение облегчает миграцию клиентов, поставщиков, складских товаров и счетов из Dynamics GP в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Если сейчас ваша компания использует Dynamics GP, вы можете экспортировать соответствующие основные записи, а затем открыть руководство по сопровождаемой настройке, чтобы добавить данные в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Дополнительные сведения см. в разделе [Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md).

## <a name="exporting-data-from-dynamics-gp"></a>Экспорт данных из Dynamics GP
Чтобы экспортировать данный, вы должны экспортировать некоторые или все существующие клиенты, поставщики, складские товары и счета в файл с помощью функции Dynamics GP. Для целей [!INCLUDE[d365fin](includes/d365fin_md.md)] можно экспортировать следующие типы данных:

* Организация  
* Клиент  
* Пункт меню  
* Поставщик  

Расширение переноса данных Dynamics GP автоматически сопоставляет экспортированные данные, чтобы вы могли быстро получить данные в новой организации в [!INCLUDE[d365fin](includes/d365fin_md.md)]. В ходе процесса создается информация по настройке, например учетные группы. Складские товары будут добавлены в систему по методу оценки себестоимости FIFO. Счета будут настроены как сегмент главного счета из Dynamics GP с измерениями, поскольку [!INCLUDE[d365fin](includes/d365fin_long_md.md)] не имеет сегменты счета.

## <a name="see-also"></a>См. также
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  

