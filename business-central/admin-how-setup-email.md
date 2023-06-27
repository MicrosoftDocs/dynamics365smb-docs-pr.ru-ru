---
title: Настройка электронной почты в Business Central (содержит видео)
description: 'Описывается, как подключить учетные записи электронной почты к Business Central, чтобы вы могли отправлять исходящие сообщения, не открывая другое приложение.'
author: brentholtorf
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'SMTP, email, Office 365, connector'
ms.search.form: '1805, 9813, 9814, 1262, 1263'
ms.date: 11/22/2022
ms.author: bholtorf
---

# <a name="set-up-email"></a>Настройка электронной почты

Сотрудники предприятий ежедневно отправляют по электронной почте информацию и документы, такие как заказы на продажу и покупку и счета-фактуры. Администраторы могут подключить одну или несколько учетных записей электронной почты к [!INCLUDE[prod_short](includes/prod_short.md)], что позволяет отправлять документы, не открывая приложение электронной почты. Вы можете составлять каждое сообщение индивидуально с помощью основных инструментов форматирования, таких как шрифты, стили, цвета и т. д., и добавлять вложения размером до 100 МБ. Кроме того, макеты отчетов позволяют администраторам включать только ключевую информацию из документов. Подробнее см. в разделе [Отправка документов по электронной почте](ui-how-send-documents-email.md).

Возможности электронной почты в [!INCLUDE[prod_short](includes/prod_short.md)] предназначены только для исходящих сообщений. Вы не можете получать ответы, то есть нет страницы "Входящие".

