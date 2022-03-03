---
title: Настройка электронной почты в Business Central (содержит видео)
description: Описывается, как подключить учетные записи электронной почты к Business Central, чтобы вы могли отправлять исходящие сообщения, не открывая другое приложение.
author: bholtorf
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: SMTP, email, Office 365, connector
ms.search.form: 1805, 9813, 9814, 1262, 1263
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: dfeb85bae0329059d4dda9b5edc302b4d0e908e6
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "8142553"
---
# <a name="set-up-email"></a>Настройка электронной почты
Сотрудники предприятий ежедневно отправляют по электронной почте информацию и документы, такие как заказы на продажу и покупку и счета-фактуры. Администраторы могут сделать это проще, подключив одну или несколько учетных записей электронной почты к [!INCLUDE[prod_short](includes/prod_short.md)], так что вы можете отправлять документы, не открывая приложение электронной почты. Вы можете составлять каждое сообщение индивидуально с помощью основных инструментов форматирования, таких как шрифты, стили, цвета и т. д., и добавлять вложения размером до 100 МБ. Администраторы также могут настроить макеты отчетов, которые включают только ключевую информацию из документов. Дополнительные сведения см. в разделе [Отправка документов по электронной почте](ui-how-send-documents-email.md).

Возможности электронной почты в [!INCLUDE[prod_short](includes/prod_short.md)] предназначены только для исходящих сообщений. Вы не можете получать ответы, то есть в [!INCLUDE[prod_short](includes/prod_short.md)] нет страницы папки "Входящие".

