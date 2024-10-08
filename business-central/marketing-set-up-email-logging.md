---
title: Настройка регистрации эл.почты
description: 'Узнайте, как превратить взаимодействие по электронной почте между продавцами и клиентами в реальные возможности продаж.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: how-to
ms.date: 09/18/2023
ms.custom: bap-template
ms.search.keywords: 'relationship, prospect, opportunity, email'
ms.search.form: '1680, 1811, 5076'
ms.service: dynamics-365-business-central
---
# <a name="track-email-message-exchanges-between-salespeople-and-contacts"></a>Отслеживание обмена сообщениями электронной почты между продавцами и контактами

[!INCLUDE[azure-ad-to-microsoft-entra-id](~/../shared-content/shared/azure-ad-to-microsoft-entra-id.md)]

Получите больше от общения между продавцами вашими и клиентами, отслеживая обмен сообщениями электронной почты, затем превращая их в реальные возможности. [!INCLUDE[prod_short](includes/prod_short.md)] может работать с Exchange Online, чтобы вести журнал входящих и исходящих сообщений. Вы можете просматривать и анализировать содержимое каждого сообщения на странице **Журналы взаимодействий**.

> [!IMPORTANT]
> В случае [!INCLUDE[prod_short](includes/prod_short.md)] Online [!INCLUDE[prod_short](includes/prod_short.md)] и Exchange Online должны быть в одном арендаторе.

## <a name="to-set-up-email-logging"></a>Настройка регистрации электронной почты

### <a name="set-up-public-folders-and-rules-for-email-logging-in-exchange-online"></a>Настройка общих папок и правил для регистрации электронной почты в Exchange Online

[!INCLUDE[admin-setup-email-public-folder](includes/admin-setup-email-public-folder.md)]

Далее вы подключаете [!INCLUDE[prod_short](includes/prod_short.md)] с Exchange Online.

### <a name="set-up-a-shared-mailbox-and-rules-for-email-logging-in-exchange-online"></a>Настройка общего почтового ящика и правил для регистрации электронной почты в Exchange Online

> [!NOTE]
> Эти шаги требуют доступа администратора для Exchange Online.

Подготовьте общий почтовый ящик в центре администрирования Exchange. Или вы также можете использовать Exchange Online PowerShell. Для получения дополнительной информации см. [Создание общего почтового ящика](/microsoft-365/admin/email/create-a-shared-mailbox) или [Exchange Online PowerShell](/powershell/exchange/exchange-online-powershell?view=exchange-ps&preserve-view=true).

> [!NOTE]
> Если вы используете Exchange Management PowerShell, ваши изменения доступны в центре администрирования Exchange через некоторое время. Задержка может составить несколько часов.

### <a name="add-a-user-account-for-members-of-the-shared-mailbox"></a>Добавить учетную запись пользователя для членов общего почтового ящика

