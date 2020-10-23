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
ms.openlocfilehash: d02740b0f4c73b96be9268cfdf5e4c3de157d5d5
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3924532"
---
# <a name="power-bi-integration-component-and-architecture-overview-for-prodshort"></a>Обзор компонентов и архитектуры интеграции Power BI для [!INCLUDE[prodshort](includes/prodshort.md)]

В этой статье вы узнаете о различных аспектах интеграции Power BI с [!INCLUDE[prodshort](includes/prodshort.md)], чтобы помочь вам разобраться в его реализации и использовании.

## <a name="components"></a>Компоненты

В следующей таблице описаны основные компоненты, связанные с интеграцией Power BI.

|Компонент|Описание|
|---------|-----------|
|Power BI|Облачная служба размещения отчетов и управления ими.|
|Power BI Desktop|Инструмент разработки для создания отчетов и панелей мониторинга, позволяющий запускать отчеты. Он доступен для бесплатной загрузки в Microsoft Store и устанавливается локально.|
|[!INCLUDE[prodshort](includes/prodshort.md)]|Сетевое или локальное решение с соединителями, доступными для Power BI, и возможностью внедрить часть Power BI.|

## <a name="whats-available-from-the-start"></a>Что доступно с самого начала

В следующей таблице описаны доступные функции.

|Функция|Поддержка [!INCLUDE[prodshort](includes/prodshort.md)] Online или On-Premises|
|-------|---------------------|
|Соединители Power BI|Оба. Различные соединители для версий Online и On-Premises. Один и тот же разъем используется для Power BI Desktop и службы Power BI |
|Встроенный интерфейс для просмотра заданного отчета внутри информационной панели в [!INCLUDE[prodshort](includes/prodshort.md)]|Оба. Требуется конфигурация для отображения отчетов в локальной среде.|
|Управление отчетами Power BI из [!INCLUDE[prodshort](includes/prodshort.md)]|Online|
|Отчеты Power BI по умолчанию в ролевых центрах, развернутых в Power BI|Online|
|Приложения Power BI в Microsoft AppSource|Online.|

## <a name="architecture"></a>Архитектура

[!INCLUDE[prodshort](includes/prodshort.md)] интегрируется с Power BI через соединитель с использованием OData. Источник данных для отчетов Power BI представляется как веб-служба OData.

![Архитектура Power BI для интеграции с Business Central](./media/power-bi-architecture.png)

## <a name="general-flow"></a>Общий поток

На следующей диаграмме показан основной рабочий процесс для пользователей при подключении [!INCLUDE[prodshort](includes/prodshort.md)] к Power BI.

![Рабочий поток Power BI для интеграции с Business Central](./media/power-bi-flow.png)

1. Пользователь регистрируется на учетную запись Power BI.
2. Пользователь подключается к Power BI из [!INCLUDE[prodshort](includes/prodshort.md)].
3. [!INCLUDE[prodshort](includes/prodshort.md)] проверяет лицензию.
4. [!INCLUDE[prodshort](includes/prodshort.md)] развертывает отчеты по умолчанию в службе Power BI. Этот шаг выполняется только для [!INCLUDE[prodshort](includes/prodshort.md)] Online.
5. [!INCLUDE[prodshort](includes/prodshort.md)] делает отчеты в Power BI доступными для выбора в [!INCLUDE[prodshort](includes/prodshort.md)]. Отчеты по умолчанию автоматически отображаются в частях Power BI.
6. Пользователь создает отчет в Power BI Desktop.
7. Пользователь публикует отчет в службе Power BI. Отчеты затем становятся доступными для выбора в [!INCLUDE[prodshort](includes/prodshort.md)].

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
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных Power BI](across-how-use-financials-data-source-powerbi.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных Power Apps](across-how-use-financials-data-source-powerapps.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в Power Automate](across-how-use-financials-data-source-flow.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
