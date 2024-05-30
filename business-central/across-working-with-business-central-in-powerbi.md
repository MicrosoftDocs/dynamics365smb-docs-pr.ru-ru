---
title: Подключение к Power BI из локальной версии Business Central | Документация Майкрософт
description: 'Получение аналитических сведений, бизнес-аналитики и ключевых показателей эффективности из данных Business Central с помощью Power BI.'
author: jswymer
ms.topic: get-started
ms.devlang: al
ms.search.keywords: 'account schedule, analysis, reporting, financial report, business intelligence, KPI'
ms.date: 01/22/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
---
# <a name="connect-to-power-bi-from-business-central-on-premises"></a>Подключение к Power BI из локальной версии Business Central

<!--In this article, you learn some of the basics about working with reports and dashboards in Power BI that use [!INCLUDE [prod_short](includes/prod_short.md)] as a data source. The article discusses some aspects that will help you get started as a [!INCLUDE[prod_short](includes/prod_short.md)] user. For general guidelines and instructions about using Power BI, see [Power BI documentation for consumers](/power-bi/consumer).

## <a name="get-ready"></a>Get ready

Sign up for the Power BI service. If you haven't already signed up, go to [https://powerbi.microsoft.com](https://powerbi.microsoft.com). When you sign up, use a work email address and password.-->

## <a name="get-started"></a>Начало работы

При использовании локального экземпляра [!INCLUDE [prod_short](includes/prod_short.md)] в нем должна быть включена интеграция с Power BI. Эту задачу обычно выполняет администратор. Дополнительную информацию о включении интеграции с Power BIв Business Central Online см. в статье [Настройка локальной версии Business Central для интеграции с Power BI](admin-powerbi-setup.md).