Учетная запись, которую вы будете использовать для ведения журнала электронной почты, является учетной записью Exchange Online. Запланированное задание будет использовать учетную запись для подключения к общему почтовому ящику и обработки сообщений электронной почты. Эта учетная запись не должна быть связана с конкретным человеком. Добавьте учетную запись электронной почты к участникам общего почтового ящика. Для получения дополнительной информации см. [Использование EAC для изменения делегирования общего почтового ящика](/exchange/collaboration-exo/shared-mailboxes#use-the-eac-to-edit-shared-mailbox-delegation).

### <a name="allow-other-users-to-see-logged-emails"></a>Разрешить другим пользователям просматривать зарегистрированные электронные письма

Вы можете разрешить другому пользователю открывать сообщение электронной почты в Exchange, связанное с записью журнала взаимодействий из [!INCLUDE[prod_short](includes/prod_short.md)]. Для этого дайте пользователю разрешение ``Read`` для папки **Архив** в общем почтовом ящике. Дополнительные сведения см. также в разделе [Exchange Online PowerShell](/powershell/exchange/exchange-online-powershell?view=exchange-ps&preserve-view=true).

### <a name="create-mail-flow-rules"></a>Создать правила потока почты

Правила обработки почты ищут определенные условия в сообщениях и выполняют над ними действия. Создайте два правила потока почты на основе информации в следующей таблице. Дополнительные сведения см. в [Управлять правилами потока почты в Exchange Online](/exchange/security-and-compliance/mail-flow-rules/manage-mail-flow-rules?preserve-view=true) и [Действия правила потока почты в Exchange Online](/exchange/security-and-compliance/mail-flow-rules/mail-flow-rule-actions?preserve-view=true).

|Назначение  |Name  |Примените это правило, если...  |Выполните следующие действия...  |
|---------|---------|---------|---------|
|Правило для входящей эл. почты     |Регистрировать сообщения электронной почты, присланные в эту организацию|Отправитель расположен вне организации, и получатель расположен внутри организации|Скрытая копия учетная запись электронной почты, указанная для общем почтовом ящике.|
|Правило для исходящей эл. почты     |Регистрировать сообщения электронной почты, отправленные из этой организации|Отправитель расположен внутри организации, и получатель расположен вне организации.|Скрытая копия учетная запись электронной почты, указанная для общем почтовом ящике.|

> [!NOTE]
> [!INCLUDE[prod_short](includes/prod_short.md)] обрабатывает только сообщения в папке Входящие в общем почтовом ящике. Если правило перемещает сообщения из папки «Входящие» в другую папку, эти сообщения не будут обрабатываться. Кроме того, сообщения в папке «Нежелательная почта» также игнорируются.

## <a name="set-up--to-log-email-messages"></a>Настройка [!INCLUDE[prod_short](includes/prod_short.md)] для регистрации сообщений электронной почты

Начните работать с регистрацией электронной почты за два простых шага:

1. Соедините [!INCLUDE[prod_short](includes/prod_short.md)] с Exchange Online для своей подписки Microsoft 365. Exchange Online обрабатывает ваши сообщения электронной почты. Мы упростили этот шаг, предоставив мастер настройки. Вам нужны только ваши учетные данные администратора для вашей учетной записи администратора в Microsoft 365. Чтобы запустить руководство, выберите страницу **Мастер настройки**, затем выберите руководство **Настройка регистрации электронной почты**.  

2. Убедитесь, что адреса электронной почты ваших продавцов и контактов в [!INCLUDE[prod_short](includes/prod_short.md)] действительны. Для этого для каждого клиента или продавца откройте карточку **Контакт** или **Менеджер по продажам/закупкам** и посмотрите в поле **Адрес эл. почты**.

    > [!Tip]
    > После выполнения шагов в руководстве вы можете проверить, было ли соединение успешным. Найдите **Регистрация электронной почты**, выберите **Действия**, а затем выберите **Проверить конфигурацию**.

## <a name="view-email-message-exchanges-in-the-interaction-log"></a>Просмотр обмена сообщениями электронной почты в журнале взаимодействия

[!INCLUDE[prod_short](includes/prod_short.md)] создает запись на странице **Журнал взаимодействия** каждый раз, когда продавец и контакт обмениваются сообщениями электронной почты. Чтобы просмотреть журнал взаимодействия, откройте карточку **Контакт** для человека, затем выберите **Связанный**, **История**, затем выберите **Журналы взаимодействий**. Есть несколько вещей, которые мы можем сделать с каждой записью в журнале, например:

* Просмотрите содержимое сообщения электронной почты, которым обменялись собеседники, выбрав **Обработка**, затем **Показать вложения**.
* Превратите обмен электронной почтой в возможную сделку продажи. Если запись выглядит многообещающе, вы можете превратить ее в возможную сделку, а затем управлять ее продвижением к продаже. Чтобы превратить обмен электронной почтой в возможную сделку, выберите запись, а затем **Обработать**, а потом **Создать возможность**. Дополнительные сведения см. в разделе [Управление возможностями продаж](marketing-manage-sales-opportunities.md).

## <a name="mailbox-and-folder-limits-in-exchange-online"></a>Ограничения на почтовые ящики и папки в Exchange Online

В Exchange Online существуют ограничения на почтовые ящики и папки, например на размер папок и количество сообщений. Дополнительные сведения см. в разделах [Ограничения Exchange Online](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#storage-limits) и [Ограничения общедоступных папок в Exchange Server](/Exchange/collaboration/public-folders/limits?view=exchserver-2019&preserve-view=true).

[!INCLUDE[prod_short](includes/prod_short.md)] хранит зарегистрированные сообщения электронной почты в папке Exchange Online. [!INCLUDE[prod_short](includes/prod_short.md)] также хранит ссылку на каждое зарегистрированное сообщение. По ссылкам открываются зарегистрированные сообщения со страниц "Журналы взаимодействий", "Карточка контакта" и "Карточка менеджера по продажам" в [!INCLUDE[prod_short](includes/prod_short.md)] в Exchange Online. Если зарегистрированное сообщение перемещено в другую папку, ссылка не будет работать. Например, сообщение может быть перемещено вручную, или Exchange Online может автоматически запустить функцию AutoSplit при достижении ограничения хранилища.

Следующие шаги могут помочь вам избежать неработающих ссылок на сообщения в Exchange Online.

1. Не перемещайте существующие сообщения в другую папку после изменения настроек журнала регистрации электронной почты. Храните существующие сообщения там, где они есть, чтобы сохранить ссылки. Ссылки на сообщения в новой папке будут действительными.
2. Не превышайте ограничения почтовых ящиков и папок. Если ограничение скоро будет достигнуто, выполните следующие действия:
    1. Настройте новый общий почтовый ящик в Exchange Online.
    2. Обновите правила потока электронной почты в Exchange Online.
    3. Обновите настройки журнала регистрации электронной почты в Business Central соответствующим образом

## <a name="connect-on-premises-versions-to-microsoft-exchange"></a>Подключение локальных версий к Microsoft Exchange

Вы можете подключить локальную версию [!INCLUDE[prod_short](includes/prod_short.md)] к локальной версии Exchange On-Premises или Exchange Online для регистрации электронной почты. Для обеих версий Exchange настройки подключения доступны на странице **Настройка модуля "Маркетинг"**. Для Exchange Online вы также можете воспользоваться мастером настройки.

<!-- [!IMPORTANT]
> The new experience doesn't support a connection to Exchange on-premises. If you must use Exchange on-premises, do not enable the feature update for the new experience.

## <a name="connect-to-exchange-on-premises"></a>Connect to Exchange on-premises
<!--
## [Current Experience](#tab/current-experience)
To connect [!INCLUDE[prod_short](includes/prod_short.md)] on-premises to Exchange on-premises, on the **Marketing Setup** page, you can use **Basic** as the **Authentication Type**, and then enter credentials for the user account for Exchange on-premises. Then turn on the **Enabled** toggle to start logging email.

## [New Experience](#tab/new-experience)
The new experience does not support connections to Exchange on-premises.
-->
## <a name="connect-to-exchange-online"></a>Подключение к Exchange Online

Для подключения к Exchange Online необходимо зарегистрировать приложение в Microsoft Entra ID. Укажите идентификатор приложения, секрет хранилища ключей и URL-адрес перенаправления для использования для регистрации. URL-адрес перенаправления предварительно задан и должен работать для большинства установок. Дополнительные сведения см. в разделе [Регистрация приложения в Microsoft Entra ID для подключения из Business Central к Exchange Online](#to-register-an-application-in-microsoft-entra-id-for-connecting-from-business-central-to-exchange-online). 

Также вы должны использовать **OAuth2** как **Тип аутентификации**. Также необходимо зарегистрировать приложение в Microsoft Entra ID. Укажите идентификатор приложения, секрет хранилища ключей и URL-адрес перенаправления для использования для регистрации. URL-адрес перенаправления предварительно заполнен и должен работать для большинства установок. Дополнительные сведения см. в разделе Регистрация приложения в Microsoft Entra ID для подключения из Business Central к Exchange Online ниже.

Вы должны настроить вашу установку на использование HTTPS. Для получения дополнительной информации см. [Настройка SSL для защиты подключения веб-клиента Business Central](/dynamics365/business-central/dev-itpro/deployment/configure-ssl-web-client-connection). Если вы настраиваете на своем сервере другую начальную страницу, вы можете изменить URL-адрес. Секрет клиента будет сохранен как зашифрованная строка в вашей базе данных.

### <a name="to-register-an-application-in-microsoft-entra-id-for-connecting-from-business-central-to-exchange-online"></a>Регистрация приложения в Microsoft Entra ID для подключения из Business Central к Exchange Online

Следующие шаги предполагают, что вы используете Microsoft Entra ID для управления удостоверениями и доступом. Дополнительные сведения см. в [Быстрый старт: зарегистрируйте приложение на платформе идентификации Microsoft](/azure/active-directory/develop/quickstart-register-app). 

1. В Azure Portal, в пункте **Управление** выберите **Аутентификация**.
2. В пункте **URL-адрес перенаправления** добавьте URL-адрес перенаправления, который предлагается на страница **Регистрация электронной почты** в [!INCLUDE[prod_short](includes/prod_short.md)]. Если поле URL-адреса перенаправления на странице регистрации электронной почты пуст, найдите предлагаемый URL-адрес перенаправления на странице **Мастер настройки**. Чтобы открыть страницу, на странице **Регистрация электронной почты**, выберите **Действия**, а потом **Мастер настройки**.

    > [!NOTE]
    > Если вы не укажете URL-адрес перенаправления, вы можете сделать это позже, выбрав **Добавить платформу**, затем выбрав **Интернет**, чтобы добавить веб-приложение и URL-адрес перенаправления.

3. В **Управление** выберите **Разрешения API** и выберите **Microsoft Graph**, а затем выберите **Делегированные разрешения**.
4. Используйте поле поиска, чтобы найти и выбрать **Почта**, а затем добавьте разрешение **Mail.ReadWrite.Shared**. 
5. В **Управление** выберите **Сертификаты и секреты**, а затем создайте новый секрет для вашего приложения. Вы будете использовать секрет в поле **Секрет клиента** на странице **Регистрация электронной почты** в [!INCLUDE[prod_short](includes/prod_short.md)].
6. Выберите **обзор**, а затем найдите значение **Код приложения (клиента)**. Это код клиента вашего приложения. Вы должны ввести его либо в поле **Код клиента** на странице **Регистрация электронной почты**.
7. В [!INCLUDE[prod_short](includes/prod_short.md)] настройте регистрацию электронной почты на странице **Регистрация электронной почты** или используйте **Мастер настройки** для помощи.

### <a name="use-another-identity-and-access-management-service"></a>Использование другой службы управления удостоверениями и доступом

Если вы не используете Microsoft Entra ID для управления удостоверениями и доступом, вам потребуется помощь разработчика. Если вы предпочитаете хранить код приложения и секрет в другом месте, вы можете оставить поля «Код клиента» и «Секрет клиента» пустыми и написать расширение для получения кода и секрета из местоположения. Вы можете предоставить секрет во время выполнения, подписавшись на события OnGetEmailLoggingClientId и OnGetEmailLoggingClientSecret в codeunit 1641 "Настройка регистрации электронной почты".

## <a name="to-start-logging-email"></a>Начала регистрации электронной почты

1. Чтобы начать регистрацию электронной почты, на странице **Регистрация электронной почты** включите переключатель **Включено**.
2. Войдите с учетной записью Exchange Online, которую запланированное задание будет использовать для подключения к общему почтовому ящику и обработки сообщений электронной почты.

    > [!NOTE]
    > Если вам не предлагается войти в систему с учетной записью Exchange Online, возможно, это связано с блокировкой всплывающих окон браузером. Чтобы войти, разрешите всплывающие окна от https://login.microsoftonline.com.

## <a name="to-stop-logging-email"></a>Остановка регистрации электронной почты

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Регистрация электронной почты**, а затем выберите связанную ссылку.
2. Выключите переключатель **Включено**.

## <a name="to-change-the-user-account-used-for-email-logging"></a>Чтобы изменить учетную запись пользователя, используемую для регистрации электронной почты

### <a name="-online"></a>[!INCLUDE[prod_short](includes/prod_short.md)] Online

1. Войдите в [!INCLUDE[prod_short](includes/prod_short.md)] с учетной записью, которую запланированное задание будет использовать для подключения к общему почтовому ящику и обработки сообщений электронной почты. Эта учетная запись должна иметь доступ к [!INCLUDE[prod_short](includes/prod_short.md)] и Exchange Online.
2. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") введите **Регистрация электронной почты**, а затем выберите связанную ссылку. 
3. Выберите **Связанный**, а потом **Операция очереди работ**.
4. Перезапустите задание **Регистрация электронной почты**.

### <a name="-on-premises"></a>Локальная версия [!INCLUDE[prod_short](includes/prod_short.md)]

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") введите **Регистрация электронной почты**, а затем выберите связанную ссылку.
2. Выберите **Действия**, а потом **Продлить маркер**.
3. Войдите с учетной записью Exchange Online, которую запланированное задание будет использовать для подключения к общему почтовому ящику и обработки сообщений электронной почты.

## <a name="see-also"></a>См. также
[Управление отношениями](marketing-relationship-management.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
