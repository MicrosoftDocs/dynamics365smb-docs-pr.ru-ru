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
ms.date: 05/19/2021
ms.author: jswymer
ms.openlocfilehash: f3c9626fa73247b2109e5f179aef405e80b44b07
ms.sourcegitcommit: 5a916b0aa0a2eef0c22b5722a0af041757e6d7c2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "6074644"
---
# <a name="teams-faq"></a>Вопросы и ответы по Teams

[!INCLUDE [online_only](includes/online_only.md)]

В этой статье даны ответы на некоторые вопросы, которые могут у вас возникнуть по работе с Teams и [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="general"></a>[Общие](#tab/general)

### <a name="how-do-i-sign-in-to-the-prod_shortmd-app-in-teams"></a>Как мне войти в приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] в Teams?

После установки приложения вам будет предложено войти в систему при первом использовании приложения, когда вы вставляете ссылку [!INCLUDE [prod_short.md](includes/prod_short.md)] в чат Teams или выбираете действие **Детали** на карточке в Teams. В зависимости от вашего клиента Teams вам может потребоваться ввести свои учетные данные, которые вы используете для доступа к [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="how-do-i-sign-out-of-the-prod_shortmd-app-in-teams"></a>Как мне выйти из приложения [!INCLUDE [prod_short.md](includes/prod_short.md)] в Teams?

Чтобы выйти из текущего удостоверения пользователя в Teams, используемого для подключения к [!INCLUDE [prod_short.md](includes/prod_short.md)], перейдите в любое окно создания чата, щелкните правой кнопкой мыши значок [!INCLUDE [prod_short.md](includes/prod_short.md)] снизу, затем выберите **Параметры**. Когда появится окно, проверьте свой идентификатор, с которым вы в настоящее время находитесь в системе, затем выберите **Выход**.

### <a name="does-the-app-for-teams-connect-to-prod_shortmd-on-premises"></a>Подключается ли приложение для Teams к [!INCLUDE [prod_short.md](includes/prod_short.md)] On Premises? 

Кол-во Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams работает только с [!INCLUDE [prod_short.md](includes/prod_short.md)] Online. Нет планов поддерживать типы развертывания [!INCLUDE [prod_short.md](includes/prod_short.md)], &mdash; например, локальное, гибридное или частное облако, &mdash; которые Microsoft не размещает и не управляет ими напрямую.

### <a name="does-the-app-work-with-multiple-companies-and-environments"></a>Работает ли приложение с несколькими компаниями и средами? 

Да. Чтобы найти контакты в другой компании, перейдите в [Параметры](across-teams-settings.md). Когда приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] разворачивает ссылку в карточку, ссылка должна содержать названия сред и компаний, чтобы приложение соответствовало записи в нужной компании. Вы можете вставлять ссылки на любые компании и среды, к которым у вас есть доступ в вашей организации, и из учетной записи [!INCLUDE [prod_short.md](includes/prod_short.md)], которую вы использовали для входа. Карточку увидят участники чата. Но они не могут просматривать данные карточки, если у них нет разрешений для компании или среды, в которой хранится эта запись.

### <a name="in-which-countries-or-regions-is-the-prod_shortmd-app-available"></a>В каких странах или регионах приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] доступно? 

Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams не ограничено страной или регионом. Приложение доступно на всех рынках, которые в настоящее время поддерживаются магазином Teams. 

### <a name="does-the-prod_shortmd-app-work-with-any-localization-of-prod_shortmd"></a>Работает ли приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] с любой локализацией [!INCLUDE [prod_short.md](includes/prod_short.md)]? 

Да. Приложение предназначено для работы с любой локализацией [!INCLUDE [prod_short.md](includes/prod_short.md)], независимо от того, предлагается ли эта локализация напрямую от Microsoft или через партнера. Дополнительные сведения см. в [Наличие в странах/регионах и поддерживаемые языки](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations?toc=/dynamics365/business-central/toc.json).

### <a name="which-languages-does-the-prod_shortmd-app-support"></a><a name="language"></a>Какие языки поддерживает приложение [!INCLUDE [prod_short.md](includes/prod_short.md)]?

Язык, используемый для карточек и деталей карточек в Teams, определяется двумя вещами:

1. Ваш язык в Teams, который вы можете увидеть в настройках своей учетной записи в Teams. 
2. Ваш язык в [!INCLUDE [prod_short.md](includes/prod_short.md)], который вы можете увидеть в веб-клиенте [!INCLUDE [prod_short.md](includes/prod_short.md)] (см. раздел [Изменение базовых настроек — язык](ui-change-basic-settings.md#language)).

В следующей таблице объясняется, чем отличается взаимодействие для авторов и получателей сообщений в зависимости от языковых настроек и доступности языков.

|Кто|Карточка|Детали карточки |
|-|----|--------------| 
|Автор сообщения |Отображается на языке, который указан для вас в Teams. Если [!INCLUDE [prod_short.md](includes/prod_short.md)] не предлагает тот же язык, карточка отображается на английском языке. |Отображается на языке, который указан для вас в [!INCLUDE [prod_short.md](includes/prod_short.md)].  которые могут включать языки из языковых приложений, предоставляемых партнерами. |
|Получатель сообщения |Отображается на языке автора сообщения. |Отображается на языке, который указан для вас в [!INCLUDE [prod_short.md](includes/prod_short.md)]. |

Список поддерживаемых языков для [!INCLUDE [prod_short.md](includes/prod_short.md)] см. в разделе [Поддерживаемые языки](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations?toc=/dynamics365/business-central/toc.json#supported-languages).

### <a name="does-the-prod_shortmd-app-work-with-industry-solutions"></a>Совместимо ли приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] с отраслевыми решениями?

Да. Но только некоторые функции приложения работают с [внедренными приложениями](/dynamics365/business-central/dev-itpro/deployment/embed-app-overview):

- Приложение работает со ссылками на основе шаблона **\*.bc.dynamics.com**, который обычно используется с внедрением приложений.
- Поиск контактов недоступен для встраиваемых приложений, заменяющих базовое приложение от Microsoft.

### <a name="where-can-i-find-teams-integration-inside-the-prod_shortmd-web-client"></a>Где я могу найти интеграцию Teams в веб-клиенте [!INCLUDE [prod_short.md](includes/prod_short.md)]? 

В настоящее время нет встраивания элементов управления Teams или наличия функций Teams внутри веб-клиента [!INCLUDE [prod_short.md](includes/prod_short.md)] или других клиентов.

### <a name="does-prod_shortmd-work-with-the-teams-mobile-app"></a>Работает ли [!INCLUDE [prod_short.md](includes/prod_short.md)] с мобильным приложением Teams?

Да. Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] может быть установлено из классического приложения Teams или браузера либо администратором для всех пользователей. После установки приложения [!INCLUDE [prod_short.md](includes/prod_short.md)] автоматически доступно в Teams для iOS и Android. На мобильных устройствах вы можете просматривать только карточки, отправленные другими, получать доступ к деталям или открывать карточку в полном объеме в мобильном приложении [!INCLUDE [prod_short.md](includes/prod_short.md)]. Вы не можете вставлять ссылки, которые расширяются в карточки при составлении сообщений или искать контакты. Минимальные требования для мобильных устройств см. в разделе [Минимальные требования для использования Business Central](product-requirements.md).

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

- Доступ к камере и местоположению невозможен из окна сведений в настольном приложении Teams.
- Номера телефонов нельзя активировать из окна сведений в Teams для iOS, Teams для Android или Teams в браузере.
- Использование Microsoft Edge с Teams в браузере позволяет легко работать с несколькими удостоверениями и учетными записями, входя в Teams из разных профилей. Чтобы узнать об использовании профилей в Microsoft Edge, см. раздел [Вход и создание нескольких профилей в Microsoft Edge](https://support.microsoft.com/office/sign-in-and-create-multiple-profiles-in-microsoft-edge-df94e622-2061-49ae-ad1d-6f0e43ce6435) в службе поддержки Microsoft.

### <a name="what-is-the-best-way-for-me-to-demonstrate-prod_shortmd-and-microsoft-teams-to-prospective-customers"></a>Как мне лучше всего продемонстрировать [!INCLUDE [prod_short.md](includes/prod_short.md)] и Microsoft Teams потенциальным клиентам?

Если вы являетесь партнером по перепродаже, вам может потребоваться среда, которую вы можете показывать потенциальным клиентам в рамках предпродажных демонстраций. Чтобы не повлиять на Microsoft Teams в своей организации, вы можете получить демонстрационную учетную запись Microsoft 365 по адресу [https://aka.ms/CDX](https://aka.ms/CDX). Эта учетная запись дает вам полный контроль над независимой организацией Azure, которая включает Microsoft Teams и [!INCLUDE [prod_short.md](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Подготовка демонстрационных сред для Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/administration/demo-environment).

### <a name="does-the-prod_shortmd-app-for-teams-cater-for-my-customization-and-personalization"></a>Учитывает ли приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams мою настройку и персонализацию?

Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams может отображать карточки для ссылок на страницы и таблицы клиентов в [!INCLUDE [prod_short.md](includes/prod_short.md)], например страницы и таблицы, созданные из ваших собственных расширений или из AppSource.

На поля, отображаемые на карточке в Teams, также могут влиять настройки [!INCLUDE [prod_short.md](includes/prod_short.md)], установленные для вашей организации. Карточки не учитывают никакую индивидуальную настройку ролей или персонализацию пользователя. Однако в окне сведений о карточке отображаются сведения о записях, как если бы вы их видели в [!INCLUDE [prod_short.md](includes/prod_short.md)], включая любые расширения, настройки ролей и персонализацию пользователей.

При поиске контактов поля, совпадающие в таблице **Контакты**, и поля, отображаемые в результатах поиска, не подвергаются никаким настройкам или персонализации.

### <a name="how-do-the-permissions-required-by-the-app-affect-my-privacy"></a>Как разрешения, требуемые приложением, влияют на мою конфиденциальность?

Перед установкой приложения [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams вы можете просмотреть минимальные разрешения, необходимые для работы приложения. Устанавливая приложение, вы соглашаетесь с тем, что у приложения есть разрешение на получение сообщений и данных, которые вы ему предоставляете, а у Teams есть разрешение на хранение и обработку этих сообщений.

Кроме того, некоторые функции [!INCLUDE [prod_short.md](includes/prod_short.md)] требуют открытия внешних ссылок или доступа к вашей камере или географическому положению. Например, предположим, что вы хотите сделать фотографию счета-фактуры на покупку для обработки. Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] не использует эти возможности без вашего согласия, и они используются только определенными функциями в окне **Подробнее**. Когда вы используете одну из этих функций в первый раз, Teams отобразит диалоговое окно с просьбой предоставить доступ к необходимым возможностям устройства.

- На рабочем столе Teams вы просматриваете и настраиваете разрешения приложений в окне **Настройки**. Выберите изображение своего профиля вверху приложения, выберите **Настройки** > **Разрешения**, затем выберите приложение [!INCLUDE [prod_short.md](includes/prod_short.md)].

- Для Teams в браузере и для Teams для iOS или Android вы можете просмотреть или изменить разрешения в настройках браузера или устройства.

> [!NOTE]
> Какие функции [!INCLUDE [prod_short.md](includes/prod_short.md)] запрашивают разрешения, зависит от дополнительных приложений и настроек, примененных к среде [!INCLUDE [prod_short.md](includes/prod_short.md)], к которой вы подключаетесь.

### <a name="where-can-i-learn-about-my-privacy"></a>Где я могу узнать о своей конфиденциальности? 

Вы можете узнать о том, как Microsoft обрабатывает ваши данные, в разделе [Заявление о конфиденциальности Microsoft](https://go.microsoft.com/fwlink/?linkid=2030602). 

Обратитесь к своему администратору, чтобы узнать, как ваша организация обеспечивает конфиденциальность ваших данных.

### <a name="how-do-i-uninstall-the-prod_shortmd-app-for-teams"></a>Как мне удалить приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams?

Чтобы удалить приложение, которое вы установили для себя, перейдите в любое окно создания чата, найдите значок [!INCLUDE [prod_short.md](includes/prod_short.md)] внизу, щелкните значок правой кнопкой мыши и выберите **Удалить**.  

### <a name="will-microsoft-continue-to-improve-the-prod_shortmd-app-for-teams"></a>Будет ли Microsoft продолжать улучшать приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams?

В Microsoft мы постоянно слушаем отзывы от нашего разнообразного сообщества пользователей и действуем по лучшим предложениям. Чтобы узнать, что будет дальше для приложения [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams, см. раздел [План выпуска Dynamics 365](/dynamics365-release-plan/2021wave1/).

Если вы хотите участвовать в улучшении приложения для Teams или у вас есть идея, которая поможет упростить вашу работу или совместную работу в Teams, добавьте идею или проголосуйте за существующие идеи на сайте [https://aka.ms/BusinessCentralIdeas](https://aka.ms/BusinessCentralIdeas).

## <a name="searching-for-contacts"></a>[Поиск контактов](#tab/contacts)

### <a name="which-tables-does-the-app-search-in"></a>В каких таблицах приложение выполняет поиск?

При поиске контактов из приложения [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams ваши условия поиска сопоставляются с записями в таблице **Контакты** в [!INCLUDE [prod_short.md](includes/prod_short.md)]. 

### <a name="which-fields-in-the-contacts-table-can-i-search"></a>В каких полях таблицы контактов я могу искать?

По мере того, как вы вводите условия поиска в поле поиска, они сопоставляются с большинством полей в таблице **Контакты**. Поля включают, например, **Номер**, **Имя**, поля **Адрес**, **Номер телефона** или **Номер мобильного телефона**, а также **Электронная почта**. 

Условия поиска не сопоставляются ни с одним настраиваемым полем, добавленным в таблицу **Контакты** приложениями и расширениями.

### <a name="do-search-results-include-companies-and-persons"></a>Включают ли результаты поиска компании и людей?

Да. В [!INCLUDE [prod_short.md](includes/prod_short.md)] контакты могут быть типа **Компания** или типа **Человек**, где одно или несколько физических лиц могут быть связаны с компанией. В результатах поиска компании и физические лица имеют разные значки.

### <a name="do-contacts-of-any-business-relationship-appear-in-the-results"></a>Появляются ли в результатах контакты, связанные с какими-либо деловыми отношениями?

Да. Некоторые контакты могут представлять клиентов или поставщиков, либо и то, и другое. Другие контакты, не имеющие определенных деловых отношений, обычно представляют потенциальных клиентов. Контакты с другими деловыми отношениями, включая любые настраиваемые отношения, которые вы настроили в [!INCLUDE [prod_short.md](includes/prod_short.md)], также будет отображаться в результатах поиска.

### <a name="can-i-look-up-contact-details-during-meetings"></a>Могу ли я посмотреть сведения о контактах во время встреч?

Да. Вы можете искать контактную информацию, историю взаимодействия и связанные документы для своего клиента или поставщика во время собрания Teams или позвонить во время собрания, не выходя из Teams.

Фактически, вы можете искать сведения о контактах из любого места в Teams, используя командное поле. Вы можете, например, найти сведения о контакте в календаре Teams, чтобы помочь вам настроить встречи.

### <a name="how-do-i-view-my-last-interactions-with-a-contact"></a>Как просмотреть мои последние взаимодействия с контактом?

В окне сведений о контакте отображаются записи журнала взаимодействий. Записи журнала взаимодействий предоставляют историю взаимодействий, которые ваша организация имела с конкретным контактом. Взаимодействия могут включать электронные письма, которыми вы обменивались, полученные звонки или отправленные вами документы.

Чтобы взаимодействия отображались, [!INCLUDE [prod_short.md](includes/prod_short.md)] должен быть настроен для отслеживания взаимодействий. Чтобы узнать больше о ведении журнала взаимодействий, см. раздел [Запись взаимодействий с контактами](marketing-interactions.md).

### <a name="how-do-i-register-a-teams-call-or-meeting-as-an-interaction"></a>Как зарегистрировать звонок или встречу Teams как взаимодействие?

В окне сведений для контакта найдите действие **Создать взаимодействие** и выберите из входящих или исходящих вызовов в качестве шаблонов взаимодействия. Вы также можете создавать собственные настраиваемые шаблоны взаимодействия специально для использования с разговорами Teams.

### <a name="can-i-call-a-contact-from-the-prod_shortmd-app-for-teams"></a>Могу ли я позвонить контакту из приложения [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams?

[!INCLUDE [prod_short.md](includes/prod_short.md)] имеет ограниченную интеграцию с возможностями вызова Teams. Невозможно мгновенно начать VOIP-звонок из карточки контакта или окна сведений о контакте. Однако при просмотре сведений о контакте в классическом приложении Teams вы можете выбрать поле номера телефона, чтобы набрать этот номер, если Teams настроено в качестве приложения для набора номера по умолчанию на вашем устройстве. Чтобы набирать номера стационарных или мобильных телефонов с помощью ТСОП, традиционной телефонной системы, Teams требуется приложение Microsoft 365 Business Voice. Чтобы узнать больше, см. раздел [Что такое Microsoft 365 Business Voice?](/MicrosoftTeams/business-voice/whats-business-voice).

### <a name="how-do-i-view-recent-documents-for-a-customer-or-vendor"></a>Как просмотреть последние документы для клиента или поставщика?

[!INCLUDE [prod_short.md](includes/prod_short.md)] обычно связывает контакт с записью клиента или поставщика, которая, в свою очередь, связана с записями бизнес-транзакций, такими как коммерческие предложения или счета-фактуры на закупку. Чтобы просмотреть связанные документы для контакта, перейдите в окно сведений о контакте, выберите значение поля **Деловые отношения** или используйте действия для перехода к связанному покупателю или поставщику. На странице клиента или поставщика разверните информационную панель, чтобы отобразить статистику по различным документам, которую можно детализировать. Ваш опыт может отличаться в зависимости от ваших настроек и персонализации.

### <a name="how-do-i-search-for-contacts-using-special-characters"></a>Как искать контакты с помощью специальных символов?

Вы можете ввести критерии поиска, используя практически любые символы Юникода. Однако [!INCLUDE [prod_short.md](includes/prod_short.md)] резервирует следующие символы для других целей: **=**, **.**, **\**_, и _*@**. Использование этих символов в поисковых запросах может не дать ожидаемых результатов. Если вы не видите ожидаемых результатов, заключите символы в условиях поиска в одинарные кавычки, например, **Contoso'='2**.

### <a name="how-can-i-search-contacts-stored-in-a-different-company"></a>Как я могу искать контакты, хранящиеся в другой компании?

Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams может искать клиентов, поставщиков и другие контакты в одной компании за раз.  
Для поиска контактов, хранящихся в другой компании [!INCLUDE [prod_short.md](includes/prod_short.md)], откройте [Параметры](across-teams-settings.md), затем измените среду и компанию оттуда.

### <a name="are-prod_shortmd-contacts-different-than-the-ones-in-the-teams-contacts-screen"></a>Отличаются ли контакты [!INCLUDE [prod_short.md](includes/prod_short.md)] от контактов на экране контактов Teams?

Да. Контакты хранящиеся в [!INCLUDE [prod_short.md](includes/prod_short.md)], представляют деловые контакты, доступные для вашей организации. Это контакты, с которыми у вас есть устоявшиеся и четко определенные деловые отношения, или контакты, которые представляют потенциальных клиентов. Эти контакты обычно являются внешними. Для сравнения, контакты, показанные в списке контактов для звонков Teams, являются вашими собственными контактами. Эти контакты не обязательно являются общими для других в вашей организации, и они обычно представляют собой контакты внутри вашей организации.

### <a name="does-prod_shortmd-synchronize-contacts-with-teams"></a>Синхронизирует ли [!INCLUDE [prod_short.md](includes/prod_short.md)] контакты с Teams?

Кол-во Контакты, хранящиеся в [!INCLUDE [prod_short.md](includes/prod_short.md)], остаются отдельными от ваших контактов, хранящихся в Teams.
В настоящее время нет планов синхронизировать два списка вместе.

### <a name="what-is-the-minimum-version-of-prod_shortmd-for-contact-search"></a>Какая минимальная версия [!INCLUDE [prod_short.md](includes/prod_short.md)] для поиска контактов?

Для поиска контактов необходимо, чтобы вы установили приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams версии 1.0.4 или более поздней, и вы подключаетесь к средам [!INCLUDE [prod_short.md](includes/prod_short.md)] версии 18 или новее.

### <a name="can-i-search-from-my-mobile-device"></a>Могу ли я искать со своего мобильного устройства?

Поиск контактов недоступен в Teams для iOS и в Teams для Android в настоящее время.

### <a name="which-permissions-do-i-need-for-contact-search"></a>Какие разрешения мне нужны для поиска контактов?

Для поиска контактов вам потребуется разрешение на уровне объекта для таблицы **Контакты** в компании [!INCLUDE [prod_short.md](includes/prod_short.md)], в которой производится поиск. Чтобы просмотреть окно сведений о контакте, вам нужно как минимум разрешение на чтение для страницы **Контакт** в компании [!INCLUDE [prod_short.md](includes/prod_short.md)] и любых других связанных объектов.

### <a name="can-i-use-contact-search-if-im-a-delegated-admin"></a>Могу ли я использовать поиск по контактам, если я уполномоченный администратор?

Да. Вы также можете искать контакты и сведения о контактах, если у вас есть делегированная роль администратора в организации.

### <a name="is-contact-search-affected-by-api-limits"></a>На поиск контактов влияют ограничения API?

Да. Поиск контактов в Teams основан на API-интерфейсах [!INCLUDE [prod_short.md](includes/prod_short.md)] v2.0 и на него распространяются все ограничения API, которые управляют использованием. Вы можете узнать больше об ограничениях в разделе [Текущие ограничения API](/dynamics-nav/api-reference/v2.0/dynamics-current-limits).

### <a name="why-does-it-sometimes-ask-me-to-set-up-the-app"></a>Почему иногда меня просят настроить приложение?

После входа в приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams впервые приложение попытается определить вашу предпочтительную компанию в [!INCLUDE [prod_short.md](includes/prod_short.md)]. Если приложение не может определить компанию, возможно, вам придется перейти в пункт **Параметры** и выбрать компанию, в которой хотите вести поиск. Такая ситуация возникает, например, если у вас есть доступ к нескольким компаниям в разных средах вашей организации. В этом случае вам нужно будет выбрать компанию, прежде чем вы сможете начать поиск.  

Приложение также может попросить вас перейти в раздел **Параметры**, если у вас нет подписки [!INCLUDE [prod_short.md](includes/prod_short.md)], нет сред [!INCLUDE [prod_short.md](includes/prod_short.md)] или в вашей учетной записи нет лицензии [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="id-like-to-search-for-items-or-records-from-other-tables-can-i-do-this-from-teams"></a>Я хочу искать элементы или записи из других таблиц. Могу ли я сделать это из Teams?

В настоящее время поиск в других таблицах невозможен. Приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams ищет только в списке контактов [!INCLUDE [prod_short.md](includes/prod_short.md)], который может включать поставщиков, клиентов и другие контакты.

Если вы хотите, чтобы возможности поиска развивались и включали другие таблицы, мы рекомендуем нашему сообществу добавить идею или проголосовать за существующие идеи на сайте https://aka.ms/BusinessCentralIdeas.

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

Когда вы составляете и отправляете в чат сообщение с карточкой, все пользователи увидят карточку, &mdash; даже если они не установили приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для Teams.

### <a name="how-do-i-find-out-which-company-a-card-in-teams-belongs-to"></a>Как узнать, какой организации принадлежит карточка в Teams?

Если вы работаете в организациях [!INCLUDE [prod_short.md](includes/prod_short.md)], обратитесь к своему администратору с вопросом о включении логотипа организации для каждой организации. Если этот параметр включен, эта понятная подсказка отображается в любом окне сведений в Teams и показывает компанию и среду, к которой принадлежит запись. Чтобы узнать, как настроить значок организации, см. [Отображение эмблемы организации для быстрого доступа к информации об организации](ui-change-basic-settings.md#badge).

## <a name="working-with-card-details"></a>[Работа со сведения карточки](#tab/carddetails)

### <a name="where-is-the-save-button-in-the-details-window-in-teams"></a>Где находится кнопка сохранения в окне сведений в Teams?

[!INCLUDE [prod_short.md](includes/prod_short.md)] автоматически сохраняет изменения, внесенные вами в любое поле, как только вы покидаете поле. Чтобы покинуть поле, щелкните/коснитесь в любом месте за пределами поля или используйте клавишу TAB для перехода к следующему полю. Когда данные появляются в диалоге в окне сведений, вам может потребоваться выбрать кнопку **ОК**, чтобы [!INCLUDE [prod_short.md](includes/prod_short.md)] сохранил ваши изменения.

### <a name="if-i-choose-to-view-details-for-a-card-will-other-users-see-my-details-window"></a>Если я выберу просмотр сведений для карточки, будут ли другие пользователи видеть мое окно сведений?

Кол-во Хотя все в чате или встрече могут просматривать саму карточку, окно с подробностями появляется только на вашем устройстве тогда, когда вы выбираете **Сведения**. Другие пользователи должны выбрать **Сведения**, если они хотят просмотреть окно со сведения на своем устройстве.

### <a name="can-i-start-a-teams-call-from-the-details-window-in-teams"></a>Могу ли я начать вызов Teams из окна сведений в Teams?

Да. Если вы используете классическое приложение Teams, начните вызов, выбрав связанный номер набора в поле номера телефона, например в поле **Номер мобильного телефона** на карточке **Контакт**. Teams должно быть назначенным вами приложением для набора номера.

Чтобы звонить на местные или международные стационарные и мобильные телефоны, для Teams требуется, чтобы вас была лицензия Business Voice для корпоративных звонков. Кроме того, вы должны настроить Teams в качестве вашего решения для звонков. Чтобы узнать больше, см. раздел [Планирование голосового решения Teams](/microsoftteams/cloud-voice-landing-page) в документации Teams.

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

Да. Приглашение гостевых пользователей из-за пределов вашей организации для участия в чате или на канале дает им аналогичный, но не идентичный опыт по сравнению с пользователями в вашей организации. Когда гость получает сообщение с карточкой, он может ее просмотреть. Гости также могут открыть окно сведений, если им предоставлено разрешение на доступ к этим данным в [!INCLUDE [prod_short.md](includes/prod_short.md)] и назначена лицензия [!INCLUDE [prod_short.md](includes/prod_short.md)] в вашей организации. Когда гость пишет сообщение, ссылки на его или ваш [!INCLUDE [prod_short.md](includes/prod_short.md)] не расширяются в карточки.

Чтобы узнать о других сходствах и различиях между гостями и членами рабочей группы, см. раздел [Опыт гостевых символов в Teams](/MicrosoftTeams/guest-experience) в документации Teams.

### <a name="how-does-a-guest-user-install-the-prod_shortmd-app"></a>Как гостевой пользователь устанавливает приложение [!INCLUDE [prod_short.md](includes/prod_short.md)]? 

Гости не имеют доступа к магазину приложений для самостоятельной установки приложений. Однако приложение может быть автоматически установлено для них в соответствии с политиками вашей организации. Другой способ для гостевого пользователя установить приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] — это когда он получает сообщение чата, содержащее карточку [!INCLUDE [prod_short.md](includes/prod_short.md)]. В этом случае пользователь выбирает кнопку или меню **Сведения** на карточке, затем устанавливает приложение [!INCLUDE [prod_short.md](includes/prod_short.md)] для использования в вашей организации. После установки приложения пользователь не получает автоматически никаких разрешений на доступ к данным из вашего [!INCLUDE [prod_short.md](includes/prod_short.md)].

---

## <a name="see-also"></a>См. также

[Обзор интеграции [!INCLUDE [prod_short](includes/prod_short.md)] и Microsoft Teams](across-teams-overview.md)  
[Установите приложение [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)  
[Устранение неполадок Teams](admin-teams-troubleshooting.md)  
[Разработка для интеграции Teams](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]