> [!NOTE]
> Вы можете использовать возможности электронной почты [!INCLUDE[prod_short](includes/prod_short.md)] онлайн только с Exchange Online. Мы не поддерживаем гибридные сценарии, такие как подключение [!INCLUDE[prod_short](includes/prod_short.md)] онлайн к локальной версии Exchange.
> 
> Если вы используете [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises, прежде чем вы сможете настроить электронную почту, вы должны создать регистрацию приложения для [!INCLUDE[prod_short](includes/prod_short.md)] на портале Azure. Регистрация приложения позволит [!INCLUDE[prod_short](includes/prod_short.md)] авторизовать и аутентифицировать вашего поставщика электронной почты. Дополнительные сведения см. в разделе [Настройка электронной почты для Business Central On-Premises](admin-how-setup-email.md#setting-up-email-for-business-central-on-premises). В [!INCLUDE[prod_short](includes/prod_short.md)] Online мы сделаем это за вас.

## <a name="required-permissions"></a>Необходимые разрешения
Чтобы настроить электронную почту, у вас должен быть набор разрешений **НАСТРОЙКА ЭЛ. ПОЧТЫ**. Дополнительные сведения см. в разделе [Назначение разрешений пользователям и группам](ui-define-granular-permissions.md). 

## <a name="adding-email-accounts"></a>Добавление учетных записей электронной почты
Вы добавляете учетные записи электронной почты через расширения, которые позволяют учетным записям разных поставщиков подключаться к [!INCLUDE[prod_short](includes/prod_short.md)]. Стандартные расширения позволяют использовать учетные записи из Microsoft Exchange Online, но могут быть доступны и другие расширения, позволяющие подключать учетные записи других поставщиков, например Gmail.

После добавления учетной записи электронной почты вы можете указать предопределенные бизнес-сценарии, в которых она будет использоваться для отправки электронных писем. Например, вы можете указать, что все пользователи отправляют документы по продаже из одной учетной записи, а документы на покупку — из другой. Для получения дополнительной информации см. раздел [Назначение сценариев электронной почты учетным записям электронной почты](admin-how-setup-email.md#assign-email-scenarios-to-email-accounts).

В следующей таблице описаны расширения электронной почты, доступные по умолчанию.

|Расширение  |Описание  |Примеры того, когда использовать  |
|---------|---------|---------|
|**Microsoft 365**|Все отправляют электронную почту из общего почтового ящика в Exchange Online.|Например, когда все сообщения происходят из одного отдела, ваша торговая организация отправляет сообщения из учетной записи sales@cronus.com. Для этого необходимо настроить общий почтовый ящик в центре администрирования Microsoft 365. Дополнительные сведения см. в разделе [Общие почтовые ящики](/Exchange/collaboration/shared-mailboxes/shared-mailboxes).|
|**Текущий пользователь**|Все отправляют электронную почту из учетной записи, с которой они входили в [!INCLUDE[prod_short](includes/prod_short.md)].|Разрешает общение из индивидуальных учетных записей.|
|**Прочее (SMTP)**|Используется протокол SMTP для отправки сообщений электронной почты.|Разрешает связь через ваш почтовый сервер SMTP. |

> [!NOTE]
> В расширениях **Microsoft 365** и **Текущий пользователь** используются учетные записи, которые вы настроили для пользователей в центре администрирования Microsoft 365 для вашей подписки Microsoft 365. Чтобы отправлять электронную почту с помощью расширений, у пользователей должна быть действующая лицензия на Exchange Online. 
>
> Кроме того, внешние пользователи, такие как делегированные администраторы и внешние бухгалтеры, не могут использовать эти расширения для отправки сообщений электронной почты из [!INCLUDE[prod_short](includes/prod_short.md)].

> [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RE4JsUk]

## <a name="legacy-smtp-settings-and-the-email---smtp-connector-extension"></a>Устаревшие настройки SMTP и электронной почты — расширение соединителя SMTP
Если вы уже используете [!INCLUDE[prod_short](includes/prod_short.md)] и настроили электронную почту через устаревшую настройку SMTP, вы можете продолжить использовать свою настройку параллельно с расширением соединителя электронной почты SMTP. Когда мы обновим ваш [!INCLUDE[prod_short](includes/prod_short.md)] в следующей версии, мы скопируем ваши устаревшие настройки SMTP в расширение соединителя электронной почты SMTP. Когда все будет готово, ваш администратор может включить расширенные возможности электронной почты, и вы начнете использовать расширение соединителя электронной почты SMTP. Дополнительные сведения см. в разделе [Об управлении функциями](/dynamics365/business-central/dev-itpro/administration/feature-management#about-feature-management). Однако нет синхронизации между расширением соединителя SMTP и устаревшими настройками. Если вы измените настройки SMTP в расширении, вы должны внести те же изменения в устаревшую настройку SMTP, и наоборот.

> [!NOTE]
> Если у вас есть настройки, основанные на устаревшей настройке электронной почты SMTP, есть вероятность, что что-то пойдет не так с вашими настройками, если вы начнете использовать расширения электронной почты. Мы рекомендуем вам настроить и протестировать расширения, прежде чем включать переключатель функций для расширенных возможностей электронной почты.

> [!IMPORTANT]
> Если вы используете [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises, вы можете использовать OAuth 2.0 для аутентификации, но вы должны создать регистрацию приложения на портале Azure, затем запустить мастер настройки **Настройка Azure Active Directory** в [!INCLUDE[prod_short](includes/prod_short.md)], чтобы подключиться к Azure AD. Дополнительные сведения см. в разделе [Создание регистрации приложения для Business Central на портале Azure](admin-how-setup-email.md#create-an-app-registration-for-business-central-in-azure-portal).

## <a name="add-email-accounts"></a>Добавление учетных записей электронной почты
Мастер настройки **Настройка электронной почты** поможет вам быстро начать работу с электронной почтой.

> [!NOTE]
> У вас должна быть учетная запись электронной почты по умолчанию, даже если вы добавляете только одну учетную запись. Учетная запись по умолчанию будет использоваться для всех сценариев электронной почты, которые не назначены учетной записи. Для получения дополнительной информации см. раздел [Назначение сценариев электронной почты учетным записям электронной почты](admin-how-setup-email.md#assign-email-scenarios-to-email-accounts).

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Настройка учетных записей электронной почты**, а затем выберите связанную ссылку.
2. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] 


<!--
> [!NOTE]
> If you choose **Other (SMTP)** and are using an account that requires two-factor authentication, the password that you enter in the **Password** field must be the same that you use for your Microsoft 365 subscription, and it must be of type **App Password**. For more information, see [Manage app passwords for two-step verification](/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords). 

is this still true?-->
## <a name="assign-email-scenarios-to-email-accounts"></a>Назначение сценариев электронной почты учетной записям электронной почты
Сценарии электронной почты — это процессы, которые включают отправку документа, например заказа на продажу или покупку, или уведомления, например приглашения внешнему бухгалтеру. Вы можете использовать определенные учетные записи электронной почты для определенных сценариев. Например, вы можете указать, что все пользователи всегда отправляют документы на продажу из одной учетной записи, документы на покупку из другой учетной записи, а складские или производственные документы — из третьей учетной записи. Вы можете назначать, переназначать и удалять сценарии в любое время, но вы можете назначать сценарий только одной учетной записи электронной почты в каждый момент времени. Учетная запись электронной почты по умолчанию будет использоваться для всех сценариев, которые не назначены учетной записи.
 
<!--
## To set up email
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **SMTP Email Setup**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]
    > If you are using an account that requires two-factor authentication, then the password that you enter in the **Password** field must be the same that you use for your Microsoft 365 subscription and it must be of type **App Password**. For more information, see [Manage app passwords for two-step verification](/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).
3. Alternatively, choose the **Apply Microsoft 365 Server Settings** action to insert any information that is already defined for your Microsoft 365 subscription.
4. When all the fields are correctly filled in, choose the **Test Email Setup** action.
5. When the test succeeds, close the page.

-->

## <a name="set-up-reusable-email-texts-and-layouts-for-sales-and-purchase-documents"></a>Настройка многоразовых текстов и макетов электронной почты для документов продажи и закупок
Вы можете использовать отчеты для включения ключевой информации из документов продаж и закупок в тексты электронных писем. Эта процедура описывает, как настроить отчет **Счет продажи** по разнесенным счетам продаж, но процесс аналогичен для других отчетов.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Выбор отчета - продажи**, а затем выберите связанную ссылку.
2. На странице **Выбор отчета - продажи** в поле **Использование** выберите **Счет**.
3. В новой строке в поле **Код отчета** выберите, например, стандартный отчет 1306.
4. Установите флажок **Использовать для содержания сообщения электронной почты**.
5. Выберите поле **Описание макета содержания сообщения электронной почты**, а затем выберите макет из списка.

    Макеты отчетов определяют стиль и содержимое сообщений электронной почты, включая такие тексты, как приветствие или инструкции, которые предшествуют информации из документа. Если у организации много макетов, можно просмотреть все доступные макеты отчетов, если выбрать пункт **Выбор из полного списка**.
6. Чтобы просмотреть или изменить макет, на котором основан текст сообщения электронной почты, выберите макет на странице **Пользовательские макеты отчетов**, затем выберите действие **Обновить макет**.
7. Если вы хотите предложить клиентам оплатить покупку с помощью электронной службы платежей, вы можете настроить электронную службу платежей, например PayPal, и включить в текст сообщения электронной почты сведения и ссылку на PayPal. Дополнительные сведения см. в разделе [Включение платежей клиентов через PayPal](sales-how-enable-payment-service-extensions.md).
8. Нажмите кнопку **ОК**.

Теперь, когда вы выбираете, например, действие **Отправить** на странице **Учтенный счет продажи**, содержание сообщения электронной почты будет включать информацию из отчета 1306, перед которой будет расположен стандартный текст в соответствии с макетом отчета, выбранном на шаге 5.

## <a name="using-a-substitute-sender-address-on-outbound-email-messages"></a>Использование замещающего адреса отправителя в исходящих сообщениях электронной почты
Если вы используете устаревшие настройки SMTP, вы можете использовать возможности **Отправить как** или **Отправить от имени** из Microsoft Exchange для изменения адреса отправителя в исходящих сообщениях. [!INCLUDE[prod_short](includes/prod_short.md)] будет использовать учетную запись SMTP для аутентификации в Exchange, но либо заменит адрес отправителя на указанный вами, либо изменит его на "от имени".

Ниже приведены примеры того, как функции "Отправить как" и "От имени" используются в [!INCLUDE[prod_short](includes/prod_short.md)]:

 * Когда вы отправляете такие документы, как заказы на покупку или продажу, поставщикам и покупателям, вы можете захотеть, чтобы они поступали с адреса _noreply@yourcompanyname.com_.
 * Когда ваш рабочий процесс отправляет запрос на утверждение по электронной почте, используя адрес электронной почты запрашивающей стороны.

> [!Note]
> Вы можете использовать только одну учетную запись для замены адресов отправителей. То есть, вы не можете иметь один замещающий адрес для процессов покупки, а другой — для процессов продажи.

### <a name="to-set-up-the-substitute-sender-address-for-all-outbound-email-messages"></a>Настройка замещающего адреса отправителя для всех исходящих сообщений электронной почты
1. В разделе **Центр администрирования Exchange** для вашей учетной записи Microsoft 365 найдите почтовый ящик для использования в качестве замещающего адреса, затем скопируйте или запишите этот адрес. Если вам нужен новый адрес, перейдите в центр администрирования Microsoft 365, чтобы создать нового пользователя и настроить его почтовый ящик.
2. В [!INCLUDE[prod_short](includes/prod_short.md)] выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Настройка эл. почты (SMTP)**, а затем выберите связанную ссылку.
3. В поле **Отправить как** введите замещающий адрес.
4. Скопируйте или запишите адрес в поле **Идентификатор пользователя**.
5. В разделе **Центр администрирования Exchange** найдите почтовый ящик для использования в качестве замещающего адреса, затем введите адрес из поля **Идентификатор пользователя** в поле **Отправить как**. Для получения дополнительной информации прочитайте [Использование EAC для назначения разрешений отдельным почтовым ящикам](/Exchange/recipients/mailbox-permissions?view=exchserver-2019&preserve-view=true#use-the-eac-to-assign-permissions-to-individual-mailboxes).

### <a name="to-use-the-substitute-address-in-approval-workflows"></a>Использование замещающего адреса в рабочих процессах утверждения
1. В [!INCLUDE[prod_short](includes/prod_short.md)] выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Настройка эл. почты (SMTP)**, а затем выберите связанную ссылку.
2. Скопируйте или запишите адрес в поле **Идентификатор пользователя**.
3. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Настройка пользователя для утверждений**, а затем выберите связанную ссылку.
4. В разделе **Центр администрирования Exchange** найдите почтовые ящики для каждого пользователя, указанного на странице **Настройка пользователя для утверждений**, и в поле **Отправить как** введите адрес из поля **Идентификатор пользователя** на странице **Настройка эл. почты (SMTP)** в [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Управление разрешениями для получателей](/Exchange/recipients/mailbox-permissions?view=exchserver-2019&preserve-view=true).
5. В [!INCLUDE[prod_short](includes/prod_short.md)] выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Настройка эл. почты (SMTP)**, а затем выберите связанную ссылку.
6. Чтобы включить замену, включите переключатель **Разрешить замену отправителя**.

> [!Note]
> [!INCLUDE[prod_short](includes/prod_short.md)] определит, какой адрес отображать, в следующем порядке: <br><br> 1. Адрес, указанный в поле **Эл. почта** на странице **Настройка пользователя для утверждений** для сообщений в рабочем процессе. <br> 2. Адрес, указанный в поле **Отправить как** на странице **Настройка эл. почты (SMTP)**. <br> 3. Адрес, указанный в поле **Идентификатор пользователя** на странице **Настройка эл. почты (SMTP)**.

## <a name="set-up-document-sending-profiles"></a>Настройка профилей отправки документов
Вы можете настроить предпочтительный метод отправки документов по продажам для каждого из ваших клиентов, чтобы вам не приходилось выбирать вариант отправки, например, отправлять ли документ по электронной почте или в виде электронного документа, каждый раз, когда вы отправляете документ. Дополнительные сведения см. в разделе [Настройка профилей отправки документов](sales-how-setup-document-send-profiles.md).

## <a name="set-up-public-folders-and-rules-for-email-logging-in-exchange-online"></a>Настройка общих папок и правил для регистрации электронной почты в Exchange Online
Получите больше от общения между продавцами и вашими существующими или потенциальными клиентами, отслеживая обмен сообщениями электронной почты, затем превращая их в реальные возможности. Дополнительные сведения см. в [Отслеживание обмена сообщениями электронной почты между продавцами и контактами](marketing-set-up-email-logging.md).  

[!INCLUDE[admin-setup-email-public-folder](includes/admin-setup-email-public-folder.md)]

Далее вы подключаете [!INCLUDE[prod_short](includes/prod_short.md)] с Exchange Online. Дополнительные сведения см. в [Отслеживание обмена сообщениями электронной почты между продавцами и контактами](marketing-set-up-email-logging.md).  

## <a name="setting-up-email-for-business-central-on-premises"></a>Настройка электронной почты для Business Central On-Premises 
[!INCLUDE[prod_short](includes/prod_short.md)] On-Premises может интегрироваться со службами, основанными на Microsoft Azure. Например, вы можете использовать Cortana Intelligence для более точного прогноза денежных потоков, Power BI для визуализации вашего бизнеса и Exchange Online для отправки электронной почты. Интеграция с этими сервисами основана на регистрации приложения в Azure Active Directory. Регистрация приложения предоставляет услуги аутентификации и авторизации для связи. Чтобы использовать возможности электронной почты в [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises, вы должны зарегистрировать [!INCLUDE[prod_short](includes/prod_short.md)] как приложение на портале Azure, а затем подключить [!INCLUDE[prod_short](includes/prod_short.md)] к регистрации приложения. В следующих разделах описано, как это сделать.

### <a name="create-an-app-registration-for-business-central-in-azure-portal"></a>Создание регистрации приложения для Business Central на портале Azure
Шаги по регистрации [!INCLUDE[prod_short](includes/prod_short.md)] на портале Azure описаны в разделе [Регистрация приложения в Azure Active Directory](/dynamics365/business-central/dev-itpro/administration/register-app-azure#register-an-application-in-azure-active-directory). Параметры, относящиеся к возможностям электронной почты, представляют собой делегированные разрешения, которые вы предоставляете при регистрации приложения. В следующей таблице перечислены минимальные разрешения.

|API / Имя разрешения  |Тип  |Описание  |
|---------|---------|---------|
|Microsoft Graph / User.Read |Делегировано|Вход в систему и чтение профиля пользователя.         |
|Microsoft Graph / Mail.ReadWrite |Делегировано|Составление сообщений электронной почты.         |
|Microsoft Graph / Mail.Send|Делегировано|Отправка сообщений электронной почты.         |
|Microsoft Graph / offline_access|Делегировано|Сохранение согласия на доступ к данным.|

Если вы используете устаревшую настройку SMTP или соединитель SMTP и хотите использовать OAuth для проверки подлинности, разрешения немного отличаются. В следующей таблице перечислены разрешения.

|API / Имя разрешения  |Тип  |Описание  |
|---------|---------|---------|
|Microsoft Graph / offline_access|Делегировано|Сохранение согласия на доступ к данным.|
|Microsoft Graph / openid|Делегировано|Вход пользователей.|
|Microsoft Graph / User.Read |Делегировано|Вход в систему и чтение профиля пользователя.         |
|Microsoft Graph / SMTP.Send|Делегировано|Отправка сообщений электронной почты из почтовых ящиков с помощью SMTP AUTH.         |
|Office 365 Exchange Online / User.Read |Делегировано|Вход в систему и чтение профиля пользователя.         |

При создании регистрации приложения, обратите внимание на следующую информацию. Она понадобится вам для подключения [!INCLUDE[prod_short](includes/prod_short.md)] к регистрации вашего приложения.
 
* Код приложения (клиента) 
* URI перенаправления (необязательно)
* Секрет клиента

Общие инструкции для регистрации приложения см. в разделе [Быстрый старт: зарегистрируйте приложение на платформе идентификации Microsoft](/azure/active-directory/develop/quickstart-register-app). 

> [!NOTE]
Если у вас возникли проблемы с использованием устаревшей настройки SMTP для отправки сообщений электронной почты после подключения [!INCLUDE[prod_short](includes/prod_short.md)] к регистрации вашего приложения, это может быть связано с тем, что проверка подлинности SMTP AUTH не включена для вашего клиента. Мы рекомендуем вместо этого использовать соединители электронной почты Microsoft 365 и Текущий пользователь, поскольку они используют API-интерфейсы Microsoft Graph Mail. Однако, если вам необходимо использовать настройку SMTP, вы можете включить SMTP AUTH. Дополнительные сведения см. в разделе [Включение или отключение отправки для аутентифицированного клиента SMTP (SMTP AUTH) в Exchange Online](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#disable-smtp-auth-in-your-organization).

### <a name="connect-prod_short-to-your-app-registration"></a>Подключение приложения [!INCLUDE[prod_short](includes/prod_short.md)] к регистрации вашего приложения
После регистрации приложения на портале Azure в [!INCLUDE[prod_short](includes/prod_short.md)] используйте мастер настройки **Регистрация AAD приложения электронной почты** для подключения [!INCLUDE[prod_short](includes/prod_short.md)] к нему.

1. В [!INCLUDE[prod_short](includes/prod_short.md)] выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Регистрация AAD приложения электронной почты**, а затем выберите связанную ссылку.
2. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!TIP]
> Также, если вы подключаетесь впервые, вы можете запустить мастер настройки **Настройка электронной почты**. Руководство потребует информацию для подключения к регистрации вашего приложения. <!--Need to verify this too. Ask John to clear the aad settings, delete the email accounts, and then run the guide.-->

<!--

1. In [!INCLUDE[prod_short](includes/prod_short.md)], start the **Email Application AAD Registration** assisted setup guide.
2. On the first page of the guide, copy the value in the **Redirect URL** field.
3. In Azure Active Directory, search for **App registrations**, and then open the **App registrations** page.
4. Choose **New registration**.
5. In the **Name** field, enter a name for your app.
6. Under **Supported account types**, choose either the **Accounts in any organizational directory (Any Azure AD Directory - Multitenant)** or **Accounts in any organizational directory (Any Azure AD Directory - Multitenant) and personal Microsoft accounts (/e.g. Skype, Xbox)** options, depending on your needs. If you're unsure, choose **Help me choose** for more information.
7. Under **Redirect URI (optional)**, choose **Web**, paste the URL you copied from the **Redirect URL** field in the assisted setup guide in Business Central, and then choose **Register**.
8. On the navigation pane, choose **Overview**, and then copy the value in the **Application (client) ID** field.
9. In [!INCLUDE[prod_short](includes/prod_short.md)], in the assisted setup guide, paste the ID in **Client ID** field.
10. In Azure Active Directory, on the navigation pane, choose **API permissions**, and then choose **Add a permission**.
11. On the **Request API permissions** pane, on the **Microsoft APIs** tab, choose **Microsoft Graph**.  
12. Choose **Delegated permissions**, and then in the **Select permissions** field, search for **Mail.ReadWrite**, **Mail.Send**, and **offline_access**. Choose those permissions, and then choose **Add permissions**.
13. On the navigation pane, choose **Certificates & secrets**.
14. Under **Client secrets**, choose **New client secret**.
15. Under **Add a client secret**, enter a description of the client, specify how long you want your secret to be available, and then choose **Add**.
16. When the secret is generated, copy it. 
17. In [!INCLUDE[prod_short](includes/prod_short.md)], in the assisted setup guide paste the secret in the **Client Secret field**.
18. The **Verify Registration** button becomes available. 

-->

## <a name="see-related-training-at-microsoft-learn"></a>Прочтите соответствующее обучение на странице [Microsoft Learn](/learn/modules/set-up-email/)

## <a name="see-also"></a>См. также

[Общие почтовые ящики в Exchange Online](/exchange/collaboration-exo/shared-mailboxes)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Отправка документов по электронной почте](ui-how-send-documents-email.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)] с помощью расширений](ui-extensions.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] в качестве рабочего почтового ящика в Outlook](admin-outlook.md)  
[Получение [!INCLUDE[prod_short](includes/prod_short.md)] на мобильном устройстве](install-mobile-app.md)
[Получение [!INCLUDE[prod_short](includes/prod_short.md)] на мобильном устройстве](install-mobile-app.md)
[Анализ телеметрии электронной почты (содержимое для администраторов)](/dynamics365/business-central/dev-itpro/administration/telemetry-email-trace)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
