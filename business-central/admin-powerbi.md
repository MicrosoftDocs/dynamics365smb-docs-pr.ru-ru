---
title: Общий сведения по Business Central и Power BI
description: Получение обзора использования Power BI для получения аналитических сведений, бизнес-аналитики и ключевых показателей эффективности из данных Business Central.
author: jswymer
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.search.form: 6316, 6317
ms.reviewer: edupont
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: c1935c51fbcabfc0371530532f18b2aaf6005dbb
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "8511809"
---
# <a name="prod_short-and-power-bi"></a>[!INCLUDE[prod_short](includes/prod_short.md)] и Power BI

Получать аналитические сведения о ваших данных [!INCLUDE[prod_short](includes/prod_short.md)] легко с помощью [Power BI](https://powerbi.microsoft.com) — системы визуализации данных от Microsoft. Power BI извлекает данные [!INCLUDE[prod_short](includes/prod_short.md)], позволяющие создавать панели мониторинга и отчеты на основе этих данных. Power BI предоставляет гибкую альтернативу встроенным отчетам [!INCLUDE[prod_short](includes/prod_short.md)], позволяя детализировать и настраивать визуализацию и даже объединять данные из разных компаний в [!INCLUDE[prod_short](includes/prod_short.md)]. Некоторые отчеты Power BI также можно встроить в Business Central и просматривать, не выходя из системы. Более сложные панели мониторинга лучше использовать с веб-сайта Power BI.

![Power BI и Business Central.](media/power-bi-intro.png)

## <a name="what-you-can-do-with-power-bi-and-prod_short"></a>Что можно делать с Power BI и [!INCLUDE[prod_short](includes/prod_short.md)]

Есть разные возможности для работы с [!INCLUDE[prod_short](includes/prod_short.md)] и Power BI. Некоторые вещи можете делать из Power BI, а все остальное делается из [!INCLUDE[prod_short](includes/prod_short.md)]. Кроме того, некоторые функции доступны только с [!INCLUDE[prod_short](includes/prod_short.md)] Online, но не с On-Premises. Следующая таблица дает вам обзор.

|Функция|Описание|Online|On-premises|Дополнительная информация|
|-------|-----------|--------------|-----------|----------------|
|Просмотр данных [!INCLUDE[prod_short](includes/prod_short.md)] в Power BI|Вы можете просматривать свои данные из [!INCLUDE[prod_short](includes/prod_short.md)] в отчетах в Power BI. [!INCLUDE[prod_short](includes/prod_short.md)] Online включает некоторые предопределенные отчеты Power BI. Или ваша организация могла предоставить вам доступ к некоторым настраиваемым отчетам.|![Работа онлайн.](media/check.png)|![Работа локально](media/check.png)|[См. ...](across-working-with-business-central-in-powerbi.md)|
|Просмотр отчетов Power BI в клиенте [!INCLUDE[prod_short](includes/prod_short.md)].| Отчеты Power BI, отображающие данные [!INCLUDE[prod_short](includes/prod_short.md)], могут быть встроены прямо в страницы частей [!INCLUDE[prod_short](includes/prod_short.md)]. Вы можете переключить часть для отображения любого отчета, который вам доступен. |![работает онлайн.](media/check.png)|![Работа локально](media/check.png)<sup>[*](#onprem)</sup>|[См. ...](across-working-with-powerbi.md).|
|Создавайте отчеты и панели мониторинга в Power BI, которые отображают данные [!INCLUDE[prod_short](includes/prod_short.md)].|Используйте Power BI Desktop для создания собственных отчетов и панелей мониторинга. Вы можете опубликовать отчеты в своей собственной службе Power BI или поделиться ими с другими пользователями в вашей организации.|![Работа онлайн.](media/check.png)|![работа локально](media/check.png)|[См. ...](across-how-use-financials-data-source-powerbi.md)
|Приложения [!INCLUDE[prod_short](includes/prod_short.md)] в Power BI| [!INCLUDE[prod_short](includes/prod_short.md)] публикует три приложения для Power BI в Microsoft AppSource. Эти приложения создают подробные отчеты и панели мониторинга в вашей службе Power BI для просмотра данных [!INCLUDE[prod_short](includes/prod_short.md)]. Доступные приложения включают: <ul><li>[!INCLUDE [prod_long](includes/prod_long.md)] — CRM </li><li>[!INCLUDE [prod_long](includes/prod_long.md)] — Finance </li><li>[!INCLUDE [prod_long](includes/prod_long.md)] — Sales </li></ul>  |![Работа онлайн.](media/check.png)||[См. ...](across-powerbi-business-central-apps.md)

<a name="onprem"><sup>*</sup></a> Для этой функции требуется зарегистрированное приложение для Business Central в Microsoft Azure. Для получения дополнительной информации см. раздел [Регистрация Business Central On-Premises в Azure AD для интеграции с другими службами](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

## <a name="getting-ready-to-use-power-bi"></a>Подготовка к использованию Power BI

Есть несколько задач, которые необходимо выполнить, прежде чем вы сможете начать использовать Power BI с [!INCLUDE[prod_short](includes/prod_short.md)]. <!-- Some of the tasks are typically only done by administrators or super users.--> Задачи будут зависеть от вашей роли в вашей организации и от того, что вы хотите делать с Power BI:

- Как *бизнес-пользователь* вы хотите просмотреть отчеты Power BI, либо в службе Power BI или в Business Central.
- Как *администратор* вы несете ответственность за управление общекорпоративными настройками, которые определяют, как работают Business Central и Power BI.
- Как *создатель отчета* вы хотите создать собственные отчеты Power BI, которыми вы можете поделиться с другими пользователями.

|Задача|Бизнес-пользователь|Администратор|Создатель отчета|Дополнительная информация|
|----|-------------|-------------|-----------------------|----------------|
|Получите учетная запись Power BI.|![и еще один флажок.](media/check.png)|![это флажок](media/check.png)|![снова флажок](media/check.png)|Перейти к [https://powerbi.microsoft.com](https://powerbi.microsoft.com). Чтобы зарегистрироваться на учетную запись, используйте рабочий адрес электронной почты и пароль. <br /><br/>Для регистрации требуется, чтобы у вас была лицензия, но в большинстве случаев у вас уже должна быть бесплатная лицензия, подробнее прочитайте в [Лицензирование Power BI](admin-powerbi-setup.md#license).|
|Поставьте Power BI Desktop|||![снова флажок.](media/check.png)|Чтобы скачать, перейдите в [Power BI Desktop](https://powerbi.microsoft.com/desktop/). Дополнительные сведения см. в разделе [Получение Power BI Desktop](/power-bi/fundamentals/desktop-get-the-desktop).
|Предоставление данных Business Central для Power BI||![это флажок.](media/check.png)|![снова флажок](media/check.png)|[Предоставлять данные через страницы API или веб-службы OData](admin-powerbi-setup.md#exposedata)
|Включение интеграции Power BI<br />(только локальная версия)||![это флажок.](media/check.png)||[Настройка локальной версии Business Central для интеграции Power BI](admin-powerbi-setup.md#setup)|


<!--



1. If you're using [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, make sure your deployment meets the requirements outlined in [Set up [!INCLUDE[prod_short](includes/prod_short.md)] on-premises for Power BI integration](admin-powerbi-setup.md#setup). This task is typically an administrative task.

2. Expose Business Central data through API pages or published web services.

    Business Central online automatically included several pages as APIs. For more information, see [Business Central API V2.0](/dynamics365/business-central/dev-itpro/api-reference/v2.0/). Application developers for Business Central online can create custom API pages that you can then consume in reports. For more information, see [Developing a Custom API](/dynamics365/business-central/dev-itpro/developer/devenv-develop-custom-api).

   Codeunit, page, and query objects can be published as OData web services. There are many web services published by default. An easy way to find the web services is to search for *web services* in [!INCLUDE[prod_short](includes/prod_short.md)]. For more information about publishing web services, see [Publish a Web Service](across-how-publish-web-service.md).

3. Get a Power BI account.

   To do anything with Power BI and [!INCLUDE[prod_short](includes/prod_short.md)], whether you're an administrator or just a consumer, you'll need Power BI service account. To get an account, go to [https://powerbi.microsoft.com](https://powerbi.microsoft.com). To sign up for an account, use your work email address and password. Sign-up requires that you have a license, but in most cases you should already have a free license. For more information, see [Power BI Licensing](admin-powerbi-setup.md#license).

4. If you want to create your own Power BI reports, get Power BI Desktop.

   You can download [Power BI Desktop](https://powerbi.microsoft.com/desktop/). For more information, see [Get Power BI Desktop](/power-bi/fundamentals/desktop-get-the-desktop).

-->

## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

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