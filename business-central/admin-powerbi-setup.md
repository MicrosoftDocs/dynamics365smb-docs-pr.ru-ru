---
title: Включение интеграции Power BI с Business Central
description: 'Узнайте, как настроить подключение к Power BI. С отчетами Power BI можно получить аналитические сведения, бизнес-аналитику и ключевые показатели эффективности из данных Business Central.'
author: jswymer
ms.topic: get-started
ms.search.keywords: 'Power BI, setup, analysis, reporting, financial report, business intelligence, KPI'
ms.date: 01/28/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# Включение интеграции Power BI с [!INCLUDE[prod_short](includes/prod_short.md)]

[!INCLUDE[azure-ad-to-microsoft-entra-id](~/../shared-content/shared/azure-ad-to-microsoft-entra-id.md)]

В этой статье описывается, как подготовить [!INCLUDE[prod_short](includes/prod_short.md)] к интеграции с Power BI. [!INCLUDE[prod_short](includes/prod_short.md)] Online уже включен для интеграции, хотя есть некоторая информация о лицензировании, которую вы, возможно, захотите прочитать. Для [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises вам требуется настроить свою среду для подключения к Power BI, прежде чем пользователи смогут с ним работать.

## <a name="license"></a>Лицензирование Power BI

С [!INCLUDE[prod_short](includes/prod_short.md)] пользователи получают бесплатную лицензию Power BI, которая обеспечивает доступ к наиболее распространенным функциям в [!INCLUDE[prod_short](includes/prod_short.md)] и Power BI. Вы также можете приобрести лицензию Power BI Pro, предоставляющую доступ к дополнительным функциям. В следующей таблице представлен обзор функций, доступных для каждой лицензии.

|Лицензия Power|Просмотр отчетов|Создание отчетов|Предоставление доступа к отчетам|Обновление отчетов| Приложения [!INCLUDE[prod_short](includes/prod_short.md)]|
|-------------|--------||
|Бесплатная Power BI|![флажок.](media/check.png)|![еще один флажок](media/check.png)|(ограничено)|(ограничено)||
|Power BI Pro|![и еще один флажок.](media/check.png)|![это флажок](media/check.png)|![снова флажок](media/check.png)|(обширная)|![последний флажок](media/check.png)|

Дополнительные сведения см. в разделе [Лицензирование службы Power BI для пользователей в вашей организации](/power-bi/admin/service-admin-licensing-organization) или [Регистрация на службу Power BI как физическое лицо](/power-bi/fundamentals/service-self-service-signup-for-power-bi).

## <a name="exposedata"></a>Предоставлять данные через API или веб-службы OData

Business Central предлагает два способа предоставления данных, которые могут быть использованы отчетами Power BI: страницы или запросы API и веб-службы Open Data Protocol (OData).

### Страницы и запросы API

> **ПРИМЕНЯЕТСЯ К:** только Business Central Online

Разработчики могут определять объекты страницы и объекты запросов типа *API*. Таким образом они могут предоставлять данные из таблиц баз данных через службу REST с поддержкой веб-перехватчиков и OData v4. Данные этого типа не могут отображаться в пользовательском интерфейсе, а предназначены для создания надежных служб интеграции.

Business Central Online поставляется с набором встроенных API-интерфейсов, которые можно использовать для получения данных о наиболее распространенных бизнес-объектах, таких как клиенты, товары, заказы на продажу и т. д. Для использования этих API в качестве источника данных для отчетов Power BI не требуются дополнительные усилия и настройка. Для получения дополнительной информации об этих API прочитайте [Business Central API V2.0](/dynamics365/business-central/dev-itpro/api-reference/v2.0/).

Business Central Online также поддерживает настраиваемые API. Разработчики приложений для решений Business Central могут создавать свои собственные страницы и запросы API и упаковывать их в приложения. Затем устанавливаются приложения на своем клиенте. После установки используются страницы API для своих отчетов Power BI, как встроенные API (v2.0). Для получения дополнительной информации о том, как создавать API для предоставления доступа к страницам и запросам, прочитайте [Разработка собственного API](/dynamics365/business-central/dev-itpro/developer/devenv-develop-custom-api).

> [!IMPORTANT]
> С февраля 2022 г. отчеты Power BI для [!INCLUDE[prod_short](includes/prod_short.md)] Online извлекаются из вторичной реплики базы данных, доступной только для чтения по соображением производительности. Как следствие, разработчикам AL следует избегать проектирования страниц API, которые вносят изменения в базу данных, когда страницы открывают или загружают записи. В частности, рассмотрим код триггеров AL: OnInit, OnOpenPage, OnFindRecord, OnNextRecord, OnAfterGetRecord и OnAfterGetCurrRecord. Эти модификации базы данных в некоторых случаях могут вызвать проблемы с производительностью и помешать обновлению данных в отчете. Для получения дополнительной информации см. [Статьи о производительности для разработчиков](/dynamics365/business-central/dev-itpro/performance/performance-developer?branch=main#writing-efficient-web-services) в материалах по разработке Business Central.
>
> В редких случаях поведение вызывает ошибку, когда пользователь пытается получить данные из API для отчета в Power BI Desktop. Однако если для пользовательского API необходимы модификации базы данных, пользователи Power BI Desktop могут форсировать такое поведение. Дополнительные сведения см. в разделе [Создание отчетов Power BI для отображения данных Business Central](across-how-use-financials-data-source-powerbi.md#fixing-problems).

### Веб-службы OData

Вы можете публиковать объекты приложения Business Central, такие как модули кода, страницы и запросы, как [Веб-службы OData](/dynamics365/business-central/dev-itpro/webservices/odata-web-services). В Business Central Online по умолчанию публикуется множество веб-служб. Простой способ найти веб-службы — найти *веб-службы* в [!INCLUDE[prod_short](includes/prod_short.md)]. На странице **Веб-службы** убедитесь, что поле **Опубликовать** выбрано для веб-служб, перечисленных выше. Дополнительные сведения о публикации веб-служб см. в разделе [Публикация веб-службы](across-how-publish-web-service.md).

Чтобы узнать, что вы можете сделать для обеспечения максимальной производительности веб-служб с точки зрения сервера Business Central Server (конечная точка) и потребителя (клиент), ознакомьтесь с разделом [Создание эффективных веб-служб](/dynamics365/business-central/dev-itpro/performance/performance-developer#writing-efficient-web-services).

### Выбор использования страниц API или веб-служб OData

По возможности рекомендуется использовать страницы API вместо веб-службы OData. Страницы API быстрее загружают данные в отчеты Power BI, чем веб-службы OData. Кроме того, они более гибкие, поскольку позволяют получать данные из полей таблицы, которые не определены в объекте страницы.

<!--## <a name="setup"></a>Set up [!INCLUDE[prod_short](includes/prod_short.md)] on-premises for Power BI integration

This section explains the requirements for a [!INCLUDE[prod_short](includes/prod_short.md)] on-premises deployment to integrate with Power BI.

1. Configure either [NavUserPassword](/dynamics365/business-central/dev-itpro/administration/authenticating-users-with-navuserpassword) or [Microsoft Entra ID](/dynamics365/business-central/dev-itpro/administration/authenticating-users-with-azure-ad-overview) as the authentication method for the deployment.  
    
    > [!NOTE]
    > Power BI integration doesn't support Windows authentication and is not supported on Windows Client.

2. Enable OData web services and the ODataV4 endpoint.

    OData web service must be enabled on the [!INCLUDE[server](includes/server.md)], and OData port opened in firewall. For more information, see [Configuring Business Central Server - OData Web Services](/dynamics365/business-central/dev-itpro/administration/configure-server-instance#ODataServices).

    The local server must be accessible from the Internet.

3. Give [!INCLUDE[prod_short](includes/prod_short.md)] user accounts a web service access key.

    A web service access key is only needed to view [!INCLUDE[prod_short](includes/prod_short.md)] data in Power BI. You can assign a web service access key to each user account. Or instead, create a specific account with a web service access key for use by all users. For more information, see [Web Services Authentication](/dynamics365/business-central/dev-itpro/webservices/web-services-authentication#generate-a-web-service-access-key).

    <!--
    > [!IMPORTANT]
    > With [!INCLUDE[prod_short](../developer/includes/prod_short.md)] online, the use of access keys (Basic Auth) for web service authentication is [deprecated](/dynamics365/business-central/dev-itpro/upgrade/deprecated-features-w1#accesskeys). We recommend that you use OAuth2 instead. For more information, see [Use OAuth to Authorize Business Central Web Services](/dynamics365/business-central/dev-itpro/webservices/authenticate-web-services-using-oauth).-->

<!--4. Create an application registration for [!INCLUDE[prod_short](includes/prod_short.md)] in Microsoft Azure.

    To view Power BI reports embedded in [!INCLUDE[prod_short](includes/prod_short.md)] pages, an application must be registered for [!INCLUDE[prod_short](includes/prod_short.md)] in Microsoft Azure. The registered application needs permission to Power BI services. At a minimum, the app requires  **User.ReadWrite.All** permission. For users to view reports from shared Power BI workspaces, the app requires **Workspace.Read.All** permission. For more information, see [Registering [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises in Microsoft Entra ID for Integrating with Other Services](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

    > [!NOTE]
    > If your deployment uses NavUserPassword authentication, [!INCLUDE[prod_short](includes/prod_short.md)] connects to the same Power BI service for all users. You'll specify this service account as part of registering the application. With Microsoft Entra authentication, [!INCLUDE[prod_short](includes/prod_short.md)] connects to the Power BI service associated with the individual user accounts.

    <!-- Windows authentication can also be used but you can't get data from BC in Power BI -->
<!--5. Make the initial connection from Business Central to Power BI.

    Before end-users can use Power BI in [!INCLUDE[prod_short](includes/prod_short.md)], an Azure application administrator will have to give consent to the Power BI service.

    To make the initial connection, open [!INCLUDE[prod_short](includes/prod_short.md)], and run **Get Started with Power BI** from the Home page. This action will lead you through the consent process, and check your Power BI license. When prompted sign in using an Microsoft Entra admin account. For more information, see [Connect to Power BI - one time only](across-working-with-powerbi.md#connect).-->

## Настройка потоков данных

Потоки данных позволяют принимать, преобразовывать и загружать данные в рабочую область Power BI, а затем использовать эти данные в качестве основы для отчетов. В некоторых случаях в этих потоках данных могут возникать временные ошибки при выполнении запланированного обновления. Сообщение об ошибке выглядит следующим образом: `DataSource.Error: OData: Unable to read data from the transport connection: An existing connection was forcibly closed by the remote host.` 

Используя PowerAutomate, вы можете настроить количество повторных попыток для таких ситуаций. Дополнительную информацию см. в статье [Автоматический повтор потока данных в случае сбоя](/power-query/dataflows/automatically-retry-dataflow).

## См. также

[Business Central и Power BI](admin-powerbi.md)  
[Обзор компонентов и архитектуры интеграции Power BI для [!INCLUDE[prod_short](includes/prod_short.md)]](admin-powerbi-overview.md)  
[Power BI для потребителей](/power-bi/consumer/end-user-consumer)  
["Новый внешний вид" службы Power BI](/power-bi/service-new-look)  
[Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Документация Power BI](/power-bi/)  
[Бизнес-аналитика](bi.md)  
[Подготовьтесь к ведению бизнеса](ui-get-ready-business.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных Power BI](across-how-use-financials-data-source-powerbi.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных Power Apps](across-how-use-financials-data-source-powerapps.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] в Power Automate](across-how-use-financials-data-source-flow.md)  




[!INCLUDE[footer-include](includes/footer-banner.md)]
