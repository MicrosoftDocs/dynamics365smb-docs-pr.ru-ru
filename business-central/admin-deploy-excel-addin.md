---
title: Получение надстройки Business Central для Excel
description: 'Узнайте, как пользователи могут получить надстройку Business Central для Excel.'
author: jswymer
ms.topic: conceptual
ms.devlang: al
ms.search.form: 1480
ms.search.keywords: 'Excel, add-in, centralized deployment, M365 admin center, individual acquisition, appsource'
ms.date: 06/13/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---
# <a name="get-the-business-central-add-in-for-excel"></a>Получение надстройки Business Central для Excel

[!INCLUDE[prod_short](includes/prod_short.md)] включает надстройку для Excel, которая позволяет пользователям выбирать действие **Изменить в Excel** на определенных страницах, чтобы открыть данные на листе Excel. Это действие отличается от действия **Открыть в Excel**, потому что оно позволяет пользователям вносить изменения в Excel, а затем публиковать изменения обратно в [!INCLUDE[prod_short](includes/prod_short.md)]

## <a name="overview"></a>Обзор

### <a name="about-the-add-in"></a>О надстройке

Надстройка называется **Надстройка Office Microsoft Dynamics** и ее можно установить из [Магазина Office (AppSource)](https://appsource.microsoft.com/). После установки надстройки действие **Изменить в Excel** доступно на большинстве страниц списков и частей списков по значку **Поделиться** ![Поделиться страницей в другом приложении.](media/share-icon.png). Дополнительную информацию по использованию надстройки см. в разделе [Просмотр и редактирование в Excel из Business Central](across-work-with-excel.md).

> [!NOTE]
> Надстройка работает только в Windows, но не в macOS.

### <a name="about-deployment-as-an-admin"></a>О развертывании в качестве администратора

С [!INCLUDE[prod_short](includes/prod_short.md)] Online есть несколько вариантов развертывания для предоставления надстройки пользователям. Один из вариантов — *индивидуальное получение*, когда вы разрешаете пользователям устанавливать надстройку самостоятельно. При использовании этого параметра у пользователей должен быть доступ к загрузке файлов из Магазина Office. Другой вариант — настроить *Централизованное развертывание* в центре администрирования Microsoft 365 для автоматического развертывания надстройки для всей организации, групп или конкретных пользователей. Централизованное развертывание позволяет предоставить надстройку пользователям, если ваша организация не предоставляет пользователям доступ к Магазину Office.

Для конечного пользователя процесс установки отличается для двух сценариев развертывания:

- При индивидуальном получении пользователи сначала выбирают действие **Изменить в Excel**, затем панель **Создать надстройку Office** открывается в Excel. Чтобы установить надстройку, пользователь выбирает **Доверять этой надстройке**, что установит надстройку прямо из магазина Office. Затем пользователи входят в [!INCLUDE[prod_short](includes/prod_short.md)], используя свое имя пользователя и пароль.

- При централизованном развертывании пользователи сначала выбирают действие **Изменить в Excel**, надстройка автоматически устанавливается в Excel из централизованного развертывания; а не магазина Office. Единственное, что нужно сделать пользователям, это войти в [!INCLUDE[prod_short](includes/prod_short.md)]

При использовании обоих этих вариантов развертывания надстройка автоматически настраивается для подключения к [!INCLUDE[prod_short](includes/prod_short.md)]. Третий вариант развертывания — это установка надстройки вручную непосредственно из Excel. С помощью этого варианта пользователям нужно будет настроить надстройку для подключения к [!INCLUDE[prod_short](includes/prod_short.md)]

### <a name="switching-from-individual-acquisition-to-centralized-deployment-or-the-other-way-around"></a><a name="switch"></a>Переход от индивидуального получения к централизованному развертыванию или наоборот

Когда вы переходите с индивидуального получения надстройки на централизованное развертывание или наоборот, это влияет на файлы Excel, созданные пользователями до перехода. После перехода пользователи по-прежнему могут открывать любые листы Excel, ранее созданные с помощью действия **Изменить в Excel** или созданные вручную путем настройки надстройки Excel. Но они не могут обновить данные в файле из Business Central или отправить обновления в Business Central.

Это условие вызвано тем, что каждому файлу Excel присваивается идентификатор «надстройки». При переходе к централизованному развертыванию или из него назначается другой идентификатор, поэтому более ранний идентификатор становится заблокированным.

## <a name="preparation-on-premises-only"></a>Подготовка (только локальная версия)

Локальная версия [!INCLUDE[prod_short](includes/prod_short.md)] требует, чтобы ваша среда была настроена для надстройки. В противном случае действие **Изменить в Excel** будет недоступно пользователям. Для получения дополнительной информации см. [Настройка надстройки Excel для редактирования данных Business Central](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin) в справке для разработчиков и ИТ-специалистов.

## <a name="deploy-the-add-in-by-using-centralized-deployment"></a>Разверните надстройку с помощью централизованного развертывания

Централизованное развертывание — это функция центра администрирования Microsoft 365, которую вы используете для автоматической установки надстроек в пользовательских приложениях Office, таких как Excel. Чтобы помочь вам с централизованным развертыванием, [!INCLUDE[prod_short](includes/prod_short.md)] содержит мастера **Централизованное развертывание надстроек Excel**.

### <a name="before-you-begin"></a>Подготовка к работе

- Чтобы узнать, как запретить пользователям скачивать файлы из магазина Office, см. [Управление надстройками в центре администрирования](/microsoft-365/admin/manage/manage-addins-in-the-admin-center).
- Убедитесь, что централизованное развертывание подойдет для вашей организации. Для получения дополнительной информации см. [Определение пригодности централизованного развертывания надстроек для вашей организации](/microsoft-365/admin/manage/centralized-deployment-of-add-ins)
- Если вы переходите от индивидуального получения, см. [Переход от индивидуального получения к централизованному развертыванию](#switch)

> [!NOTE]
> Включение централизованного развертывания влияет на функции, использующие надстройку Excel, такие как действие **Изменить в Excel**. Это не влияет на другие связанные с Excel функции и/или разрешения, назначенные пользователям в [!INCLUDE[prod_short](includes/prod_short.md)]

### <a name="set-up-centralized-deployment-of-the-add-in"></a>Настроить централизованное развертывание надстройки

Вы будете работать в [!INCLUDE[prod_short](includes/prod_short.md)] и в центре администрирования Microsoft 365.

1. В [!INCLUDE[prod_short](includes/prod_short.md)] выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") введите **Централизованное развертывание надстроек Excel**, затем выберите связанную ссылку.
2. Прочтите информацию на странице **Настройка надстройки Excel для Business Central** и выберите **Далее**.
3. Войдите в [центр администрирования Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2163967) и перейдите в **Интегрированные приложения**.<!--**Add-ins**-->.

    Выполните следующие шаги, чтобы настроить надстройку для развертывания из Магазина Office: 
    1. Выберите **Получить приложения**, чтобы открыть Магазин Office (AppSource). <!--**Deploy Add-in** 5. In the **Deploy a new add-in**, select **Choose from the store**.-->
    2. Найдите **Надстройка Microsoft Dynamics Office**, затем выберите **Получить сейчас**. <!--On the **Select add-in** page, search for and select **Microsoft Dynamics Office Add-in** > **Add** > **Continue**.-->
    3. На странице **Добавить пользователей** укажите пользователей, для которых вы хотите развернуть надстройку, затем выберите **Далее**.<!--On the **Configure add-in**, specify the users that you want to deploy the add-in for.-->
    4. Проверьте **Принимать запросы разрешений**, затем выберите **Далее** > **Завершить развертывание**.
    5. Подождите, пока появится зеленая галочка рядом с **Развернуто** для надстройки, затем выберите **Готово**. <!--Select **Deploy** and wait til successful, then **Next** > **Continue**.-->

       Надстройка появится на странице **Надстройки**. Дополнительные сведения о развертывании надстроек в центре администрирования Microsoft 365 см. в разделе [Развертывание надстроек в центре администрирования](/power-platform/admin/use-service-admin-role-manage-tenant?azure-portal=true).
4. Вернитесь к мастеру настройки **Централизованное развертывание надстройки Excel** в [!INCLUDE[prod_short](includes/prod_short.md)] и выберите **Далее**.
5. Включите **Использовать централизованное развертывание**, и выберите **Готово**.

    Если вы не включите этот переключатель, [!INCLUDE[prod_short](includes/prod_short.md)] получит надстройку прямо из Магазина Office.

По завершении вы всегда можете изменить развертывание в центре администрирования Microsoft 365, например назначить больше пользователей. Дополнительные сведения о развертывании надстроек в центре администрирования см. в разделе [Развертывание надстроек в центре администрирования](/power-platform/admin/use-service-admin-role-manage-tenant?azure-portal=true).

> [!IMPORTANT]
> Если у вас более одной среды, вы должны запустить мастер настройки **Централизованное развертывание надстройки Excel** в каждой среде, в которой вы хотите использовать централизованное развертывание. Однако вам не нужно снова настраивать централизованное развертывание в Microsoft 365. Единственное, что вам нужно сделать, это включить переключатель **Использовать централизованное развертывание** в мастере настройки. 

> [!NOTE]
> Может пройти до 24 часов, прежде чем надстройка будет автоматически развернута пользователями в Excel.

## <a name="individual-acquisition-install-the-add-in-manually-for-your-own-use"></a><a name="install"></a>Индивидуальное получение. Установка надстройки вручную для собственного использования

В большинстве случаев, когда вы открываете Excel из Business Central, надстройка либо устанавливается автоматически, либо вам будет предложено установить ее. Однако могут быть случаи, когда вам придется вручную установить надстройку.

1. Откройте Excel, затем откройте любую книгу Excel.
1. На вкладке **Главная** выберите **Надстройки** > **Другие надстройки**.
1. Перейдите **Управляется администратором** и найдите **Надстройка Microsoft Dynamics Office**. Если она там есть, выберите ее, затем выберите **Добавить**. Если ее там нет, перейдите в **Магазин**, затем найдите *Надстройка Microsoft Dynamics Office* и следуйте инструкциям на экране, чтобы добавить ее.

Когда надстройка установлена, она отображается в Excel в виде панели. Далее настройте подключение.

### <a name="configure-the-business-central-connection"></a>Настроить соединение с Business Central

Если пользователь не может подключиться автоматически, вы можете разблокировать его, попросив его выполнить следующие действия:

1. В области надстройки **Microsoft Dynamics** в Excel выберите **Добавить информацию о сервере**. Если этого нет, выберите ![Кнопка дополнительных параметров в Excel.](media/cogwheel.png) вверху, чтобы открыть диалоговое окно параметров. 
2. Для [!INCLUDE[prod_short](includes/prod_short.md)] Online установите **URL-адрес сервера** как `https://exceladdinprovider.smb.dynamics.com`. Для локальной версии [!INCLUDE[prod_short](includes/prod_short.md)] установите для него URL-адрес веб-клиента, например `https://myBCserver/240`.
3. Выберите **ОК**, а затем убедитесь, что приложение перезагружается.
4. При появлении подсказки войдите в Business Central со своими именем пользователя и паролем.
5. Необязательно: выберите среду и организацию, к которым вы хотите подключиться.

Надстройка теперь подключена к [!INCLUDE [prod_short](includes/prod_short.md)], и вы можете редактировать данные и публиковать изменения в [!INCLUDE [prod_short](includes/prod_short.md)].  

## <a name="prepare-devices-and-network-for-the-excel-add-in"></a>Подготовьте устройства и сеть для надстройки Excel

Сетевые службы, такие как прокси или брандмауэры, должны разрешать маршрутизацию между каждым клиентским устройством, на котором установлена надстройка, и многими конечными точками служб. Список конечных точек см. в [Подготовка сети к надстройке Excel](/dynamics365/business-central/dev-itpro/administration/configuring-network-for-addins).

## <a name="troubleshooting"></a>Устранение неполадок

Иногда у пользователей возникают проблемы с надстройкой Excel. В этом разделе дается несколько советов, как разблокировать пользователей в определенных обстоятельствах.

|Проблема  |Решение или обходной путь  |Комментарии  |
|---------|---------|---------|
|Надстройка не запускается <br><br>Например, пользователь получает сообщение «Предупреждение надстройки: эта надстройка больше недоступна». при попытке использовать надстройку. Эта конкретная проблема может возникнуть, если централизованное развертывание настроено правильно, но пользователю не назначен доступ.|Убедитесь, что надстройка развернута централизованно. Или проверьте, не заблокирована ли пользователю возможность ее локальной установки. | Администратор может настроить Office так, чтобы пользователи не могли получать надстройки. В таких случаях администратор должен развернуть надстройку централизованно. Для получения дополнительной информации см. [Развертывание надстроек в центре администрирования](/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide&preserve-view=true).|
|Данные не загружаются в Excel|Проверьте соединение, открыв другой список в Excel из [!INCLUDE [prod_short](includes/prod_short.md)]. Или откройте книгу в Excel в браузере.|Если пользователь указал название компании, содержащее специальные символы, надстройка не сможет подключиться. |
|Данные не могут быть опубликованы обратно в [!INCLUDE [prod_short](includes/prod_short.md)].|Проверьте соединение, открыв книгу в Excel в браузере. |Иногда расширение может блокировать публикацию. Если страница развернута или настроена, удалите расширения и повторите попытку.|
|Даты неправильные  |Excel может отображать время и даты в формате, отличном от [!INCLUDE [prod_short](includes/prod_short.md)]. Это условие не делает их неправильными, и данные в [!INCLUDE [prod_short](includes/prod_short.md)] не будут перепутаны.|         |
|Для некоторых страниц списков редактирование нескольких строк в Excel постоянно вызывает ошибки. Это состояние может возникнуть, если вызовы OData включают FlowFields и поля вне элемента управления повторителя.|На странице **Веб-службы** установите флажки **Исключить нередактируемые поля FlowFields** и **Исключить поля за пределами повторителя** для опубликованной страницы. Установка этих флажков исключает нередактируемые поля FlowFields и поля из расчета eTag. |Эти флажки по умолчанию скрыты. Чтобы показать их на странице **Веб-службы**, используйте [персонализацию](/dynamics365/business-central/ui-personalization-user). |
|Пользователи больше не могут войти в надстройку. Когда они пытаются войти, процесс останавливается без завершения.| Эта проблема может быть вызвана обновлением, которое мы внесли в надстройку где-то в июле 2022 года. Дополнительную информацию и сведения об исправлении см. в разделе [Изменение конфигурации надстройки Excel для поддержки обновления за июль 2022 г.](/dynamics365/business-central/dev-itpro/administration/update-excel-addin-configuration).|Применимо только в локальной версии [!INCLUDE [prod_short](includes/prod_short.md)] On-Premises|
| Надстройка осуществляет взаимодействие с помощью API версии 2.0 для Dynamics 365 Business Central, и все ограничения этого API наследуются автоматически. Примером такого ограничения является ситуация, когда вы пытаетесь отредактировать список, а в логике AL лежащей в его основе карточки используется диалоговое окно подтверждения — например, в качестве логики проверки. | Иногда ничего делать не нужно, потому что необходимость явного подтверждения изменения пользователем является элементом функциональности. Если подтверждением при использовании функции **Редактировать в Excel** можно пренебречь, вы можете обернуть вызов диалогового окна подтверждения в условный оператор, который проверяет, отличается ли тип клиента от ODataV4, например: `if SESSION.CurrentClientType() <> ClientType::ODataV4 then`. | Возможно, существуют другие клиенты, из которых вы хотите удалить диалоговое окно подтверждения, такие как OData и SOAP. |

## <a name="known-limitations-in-business-logic"></a>Известные ограничения в бизнес-логике

|Стр.  |Ограничение| Комментарии  |
|-------|---------|---------|
|Заказы на продажу|Сообщение об ошибке: «Службы Microsoft Dynamics 365 Business Central Data Services попытались выполнить обратный вызов клиента для запуска страницы 301 «Список адресов доставки» как модальной». Клиентские обратные вызовы не поддерживаются в Microsoft Dynamics 365 Business Central Data Services. |  **Код получателя** на странице **Заказ на продажу** можно редактировать только с определенными параметрами получателя. При установке **альтернативного адреса доставки** назначения **адрес доставки** открывается модальное диалоговое окно **Список адресов доставки**, которое несовместимо с функцией редактирования в Excel.|  
|Журнал проектов|Обновление поля **Цена единицы** не приводит к обновлению поля **Сумма строки**. Вместо этого он обновляет **скидку по строке**.| Используя веб-клиент, вы можете обновлять поля в любом заказе:&; цена, сумма, скидка по строке. Остальные поля обновляются автоматически. Чтобы избежать каскадных обновлений, поля имеют расширенную логику, основанную на xRec, которая ведет себя по-другому при вызове через API.|



<!--
## <a name="deploy-the-excel-add-in-for-business-central-online"></a>Deploy the Excel add-in for Business Central online

For [!INCLUDE [prod_short](includes/prod_short.md)] online, the administrator can deploy the add-in for all users. But users can also install the add-in themselves, provided they have permission to configure their Office experience.  

> [!TIP]
> In some organizations, administrators cannot deploy add-ins centrally. For more information, see [Determine if Centralized Deployment of add-ins works for your organization](/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide&preserve-view=true).

### <a name="to-deploy-the-excel-add-in-for-all-users"></a>To deploy the Excel add-in for all users

1. As the administrator, sign in to the Microsoft commercial website and find the add-in at [https://appsource.microsoft.com/product/office/WA104379629](https://appsource.microsoft.com/product/office/WA104379629).
2. Choose the **Get it now** button.

    You'll be redirected to the Microsoft 365 admin center.
3. In the left panel, go to **Settings**, and then choose **Add-ins**.
4. In the **Configure add-in** pane, specify which users to grant access to the add-in.
5. Save your changes.


### <a name="to-add-the-excel-add-in-locally"></a>To add the Excel add-in locally

1. Open Excel, and then open any Excel workbook.
2. On the **Insert** menu, choose **Office Add-ins**, and then choose **Admin managed** or **Store** as appropriate.
3. Search for *Dynamics Office Add-In*, and then install the add-in.

When the add-in is installed, it shows up as a panel in Excel. Next, you must configure the connection.

> [!TIP]
> If the workbook is not automatically saved to the user's OneDrive, then recommend them to save all workbooks that they export from [!INCLUDE [prod_short](includes/prod_short.md)].When they open the workbook again, the connection is still available, so they do not have to configure the connection again.

> [!NOTE]
> In certain deployments, the administrator must configure network access to unblock the Excel add-in. For more information, see [Preparing Your Network for the Excel Add-In](configuring-network-for-addins.md).-->

## <a name="see-also"></a>См. также

[Анализ финансовых отчетов в Microsoft Excel](finance-analyze-excel.md)  
[Работа с Business Central](ui-work-product.md)  
[Улучшения интеграции с Excel в волне 2 выпуска 2019 года](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
