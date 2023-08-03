---
title: Общий сведения по Business Central и Power BI
description: 'Получение обзора использования Power BI для получения аналитических сведений, бизнес-аналитики и ключевых показателей эффективности из данных Business Central.'
author: jswymer
ms.topic: overview
ms.search.keywords: 'account schedule, analysis, reporting, financial report, business intelligence, KPI'
ms.search.form: '6316, 6317'
ms.reviewer: jswymer
ms.date: 07/17/2023
ms.author: jswymer
ms.custom: bap-template
---
# Введение в [!INCLUDE[prod_short](includes/prod_short.md)] и Power BI

Получать аналитические сведения о ваших данных [!INCLUDE[prod_short](includes/prod_short.md)] легко с помощью [Power BI](https://powerbi.microsoft.com) — системы визуализации данных от Microsoft. Power BI извлекает данные [!INCLUDE[prod_short](includes/prod_short.md)], позволяющие вам создавать панели мониторинга и отчеты на основе этих данных. Power BI предоставляет гибкую альтернативу встроенным отчетам [!INCLUDE[prod_short](includes/prod_short.md)], позволяя детализировать и настраивать визуализацию и даже объединять данные из разных компаний в [!INCLUDE[prod_short](includes/prod_short.md)]. Некоторые отчеты Power BI также можно встроить в Business Central и просматривать, не выходя из системы. Более сложные панели мониторинга лучше использовать с веб-сайта Power BI.

![Power BI и Business Central.](media/power-bi-intro.png)

## Что можно делать с Power BI и [!INCLUDE[prod_short](includes/prod_short.md)]

Есть разные возможности для работы с [!INCLUDE[prod_short](includes/prod_short.md)] и Power BI. Некоторые вещи можете делать из Power BI, а все остальное делается из [!INCLUDE[prod_short](includes/prod_short.md)]. Кроме того, некоторые функции доступны только с [!INCLUDE[prod_short](includes/prod_short.md)] Online, но не с On-Premises. Следующая таблица дает вам обзор.

|Функция|Описанием|Online|Локальная служба|Узнать больше|
|-------|-----------|--------------|-----------|----------------|
|Просмотр данных [!INCLUDE[prod_short](includes/prod_short.md)] в Power BI|Вы можете просматривать свои данные из [!INCLUDE[prod_short](includes/prod_short.md)] в отчетах в Power BI. [!INCLUDE[prod_short](includes/prod_short.md)] Online включает некоторые предопределенные отчеты Power BI. Или ваша организация могла предоставить вам доступ к некоторым настраиваемым отчетам.|![Работа онлайн.](media/check.png)|![Работа локально](media/check.png)|[Здесь...](across-working-with-business-central-in-powerbi.md)|
|Просмотр отчетов Power BI в клиенте [!INCLUDE[prod_short](includes/prod_short.md)].| Отчеты Power BI, отображающие данные [!INCLUDE[prod_short](includes/prod_short.md)], могут быть встроены прямо в страницы частей [!INCLUDE[prod_short](includes/prod_short.md)]. Вы можете переключить часть для отображения любого отчета, который вам доступен. |![работает онлайн.](media/check.png)|![Работа локально](media/check.png)<sup>[*](#onprem)</sup>|[Здесь...](across-working-with-powerbi.md).|
|Создавайте отчеты и панели мониторинга в Power BI, которые отображают данные [!INCLUDE[prod_short](includes/prod_short.md)].|Используйте Power BI Desktop для создания собственных отчетов и панелей мониторинга. Вы можете опубликовать отчеты в своей собственной службе Power BI или поделиться ими с другими пользователями в вашей организации.|![Работа онлайн.](media/check.png)|![работа локально](media/check.png)|[Здесь...](across-how-use-financials-data-source-powerbi.md)|
|Приложения [!INCLUDE[prod_short](includes/prod_short.md)] в Power BI| [!INCLUDE[prod_short](includes/prod_short.md)] публикует три приложения для Power BI в Microsoft AppSource. Эти приложения создают подробные отчеты и панели мониторинга в вашей службе Power BI для просмотра данных [!INCLUDE[prod_short](includes/prod_short.md)]. Доступные приложения включают: <ul><li>[!INCLUDE [prod_long](includes/prod_long.md)] — CRM </li><li>[!INCLUDE [prod_long](includes/prod_long.md)] — Finance </li><li>[!INCLUDE [prod_long](includes/prod_long.md)] — Sales </li></ul>  |![Работа онлайн.](media/check.png)||[Здесь...](across-powerbi-business-central-apps.md)|
|Работа с данными [!INCLUDE [prod_short](includes/prod_short.md)] в витринах и потоках данных|С июля 2022 года вы можете использовать соединитель [!INCLUDE [prod_short](includes/prod_short.md)] в Power Query Online для потоков данных, которыми вы делитесь в разных отчетах и информационных панелях.|![работает онлайн.](media/check.png)||[Здесь...](across-powerbi-business-central-apps.md)|

<a name="onprem"><sup>*</sup></a> Для этой функции требуется зарегистрированное приложение для Business Central в Microsoft Azure. Для получения дополнительной информации см. статью [Регистрация Business Central On-Premises в Azure AD для интеграции с другими службами](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

## Подготовка к использованию Power BI

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

## Отслеживание КПЭ вашего бизнеса с помощью метрик Power BI

Если вы используете Power BI для обработки данных [!INCLUDE[prod_short](includes/prod_short.md)], вы легко можете отслеживать важные для вас КПЭ или метрики. 

С помощью метрик в Power BI вы можете создавать свои собственные метрики и отслеживать их в сравнении со своими ключевыми бизнес-целями на одной панели. Эта функция способствует выработке культуры данных, стимулируя ответственность, единообразие и прозрачность для команд и инициатив в организациях. 

Настройка метрик Power BI предполагает четыре шага:

1. Создайте систему показателей в службе Power BI . Подробнее см. в статье [Создание систем показателей в Power BI](/power-bi/create-reports/service-goals-create).  
2. Добавьте _метрики_ , которые вы хотите отслеживать, подключившись к своему отчету Power BI по телеметрии. Подробнее см. в статье [Создание подключенных метрик](/power-bi/create-reports/service-goals-create-connected).  
3. Чтобы добавить оповещения, определите правила статуса для своих метрик. Подробнее см. в статье [Создание автоматических правил состояния для метрик](/power-bi/create-reports/service-metrics-status-rules).  

    Этот шаг позволяет автоматизировать обновления статуса на основе правил, регулирующих данную метрику. Правила инициируют изменения в зависимости от значения, процента достижения цели, условий по дате или комбинации этих трех факторов, что делает правила максимально универсальными. Для подключенных метрик эти правила статуса обновляются каждый раз, когда обновляются данные в вашей системе показателей.
4. Наконец, следите за метриками, получая оповещения в Teams или по электронной почте. Подробнее см. в статье [Отслеживание метрик](/power-bi/create-reports/service-metrics-follow).  

Подробнее о метриках Power BI см. в статье [Начало работы с метриками в Power BI](/power-bi/create-reports/service-goals-introduction).

> [!NOTE]
> В настоящее встраивать системы показателей из метрик Power BI в [!INCLUDE[prod_short](includes/prod_short.md)] невозможно.

## Дальнейшие шаги

- Если вы администратор, которому нужно настроить Power BI в [!INCLUDE[prod_short](includes/prod_short.md)], см. статью [Включение интеграции Power BI](admin-powerbi-setup.md).
- Если интеграция с Power BI уже настроена и вы хотите опробовать ее функции, см. статью [Работа с отчетами Power BI в Business Central](across-working-with-powerbi.md).

## См. соответствующее [обучение Microsoft](/training/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## См. также

[Бизнес-аналитика](bi.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных Power BI](across-how-use-financials-data-source-powerbi.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных Power Apps](across-how-use-financials-data-source-powerapps.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] в Power Automate](across-how-use-financials-data-source-flow.md)  
[Документация Power BI](/power-bi/)  
[Что такое Power BI?](/power-bi/fundamentals/power-bi-overview)  
[Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Введение в витрины данных](/power-bi/transform-model/datamarts/datamarts-overview)  
[Введение в потоки данных и самостоятельную подготовку данных](/power-bi/transform-model/dataflows/dataflows-introduction-self-service)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
