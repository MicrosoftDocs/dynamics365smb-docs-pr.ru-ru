---
title: Расширения облачной миграции
description: Используйте расширения облачной миграции для переноса локальных данных в сетевую версию Business Central. Эти расширения перемещают ваши локальные данные в облако, чтобы вы могли использовать сетевую версию Business Central с вашими существующими данными.
author: jenolson
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.reviewer: edupont
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: f02face497affd1fd1467c118e10e69f2be39b85
ms.sourcegitcommit: 951d3c9d541f0b1d26712d37e253c2958dae3321
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "5889128"
---
# <a name="cloud-migration-extensions-for-migrating-to-business-central-online"></a>Расширения облачной миграции для перехода на Business Central Online

В зависимости от вашего локального решения вы должны использовать разные расширения для подключения ваших данных к [!INCLUDE[prod_short](includes/prod_short.md)] Online с целью переноса вашего решения в облако.  

Если используется локальная версия одного из поддерживаемых продуктов, можно настроить среду облака на основе специального расширения для этого продукта. После настройки вашей среды облака можно будет перенести данные из вашего локального решения в [!INCLUDE[prod_short](includes/prod_short.md)]. Это позволит вам полностью использовать преимущества облака для вашего бизнеса, такие как улучшенный анализ бизнеса, искусственный интеллект, доступ с нескольких устройств и доступ в любой момент из любого места.  

Для получения дополнительной информации см. раздел [Миграция локальных данных в Business Central Online](/dynamics365/business-central/dev-itpro/administration/migrate-data) в материалах для администраторов [!INCLUDE[prod_short](includes/prod_short.md)].  

## <a name="business-central-on-premises"></a>Локальная версия Business Central

Если используется локальное развертывание [!INCLUDE[prod_short](includes/prod_short.md)], получите расширения **Основа интеллектуального облака** и **Интеллектуальное облако Business Central**, затем выполните мастер настройки **Настройка миграции в облако**.  

## <a name="dynamics-gp"></a>Dynamics GP

Если используется Dynamics GP, получите расширения **Базовое расширение интеллектуального облака** и **Интеллектуальное облако Dynamics GP**, затем запустите мастер настройки **Настройка миграции в облако**.  

> [!IMPORTANT]
> Миграция из Dynamics GP с использованием мастер настройки **Настройка миграции в облако** в настоящее время поддерживается только для следующих рынков: США, Канада, Соединенное Королевство.

## <a name="dynamics-sl"></a>Dynamics SL

Если используется Dynamics SL, получите расширения **База интеллектуального облака**, **Интеллектуальное облако Microsoft Dynamics SL** и **Смарт-листы истории Microsoft Dynamics SL**, затем запустите мастер настройки **Настройка миграции в облако**.  

## <a name="see-also"></a>См. также

[Базовое расширение миграции в облако](ui-extensions-intelligent-cloud.md)  
[Миграция локальных данных в Business Central Online](/dynamics365/business-central/dev-itpro/administration/migrate-data)  

[!INCLUDE[footer-include](includes/footer-banner.md)]