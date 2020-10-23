---
title: Включение интеграции Power BI с Business Central
description: Узнайте, как настроить подключение к Power Bi, чтобы вы могли получать аналитические данные, бизнес-аналитику и ключевые показатели эффективности из данных Business Central с помощью приложений Business Central для Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: ce4b45dbe80ab1972c92cde144b457eeeaff3402
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3927076"
---
# <a name="enabling-power-bi-integration-with-prodshort"></a>Включение интеграции Power BI с [!INCLUDE[prodshort](includes/prodshort.md)]

В этой статье описывается, как подготовить [!INCLUDE[prodshort](includes/prodshort.md)] к интеграции с Power BI. [!INCLUDE[prodshort](includes/prodshort.md)] Online уже включен для интеграции, хотя есть некоторая информация о лицензировании, которую вы, возможно, захотите прочитать. Для [!INCLUDE[prodshort](includes/prodshort.md)] On-Premises вам требуется настроить свою среду для подключения к Power BI, прежде чем пользователи смогут с ним работать.

## <a name="power-bi-licensing"></a><a name="license"></a>Лицензирование Power BI

С [!INCLUDE[prodshort](includes/prodshort.md)] пользователи получают бесплатную лицензию Power BI, которая обеспечивает доступ к наиболее распространенным функциям в [!INCLUDE[prodshort](includes/prodshort.md)] и Power BI. Вы также можете приобрести лицензию Power BI Pro, предоставляющую доступ к дополнительным функциям. В следующей таблице представлен обзор функций, доступных для каждой лицензии.

|Лицензия Power|Просмотр отчетов|Создание отчетов|Предоставление доступа к отчетам|Обновление отчетов| Приложения [!INCLUDE[prodshort](includes/prodshort.md)]|
|-------------|--------||
|Бесплатная Power BI|![флажок](media/check.png)|![еще один флажок](media/check.png)|(ограничено)|(ограничено)||
|Power BI Pro|![и еще один флажок](media/check.png)|![это флажок](media/check.png)|![снова флажок](media/check.png)|(обширная)|![последний флажок](media/check.png)|

Дополнительные сведения см. в разделе [Лицензирование службы Power BI для пользователей в вашей организации](/power-bi/admin/service-admin-licensing-organization) или [Регистрация на службу Power BI как физическое лицо](/power-bi/fundamentals/service-self-service-signup-for-power-bi).

## <a name="set-up-prodshort-on-premises-for-power-bi-integration"></a><a name="setup"></a>Настройка [!INCLUDE[prodshort](includes/prodshort.md)] On-Premises для интеграции с Power BI

В этом разделе объясняются требования к развертыванию [!INCLUDE[prodshort](includes/prodshort.md)] On-Premises для интеграции с Power BI.

1. Веб-службы OData и конечная точка ODataV4 включены.

    Веб-служба OData должна быть включена на [!INCLUDE[server](includes/server.md)], и порт OData открыт в брандмауэре. Дополнительные сведения см. в разделе [Настройка Business Central Server — веб-службы OData](/dynamics365/business-central/dev-itpro/administration/configure-server-instance#ODataServices).
    
    Локальный сервер должен быть доступен из Интернета.

2. Учетные записи пользователей [!INCLUDE[prodshort](includes/prodshort.md)] имеют ключ доступа к веб-службам.

    Ключ доступа к веб-службе необходим для просмотра данных [!INCLUDE[prodshort](includes/prodshort.md)] в Power BI. Вы можете назначить ключ доступа к веб-службе для каждой учетной записи пользователей. Или вместо этого создайте конкретную учетную запись с ключом доступа к веб-службе для использования всеми пользователями. Дополнительные сведения см. в разделе [Проверка подлинности для веб-служб](/dynamics365/business-central/dev-itpro/webservices/web-services-authentication#generate-a-web-service-access-key).

3. NavUserPassword или проверка подлинности Azure Active Directory настроена.

4. Для просмотра отчетов Power BI, встроенных в страницы [!INCLUDE[prodshort](includes/prodshort.md)], необходимо зарегистрировать приложение для [!INCLUDE[prodshort](includes/prodshort.md)] в Microsoft Azure.

    Зарегистрированному приложению требуется разрешение на службы Power BI. Для получения дополнительной информации см. раздел [Регистрация [!INCLUDE[prodshort](includes/prodshort.md)] On-Premises в Azure AD для интеграции с другими службами](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

    > [!NOTE]
    > Если ваше развертывание использует аутентификацию NavUserPassword, [!INCLUDE[prodshort](includes/prodshort.md)] подключается к одной службе Power BI для всех пользователей. Вы укажете эту учетную запись службы при регистрации приложения. С аутентификацией Azure AD [!INCLUDE[prodshort](includes/prodshort.md)] подключается к службе Power BI, связанно с отдельными учетными записями пользователей.

    <!-- Windows authentication can also be used but you can't get data from BC in Power BI -->

## <a name="publish-data-as-web-services"></a>Публикация данных как веб-служб

Модули Codeunit, страницы и запросы, которые вы хотите использовать в качестве источника данных в отчетах Power BI, должны публиковаться как веб-службы. По умолчанию опубликовано множество веб-служб. Простой способ найти веб-службы — найти *веб-службы* в [!INCLUDE[prodshort](includes/prodshort.md)]. На странице **Веб-службы** убедитесь, что поле **Опубликовать** выбрано для веб-служб, перечисленных выше. Эту задачу обычно является административной задачей.

Дополнительные сведения о публикации веб-служб см. в разделе [Публикация веб-службы](across-how-publish-web-service.md).

> [!TIP]
> Чтобы узнать, что вы можете сделать для обеспечения максимальной производительности веб-служб с точки зрения сервера Business Central Server (конечная точка) и потребителя (клиент), ознакомьтесь с разделом [Создание эффективных веб-служб](/dynamics365/business-central/dev-itpro/performance/performance-developer#writing-efficient-web-services).




## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/Configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Business Central и Power BI](admin-powerbi.md)  
[Обзор компонентов и архитектуры интеграции Power BI для [!INCLUDE[prodshort](includes/prodshort.md)]](admin-powerbi-overview.md)  
[Power BI для потребителей](/power-bi/consumer/end-user-consumer)  
["Новый внешний вид" службы Power BI](/power-bi/service-new-look)  
[Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Документация Power BI](/power-bi/)  
[Бизнес-аналитика](bi.md)  
[Приступая к работе](product-get-started.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных Power BI](across-how-use-financials-data-source-powerbi.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных Power Apps](across-how-use-financials-data-source-powerapps.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в Power Automate](across-how-use-financials-data-source-flow.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
