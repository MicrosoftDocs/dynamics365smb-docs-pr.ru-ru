---
title: Вопросы и ответы по OneDrive для бизнеса
description: Получите ответы на некоторые типичные вопросы о работе с OneDrive для бизнеса и Business Central.
author: bholtorf
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: OneDrive, integration, share, browser
ms.date: 05/19/2021
ms.author: bholtorf
ms.openlocfilehash: f54e8b6290e9dd653180b3ea05246255b84dc2ae
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "8144054"
---
# <a name="onedrive-for-business-faq"></a>Вопросы и ответы по OneDrive для бизнеса

[!INCLUDE [online_only](includes/online_only.md)]

В этой статье даны ответы на некоторые вопросы, которые могут у вас возникнуть по работе с OneDrive и [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="does-this-work-with-all-prod_short-clients"></a>Это работает со всеми клиентами [!INCLUDE[prod_short](includes/prod_short.md)]?

Да. Вы можете открывать файлы в OneDrive в мобильных приложениях [!INCLUDE[prod_short](includes/prod_short.md)] при просмотре сведений карточки в Microsoft Teams или даже из надстройки Outlook.  

## <a name="is-onedrive-the-same-as-sharepoint-for-storing-files"></a>OneDrive то же самое, что и SharePoint, для хранения файлов?

В рамках подписки на Microsoft 365 ваша организация предоставляет вам OneDrive — файловое хранилище в облаке. OneDrive по умолчанию является частным, где вы упорядочиваете свой контент и выбираете, какими файлами или папками делиться и с кем. SharePoint, с другой стороны, предоставляет файловый репозиторий в облаке, который используется совместно с другими пользователями вашей организации.  

## <a name="does-prod_short-support-consumer-onedrive"></a>Поддерживает ли [!INCLUDE[prod_short](includes/prod_short.md)] OneDrive для потребителей?

Кол-во Эта интеграция предназначена исключительно для OneDrive для бизнеса и поддерживает только вашу рабочую учетную запись. 

## <a name="are-all-onedrive-for-business-plans-supported"></a>Поддерживаются все планы OneDrive для бизнеса?

[!INCLUDE[prod_short](includes/prod_short.md)] не поддерживает автономные планы для OneDrive для бизнеса. OneDrive приобретается в составе плана Microsoft 365 "бизнес" или "корпоративный". Для получения дополнительной информации см. [Сравнивать цены и планы на облачное хранилище OneDrive](https://www.microsoft.com/microsoft-365/onedrive/compare-onedrive-plans?market=af&activetab=tab:primaryr2).  

## <a name="where-can-i-see-onedrive-service-health"></a>Где посмотреть работоспособность службы OneDrive?

Администраторы могут получить доступ к панели мониторинга работоспособности службы в центре администрирования Microsoft 365. Панель мониторинга включает доступность службы OneDrive. 
 
## <a name="is-onedrive-integration-available-to-prod_short-on-premises"></a>Доступна ли интеграция OneDrive для локальной версии [!INCLUDE[prod_short](includes/prod_short.md)]?

Да, но в отличие от [!INCLUDE[prod_short](includes/prod_short.md)] Online, требуется дополнительная настройка. Дополнительные сведения см. в разделе [Настройка локальной версии Business Central](admin-onedrive-integration.md#configuring-business-central-on-premises).  

## <a name="does-prod_short-on-premises-connect-with-sharepoint-server"></a>Подключается ли локальная версия [!INCLUDE[prod_short](includes/prod_short.md)] к серверу SharePoint?

Кол-во Эта комбинация развертывания не поддерживается, даже если на сервере SharePoint включены Мои сайты.  

## <a name="does-prod_short-online-connect-with-sharepoint-server"></a>Подключается ли [!INCLUDE[prod_short](includes/prod_short.md)] Online к серверу SharePoint?

Кол-во Эта комбинация развертывания не поддерживается, даже если на сервере SharePoint включены Мои сайты.  

## <a name="how-does-this-work-in-an-organization-with-multiple-environments"></a>Как это работает в организации с несколькими средами?

Интеграция предполагает, что названия компаний уникальны в средах [!INCLUDE[prod_short](includes/prod_short.md)]. Если названия компаний уникальны для всей организации, при открытии файла в OneDrive файл будет скопирован в папку с именем текущей компании. Если названия компаний не уникальны в разных средах, файлы с одинаковыми названиями компаний могут быть помещены вместе в одну и ту же папку.  

## <a name="weve-changed-company-name-what-happens-to-my-previous-files"></a>Мы изменили название компании. Что происходит с моими предыдущими файлами?

[!INCLUDE[prod_short](includes/prod_short.md)] не переносит автоматически файлы, открытые ранее в OneDrive, в новую папку. После переименования вашей компании действие Открыть в OneDrive скопирует файлы в папку с новым названием компании.   

## <a name="when-attaching-files-to-prod_short-how-do-i-pick-a-file-from-onedrive"></a>При прикреплении файлов к [!INCLUDE[prod_short](includes/prod_short.md)] как мне выбрать файл из OneDrive? 
[!INCLUDE[prod_short](includes/prod_short.md)] не предоставляет средства выбора облачных файлов. Вы должны скачать файл из OneDrive на свое устройство, а затем отправить его в [!INCLUDE[prod_short](includes/prod_short.md)]. 

## <a name="i-want-to-open-files-in-sharepoint-instead-how-do-i-do-this"></a>Я хочу открывать файлы в SharePoint вместо этого. Как это сделать?

[!INCLUDE[prod_short](includes/prod_short.md)] не предоставляет функции для копирования файлов в SharePoint и их открытия из библиотеки SharePoint. Обратитесь к партнеру Microsoft, чтобы узнать о возможных вариантах, или поищите приложения в AppSource.  

## <a name="how-do-i-turn-off-integration-to-onedrive"></a>Как отключить интеграцию с OneDrive?

[!INCLUDE[prod_short](includes/prod_short.md)] Online не дает возможности включить или отключить интеграцию с OneDrive.  

## <a name="should-i-use-the-sharepoint-connection-setup-page-to-connect-to-sharepoint"></a>Следует ли мне использовать страницу Настройка подключения SharePoint для подключения к SharePoint?

Это устаревшая функция, в которой все файлы [!INCLUDE[prod_short](includes/prod_short.md)] от всех пользователей отправляются в одну папку SharePoint. Мы рекомендуем не настраивать экспресс-вкладку «Общие документы» на странице настройки подключения SharePoint, потому что мы работаем над прекращением поддержки этой функции.  

## <a name="which-version-of-prod_short-supports-onedrive"></a>Какая версия [!INCLUDE[prod_short](includes/prod_short.md)] поддерживает OneDrive?

Интеграция с OneDrive стала доступна в выпуске 2021 года, волна 2.  

## <a name="will-microsoft-continue-to-improve-the-integration-to-onedrive"></a>Будет ли Microsoft продолжать улучшать интеграцию с OneDrive?

В Microsoft мы постоянно слушаем отзывы от нашего разнообразного сообщества пользователей и действуем по лучшим предложениям. Чтобы узнать, что дальше будет с интеграцией с приложениями Microsoft 365, см. [План выпуска Dynamics 365](/dynamics365-release-plan/2021wave1).  

Если вы хотите участвовать в улучшении интеграции OneDrive или у вас есть идея, которая улучшит обмен файлами и совместную работу в [!INCLUDE[prod_short](includes/prod_short.md)], добавьте идею или проголосуйте за существующие идеи на [https://aka.ms/BusinessCentralIdeas](https://aka.ms/BusinessCentralIdeas).

## <a name="troubleshooting"></a>Устранение неполадок

В этом разделе представлена информация о том, как определить и исправить проблемы, которые могут возникнуть при использовании OneDrive с [!INCLUDE[prod_short](includes/prod_short.md)].  

### <a name="i-have-to-sign-in-each-time-i-open-a-file"></a>Мне нужно входить в систему каждый раз, когда я открываю файл

Извините, это известная проблема, и мы над ней работаем. Мы надеемся, что в грядущем обновлении ситуация улучшится.  

### <a name="business-central-cant-find-my-onedrive"></a>Business Central не может найти мой OneDrive

При появлении этого сообщения "Не удалось определить местонахождение вашего OneDrive для бизнеса, обратитесь к партнеру для настройки", проверьте, получил ли пользователь доступ к своему OneDrive по крайней мере один раз. Если нет, попросите пользователя перейти на сайт portal.office.com/onedrive, чтобы настроить его. Это может занять некоторое время. Если сообщение по-прежнему отображается через 24 часа, обратитесь в службу поддержки.  
 

## <a name="see-also"></a>См. также
[Интеграция Business Central и OneDrive](across-onedrive-overview.md)  
[Управление интеграцией OneDrive с Business Central](admin-onedrive-integration.md)  
[Открытие файлов Business Central в OneDrive](across-share-onedrive.md)  
