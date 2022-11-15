---
title: Устранение неполадок с доступом с лицензиями на Microsoft 365
description: Узнайте, как устранить проблемы с доступом к Business Central при наличии лицензии только на Microsoft 365.
author: mikebc
ms.author: mikebc
ms.reviewer: jswymer
ms.service: dynamics365-business-central
ms.topic: troubleshooting
ms.date: 11/03/2022
ms.custom: bap-template
ms.search.keywords: License, access, Microsoft 365, collaborate, collaboration, Teams, Microsoft Teams
ms.openlocfilehash: 750a78eb32568bea07d6851ff69c0b2cfea3ab49
ms.sourcegitcommit: 61fdaded30310ba8bdf95f99e76335372f583642
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2022
ms.locfileid: "9745017"
---
# <a name="troubleshoot-access-with-microsoft-365-licenses"></a>Устранение неполадок с доступом с лицензиями на Microsoft 365

## <a name="symptoms"></a>Признаки

При доступе к записи в Teams на вкладке или в подробностях карточки появляется сообщение об ошибке, похожее на следующее:

"На этой странице используются данные из связанных таблиц, к которым у вас нет доступа. Для работы со всеми функциями этой страницы обратитесь к администратору".

## <a name="cause"></a>Причина

Скорее всего, у вас нет разрешений в отношении объектов — таблиц, на которые ссылается текущая страница или запись.

## <a name="symptoms"></a>Признаки

Доступ включен, но при попытке доступа к какой-либо записи пользователи видят ошибку, связанную с отсутствием разрешений.

## <a name="cause"></a>Причина

Если включить доступ в центре администрирования Business Central, но не назначить разрешения на странице "Конфигурация лицензии", у пользователей, которые попытаются осуществить доступ к записям Business Central в Teams, запись пользователя будет подготовлена без разрешений в отношении каких-либо объектов. В Business Central по умолчанию реализована защита: администратор должен сначала указать, к каким данным можно получить доступ в Teams. 

## <a name="resolution"></a>Разрешение

Настройка разрешений на странице "Конфигурация лицензии" повлияет только на вновь созданных пользователей. Вы также должны назначить отсутствующие разрешения пользователям, которые уже созданы на странице-списке "Пользователи". 

## <a name="symptoms"></a>Признаки

Когда я делюсь ссылкой в Teams, другие пользователи видят ошибку "При доступе к Business Central с лицензией на Microsoft 365 вы можете только просматривать данные в Microsoft Teams".

## <a name="cause"></a>Причина

При публикации ссылки на Business Central в чате или в каналах Teams переход по этой ссылке всегда означает выход за пределы Microsoft Teams, где данные перестают быть доступны пользователю с лицензией Microsoft 365.

## <a name="resolution"></a>Разрешение

При публикации страниц или записей либо включайте предварительный просмотр ссылки в виде карточки, либо публикуйте данные в виде вкладки в чате или канале.

## <a name="see-also"></a>См. также

[Доступ к Business Central с лицензиями на Microsoft 365](admin-access-with-m365-license.md#minimum-requirements)  
[Настройка доступа с лицензиями на Microsoft 365](admin-access-with-m365-license-setup.md)  
[Интеграция Business Central и Microsoft Teams](across-teams-overview.md)
[Совместное использование записей Business Central и ссылок на страницы в Microsoft Teams](across-working-with-teams.md)  
[Интеграция устранения неполадок в Teams](admin-teams-troubleshooting.md)  