---
title: Включение интеграции Power BI с Business Central
description: Узнайте, как настроить подключение к Power BI. С отчетами Power BI можно получить аналитические сведения, бизнес-аналитику и ключевые показатели эффективности из данных Business Central.
author: jswymer
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Power BI, setup, analysis, reporting, financial report, business intelligence, KPI
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: b3eb777c7a495c5b4b73ace26151e53403f81f00
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "8521206"
---
# <a name="enabling-power-bi-integration-with-prod_short"></a>Включение интеграции Power BI с [!INCLUDE[prod_short](includes/prod_short.md)]

В этой статье описывается, как подготовить [!INCLUDE[prod_short](includes/prod_short.md)] к интеграции с Power BI. [!INCLUDE[prod_short](includes/prod_short.md)] Online уже включен для интеграции, хотя есть некоторая информация о лицензировании, которую вы, возможно, захотите прочитать. Для [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises вам требуется настроить свою среду для подключения к Power BI, прежде чем пользователи смогут с ним работать.

## <a name="power-bi-licensing"></a><a name="license"></a>Лицензирование Power BI

С [!INCLUDE[prod_short](includes/prod_short.md)] пользователи получают бесплатную лицензию Power BI, которая обеспечивает доступ к наиболее распространенным функциям в [!INCLUDE[prod_short](includes/prod_short.md)] и Power BI. Вы также можете приобрести лицензию Power BI Pro, предоставляющую доступ к дополнительным функциям. В следующей таблице представлен обзор функций, доступных для каждой лицензии.

|Лицензия Power|Просмотр отчетов|Создание отчетов|Предоставление доступа к отчетам|Обновление отчетов| Приложения [!INCLUDE[prod_short](includes/prod_short.md)]|
|-------------|--------||
|Бесплатная Power BI|![флажок.](media/check.png)|![еще один флажок](media/check.png)|(ограничено)|(ограничено)||
|Power BI Pro|![и еще один флажок.](media/check.png)|![это флажок](media/check.png)|![снова флажок](media/check.png)|(обширная)|![последний флажок](media/check.png)|

Дополнительные сведения см. в разделе [Лицензирование службы Power BI для пользователей в вашей организации](/power-bi/admin/service-admin-licensing-organization) или [Регистрация на службу Power BI как физическое лицо](/power-bi/fundamentals/service-self-service-signup-for-power-bi).

## <a name="expose-data-through-api-pages-or-odata-web-services"></a><a name="exposedata"></a>Предоставлять данные через страницы API или веб-службы OData

Business Central предлагает два способа предоставления данных, которые могут быть использованы отчетами Power BI: страницы API и веб-службы Open Data Protocol (OData).

### <a name="api-pages"></a>Страницы API

> **ПРИМЕНЯЕТСЯ К:** только Business Central Online 

Страница API — это определенный тип страницы, созданный в коде AL, который обеспечивает доступ к таблицам базы данных через службу REST с поддержкой веб-перехватчика и OData v4. Страницы этого типа не могут отображаться в пользовательском интерфейсе, а предназначены для создания надежных служб интеграции.

Business Central Online поставляется с набором встроенных API-интерфейсов, которые можно использовать для получения данных о наиболее распространенных бизнес-объектах, таких как клиенты, товары, заказы на продажу и т. д. Для использования этих API в качестве источника данных для отчетов Power BI не требуются дополнительные усилия и настройка. Для получения дополнительной информации об этих API прочитайте [Business Central API V2.0](/dynamics365/business-central/dev-itpro/api-reference/v2.0/).

Business Central Online также поддерживает настраиваемые API. Разработчики приложений для решений Business Central могут создавать свои собственные страницы API и упаковывать их в расширения. Затем устанавливаются расширения на своем клиенте. После установки используются страницы API для своих отчетов Power BI, как встроенные API (v2.0). Для получения дополнительной информации о том, как создавать страницы API, прочитайте [Разработка собственного API](/dynamics365/business-central/dev-itpro/developer/devenv-develop-custom-api).

> [!IMPORTANT]
> С февраля 2022 г. отчеты Power BI для [!INCLUDE[prod_short](includes/prod_short.md)] Online извлекаются из вторичной реплики базы данных, доступной только для чтения по соображением производительности. Как следствие, разработчикам AL следует избегать проектирования страниц API, которые вносят изменения в базу данных, когда страницы открывают или загружают записи. В частности, рассмотрим код триггеров AL: OnInit, OnOpenPage, OnFindRecord, OnNextRecord, OnAfterGetRecord и OnAfterGetCurrRecord. Эти модификации базы данных в некоторых случаях могут вызвать проблемы с производительностью и помешать обновлению данных в отчете. Для получения дополнительной информации см. [Статьи о производительности для разработчиков](/dynamics365/business-central/dev-itpro/performance/performance-developer?branch=main#writing-efficient-web-services) в справке по разработке Business Central.
>
> В редких случаях поведение вызывает ошибку, когда пользователь пытается получить данные со страницы API для отчета в Power BI Desktop. Однако, если на пользовательской странице API необходимы модификации базы данных, пользователи Power BI Desktop могут форсировать поведение. Дополнительные сведения см. в разделе [Создание отчетов Power BI для отображения данных Business Central](across-how-use-financials-data-source-powerbi.md#fixing-problems).

### <a name="odata-web-services"></a>Веб-службы OData

Вы можете публиковать объекты приложения Business Central, такие как модули кода, страницы и запросы, как [Веб-службы OData](/dynamics365/business-central/dev-itpro/webservices/odata-web-services). В Business Central Online по умолчанию публикуется множество веб-служб. Простой способ найти веб-службы — найти *веб-службы* в [!INCLUDE[prod_short](includes/prod_short.md)]. На странице **Веб-службы** убедитесь, что поле **Опубликовать** выбрано для веб-служб, перечисленных выше. Дополнительные сведения о публикации веб-служб см. в разделе [Публикация веб-службы](across-how-publish-web-service.md).

Чтобы узнать, что вы можете сделать для обеспечения максимальной производительности веб-служб с точки зрения сервера Business Central Server (конечная точка) и потребителя (клиент), ознакомьтесь с разделом [Создание эффективных веб-служб](/dynamics365/business-central/dev-itpro/performance/performance-developer#writing-efficient-web-services).

### <a name="choosing-whether-to-use-api-pages-or-odata-web-services"></a>Выбор использования страниц API или веб-служб OData

По возможности рекомендуется использовать страницы API вместо веб-службы OData. Страницы API обычно быстрее загружают данные в отчеты Power BI, чем веб-службы OData. Кроме того, они более гибкие, поскольку позволяют получать данные из полей таблицы, которые не определены в объекте страницы.

## <a name="set-up-prod_short-on-premises-for-power-bi-integration"></a><a name="setup"></a>Настройка [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises для интеграции с Power BI

В этом разделе объясняются требования к развертыванию [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises для интеграции с Power BI.

1. Настройте либо NavUserPassword, либо проверку подлинности Azure Active Directory для развертывания.

    Интеграция Power BI не поддерживает проверку подлинности Windows.  

2. Включите веб-службы OData и конечную точку ODataV4.

    Веб-служба OData должна быть включена на [!INCLUDE[server](includes/server.md)], и порт OData открыт в брандмауэре. Дополнительные сведения см. в разделе [Настройка Business Central Server — веб-службы OData](/dynamics365/business-central/dev-itpro/administration/configure-server-instance#ODataServices).

    Локальный сервер должен быть доступен из Интернета.

3. Дайте учетным записям пользователей [!INCLUDE[prod_short](includes/prod_short.md)] ключ доступа к веб-службам.

    Ключ доступа к веб-службе необходим только для просмотра данных [!INCLUDE[prod_short](includes/prod_short.md)] в Power BI. Вы можете назначить ключ доступа к веб-службе для каждой учетной записи пользователей. Или вместо этого создайте конкретную учетную запись с ключом доступа к веб-службе для использования всеми пользователями. Дополнительные сведения см. в разделе [Проверка подлинности для веб-служб](/dynamics365/business-central/dev-itpro/webservices/web-services-authentication#generate-a-web-service-access-key).

    <!--
    > [!IMPORTANT]
    > With [!INCLUDE[prod_short](../developer/includes/prod_short.md)] online, the use of access keys (Basic Auth) for web service authentication is [deprecated](/dynamics365/business-central/dev-itpro/upgrade/deprecated-features-w1#accesskeys). We recommend that you use OAuth2 instead. For more information, see [Use OAuth to Authorize Business Central Web Services](/dynamics365/business-central/dev-itpro/webservices/authenticate-web-services-using-oauth).-->

4. Создайте регистрацию приложения [!INCLUDE[prod_short](includes/prod_short.md)] в Microsoft Azure.

    Чтобы просмотреть отчеты Power BI, встроенные в страницы [!INCLUDE[prod_short](includes/prod_short.md)], необходимо зарегистрировать приложение для [!INCLUDE[prod_short](includes/prod_short.md)] в Microsoft Azure. Зарегистрированному приложению требуется разрешение на службы Power BI. Для получения дополнительной информации см. раздел [Регистрация [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises в Azure AD для интеграции с другими службами](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

    > [!NOTE]
    > Если ваше развертывание использует аутентификацию NavUserPassword, [!INCLUDE[prod_short](includes/prod_short.md)] подключается к одной службе Power BI для всех пользователей. Вы укажете эту учетную запись службы при регистрации приложения. С аутентификацией Azure AD [!INCLUDE[prod_short](includes/prod_short.md)] подключается к службе Power BI, связанно с отдельными учетными записями пользователей.

    <!-- Windows authentication can also be used but you can't get data from BC in Power BI -->
5. Выполните первоначальное подключение Business Central к Power BI.

    Прежде чем конечные пользователи смогут использовать Power BI в [!INCLUDE[prod_short](includes/prod_short.md)], администратор приложения Azure должен будет дать согласие на службу Power BI.

    Для первоначального подключения откройте [!INCLUDE[prod_short](includes/prod_short.md)] и выполните **Начать с Power BI** из ролевого центра. Это действие проведет вас через процесс получения согласия и проверит вашу лицензию Power BI. При появлении запроса войдите в систему, используя учетную запись администратора Azure. Дополнительные сведения см. в разделе [Подключение к Power BI — только один раз](across-working-with-powerbi.md#connect).


## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/Configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

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