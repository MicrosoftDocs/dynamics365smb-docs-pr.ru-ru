---
title: Устранение неполадок с доступом с лицензиями на Microsoft 365
description: 'Узнайте, как устранить проблемы с доступом к Business Central при наличии лицензии только на Microsoft 365.'
author: mikebc
ms.author: mikebc
ms.reviewer: jswymer
ms.topic: troubleshooting
ms.date: 02/07/2023
ms.custom: bap-template
ms.search.keywords: 'License, access, Microsoft 365, collaborate, collaboration, Teams, Microsoft Teams'
ms.service: dynamics-365-business-central
---

# <a name="troubleshoot-access-with-microsoft-365-licenses"></a>Устранение неполадок с доступом с лицензиями на Microsoft 365

## <a name="this-page-uses-data-from-related-tables-that-you-do-not-have-access-to-error-message"></a>Сообщение об ошибке "На этой странице используются данные из связанных таблиц, к которым у вас нет доступа"

### <a name="symptoms"></a>Признаки

При доступе к записи в Teams на вкладке или в сведениях карточки отображается сообщение об ошибке, похожее на следующее:

"На этой странице используются данные из связанных таблиц, к которым у вас нет доступа. Для работы со всеми функциями этой страницы обратитесь к администратору".

### <a name="cause"></a>Причина

Скорее всего, у вас нет разрешений в отношении объектов — таблиц, на которые ссылается текущая страница или запись.

## <a name="microsoft-365-access-has-been-enabled-but-users-get-a-permission-error"></a>Доступ Microsoft 365 включен, но для пользователей отображается ошибка, связанная с разрешениями

### <a name="symptoms-1"></a>Признаки

В центре администрирования Business Central включен доступ Microsoft 365, но при попытке доступа к какой-либо записи для пользователей отображается ошибка, связанная с разрешениями.

### <a name="cause-1"></a>Причина

Если включить доступ в центре администрирования Business Central, но не назначить разрешения на странице **Конфигурация лицензии**, все, кто будет пытаться получать доступ к записям Business Central в Teams, будут получать запись пользователя без права доступа к каким-либо объектам. В Business Central по умолчанию реализована защита: администратор должен сначала указать, к каким данным можно получить доступ в Teams. 

### <a name="resolution"></a>Разрешение

Настройка разрешений на странице "Конфигурация лицензии" повлияет только на вновь созданных пользователей. Вы также должны назначить отсутствующие разрешения пользователям, которые уже созданы на странице-списке "Пользователи". 

## <a name="you-shared-a-link-in-teams-but-users-get-a-message-that-they-can-only-view-data"></a>Вы поделились ссылкой в Teams, но пользователи получают сообщение о том, что они могут только просматривать данные

### <a name="symptoms-2"></a>Признаки

Когда вы делитесь ссылкой в Teams в качестве пользователя Business Central, другие пользователи видят ошибку "При доступе к Business Central с лицензией на Microsoft 365 вы можете только просматривать данные в Microsoft Teams".

### <a name="cause-2"></a>Причина

При публикации ссылки на Business Central в чате или в каналах Teams переход по этой ссылке всегда означает выход за пределы Microsoft Teams, где данные перестают быть доступны пользователю с лицензией Microsoft 365.

### <a name="resolution-1"></a>Разрешение

При публикации страниц или записей либо включайте предварительный просмотр ссылки в виде карточки, либо публикуйте данные в виде вкладки в чате или канале.

## <a name="card-from-shared-link-is-minimal-and-doesnt-include-details-button"></a>Карточка из общей ссылки минимальна и не включает кнопку «Подробности»

### <a name="symptoms-3"></a>Признаки

Когда владелец лицензии Microsoft 365, не имеющий лицензии Business Central, делится в Teams ссылкой Business Central, она автоматически разворачивается в карточку, которая не содержит полезной информации и показывает только Business Central без кнопки **Подробности**.

### <a name="cause-3"></a>Причина

Пользователи, у которых есть лицензия Microsoft 365, но нет лицензии Business Central, не могут делиться ссылками в виде карточек. Если у пользователя установлено приложение Business Central для Teams и пользователь вставляет ссылку в область создания, отображается только минимальная карточка. 

## <a name="see-also"></a>См. также

[Доступ к Business Central с лицензиями на Microsoft 365](admin-access-with-m365-license.md#minimum-requirements)  
[Настройка доступа с лицензиями на Microsoft 365](admin-access-with-m365-license-setup.md)  
[Интеграция Business Central и Microsoft Teams](across-teams-overview.md)
[Совместное использование записей Business Central и ссылок на страницы в Microsoft Teams](across-working-with-teams.md)  
[Интеграция устранения неполадок в Teams](admin-teams-troubleshooting.md)  
