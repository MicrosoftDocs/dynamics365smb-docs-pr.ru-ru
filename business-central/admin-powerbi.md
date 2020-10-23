---
title: Введение в Business Central и Power BI | Документация Майкрософт
description: Анализ данных, бизнес-аналитика и КПЭ на основе данных Business Central становятся проще благодаря приложениям Business Central для Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.reviewer: edupont
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: e339033e8529f59f548e8bf71fd683f9a2a17eba
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3917880"
---
# <a name="prodshort-and-power-bi"></a>[!INCLUDE[prodshort](includes/prodshort.md)] и Power BI

Получать аналитические сведения о ваших данных [!INCLUDE[prodshort](includes/prodshort.md)] легко с помощью [Power BI](https://powerbi.microsoft.com) — системы визуализации данных от Microsoft. Power BI извлекает данные [!INCLUDE[prodshort](includes/prodshort.md)], позволяющие создавать панели мониторинга и отчеты на основе этих данных. Power BI предоставляет гибкую альтернативу встроенным отчетам [!INCLUDE[prodshort](includes/prodshort.md)], позволяя детализировать и настраивать визуализацию и даже объединять данные из разных компаний в [!INCLUDE[prodshort](includes/prodshort.md)]. Некоторые отчеты Power BI также можно встроить в Business Central и просматривать, не выходя из системы. Более сложные панели мониторинга лучше использовать с веб-сайта Power BI.

![Power BI и Business Central](media/power-bi-intro.png)


## <a name="what-you-can-do-with-power-bi-and-prodshort"></a>Что можно делать с Power BI и [!INCLUDE[prodshort](includes/prodshort.md)]

Есть разные возможности для работы с [!INCLUDE[prodshort](includes/prodshort.md)] и Power BI. Некоторые вещи можете делать из Power BI, а все остальное делается из [!INCLUDE[prodshort](includes/prodshort.md)]. Кроме того, некоторые функции доступны только с [!INCLUDE[prodshort](includes/prodshort.md)] Online, но не с On-Premises. Следующая таблица дает вам обзор.

|Функция|Описание|Online|On-premises|Дополнительная информация|
|-------|-----------|--------------|-----------|----------------|
|Просмотр данных [!INCLUDE[prodshort](includes/prodshort.md)] в Power BI|Вы можете просматривать свои данные из [!INCLUDE[prodshort](includes/prodshort.md)] в отчетах в Power BI. [!INCLUDE[prodshort](includes/prodshort.md)] Online включает некоторые предопределенные отчеты Power BI. Или ваша организация могла предоставить вам доступ к некоторым настраиваемым отчетам.|![Работа онлайн](media/check.png)|![Работа локально](media/check.png)|[См. ...](across-working-with-powerbi.md)|
|Просмотр отчетов Power BI в клиенте [!INCLUDE[prodshort](includes/prodshort.md)].| Отчеты Power BI, отображающие данные [!INCLUDE[prodshort](includes/prodshort.md)], могут быть встроены прямо в страницы частей [!INCLUDE[prodshort](includes/prodshort.md)]. Вы можете переключить часть для отображения любого отчета, который вам доступен. |![работа онлайн](media/check.png)|![Работа локально](media/check.png)<sup>[*](#onprem)</sup>|[См. ...](across-working-with-business-central-in-powerbi.md).|
|Создавайте отчеты и панели мониторинга в Power BI, которые отображают данные [!INCLUDE[prodshort](includes/prodshort.md)].|Используйте Power BI Desktop для создания собственных отчетов и панелей мониторинга. Вы можете опубликовать отчеты в своей собственной службе Power BI или поделиться ими с другими пользователями в вашей организации.|![Работа онлайн](media/check.png)|![работа локально](media/check.png)|[См. ...](across-how-use-financials-data-source-powerbi.md)
|Приложения [!INCLUDE[prodshort](includes/prodshort.md)] в Power BI| [!INCLUDE[prodshort](includes/prodshort.md)] публикует три приложения для Power BI в Microsoft AppSource. Эти приложения создают подробные отчеты и панели мониторинга в вашей службе Power BI для просмотра данных [!INCLUDE[prodshort](includes/prodshort.md)]. Доступные приложения включают: <ul><li>[!INCLUDE [prodlong](includes/prodlong.md)] — CRM </li><li>[!INCLUDE [prodlong](includes/prodlong.md)] — Finance </li><li>[!INCLUDE [prodlong](includes/prodlong.md)] — Sales </li></ul>  |![Работа онлайн](media/check.png)||[См. ...](across-powerbi-business-central-apps.md)

<a name="onprem"><sup>*</sup></a> Для этой функции требуется зарегистрированное приложение для Business Central в Microsoft Azure. Для получения дополнительной информации см. раздел [Регистрация Business Central On-Premises в Azure AD для интеграции с другими службами](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

## <a name="getting-ready-to-use-power-bi"></a>Подготовка к использованию Power BI

Есть несколько задач, которые необходимо выполнить, прежде чем вы сможете начать использовать Power BI с [!INCLUDE[prodshort](includes/prodshort.md)]. Некоторые задачи обычно выполняются только администраторами или суперпользователями.

1. Если вы используете [!INCLUDE[prodshort](includes/prodshort.md)] On-Premises, убедитесь, что ваше развертывание соответствует требованиям, изложенным в разделе [Настройка [!INCLUDE[prodshort](includes/prodshort.md)] On-Premises для интеграции Power BI](admin-powerbi-setup.md#setup). Эту задачу обычно является административной задачей.

2. Опубликуйте данные как веб-службы.

    Модули Codeunit, страницы и запросы, которые вы хотите использовать в качестве источника данных в отчетах Power BI, должны публиковаться как веб-службы. По умолчанию опубликовано множество веб-служб. Простой способ найти веб-службы — найти *веб-службы* в [!INCLUDE[prodshort](includes/prodshort.md)].
    
    Дополнительные сведения о публикации веб-служб см. в разделе [Публикация веб-службы](across-how-publish-web-service.md).

3. Получите учетная запись Power BI.

    Чтобы делать что-то с Power BI и [!INCLUDE[prodshort](includes/prodshort.md)], независимо от того, являетесь ли вы администратором или просто пользователем, вам понадобится учетная данная службы Power BI. Чтобы получить учетную запись, перейдите на сайт [https://powerbi.microsoft.com](https://powerbi.microsoft.com). Чтобы зарегистрироваться на учетную запись, используйте рабочий адрес электронной почты и пароль. Для регистрации требуется, чтобы у вас была лицензия, но в большинстве случаев у вас уже должна быть бесплатная лицензия. Дополнительные сведения см. в разделе [Лицензирование Power BI](admin-powerbi-setup.md#license).

4. Если вы хотите создавать свои собственные отчеты Power BI, получите Power BI Desktop.

    Вы можете скачать [Power BI Desktop](https://powerbi.microsoft.com/desktop/). Дополнительные сведения см. в разделе [Получение Power BI Desktop](/power-bi/fundamentals/desktop-get-the-desktop).

## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

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
