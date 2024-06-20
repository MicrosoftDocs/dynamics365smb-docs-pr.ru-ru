---
title: Отслеживание КПЭ вашего бизнеса с помощью метрик Power BI
description: Обзор использования Power BI для получения аналитических сведений и КПЭ из данных Business Central.
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: overview
ms.search.keywords: 'account schedule, analysis, reporting, financial report, business intelligence, KPI'
ms.search.form: '6316, 6317'
ms.date: 04/24/2024
ms.custom: bap-template
ms.service: dynamics-365-business-central
---

# Отслеживание КПЭ вашего бизнеса с помощью метрик Power BI

Если вы используете Power BI для обработки данных [!INCLUDE[prod_short](includes/prod_short.md)], вы легко можете отслеживать важные для вас КПЭ или метрики.

С помощью метрик в Power BI вы можете создавать свои собственные метрики и отслеживать их в сравнении со своими ключевыми бизнес-целями на одной панели. Эта функция способствует выработке культуры данных, стимулируя ответственность, единообразие и прозрачность для команд и инициатив в организациях.

Настройка метрик Power BI предполагает четыре шага:

1. Создание системы показателей в Power BI. Подробнее см. в статье [Создание систем показателей в Power BI](/power-bi/create-reports/service-goals-create).  
2. Добавление метрик, которые вы хотите отслеживать, путем подключения к отчету Power BI по телеметрии. Подробнее см. в статье [Создание подключенных метрик](/power-bi/create-reports/service-goals-create-connected).  
3. Добавление оповещений (при необходимости) для определения правил статуса для используемых метрик. Подробнее см. в статье [Создание автоматических правил состояния для метрик](/power-bi/create-reports/service-metrics-status-rules).  

    Этот шаг позволяет автоматизировать обновления статуса на основе правил, относящихся к данной метрике. Правила инициируют изменения в зависимости от значения, процента достижения цели, условий по дате или комбинации этих трех факторов, что делает правила универсальными. Для подключенных метрик эти правила статуса обновляются каждый раз, когда обновляются данные в вашей системе показателей.
4. Следите за метриками, получая оповещения в Teams или по электронной почте. Подробнее см. в статье [Отслеживание метрик](/power-bi/create-reports/service-metrics-follow).  

Подробнее о метриках Power BI см. в статье [Начало работы с метриками в Power BI](/power-bi/create-reports/service-goals-introduction).

> [!NOTE]
> Начиная с волны 2 выпуска Business Central 2023 можно встраивать системы показателей из метрик Power BI в [!INCLUDE[prod_short](includes/prod_short.md)].

## См. также

[Использование ключевых показателей эффективности (КПЭ) для достижения бизнес-целей](analytics-about-kpis.md)  
[Знакомство с Business Central и Power BI](admin-powerbi.md)  
[Работа с отчетами Power BI](across-working-with-powerbi.md)  
[Обзор аналитики](reports-bi-reporting.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
