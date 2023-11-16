---
title: Вопросы и ответы по OneDrive для бизнеса
description: Получите ответы на некоторые типичные вопросы о работе с OneDrive для бизнеса и Business Central.
author: brentholtorf
ms.topic: get-started
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'OneDrive, integration, share, browser'
ms.date: 09/09/2022
ms.author: bholtorf
---
# <a name="onedrive-for-business-faq"></a>Вопросы и ответы по OneDrive для бизнеса

[!INCLUDE [online_only](includes/online_only.md)]

В этой статье даны ответы на некоторые вопросы, которые могут у вас возникнуть по работе с OneDrive и [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="does-this-work-with-all--clients"></a>Это работает со всеми клиентами [!INCLUDE[prod_short](includes/prod_short.md)]?

Да. Вы можете открывать файлы в OneDrive в мобильных приложениях [!INCLUDE[prod_short](includes/prod_short.md)] при просмотре сведений карточки в Microsoft Teams или даже из надстройки Outlook.  

## <a name="is-onedrive-the-same-as-sharepoint-for-storing-files"></a>OneDrive то же самое, что и SharePoint, для хранения файлов?

В рамках подписки на Microsoft 365 ваша организация предоставляет вам OneDrive — файловое хранилище в облаке. OneDrive по умолчанию является частным, где вы упорядочиваете свой контент и выбираете, какими файлами или папками делиться и с кем. SharePoint, с другой стороны, предоставляет файловый репозиторий в облаке, который используется совместно с другими пользователями вашей организации.  

## <a name="does--support-consumer-onedrive"></a>Поддерживает ли [!INCLUDE[prod_short](includes/prod_short.md)] OneDrive для потребителей?

Нет. Эта интеграция предназначена исключительно для OneDrive для бизнеса и поддерживает только вашу рабочую учетную запись. 

## <a name="are-all-onedrive-for-business-plans-supported"></a>Поддерживаются все планы OneDrive для бизнеса?

[!INCLUDE[prod_short](includes/prod_short.md)] не поддерживает отдельные планы для OneDrive для бизнеса. OneDrive приобретается в составе плана Microsoft 365 "бизнес" или "корпоративный". Для получения дополнительной информации см. [Сравнивать цены и планы на облачное хранилище OneDrive](https://www.microsoft.com/microsoft-365/onedrive/compare-onedrive-plans?market=af&activetab=tab:primaryr2).  

## <a name="where-can-i-see-onedrive-service-health"></a>Где посмотреть работоспособность службы OneDrive?

Администраторы могут получить доступ к панели мониторинга работоспособности службы в центре администрирования Microsoft 365. Панель мониторинга включает доступность службы OneDrive. Перейдите на [https://admin.microsoft.com/Adminportal/Home?#/servicehealth](https://admin.microsoft.com/Adminportal/Home?#/servicehealth).
 
## <a name="is-onedrive-integration-available-to--on-premises"></a>Доступна ли интеграция OneDrive для локальной версии [!INCLUDE[prod_short](includes/prod_short.md)]?

Да, но в отличие от [!INCLUDE[prod_short](includes/prod_short.md)] Online, требуется дополнительная настройка. Дополнительные сведения см. в разделе [Настройка локальной версии Business Central](admin-onedrive-integration-onpremises.md).  

## <a name="does--on-premises-connect-with-sharepoint-server"></a>Подключается ли локальная версия [!INCLUDE[prod_short](includes/prod_short.md)] к серверу SharePoint?

Нет. Эта комбинация развертываний не поддерживается, даже если на сервере SharePoint включены "Мои сайты".  

## <a name="does--online-connect-with-sharepoint-server"></a>Подключается ли [!INCLUDE[prod_short](includes/prod_short.md)] Online к серверу SharePoint?

Нет. Эта комбинация развертываний не поддерживается, даже если на сервере SharePoint включены "Мои сайты".  

## <a name="how-does-this-work-in-an-organization-with-multiple-environments"></a>Как это работает в организации с несколькими средами?

Интеграция предполагает, что названия компаний уникальны в средах [!INCLUDE[prod_short](includes/prod_short.md)]. Если названия компаний уникальны для всей организации, при открытии файла в OneDrive файл будет скопирован в папку с именем текущей компании. Если названия компаний не уникальны в разных средах, файлы с одинаковыми названиями компаний могут быть помещены вместе в одну и ту же папку.  

## <a name="weve-changed-company-name-what-happens-to-my-previous-files"></a>Мы изменили название компании. Что происходит с моими предыдущими файлами?

[!INCLUDE[prod_short](includes/prod_short.md)] не переносит автоматически файлы, открытые ранее в OneDrive, в новую папку. После переименования вашей компании действие Открыть в OneDrive скопирует файлы в папку с новым названием компании.   

## <a name="when-attaching-files-to--how-do-i-pick-a-file-from-onedrive"></a>При прикреплении файлов к [!INCLUDE[prod_short](includes/prod_short.md)] как мне выбрать файл из OneDrive?

[!INCLUDE[prod_short](includes/prod_short.md)] не предоставляет средства выбора облачных файлов. Вы должны скачать файл из OneDrive на свое устройство, а затем отправить его в [!INCLUDE[prod_short](includes/prod_short.md)]. 

## <a name="i-want-to-open-files-in-sharepoint-instead-how-do-i-do-this"></a>Я хочу открывать файлы в SharePoint вместо этого. Как это сделать?

[!INCLUDE[prod_short](includes/prod_short.md)] не предоставляет функций для копирования файлов в SharePoint и их открытия из библиотеки SharePoint. Обратитесь к партнеру Microsoft, чтобы узнать о возможных вариантах, или поищите приложения в AppSource.  

## <a name="how-do-i-turn-off-integration-to-onedrive"></a>Как отключить интеграцию с OneDrive?

Запустите мастер настройки **Настройка OneDrive** и выключите переключатели **Использовать OneDrive для функций приложения** и **ИспользоватьOneDrive для системных функций**. 

## <a name="should-i-use-the-sharepoint-connection-setup-page-to-connect-to-sharepoint"></a>Следует ли мне использовать страницу Настройка подключения SharePoint для подключения к SharePoint?

Это устаревшая функция, в которой все файлы [!INCLUDE[prod_short](includes/prod_short.md)] от всех пользователей отправляются в одну папку SharePoint. Мы рекомендуем не настраивать экспресс-вкладку «Общие документы» на странице **Настройка подключения к SharePoint**, потому что эта страница [устарела](/dynamics365/business-central/dev-itpro/upgrade/deprecated-features-w1#microsoft-sharepoint-connection-setup) и будет удалена в волне 2 выпуска 2023 года (версии 23.0).  Рекомендуем вместо этого использовать мастер **Настройка OneDrive**.  

## <a name="which-version-of--supports-onedrive"></a>Какая версия [!INCLUDE[prod_short](includes/prod_short.md)] поддерживает OneDrive?

Интеграция с OneDrive стала доступна в выпуске 2021 года, волна 2.  

## <a name="which-features-are-affected-by-onedrive-integration"></a><a name="features"></a>На какие функции влияет интеграция с OneDrive?

В мастере настройки **Настройка OneDrive** для настройки интеграции с OneDrive вы можете включить или отключить функции для обработки файлов Business Central в OneDrive. За эти функции отвечают два параметра:

|Параметр|Описание|
|------|----------|
|**Использовать OneDrive для функций приложения**|Если вы включите этот параметр, действия **Открыть в OneDrive** и **Поделиться** станут доступны для файлов в Business Central, таких как файлы, прикрепленные к документам, или файлы в папке «Входящие отчеты». Эти действия позволяют пользователям копировать и открывать файлы, а также предоставлять доступ к ним через OneDrive. Дополнительные сведения см. в статье [Открытие и совместное использование файлов Business Central в OneDrive](across-share-onedrive.md).
|**Использовать OneDrive для системных функций**|Включение этого параметра активирует следующие функции:<ul><li> Действия **Открыть в Excel** и **Изменить в Excel** на страницах списков будут автоматически копировать файл Excel в OneDrive, а затем открывать его в Excel Online. Для получения дополнительной информации см. статью [Просмотр и редактирование в Excel](across-work-with-excel.md).</li><li> При отправке отчета в файл Excel или Word он автоматически копируется в OneDrive, затем открывается в Excel Online или Word Online. Дополнительные сведения см. в статье [Сохранение отчета в файл](ui-work-report.md#saving-a-report-to-a-file).|

## <a name="will-microsoft-continue-to-improve-the-integration-to-onedrive"></a>Будет ли Microsoft продолжать улучшать интеграцию с OneDrive?

В Microsoft мы постоянно слушаем отзывы от нашего разнообразного сообщества пользователей и действуем по лучшим предложениям. Чтобы узнать, что дальше будет с интеграцией с приложениями Microsoft 365, см. [План выпуска Dynamics 365](/dynamics365-release-plan/2021wave1).  

Если вы хотите участвовать в улучшении интеграции OneDrive или у вас есть идея, которая улучшит обмен файлами и совместную работу в [!INCLUDE[prod_short](includes/prod_short.md)], добавьте идею или проголосуйте за существующие идеи на [https://aka.ms/BusinessCentralIdeas](https://aka.ms/BusinessCentralIdeas).

## <a name="troubleshooting"></a>Устранение неполадок

В этом разделе представлена информация о том, как определить и исправить проблемы, которые могут возникнуть при использовании OneDrive с [!INCLUDE[prod_short](includes/prod_short.md)].  

### <a name="business-central-cant-find-my-onedrive"></a>Business Central не может найти мой OneDrive

При появлении этого сообщения "Не удалось определить местонахождение вашего OneDrive для бизнеса, обратитесь к партнеру для настройки", проверьте, получил ли пользователь доступ к своему OneDrive по крайней мере один раз. Если нет, попросите пользователя перейти на сайт portal.office.com/onedrive, чтобы настроить его. Это может занять некоторое время. Если сообщение по-прежнему отображается через 24 часа, обратитесь в службу поддержки.  
 
### <a name="im-having-problems-sharing-from-outlook"></a>У меня не получается делиться файлами из Outlook

См. статью [Не могу поделиться файлами OneDrive из Outlook.com](https://support.microsoft.com/en-us/office/can-t-share-onedrive-files-from-outlook-com-05d4cb21-40a2-40e3-b111-82cddb82d22f) на сайте службы поддержки Майкрософт.

### <a name="actions-open-in-onedrive-and-share-are-missing"></a>Действия "Открыть в OneDrive" и "Поделиться отсутствуют"

Есть пара вещей, которые вы можете проверить:

- Убедитесь, что функции приложения для OneDrive включены в мастере настройки **Настройка OneDrive**. См. статью [Настройка OneDrive с использованием мастера "Настройка OneDrive"](admin-onedrive-integration.md#configure-onedrive-using-onedrive-setup).
- Убедитесь, что на странице **Статус уведомлений о конфиденциальности** для Microsoft OneDrive установлено значение **Принять**. См. статью [Статус уведомлений о конфиденциальности](privacy-notices-status.md).

## <a name="see-also"></a>См. также

[Интеграция Business Central и OneDrive](across-onedrive-overview.md)  
[Управление интеграцией OneDrive с Business Central](admin-onedrive-integration.md)  
[Открытие файлов Business Central в OneDrive](across-share-onedrive.md)  