Некоторые функции доступны только при использовании Business Central Online, но не при использовании локальной версии. Дополнительные сведения см. в статье [Общие сведения о Business Central и Power BI](admin-powerbi.md#what-you-can-do-with-power-bi-and-business-central)

## <a name="set-up--on-premises-for-power-bi-integration"></a><a name="setup"></a>Настройка [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises для интеграции с Power BI

В этом разделе объясняются требования к развертыванию [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises для интеграции с Power BI.

1. Настройте либо [NavUserPassword](/dynamics365/business-central/dev-itpro/administration/authenticating-users-with-navuserpassword), либо [Microsoft Entra ID](/dynamics365/business-central/dev-itpro/administration/authenticating-users-with-azure-ad-overview) в качестве метода проверки подлинности для развертывания.  
    
    > [!NOTE]
    > Интеграция с Power BI не поддерживает проверку подлинности Windows и не поддерживается в клиенте Windows.

2. Включите веб-службы OData и конечную точку ODataV4.

    Веб-служба OData должна быть включена на [!INCLUDE[server](includes/server.md)], и порт OData открыт в брандмауэре. Дополнительные сведения см. в разделе [Настройка Business Central Server — веб-службы OData](/dynamics365/business-central/dev-itpro/administration/configure-server-instance#ODataServices).

    Локальный сервер должен быть доступен из Интернета.

3. Дайте учетным записям пользователей [!INCLUDE[prod_short](includes/prod_short.md)] ключ доступа к веб-службам.

    Ключ доступа к веб-службе необходим только для просмотра данных [!INCLUDE[prod_short](includes/prod_short.md)] в Power BI. Вы можете назначить ключ доступа к веб-службе для каждой учетной записи пользователей. Или вместо этого создайте конкретную учетную запись с ключом доступа к веб-службе для использования всеми пользователями. Дополнительные сведения см. в разделе [Проверка подлинности для веб-служб](/dynamics365/business-central/dev-itpro/webservices/web-services-authentication#generate-a-web-service-access-key).

4. Создайте регистрацию приложения [!INCLUDE[prod_short](includes/prod_short.md)] в Microsoft Azure.

    Для просмотра отчетов Power BI, встроенных в страницы [!INCLUDE[prod_short](includes/prod_short.md)], необходимо зарегистрировать приложение для [!INCLUDE[prod_short](includes/prod_short.md)] в Microsoft Azure. Зарегистрированному приложению требуется разрешение на службы Power BI. Как минимум, приложение требует разрешения **User.ReadWrite.All**. Чтобы пользователи могли просматривать отчеты из общих рабочих областей Power BI, приложению требуется разрешение **Workspace.Read.All**. Дополнительные сведения см. в статье [Регистрация локального экземпляра [!INCLUDE[prod_short](includes/prod_short.md)] в Microsoft Entra для интеграции с другими службами](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

    > [!NOTE]
    > Если ваше развертывание использует аутентификацию NavUserPassword, [!INCLUDE[prod_short](includes/prod_short.md)] подключается к одной службе Power BI для всех пользователей. Вы укажете эту учетную запись службы при регистрации приложения. С аутентификацией Microsoft Entra [!INCLUDE[prod_short](includes/prod_short.md)] подключается к службе Power BI, связанно с отдельными учетными записями пользователей.

    <!-- Windows authentication can also be used but you can't get data from BC in Power BI -->
5. Выполните первоначальное подключение Business Central к Power BI.

    Прежде чем конечные пользователи смогут использовать Power BI в [!INCLUDE[prod_short](includes/prod_short.md)], администратор приложения Azure должен будет дать согласие на службу Power BI.

    Для первоначального подключения откройте [!INCLUDE[prod_short](includes/prod_short.md)] и выполните на главной странице процедуру **Начало работы с Power BI**. Это действие проведет вас через процесс получения согласия и проверит вашу лицензию Power BI. При появлении запроса войдите в систему, используя учетную запись администратора Microsoft Entra. Дополнительные сведения см. в разделе [Подключение к Power BI — только один раз](across-working-with-powerbi.md#connect).

## <a name="build-power-bi-reports-to-display--data"></a>Создание отчетов Power BI для отображения данных [!INCLUDE [prod_long](includes/prod_long.md)]

Можно сделать данные Dynamics 365 Business Central доступными в качестве источника данных в Power BI Desktop и создать мощные отчеты о состоянии вашего бизнеса.

Используйте Power BI Desktop для создания отчетов, в которых отображаются данные Dynamics 365 Business Central. После создания отчетов вы можете опубликовать их в своей службе Power BI или поделиться ими со всеми пользователями в вашей организации. Как только эти отчеты будут в службе Power BI, пользователи, которые настроены для нее, могут затем просматривать отчеты в Dynamics 365 Business Central.

- Для [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises получите следующую информацию:

  - URL-адрес OData для [!INCLUDE[prod_short](includes/prod_short.md)].
  
    Обычно этот URL-адрес имеет формат `http[s]://[computer]:[port]/[serverinstance]/ODataV4`, например `https://localhost:7048/BC190/ODataV4`. Если у вас есть развертывание в нескольких клиентах, включите клиент в URL-адрес, например `https://localhost:7048/BC190/ODataV4?tenant=tenant1`.
  - Имя пользователя и ключ доступа к веб-сервису учетной записи [!INCLUDE[prod_short](includes/prod_short.md)].

    Чтобы получить данные из [!INCLUDE[prod_short](includes/prod_short.md)], Power BI использует базовую аутентификацию. Итак, для подключения вам понадобятся имя пользователя и ключ доступа к веб-службе. Учетная запись может быть вашей собственной учетной записью пользователя, или ваша организация может иметь специальную учетную запись для этой цели.

## <a name="add--as-a-data-source-in-power-bi-desktop"></a><a name="getdata"></a>Добавление [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных в Power BI Desktop

Первая задача при создании отчетов — добавить [!INCLUDE[prod_short](includes/prod_short.md)] как источник данных в Power BI Desktop. После подключения вы можете приступить к созданию отчета.

1. Запустите Power BI Desktop.
2. Выберите **Получить данные**.

    Если вы не видите пункт **Получить данные**, выберите меню **Файл**, затем **Получить данные**.
3. На странице **Получить данные** выберите **Веб-службы**.
4. В области **Веб-службы** подключитесь к локальному экземпляру [!INCLUDE [prod_short](includes/prod_short.md)], выберите **Dynamics 365 Business Central (локальная версия)**, а затем **Подключиться**.
5. Войдите в [!INCLUDE [prod_short](includes/prod_short.md)] (только один раз).

    Если вы еще не вошли в [!INCLUDE [prod_short](includes/prod_short.md)] из Power BI Desktop, вам будет предложено войти в систему.

   - Для локальной версии [!INCLUDE [prod_short](includes/prod_short.md)] сначала введите URL-адрес OData для [!INCLUDE[prod_short](includes/prod_short.md)], затем выберите **ОК**. Когда будет предложено, введите имя пользователя и пароль учетной записи, которая будет использоваться для подключения к [!INCLUDE[prod_short](includes/prod_short.md)]. В поле **Пароль** введите ключ доступа к веб-службе. Когда готово, выберите **Подключить**.
   
    > [!NOTE]  
    > После успешного подключения к [!INCLUDE[prod_short](includes/prod_short.md)] выполнять повторный вход не требуется. [Как изменить или удалить учетную запись, которую я сейчас использую для подключения к Business Central из Power BI Desktop?](/dynamics365/business-central/power-bi-faq?tabs=designer#perms)

6. После подключения Power BI связывается со службой Business Central. Появляется окно **Навигатор**, в котором отображаются доступные источники данных для построения отчетов. Выберите папку, чтобы развернуть ее и просмотреть доступные источники данных. 

   Эти источники данных представляют все веб-службы и страницы API, которые опубликованы для [!INCLUDE [prod_short](includes/prod_short.md)]. Источники данных сгруппированы по средам Business Central и компаниям.

   > [!NOTE]
    > Структура локальной версии Business Central отличается, поскольку она не поддерживает страницы API.

7. Выберите источник данных или источники, которые требуется добавить в модель данных, а затем нажмите кнопку **Загрузить**.
8. Если позже вы захотите добавить дополнительные данные Business Central, вы можете повторить предыдущие шаги.

После загрузки данных они отображаются в правой области навигации на странице. На этом шаге вы успешно подключились с данным [!INCLUDE[prod_short](includes/prod_short.md)] и можете начать создание отчета Power BI.  

> [!TIP]
> Дополнительные сведения об использовании Power BI Desktop см. в разделе [Приступая к работе с Power BI Desktop](/power-bi/fundamentals/desktop-getting-started).

## <a name="manage-and-modify-reports"></a>Управление отчетами и их изменение

> [!NOTE]
> Управлять отчетами и вносить в них изменения невозможно. 

## <a name="upload-reports"></a>Отправка отчетов

Для локальной версии [!INCLUDE [prod_short](includes/prod_short.md)] демонстрационных отчетов не предусмотрено, поэтому вам придется начинать с нуля, используя Power BI Desktop. Другой вариант — распространять отчеты Power BI в виде файлов, отправляемых непосредственно из веб-службы Power BI. Дополнительные сведения см. в разделе [Отправка отчета в службу](/power-bi/paginated-reports/paginated-reports-quickstart-aw#upload-the-report-to-the-service).

<!--
> [!NOTE]
> Uploading a report requires that you have SUPER user permissions in [!INCLUDE[prod_short](includes/prod_short.md)]. Also, you can't upload reports with [!INCLUDE [prod_short](includes/prod_short.md)] on-premises. With on-premises, you upload reports directly to your Power BI workspace. For more information, see [Connect to Power BI from [!INCLUDE [prod_short](includes/prod_short.md)] on-premises](across-working-with-business-central-in-powerbi.md).

<!--Once you have a Power BI account, you can sign in at [https://powerbi.microsoft.com/](https://powerbi.microsoft.com/).

The Power BI service hosts all the reports available to you. To see the report, select **My Workspace** > **Reports**. Then just select the report that you want to view.

With [!INCLUDE[prod_short](includes/prod_short.md)] online, you'll automatically have a set of default reports on your workspace. If you want to create your own reports, you can use Power BI Desktop to create reports, and then publish them to your workspace. For more information, see [Getting Started Building Reports in Power BI Desktop to Display [!INCLUDE [prod_long](includes/prod_long.md)] Data](across-how-use-financials-data-source-powerbi.md).

[!INCLUDE[note-multicompany-reports](includes/note-multicompany-reports.md)]

If you're using [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, you'll have to start from scratch by using Power BI Desktop. Optionally, Power BI reports can be distributed as files, that you can upload.

<!--## Get the latest data

Each Power BI report is based on a dataset that gets data from the [!INCLUDE[prod_short](includes/prod_short.md)] sources. You want to make sure that the data in your Power BI reports is up to date with the data in [!INCLUDE[prod_short](includes/prod_short.md)]. This concept is referred to as *refreshing*.  Depending on how your organization has set up Power BI, refreshing might not happen automatically. There are two ways to refresh data: manually or by scheduling a refresh. Manual refreshing is done on-demand, as needed. Scheduled refreshing lets you refresh automatically at defined time intervals.

### <a name="refresh-manually"></a>Refresh manually

In the navigation pane, under **Datasets**, select **More options (...)** next to the dataset, then select **Refresh now**.

### <a name="schedule-a-refresh"></a>Schedule a refresh

In the navigation pane, under Datasets, select More options (...) next to the dataset, then select **Schedule refresh**. Fill in the information under the **Schedule refresh** section, and select **Apply**.

For more information, see [Configure scheduled refresh](/power-bi/connect-data/refresh-scheduled-refresh)-->

<!--## <a name="upload"></a>Upload reports from files

Power BI Reports can be distributed among users as .pbix files. If you have a .pbix file, you can upload the file to a workspace. To upload a report, do the following steps:

1. In your new workspace, select **Get Data**.

2. In the Files box, select **Get**.

3. Select **Local File**, navigate to where you saved the file, and select **Open**.

For more information, see [Upload the report to the service](/power-bi/paginated-reports/paginated-reports-quickstart-aw#upload-the-report-to-the-service).

> [!NOTE]
> Uploading a report requires that you have a [Premium capacity](/power-bi/service-premium-what-is) work space. For more information, see [Managing Premium capacities](/power-bi/admin/service-premium-capacity-manage). 

> [!TIP]
> If you're using [!INCLUDE[prod_short](includes/prod_short.md)] online, you can also upload a report from within [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Work with Power BI Reports in [!INCLUDE [prod_short](includes/prod_short.md)] - Upload Reports](across-working-with-powerbi.md#upload).

## <a name="share-reports-with-others"></a><a name="share"></a>Share reports with others

Once a report is in your workspace, you can share it with others in your organization.

To share a report, in a list reports, or in an open report, select **Share**. In the **Share report** pane, enter the full email addresses for individuals or distribution groups you want to share with. Follow the instructions on screen to complete the sharing. For more information, see [Share a dashboard or report](/power-bi/collaborate-share/service-share-dashboards#share-a-dashboard-or-report).

> [!NOTE]
> You must have  [Power BI Pro license](/power-bi/service-features-license-type), and the people you share with do too. The content must be in a workspace in a [Premium capacity](/power-bi/service-premium-what-is). For more information, see [Ways to share your work in Power BI](/power-bi/service-how-to-collaborate-distribute-dashboards-reports).-->

## <a name="see-also"></a>См. также

[Business Central и Power BI](admin-powerbi.md)  
[Отправка отчета из файлов](across-working-with-powerbi.md#upload-reports)  
 
[!INCLUDE[footer-include](includes/footer-banner.md)]
