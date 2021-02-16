---
title: Обзор компонентов интеграции и архитектуры Power BI для Business Central | Документация Майкрософт
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
ms.openlocfilehash: 23a0c72775dbddc89a81105de3b2ed79d1f09432
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4753774"
---
# <a name="power-bi-integration-component-and-architecture-overview-for-prod_short"></a>Обзор компонентов и архитектуры интеграции Power BI для [!INCLUDE[prod_short](includes/prod_short.md)]

В этой статье вы узнаете о различных аспектах интеграции Power BI с [!INCLUDE[prod_short](includes/prod_short.md)], чтобы помочь вам разобраться в его реализации и использовании.

## <a name="components"></a>Компоненты

В следующей таблице описаны основные компоненты, связанные с интеграцией Power BI.

|Компонент|Описание|
|---------|-----------|
|Power BI|Облачная служба размещения отчетов и управления ими.|
|Power BI Desktop|Инструмент разработки для создания отчетов и панелей мониторинга, позволяющий запускать отчеты. Он доступен для бесплатной загрузки в Microsoft Store и устанавливается локально.|
|[!INCLUDE[prod_short](includes/prod_short.md)]|Сетевое или локальное решение с соединителями, доступными для Power BI, и возможностью внедрить часть Power BI.|

## <a name="whats-available-from-the-start"></a>Что доступно с самого начала

В следующей таблице описаны доступные функции.

|Функция|Поддержка [!INCLUDE[prod_short](includes/prod_short.md)] Online или On-Premises|
|-------|---------------------|
|Соединители Power BI|Оба. Различные соединители для версий Online и On-Premises. Один и тот же разъем используется для Power BI Desktop и службы Power BI |
|Встроенный интерфейс для просмотра заданного отчета внутри информационной панели в [!INCLUDE[prod_short](includes/prod_short.md)]|Оба. Требуется конфигурация для отображения отчетов в локальной среде.|
|Управление отчетами Power BI из [!INCLUDE[prod_short](includes/prod_short.md)]|Online|
|Отчеты Power BI по умолчанию в ролевых центрах, развернутых в Power BI|Online|
|Приложения Power BI в Microsoft AppSource|Online.|

## <a name="architecture"></a>Архитектура

[!INCLUDE[prod_short](includes/prod_short.md)] интегрируется с Power BI через соединитель с использованием OData. Источник данных для отчетов Power BI представляется как веб-служба OData.

![Архитектура Power BI для интеграции с Business Central](./media/power-bi-architecture.png)

## <a name="general-flow"></a>Общий поток

На следующей диаграмме показан основной рабочий процесс для пользователей при подключении [!INCLUDE[prod_short](includes/prod_short.md)] к Power BI.

![Рабочий поток Power BI для интеграции с Business Central](./media/power-bi-flow.png)

1. Пользователь регистрируется на учетную запись Power BI.
2. Пользователь подключается к Power BI из [!INCLUDE[prod_short](includes/prod_short.md)].
3. [!INCLUDE[prod_short](includes/prod_short.md)] проверяет лицензию.
4. [!INCLUDE[prod_short](includes/prod_short.md)] развертывает отчеты по умолчанию в службе Power BI. Этот шаг выполняется только для [!INCLUDE[prod_short](includes/prod_short.md)] Online.
5. [!INCLUDE[prod_short](includes/prod_short.md)] делает отчеты в Power BI доступными для выбора в [!INCLUDE[prod_short](includes/prod_short.md)]. Отчеты по умолчанию автоматически отображаются в частях Power BI.
6. Пользователь создает отчет в Power BI Desktop.
7. Пользователь публикует отчет в службе Power BI. Отчеты затем становятся доступными для выбора в [!INCLUDE[prod_short](includes/prod_short.md)].

## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Business Central и Power BI](admin-powerbi.md)  
[Power BI для потребителей](/power-bi/consumer/end-user-consumer)  
["Новый внешний вид" службы Power BI](/power-bi/service-new-look)  
[Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Документация Power BI](/power-bi/)  
[Бизнес-аналитика](bi.md)  
[Приступая к работе](product-get-started.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных Power BI](across-how-use-financials-data-source-powerbi.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных Power Apps](across-how-use-financials-data-source-powerapps.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] в Power Automate](across-how-use-financials-data-source-flow.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  
