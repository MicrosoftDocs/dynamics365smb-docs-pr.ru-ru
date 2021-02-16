---
title: Вопросы и ответы по Teams
description: Получите ответы на некоторые типичные вопросы о работе с Teams и Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork, faq, errors
ms.date: 01/26/2021
ms.author: jswymer
ms.openlocfilehash: 79b6069ffb4c73d783b2c05d3a44a55763805a52
ms.sourcegitcommit: 1c9eec7554305603d688bf85ce3986d0b1f72ede
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "5068438"
---
# <a name="teams-faq"></a>Вопросы и ответы по Teams

[!INCLUDE [online_only](includes/online_only.md)]

В этой статье даны ответы на некоторые вопросы, которые могут у вас возникнуть по работе с Teams и [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="general"></a>[Общие](#tab/general)

### <a name="how-do-i-sign-in-to-the-prod_shortmd-app-in-teams"></a>Как мне войти в приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] в Teams? 

После установки приложения вам будет предложено войти в систему при первой вставке ссылки [!INCLUDE [prod_short.md](includes/prod_short.md)] в чат Teams или когда вы выбираете действие **Детали** на карточке в Teams. В зависимости от вашего клиента Teams вам может потребоваться ввести свои учетные данные, которые вы используете для доступа к [!INCLUDE [prod_short.md](includes/prod_short.md)]. 

### <a name="how-do-i-sign-out-of-the-prod_shortmd-app-in-teams"></a>Как мне выйти из приложения [!INCLUDE [prod_short.md](includes/prod_short.md)] в Teams? 

Чтобы выйти из текущего удостоверения пользователя в Teams, используемого для подключения к [!INCLUDE [prod_short.md](includes/prod_short.md)], перейдите в любое окно создания чата и выберите значок [!INCLUDE [prod_short.md](includes/prod_short.md)] внизу. Когда появится окно, проверьте свое текущее удостоверение, с которым вы вошли в систему, затем выберите **Выйти**. Если вы используете Teams в браузере, вы также выйдете из любого веб-клиента [!INCLUDE [prod_short.md](includes/prod_short.md)] в том же окне браузера.

### <a name="does-the-app-for-teams-connect-to-prod_shortmd-on-premises"></a>Подключается ли приложение для Teams к [!INCLUDE [prod_short.md](includes/prod_short.md)] On Premises? 

Кол-во Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams работает только с [!INCLUDE [prod_short.md](includes/prod_short.md)] Online. Нет планов поддерживать типы развертывания [!INCLUDE [prod_short.md](includes/prod_short.md)], &mdash; например, локальное, гибридное или частное облако, &mdash; которые Microsoft не размещает и не управляет ими напрямую.

### <a name="does-the-app-work-with-multiple-companies-and-environments"></a>Работает ли приложение с несколькими компаниями и средами? 

Да. Когда приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] разворачивает ссылку в карточку, ссылка должна содержать названия сред и компаний, чтобы приложение соответствовало записи в нужной компании. Вы можете вставлять ссылки на любые компании и среды, к которым у вас есть доступ в вашей организации, и из учетной записи [!INCLUDE [prod_short.md](includes/prod_short.md)], которую вы использовали для входа. Карточку увидят участники чата. Но они не могут просматривать данные карточки, если у них нет разрешений для компании или среды, в которой хранится эта запись.

### <a name="in-which-countries-or-regions-is-the-prod_shortmd-app-available"></a>В каких странах или регионах приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] доступно? 

Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams не ограничено страной или регионом. Приложение доступно на всех рынках, которые в настоящее время поддерживаются магазином Teams. 

### <a name="does-the-prod_shortmd-app-work-with-any-localization-of-prod_shortmd"></a>Работает ли приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] с любой локализацией [!INCLUDE [prod_short.md](includes/prod_short.md)]? 

Да. Приложение предназначено для работы с любой локализацией [!INCLUDE [prod_short.md](includes/prod_short.md)], независимо от того, предлагается ли эта локализация напрямую от Microsoft или через партнера. Дополнительные сведения см. в [Наличие в странах/регионах и поддерживаемые языки](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations?toc=/dynamics365/business-central/toc.json).

### <a name="which-languages-does-the-prod_shortmd-app-support"></a><a name="language"></a>Какие языки поддерживает приложение [!INCLUDE [prod_short.md](includes/prod_short.md)]?
<!--TODO Run by Mike -->

Язык, используемый для карточек и деталей карточек в Teams, определяется двумя вещами:

1. Ваш язык в Teams, который вы можете увидеть в настройках своей учетной записи в Teams. 
2. Ваш язык в [!INCLUDE [prod_short.md](includes/prod_short.md)], который вы можете увидеть в веб-клиенте [!INCLUDE [prod_short.md](includes/prod_short.md)] (см. раздел [Изменение базовых настроек — язык](ui-change-basic-settings.md#language)).

В следующей таблице объясняется, чем отличается взаимодействие для авторов и получателей сообщений в зависимости от языковых настроек и доступности языков.

|Кто|Карточка|Детали карточки |
|-|----|--------------| 
|Автор сообщения |Отображается на языке, который указан для вас в Teams. Если [!INCLUDE [prod_short.md](includes/prod_short.md)] не предлагает тот же язык, карточка отображается на английском языке. |Отображается на языке, который указан для вас в [!INCLUDE [prod_short.md](includes/prod_short.md)].  которые могут включать языки из языковых приложений, предоставляемых партнерами. |
|Получатель сообщения |Отображается на языке автора сообщения. |Отображается на языке, который указан для вас в [!INCLUDE [prod_short.md](includes/prod_short.md)]. |

Список поддерживаемых языков для [!INCLUDE [prod_short.md](includes/prod_short.md)] см. в разделе [Поддерживаемые языки](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations?toc=/dynamics365/business-central/toc.json#supported-languages).

### <a name="where-can-i-find-teams-integration-inside-the-prod_shortmd-web-client"></a>Где я могу найти интеграцию Teams в веб-клиенте [!INCLUDE [prod_short.md](includes/prod_short.md)]? 

В настоящее время нет встраивания элементов управления Teams или наличия функций Teams внутри веб-клиента [!INCLUDE [prod_short.md](includes/prod_short.md)] или других клиентов.  

### <a name="does-prod_shortmd-work-with-the-teams-mobile-app"></a>Работает ли [!INCLUDE [prod_short.md](includes/prod_short.md)] с мобильным приложением Teams?

Да. Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] может быть установлено из классического приложения Teams или браузера либо администратором для всех пользователей. После установки приложения [!INCLUDE [prod_short.md](includes/prod_short.md)] автоматически доступно в Teams для iOS и Android. На мобильных устройствах вы можете просматривать карточки, отправленные другими, получать доступ к деталям или открывать карточку в полном объеме в мобильном приложении [!INCLUDE [prod_short.md](includes/prod_short.md)]. Однако вы не можете вставлять ссылки, которые расширяются в карточки при составлении сообщений. Минимальные требования для мобильных устройств см. в разделе [Минимальные требования для использования Business Central](product-requirements.md).

### <a name="is-the-prod_shortmd-app-for-teams-the-same-as-the-prod_shortmd-app-for-ios-and-android"></a>Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams такое же, как приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для iOS и Android? 

Кол-во Приложение для Teams — это надстройка к Microsoft Teams и предназначено исключительно для совместной работы, которая сигнализируется в Teams. С другой стороны, мобильное приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] предлагает богатый опыт работы с данными [!INCLUDE [prod_short.md](includes/prod_short.md)] на ваших мобильных устройствах.

Мобильным пользователям рекомендуется установить как мобильное приложение, так и приложение для Teams, чтобы получить максимальную отдачу от [!INCLUDE [prod_short.md](includes/prod_short.md)]. Когда оба установлены, вы можете выбрать действие **Открыть на новой вкладке** над карточкой в Teams, чтобы открыть детали карточки в мобильном приложении [!INCLUDE [prod_short.md](includes/prod_short.md)]. Для получения информации об установке [!INCLUDE [prod_short.md](includes/prod_short.md)] и мобильных приложений Teams см.:

- [Получение Business Central на мобильном устройстве](install-mobile-app.md)
- [Получение мобильного приложения Teams](https://support.microsoft.com/office/download-the-mobile-app-for-teams-5940ebdc-0082-4fb1-83c4-751edc23dcb5) в службе поддержки Microsoft

### <a name="does-the-prod_shortmd-app-work-in-all-teams-clients"></a>Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] работает во всех клиентах Teams?

Кол-во Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams не поддерживается при установке в виде пакета для macOS или Linux. На этих платформах вы можете получить доступ к Teams с помощью поддерживаемого браузера.

Минимальные требования в [!INCLUDE [prod_short.md](includes/prod_short.md)] см. в разделе [Минимальные требования для использования Business Central](product-requirements.md#teams).

Для получения информации о выборе клиентов Teams и о том, как их установить, см. раздел [Получение клиентов для Microsoft Teams](/microsoftteams/get-clients) в документации Teams.

### <a name="which-teams-client-is-best-for-prod_shortmd"></a>Какой клиент Teams лучше всего подходит для [!INCLUDE [prod_short.md](includes/prod_short.md)]?

Между клиентами Teams есть лишь незначительные различия и ограничения, которые могут повлиять на ваш опыт работы с приложением [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams. При выборе клиента Teams учитывайте:

- Доступ к камере и местоположению невозможен из окна сведений в настольном приложении Teams 
- Использование Microsoft Edge с Teams в браузере позволяет легко работать с несколькими удостоверениями и учетными записями, входя в Teams из разных профилей. Чтобы узнать об использовании профилей в Microsoft Edge, см. раздел [Вход и создание нескольких профилей в Microsoft Edge](https://support.microsoft.com/office/sign-in-and-create-multiple-profiles-in-microsoft-edge-df94e622-2061-49ae-ad1d-6f0e43ce6435) в службе поддержки Microsoft.

### <a name="what-is-the-best-way-for-me-to-demonstrate-prod_shortmd-and-microsoft-teams-to-prospective-customers"></a>Как мне лучше всего продемонстрировать [!INCLUDE [prod_short.md](includes/prod_short.md)] и Microsoft Teams потенциальным клиентам?

Если вы являетесь партнером по перепродаже, вам может потребоваться среда, которую вы можете показывать потенциальным клиентам в рамках предпродажных демонстраций. Чтобы не повлиять на Microsoft Teams в своей организации, вы можете получить демонстрационную учетную запись Microsoft 365 по адресу [https://aka.ms/CDX](https://aka.ms/CDX). Эта учетная запись дает вам полный контроль над независимой организацией Azure, которая включает Microsoft Teams и [!INCLUDE [prod_short.md](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Подготовка демонстрационных сред для Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/administration/demo-environment).

### <a name="does-the-prod_shortmd-app-for-teams-cater-for-my-customization-and-personalization"></a>Учитывает ли приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams мою настройку и персонализацию?

Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams может отображать карточки для ссылок на страницы и таблицы клиентов в [!INCLUDE [prod_short.md](includes/prod_short.md)], например страницы и таблицы, созданные из ваших собственных расширений или из AppSource.

На поля, отображаемые на карточке в Teams, также могут влиять настройки [!INCLUDE [prod_short.md](includes/prod_short.md)], установленные для вашей организации. Карточки не учитывают никакую индивидуальную настройку ролей или персонализацию пользователя. Однако в окне сведений о карточке отображаются сведения о записях, как если бы вы их видели в [!INCLUDE [prod_short.md](includes/prod_short.md)], включая любые расширения, настройки ролей и персонализацию пользователей.

### <a name="where-can-i-learn-about-my-privacy"></a>Где я могу узнать о своей конфиденциальности? 

Вы можете узнать о том, как Microsoft обрабатывает ваши данные, в разделе [Заявление о конфиденциальности Microsoft](https://go.microsoft.com/fwlink/?linkid=2030602). 

Обратитесь к своему администратору, чтобы узнать, как ваша организация обеспечивает конфиденциальность ваших данных. 

### <a name="how-do-i-uninstall-the-prod_shortmd-app-for-teams"></a>Как мне удалить приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams? 

Чтобы удалить приложение, которое вы установили для себя, перейдите в любое окно создания чата, найдите значок [!INCLUDE [prod_short.md](includes/prod_short.md)] внизу, щелкните значок правой кнопкой мыши и выберите "Удалить".  

### <a name="will-microsoft-continue-to-improve-the-prod_shortmd-app-for-teams"></a>Будет ли Microsoft продолжать улучшать приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams?

В Microsoft мы постоянно слушаем отзывы от нашего разнообразного сообщества пользователей и действуем по лучшим предложениям. Чтобы узнать, что будет дальше для приложения [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams, см. раздел [План выпуска Dynamics 365](https://aka.ms/dynamics365releaseplan).

Если вы хотите участвовать в улучшении приложения для Teams или у вас есть отличная идея, которая поможет упростить вашу работу или совместную работу в Teams, добавьте идею или проголосуйте за существующие идеи на сайте [https://aka.ms/BusinessCentralIdeas](https://aka.ms/BusinessCentralIdeas).

## <a name="working-with-cards"></a>[Работа с карточками](#tab/cards)

### <a name="which-types-of-links-does-the-app-support"></a>Какие типы ссылок поддерживает приложение?

Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams реагирует на большинство ссылок веб-клиента [!INCLUDE [prod_short.md](includes/prod_short.md)]. Если ссылка относится к отдельной записи на странице, на карточке будут отображаться поля для этой записи. Поддерживаемые типы страниц включают: 

- Страницы карточек, например карточка товара
- Страницы документов, такие как документ заказа на продажу
- Страницы ListPlus, которые представляют собой одну запись, состоящую из других записей, например, отчет о сверке банковского счета
- Простые страницы со списком, на которых запись не дает возможности перейти к отдельной странице с подробностями, например список почтовых индексов

При вставке ссылки на корневой URL-адрес веб-клиента, например https://businesscentral.dynamics.com, карточка вместо этого отображает информацию, чтобы помочь новым пользователям получить доступ к [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="how-do-i-delete-a-card-i-sent-to-a-chat"></a>Как удалить карточку, отправленную в чат? 

Вы не можете удалить карточку, которую уже отправили в чат. Но вы можете удалить все сообщение, частью которого является карточка.

Как автор сообщения, вы можете удалить любые сообщения, отправленные в чаты с человеком, группой или каналом &mdash; если только ваш администратор не установил политики, предотвращающие удаление сообщений. Если вы модерируете канал как владелец канала, ваш администратор может также предоставить вам разрешение на удаление любых сообщений в канале, включая сообщения, отправленные другими пользователями.

Удаление сообщения, содержащего карточку, не удаляет данные и не влияет на данные в [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="do-cards-always-show-up-to-date-information"></a>Всегда ли на карточках отображается актуальная информация?

Кол-во Значения полей на карточке в Teams, включая любые изображения, основаны на данных, доступных на момент отправки этой карточки в чат. Карточки [!INCLUDE [prod_short.md](includes/prod_short.md)] не обновляются автоматически в Teams. 

### <a name="will-others-see-my-card-if-they-dont-have-the-prod_shortmd-app-for-teams"></a>Увидят ли мою карточку другие пользователи, если у них нет приложения [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams? 

Когда вы составляете и отправляете в чат сообщение с карточкой, все пользователи увидят карточку, даже если они не установили приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams.

## <a name="working-with-card-details"></a>[Работа со сведения карточки](#tab/carddetails)

### <a name="where-is-the-save-button-in-the-details-window-in-teams"></a>Где находится кнопка сохранения в окне сведений в Teams? 

[!INCLUDE [prod_short.md](includes/prod_short.md)] автоматически сохраняет изменения, внесенные вами в любое поле, как только вы покидаете поле. Чтобы покинуть поле, щелкните/коснитесь в любом месте за пределами поля или используйте клавишу TAB для перехода к следующему полю. Когда данные появляются в диалоге в окне сведений, вам может потребоваться выбрать кнопку **ОК**, чтобы [!INCLUDE [prod_short.md](includes/prod_short.md)] сохранил ваши изменения.

### <a name="if-i-choose-to-view-details-for-a-card-will-other-users-see-my-details-window"></a>Если я выберу просмотр сведений для карточки, будут ли другие пользователи видеть мое окно сведений? 

Кол-во Хотя все в чате могут просматривать саму карточку, окно с подробностями появляется только на вашем устройстве тогда, когда вы выбираете **Сведения**. Другие пользователи должны выбрать **Сведения**, если они хотят просмотреть окно со сведения на своем устройстве.

### <a name="can-i-start-a-teams-call-from-the-details-window-in-teams"></a>Могу ли я начать вызов Teams из окна сведений в Teams? 

Да. Вы можете начать вызов, выбрав связанный номер набора в поле номера телефона, например поле **Номер мобильного телефона** на карточке **Контакт**. Teams должно быть назначенным вами приложением для набора номера.

Чтобы звонить на местные или международные стационарные и мобильные телефоны из Teams, у вас должна быть лицензия Teams для корпоративных звонков. Кроме того, вы должны настроить Teams в качестве вашего решения для звонков. Чтобы узнать больше, см. раздел [Планирование голосового решения Teams](/microsoftteams/cloud-voice-landing-page) в документации Teams.

### <a name="can-i-print-documents-from-the-details-window-in-teams"></a>Могу ли я распечатать документы из окна сведений в Teams? 

Да. Вы распечатываете отчеты и другие документы, используя стандартные функции печати [!INCLUDE [prod_short.md](includes/prod_short.md)] и любой облачный принтер, настроенный на странице **Управление принтером** в [!INCLUDE [prod_short.md](includes/prod_short.md)]. Вы не можете печатать из Teams на локальные принтеры, известные вашему клиентскому устройству, такие как принтеры, на которых вы обычно печатаете из своего браузера. По этой причине вы не можете печатать из окна предварительного просмотра отчета, а только с главной страницы запроса отчета, прямо на свои облачные принтеры.

Для получения дополнительной информации о настройке облачных принтеров см. раздел [Настройка принтеров](ui-specify-printer-selection-reports.md).

### <a name="can-i-access-the-camera-from-the-details-window-in-teams"></a>Могу ли я получить доступ к камере из окна сведений в Teams? 

Да. Любые функции [!INCLUDE [prod_short.md](includes/prod_short.md)] в окне сведений, использующие камеру, доступны во всех клиентах Teams.

### <a name="can-i-access-my-location-from-the-details-window-in-teams"></a><a name="location"></a>Могу ли я получить доступ к моему местоположению из окна сведений в Teams?

Если вы используете функции в [!INCLUDE [prod_short.md](includes/prod_short.md)], которые обращаются к вашим текущим координатам местоположения, например на картах, вы должны использовать Teams в браузере или мобильное приложение Teams. Местоположение недоступно при использовании классического приложения Teams. 

## <a name="collaborating-with-guests"></a>[Сотрудничество с гостями](#tab/collaborating)

### <a name="can-i-share-cards-with-users-outside-my-organization"></a>Могу ли я поделиться карточками с пользователями за пределами моей организации? 

Да. Когда вы составляете и отправляете сообщение с карточкой, все получатели в чате увидят карточку &mdash; даже если они гости или посторонние по отношению к вашей организации. Гости также могут открыть окно сведений, если им предоставлено разрешение на доступ к этим данным в [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="is-the-experience-any-different-for-users-that-are-guests"></a>Отличается ли опыт пользователей, которые являются гостями?

Да. Приглашение гостевых пользователей из-за пределов вашей организации для участия в чате или на канале дает им аналогичный, но не идентичный опыт по сравнению с пользователями в вашей организации. Когда гость получает сообщение с карточкой, он может ее просмотреть. Гости также могут открыть окно сведений, если им предоставлено разрешение на доступ к этим данным в [!INCLUDE [prod_short.md](includes/prod_short.md)] и назначена лицензия [!INCLUDE [prod_short.md](includes/prod_short.md)] в вашей организации. Когда гость пишет сообщение, ссылки на ваш [!INCLUDE [prod_short.md](includes/prod_short.md)] не расширяются в карточки.

Чтобы узнать о других сходствах и различиях между гостями и членами рабочей группы, см. раздел [Опыт гостевых символов в Teams](/MicrosoftTeams/guest-experience) в документации Teams.

### <a name="how-does-a-guest-user-install-the-prod_shortmd-app"></a>Как гостевой пользователь устанавливает приложение [!INCLUDE [prod_short.md](includes/prod_short.md)]? 

Гости не имеют доступа к магазину приложений для самостоятельной установки приложений. Однако приложение может быть автоматически установлено для них в соответствии с политиками вашей организации. Другой способ для гостевого пользователя установить приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] — это когда он получает сообщение чата, содержащее карточку [!INCLUDE [prod_short.md](includes/prod_short.md)]. В этом случае пользователь выбирает кнопку или меню **Сведения** на карточке, затем устанавливает приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для использования в вашей организации. После установки приложения пользователь не получает автоматически никаких разрешений на доступ к данным из вашего [!INCLUDE [prod_short.md](includes/prod_short.md)].

<!--TODO - check with Mike on this -->
---

## <a name="see-also"></a>См. также

[Обзор интеграции [!INCLUDE [prod_short](includes/prod_short.md)] и Microsoft Teams](across-teams-overview.md)  
[Установите приложение [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)  
[Устранение неполадок Teams](admin-teams-troubleshooting.md)  
[Разработка для интеграции Teams](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