> [!NOTE]
> Вы можете использовать возможности электронной почты [!INCLUDE[prod_short](includes/prod_short.md)] онлайн только с Exchange Online. Мы не поддерживаем гибридные сценарии, такие как подключение [!INCLUDE[prod_short](includes/prod_short.md)] онлайн к локальной версии Exchange.
>
> Если вы используете локальную версию [!INCLUDE[prod_short](includes/prod_short.md)], прежде чем вы сможете настроить электронную почту, вы должны создать регистрацию приложения для [!INCLUDE[prod_short](includes/prod_short.md)] на портале Azure. Регистрация приложения позволит [!INCLUDE[prod_short](includes/prod_short.md)] авторизовать и аутентифицировать вашего поставщика электронной почты. Дополнительные сведения см. в разделе [Настройка электронной почты для Business Central On-Premises](admin-how-setup-email.md#setting-up-email-for-business-central-on-premises). В [!INCLUDE[prod_short](includes/prod_short.md)] Online мы сделаем это за вас.

## <a name="requirements"></a>Требования

Существует несколько требований, которые должны быть выполнены для настройки и использования функций электронной почты.

* Чтобы настроить электронную почту, у вас должен быть набор разрешений **НАСТРОЙКА ЭЛ. ПОЧТЫ**. Дополнительные сведения см. в разделе [Назначение разрешений пользователям и группам](ui-define-granular-permissions.md).
* Каждый, кто будет использовать функции электронной почты, должен иметь полную лицензию на [!INCLUDE [prod_short](includes/prod_short.md)]. Например, делегированные администраторы и гостевые пользователи не могут использовать учетную запись электронной почты арендатора.

## <a name="adding-email-accounts"></a>Добавление учетных записей электронной почты

Вы добавляете учетные записи электронной почты через расширения, которые позволяют учетным записям разных поставщиков подключаться к [!INCLUDE[prod_short](includes/prod_short.md)]. Стандартные расширения позволяют использовать учетные записи из Microsoft Exchange Online. Однако могут быть доступны и другие расширения, позволяющие подключать учетные записи других поставщиков, например Gmail.

Вы можете указать предопределенные бизнес-сценарии, в которых будет использоваться учетная запись электронной почты для отправки сообщений электронной почты. Например, вы можете указать, что все пользователи отправляют документы по продаже из одной учетной записи, а документы на покупку — из другой. Подробнее см. в статье [Назначение сценариев электронной почты учетной записям электронной почты](admin-how-setup-email.md#assign-email-scenarios-to-email-accounts).

В следующей таблице описаны расширения электронной почты, доступные по умолчанию.

|Расширение  |Описание  |Примеры того, когда использовать  |
|---------|---------|---------|
|**Соединитель Microsoft 365**|Все отправляют электронную почту из общего почтового ящика в Exchange Online.|Например, когда все сообщения происходят из одного отдела, ваша торговая организация отправляет сообщения из учетной записи sales@cronus.com. Для этого параметра необходимо настроить общий почтовый ящик в центре администрирования Microsoft 365. Дополнительные сведения см. в разделе [Общие почтовые ящики](/Exchange/collaboration/shared-mailboxes/shared-mailboxes).|
|**Соединитель текущего пользователя**|Все отправляют электронную почту из учетной записи, с которой они входили в [!INCLUDE[prod_short](includes/prod_short.md)].|Разрешает общение из индивидуальных учетных записей.|
|**Соединитель SMTP**|Используется протокол SMTP для отправки сообщений электронной почты.|Разрешает связь через ваш почтовый сервер SMTP. |

> [!NOTE]
> В расширениях **Соединитель Microsoft 365** и **Соединитель текущего пользователя** используются учетные записи, которые вы настроили для пользователей в центре администрирования Microsoft 365 для вашей подписки Microsoft 365. Чтобы отправлять электронную почту с помощью расширений, у пользователей должна быть действующая лицензия на Exchange Online. Кроме того, в средах песочницы эти расширения требуют, чтобы параметр **Разрешить запросы HttpClient** был включен. Чтобы проверить, включен ли он для этих расширений, перейдите на страницу **Управление расширениями**, выберите расширение, а затем выберите параметр **Настроить**.

> Внешние пользователи, такие как делегированные администраторы и внешние бухгалтеры, не могут использовать эти расширения для отправки сообщений электронной почты из [!INCLUDE[prod_short](includes/prod_short.md)].

> [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RE4JsUk]

## <a name="using-smtp"></a>Использование SMTP

Если вы хотите использовать протокол SMTP для отправки сообщений электронной почты из [!INCLUDE[prod_short](includes/prod_short.md)], вы можете использовать расширение соединителя SMTP. При настройке учетной записи, использующей SMTP, важным полем является **Тип отправителя**. Если вы выберете **Конкретный пользователь**, сообщения электронной почты будут отправляться с использованием имени и другой информации из учетной записи, которую вы настраиваете. Однако, если вы выберете **Текущий пользователь**, сообщения электронной почты будут отправляться с учетной записи электронной почты, указанной для учетной записи каждого пользователя. Текущий пользователь похож на функцию «Отправить как». Дополнительные сведения см. в разделе [Использование замещающего адреса отправителя в исходящих сообщениях электронной почты](admin-how-setup-email.md#use-a-substitute-sender-address-on-outbound-email-messages). 

> [!IMPORTANT]
> Если вы используете локальную версию [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises, вы можете использовать для аутентификации протокол OAuth 2.0. Вы должны создать регистрацию приложения на портале Azure, а затем запустить мастер настройки **Настройка Azure Active Directory** в [!INCLUDE[prod_short](includes/prod_short.md)], чтобы подключиться к Azure AD. Дополнительные сведения см. в разделе [Создание регистрации приложения для Business Central на портале Azure](admin-how-setup-email.md#create-an-app-registration-for-business-central-in-azure-portal).
>
> В Exchange Online использовать обычную аутентификацию для SMTP больше не рекомендуется. Это изменение не затронет арендаторов, которые в настоящее время используют SMTP AUTH. Однако мы настоятельно рекомендуем использовать последнюю версию [!INCLUDE [prod_short](includes/prod_short.md)] и настроить аутентификацию OAuth 2.0 для SMTP. Мы не будем добавлять аутентификацию на основе сертификатов для более ранних версий [!INCLUDE [prod_short](includes/prod_short.md)], например версии 14. Если у вас нет возможности настроить аутентификацию OAuth 2.0, рекомендуем изучить сторонние альтернативы, если вы хотите использовать электронную почту SMTP в более ранних версиях.

[!INCLUDE [email-copy-company](includes/email-copy-company.md)]

## <a name="add-email-accounts"></a>Добавление учетных записей электронной почты

Мастер настройки **Настройка электронной почты** поможет вам быстро начать работу с электронной почтой.

> [!NOTE]
> У вас должна быть учетная запись электронной почты по умолчанию, даже если вы добавляете только одну учетную запись. Учетная запись по умолчанию будет использоваться для всех сценариев электронной почты, которые не назначены учетной записи. Подробнее см. в статье [Назначение сценариев электронной почты учетной записям электронной почты](admin-how-setup-email.md#assign-email-scenarios-to-email-accounts).

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок введите **Настройка учетных записей электронной почты**, а затем выберите связанную ссылку.
2. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] 


<!--
> [!NOTE]
> If you choose **Other (SMTP)** and are using an account that requires two-factor authentication, the password that you enter in the **Password** field must be the same that you use for your Microsoft 365 subscription, and it must be of type **App Password**. For more information, see [Manage app passwords for two-step verification](/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords). 

is this still true?-->
## <a name="assign-email-scenarios-to-email-accounts"></a>Назначение сценариев электронной почты учетной записям электронной почты

Сценарии электронной почты — это процессы, которые включают отправку документа. Например, заказ на продажу или покупку или уведомление, такое как приглашение внешнего бухгалтера. Определенные учетные записи электронной почты могут использоваться для определенных сценариев. Например, вы можете указать, что все пользователи всегда отправляют документы на продажу из одной учетной записи, документы на покупку из другой учетной записи, а складские или производственные документы — из третьей учетной записи. Вы можете назначать, переназначать и удалять сценарии в любое время. Сценарий может быть назначен только одной учетной записи электронной почты одновременно. Учетная запись электронной почты по умолчанию будет использоваться для всех сценариев, которые не назначены учетной записи.

На странице **Назначение сценариев электронной почты** можно выбрать действие **Задать вложения по умолчанию** для добавления вложений к сценариям электронной почты. Эти вложения будут доступны всегда, когда вы составляете сообщение электронной почты для документа, связанного со сценарием. Каждый сценарий электронной почты может иметь одно или несколько вложений по умолчанию. Вложения по умолчанию автоматически добавляются в сообщения для сценария электронной почты. Например, когда вы отправляете по электронной почте заказ на продажу, будет добавлено вложение по умолчанию, указанное для сценария "Заказ на продажу". Вложения по умолчанию отображаются в разделе **Вложения** в нижней части страницы **Напишите сообщение**. Вы можете вручную добавить в сообщение вложения, не предусмотренные по умолчанию.

<!--
## <a name="to-set-up-email"></a>To set up email
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **SMTP Email Setup**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]
    > If you are using an account that requires two-factor authentication, then the password that you enter in the **Password** field must be the same that you use for your Microsoft 365 subscription and it must be of type **App Password**. For more information, see [Manage app passwords for two-step verification](/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).
3. Alternatively, choose the **Apply Microsoft 365 Server Settings** action to insert any information that is already defined for your Microsoft 365 subscription.
4. When all the fields are correctly filled in, choose the **Test Email Setup** action.
5. When the test succeeds, close the page.

-->

## <a name="set-up-view-policies"></a>Настройка политик просмотра

Вы можете управлять сообщениями электронной почты, которые пользователь может видеть на страницах «Исходящие сообщения» и «Отправленные сообщения».

В **Политики просмотра электронной почты пользователя** выберите пользователя, а затем выберите один из следующих параметров в поле **Политика просмотра электронной почты**:

* **Просмотр собственных писем** - Пользователь может просматривать только свои собственные сообщения электронной почты.
* **Просмотреть все электронные письма** - Пользователь может просматривать все сообщения электронной почты, включая электронные письма, отправленные другими пользователями.
* **Просмотр при наличии доступа ко всем связанным записям** — эта политика просмотра используется, если не указана никакая другая политика. Пользователь может просматривать сообщения электронной почты, отправленные другими пользователями, если у него есть доступ к отправленной записи и всем связанным с ней записям. Например, пользователь А отправил покупателю опубликованный счет-фактуру. Пользователь B может видеть сообщение электронной почты, если у него есть доступ как к счету, так и к клиенту.
* **Просмотр, если доступ к любым связанным записям** - Пользователь может просматривать сообщения электронной почты, отправленные другими людьми, если у него есть доступ хотя бы к одной записи, связанной с отправленной записью. Например, пользователь А отправил покупателю опубликованный счет-фактуру. Пользователь B может видеть сообщение электронной почты, если у него есть доступ к счету или к клиенту.

> [!NOTE]
> Если вы оставите поле **ИД пользователя** пустым, а затем выберете действие **Политика просмотра электронной почты**, политика будет применяться ко всем пользователям.

## <a name="specify-how-many-messages-an-account-can-send-per-minute"></a>Задание максимального количества сообщений, которое учетная запись может отправлять в минуту

Некоторые поставщики услуг электронной почты (интернет-провайдеры) ограничивают количество сообщений электронной почты, которые учетная запись электронной почты может отправить за один раз или в течение определенного периода времени (или и то, и другое). Эта практика, известная как  *регулирование электронной почты*, помогает интернет-провайдерам контролировать трафик на своих серверах и предотвращать рассылку спама. Если учетная запись электронной почты превышает лимит, интернет-провайдер может заблокировать сообщения. Чтобы количество сообщений, отправляемых из [!INCLUDE [prod_short](includes/prod_short.md)], не превышало установленный вашим интернет-провайдером лимит, укажите лимит для каждой из своих учетных записей электронной почты.

По умолчанию лимит для учетных записей типа Microsoft 365 и «Текущий пользователь» составляет 30, что соответствует лимиту, установленному в Exchange Online.

Существует два способа задать лимит:

* При использовании мастера настройки «Настройка электронной почты» укажите лимит в поле **Лимит отправки сообщений в минуту**.
* Для существующих учетных записей электронной почты укажите лимит в поле **Лимит отправки электронной почты** в учетной записи.

## <a name="set-up-reusable-email-texts-and-layouts"></a>Настройка многократно используемых текстов и макетов сообщений электронной почты

Вы можете использовать отчеты для включения ключевой информации из документов продаж покупок и сервиса в тексты сообщений электронной почты. Макеты отчетов определяют стиль и содержание текста в электронном письме. Например, содержание может включать такие тексты, как приветствие или инструкции, которые предшествуют информации о документе. Эта процедура описывает, как настроить отчет **Счет продажи** по разнесенным счетам продаж, но процесс аналогичен для других отчетов.

> [!NOTE]
> Чтобы использовать макет для создания содержимого для сообщений электронной почты, вы должны использовать для макета тип файла Word.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") введите **Выбор отчета - продажи**, а затем выберите соответствующую ссылку.
2. На странице **Выбор отчета - продажи** в поле **Использование** выберите **Счет**.
3. В новой строке в поле **Код отчета** выберите, например, стандартный отчет 1306.
4. Установите флажок **Использовать для содержания сообщения электронной почты**.
5. Выберите поле **Описание макета содержания сообщения электронной почты**, а затем выберите макет из списка.
6. Чтобы просмотреть или изменить макет, на котором основан текст сообщения электронной почты, выберите макет на странице **Пользовательские макеты отчетов**, затем выберите действие **Обновить макет**. Если вы настраиваете макет, используйте действие **Импортировать макет** , чтобы отправить новый макет.
    > [!NOTE]
    > Чтобы настроить макет стандартного отчета, например 1306, необходимо сделать копию отчета. [!INCLUDE [prod_short](includes/prod_short.md)] поможет вам создать копию при импорте пользовательского макета для стандартного отчета. Имя вашего нового пользовательского макета отчета будет иметь префикс «Копия».
7. Если вы хотите, чтобы клиенты могли использовать платежную службу, например PayPal, вам необходимо настроить эту службу. После этого информация PayPal и ссылка вставляются в текст электронного письма. Дополнительные сведения см. в разделе [Включение платежей клиентов через PayPal](sales-how-enable-payment-service-extensions.md).
8. Нажмите кнопку **ОК**.

Теперь, когда вы выбираете, например, действие **Отправить** на странице **Учтенный счет продажи**, содержание сообщения электронной почты будет включать информацию из отчета 1306, перед которой будет расположен стандартный текст в соответствии с макетом отчета, выбранном на шаге 5.

## <a name="use-a-substitute-sender-address-on-outbound-email-messages"></a>Использование замещающего адреса отправителя в исходящих сообщениях электронной почты

Если вы используете расширение соединителя SMTP, вы можете использовать возможности **Отправить как** или **Отправить от имени** из Microsoft Exchange для изменения адреса отправителя в исходящих сообщениях. [!INCLUDE[prod_short](includes/prod_short.md)] будет использовать учетную запись SMTP для аутентификации в Exchange, но либо заменит адрес отправителя на указанный вами, либо добавит к нему "от имени".

Когда вы настраиваете учетную запись и хотите использовать возможности «Отправить как» или «Отправить от имени» из Exchange, в поле **Тип отправителя** выберите **Конкретный пользователь**.

Кроме того, вы можете выбрать **Текущий пользователь**, чтобы разрешить людям отправлять сообщения через соединитель SMTP. Сообщение будет выглядеть как отправленное с учетной записи электронной почты, указанной в поле «Контактный адрес электронной почты» в карточке пользователя для пользователя, под которым выполнен вход. Однако он будет работать аналогично функции «Отправить как» и будет отправлен с учетной записи, указанной в настройках соединителя SMTP.

Ниже приведены примеры того, как функции "Отправить как" и "От имени" используются в [!INCLUDE[prod_short](includes/prod_short.md)]:

* Возможно, вы хотите, чтобы заказы на покупку или продажу, отправляемые вами поставщикам и покупателям, поступали с адреса _noreply@yourcompanyname.com_.
* Когда ваш рабочий процесс отправляет запрос на утверждение по электронной почте, используя адрес электронной почты запрашивающей стороны.

> [!Note]
> Вы можете использовать только одну учетную запись для замены адресов отправителей. То есть, вы не можете иметь один замещающий адрес для процессов покупки, а другой — для процессов продажи.

<!--
### <a name="to-set-up-the-substitute-sender-address-for-all-outbound-email-messages"></a>To set up the substitute sender address for all outbound email messages
1. In the **Exchange admin center** for your Microsoft 365 account, find the mailbox to use as the substitute address, and then copy or make a note of the address. If you need a new address, go to your Microsoft 365 admin center to create a new user and set up their mailbox.
2. In [!INCLUDE[prod_short](includes/prod_short.md)] choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **SMTP Email Setup**, and then choose the related link.
3. In the **Send As** field, enter the substitute address.
4. Copy or make a note of the address in the **User ID** field.
5. In the **Exchange admin center**, find the mailbox to use as the substitute address, and then enter the address from the **User ID** field in the **Send As** field. For more information, see [Use the EAC to assign permissions to individual mailboxes](/Exchange/recipients/mailbox-permissions?view=exchserver-2019&preserve-view=true#use-the-eac-to-assign-permissions-to-individual-mailboxes).

### <a name="to-use-the-substitute-address-in-approval-workflows"></a>To use the substitute address in approval workflows
1. In [!INCLUDE[prod_short](includes/prod_short.md)] choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **SMTP Email Setup**, and then choose the related link.
2. Copy or make a note of the address in the **User ID** field.
3. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Approval User Setup**, and then choose the related link.
4. In the **Exchange admin center**, find the mailboxes for each user listed in the **Approval User Setup** page, and in the **Send As** field enter the address from the **User ID** field of the **SMTP Email Setup** page in [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Manage permissions for recipients](/Exchange/recipients/mailbox-permissions?view=exchserver-2019&preserve-view=true).
5. In [!INCLUDE[prod_short](includes/prod_short.md)] choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **SMTP Email Setup**, and then choose the related link.
6. To enable substitution, turn on the **Allow Sender Substitution** toggle.

> [!Note]
> [!INCLUDE[prod_short](includes/prod_short.md)] will determine which address to display in the following order: <br><br> 1. The address specified in the **E-Mail** field on the **Approval User Setup** page for messages in a workflow. <br> 2. The address specified in the **Send As** field in the **SMTP Email Setup** page. <br> 3. The address specified in the **User ID** field in the **SMTP Email Setup** page. -->

## <a name="set-up-document-sending-profiles"></a>Настройка профилей отправки документов

Вы можете сэкономить время, настроив предпочтительный способ отправки торговых документов для каждого из ваших клиентов. Вам не нужно будет выбирать вариант отправки, например, отправлять ли документ по электронной почте или в виде электронного документа, каждый раз, когда вы отправляете документ. Дополнительные сведения см. в разделе [Настройка профилей отправки документов](sales-how-setup-document-send-profiles.md).

## <a name="optional-set-up-email-logging-in-exchange-online"></a>(Необязательно) Настройка регистрации электронной почты в Exchange Online

Получите больше от общения между продавцами и вашими существующими или потенциальными клиентами. Вы можете отслеживать обмен сообщениями электронной почты, а затем превращать его в действенные возможности. Подробнее см. в статье [Отслеживание обмена сообщениями электронной почты между продавцами и контактами](marketing-set-up-email-logging.md).  
<!--
[!INCLUDE[admin-setup-email-public-folder](includes/admin-setup-email-public-folder.md)]

Next, you connect [!INCLUDE[prod_short](includes/prod_short.md)] with Exchange Online. For more information, see [Track Email Message Exchanges Between Salespeople and Contacts](marketing-set-up-email-logging.md).  -->

## <a name="setting-up-email-for-business-central-on-premises"></a>Настройка электронной почты для Business Central On-Premises

[!INCLUDE[prod_short](includes/prod_short.md)] On-Premises может интегрироваться со службами, основанными на Microsoft Azure. Например, вы можете использовать Cortana Intelligence для более точного прогноза денежных потоков, Power BI для визуализации вашего бизнеса и Exchange Online для отправки электронной почты. Интеграция с этими сервисами основана на регистрации приложения в Azure Active Directory. Регистрация приложения предоставляет услуги аутентификации и авторизации для связи. Чтобы использовать возможности электронной почты в [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises, вы должны зарегистрировать [!INCLUDE[prod_short](includes/prod_short.md)] как приложение на портале Azure, а затем подключить [!INCLUDE[prod_short](includes/prod_short.md)] к регистрации приложения. В следующих разделах описано, как это сделать.

### <a name="create-an-app-registration-for-business-central-in-azure-portal"></a>Создание регистрации приложения для Business Central на портале Azure

Шаги по регистрации [!INCLUDE[prod_short](includes/prod_short.md)] на портале Azure описаны в разделе [Регистрация приложения в Azure Active Directory](/dynamics365/business-central/dev-itpro/administration/register-app-azure#register-an-application-in-azure-active-directory).

> [!NOTE]
> Чтобы использовать функции электронной почты, при регистрации вашего приложения должна использоваться конфигурация с несколькими клиентами.

Параметры, относящиеся к возможностям электронной почты, представляют собой делегированные разрешения, которые вы предоставляете при регистрации приложения. В следующей таблице перечислены минимальные разрешения.

|API / Имя разрешения  |Тип  |Описание  |
|---------|---------|---------|
|Microsoft Graph / User.Read |Делегировано|Вход в систему и чтение профиля пользователя.         |
|Microsoft Graph / Mail.ReadWrite |Делегировано|Составление сообщений электронной почты.         |
|Microsoft Graph / Mail.Send|Делегировано|Отправка сообщений электронной почты.         |
|Microsoft Graph / offline_access|Делегировано|Сохранение согласия на доступ к данным.|

Если вы используете соединитель SMTP и хотите использовать OAuth 2.0 для проверки подлинности, разрешения немного отличаются. В следующей таблице перечислены разрешения.

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

Подробнее об общем порядке регистрации приложения см. в статье [Краткое руководство. Регистрация приложения с помощью платформы удостоверений Майкрософт](/azure/active-directory/develop/quickstart-register-app).

> [!NOTE]
Если у вас возникли проблемы с использованием протокола SMTP для отправки сообщений электронной почты после подключения [!INCLUDE[prod_short](includes/prod_short.md)] к регистрации вашего приложения, это может быть связано с тем, что проверка подлинности SMTP AUTH не включена для вашего клиента. Мы рекомендуем вместо этого использовать соединители электронной почты Microsoft 365 и Текущий пользователь, поскольку они используют API-интерфейсы Microsoft Graph Mail. Однако, если вам необходимо использовать протокол SMTP, вы можете включить SMTP AUTH. Дополнительные сведения см. в разделе [Включение или отключение отправки для аутентифицированного клиента SMTP (SMTP AUTH) в Exchange Online](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#disable-smtp-auth-in-your-organization).

### <a name="connect--to-your-app-registration"></a>Подключение [!INCLUDE[prod_short](includes/prod_short.md)] к регистрации приложения

После регистрации приложения на портале Azure в [!INCLUDE[prod_short](includes/prod_short.md)] используйте страницу **Регистрация AAD приложения электронной почты** для подключения [!INCLUDE[prod_short](includes/prod_short.md)] к нему.

1. В [!INCLUDE[prod_short](includes/prod_short.md)] выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Регистрация AAD приложения электронной почты**, а затем выберите связанную ссылку.
2. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!TIP]
> Также, если вы подключаетесь впервые, вы можете запустить мастер настройки **Настройка электронной почты**. В этом случае мастер также будет включать страницу "Регистрация AAD приложения электронной почты", позволяющую добавить информацию для подключения к регистрации вашего приложения. <!--Need to verify this too. Ask John to clear the aad settings, delete the email accounts, and then run the guide.-->

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

## <a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/set-up-email/)

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
