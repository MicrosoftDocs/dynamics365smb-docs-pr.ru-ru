---
title: Работа с данными Business Central в Power BI | Документация Майкрософт
description: Получение аналитических сведений, бизнес-аналитики и ключевых показателей эффективности из данных Business Central с помощью Power BI.
author: jswymer
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 67e564271e54c7c6c7f1b141172a537cd2bd6286
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "8510947"
---
# <a name="work-with-prod_short-data-in-power-bi"></a>Работа с данными [!INCLUDE [prod_short](includes/prod_short.md)] в Power BI

В этой статье вы узнаете некоторые основы работы с отчетами и панелями мониторинга в Power BI с использованием [!INCLUDE [prod_short](includes/prod_short.md)] как источника данных. В статье обсуждаются некоторые аспекты, которые помогут вам начать работу в качестве пользователя [!INCLUDE[prod_short](includes/prod_short.md)]. Общие рекомендации и инструкции по использованию Power BI см. в [документации для пользователей Power BI](/power-bi/consumer).

## <a name="get-ready"></a>Подготовка

Подпишитесь на службу Power BI. Если вы еще не зарегистрировались, перейдите на [https://powerbi.microsoft.com](https://powerbi.microsoft.com). При регистрации используйте рабочий адрес электронной почты и пароль.

## <a name="get-started"></a>Начало работы

Как только у вас будет учетная запись Power BI, вы можете войти в [https://powerbi.microsoft.com/](https://powerbi.microsoft.com/).

В службе Power BI размещаются все доступные вам отчеты. Чтобы просмотреть отчет, выберите **Моя рабочая область** > **Отчеты**. Затем просто выберите отчет, который хотите просмотреть.

С [!INCLUDE[prod_short](includes/prod_short.md)] Online вы автоматически получаете набор отчетов по умолчанию в вашей рабочей области. Если вы хотите создавать свои собственные отчеты, вы можете использовать Power BI Desktop для создания отчетов, а затем их публикации в вашей рабочей области. Дополнительные сведения см. в разделе [Приступая к созданию отчетов в Power BI Desktop для отображения данных [!INCLUDE [prod_long](includes/prod_long.md)]](across-how-use-financials-data-source-powerbi.md).

Если вы используете [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises, вам придется начать с нуля, используя Power BI Desktop. Дополнительно отчеты Power BI могут распространяться в виде файлов, которые вы можете отправлять.

## <a name="get-the-latest-data"></a>Получение новейших данных

Каждый отчет Power BI основан на наборе данных, который получает данные из источников [!INCLUDE[prod_short](includes/prod_short.md)]. Вы хотите убедиться, что данные в ваших отчетах Power BI актуальны относительно данных в [!INCLUDE[prod_short](includes/prod_short.md)]. Эта концепция называется *обновлением*.  В зависимости от того, как ваша организация настроила Power BI, обновление может не производиться автоматически. Есть два способа обновить данные: вручную или по расписанию. Ручное обновление выполняется по запросу по мере необходимости. Обновление по расписанию позволяет выполнять автоматическое обновление через определенные промежутки времени.

### <a name="refresh-manually"></a>Обновление вручную

На панели навигации в разделе **Наборы данных** выберите **Больше параметров (...)** рядом с набором данных, затем выберите **Обновить сейчас**.

### <a name="schedule-a-refresh"></a>Обновление по расписанию

На панели навигации в разделе "Наборы данных" выберите "Больше параметров (...)" рядом с набором данных, затем выберите **Запланировать обновление**. Заполните информацию в разделе **Запланировать обновление** и выберите **Применить**.

Дополнительные сведения см. в разделе [Настройка обновления по расписанию](/power-bi/connect-data/refresh-scheduled-refresh)

## <a name="upload-reports-from-files"></a><a name="upload"></a>Отправка отчетов из файлов

Отчеты Power BI можно распространять среди пользователей в виде файлов .pbix. Если у вас есть файл .pbix, вы можете отправить его в рабочую область. Чтобы отправить отчет, выполните следующие действия:

1. В новой рабочей области выберите **Получить данные**.

2. В поле "Файлы" выберите **Получить**.

3. Выберите **Локальный файл**, перейдите туда, где вы сохранили файл, и выберите **Открыть**.

Дополнительные сведения см. в разделе [Отправка отчета в службу](/power-bi/paginated-reports/paginated-reports-quickstart-aw#upload-the-report-to-the-service).

> [!NOTE]
> Для отправки отчета необходимо наличие рабочей области с [премиум-емкостью](/power-bi/service-premium-what-is). Дополнительные сведения см. в разделе [Управление премиум-емкостью](/power-bi/admin/service-premium-capacity-manage). 

> [!TIP]
> Если вы используете [!INCLUDE[prod_short](includes/prod_short.md)] Online, вы также можете отправить отчет из [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Работа с отчетами Power BI в [!INCLUDE [prod_short](includes/prod_short.md)] — отправка отчетов](across-working-with-powerbi.md#upload).

## <a name="share-reports-with-others"></a><a name="share"></a>Предоставление доступа к отчетам другим пользователям

Когда отчет появится в вашей рабочей области, вы можете поделиться им с другими в своей организации.

Чтобы поделиться отчетом, в списке отчетов или в открытом отчете выберите **Поделиться**. На панели **Поделиться отчетом** введите полные адреса электронной почты отдельных лиц или групп рассылки, с которыми вы хотите поделиться. Следуйте инструкциям на экране, чтобы завершить предоставление доступа. Дополнительные сведения см. в разделе [Предоставление доступа к панели мониторинга или отчету](/power-bi/collaborate-share/service-share-dashboards#share-a-dashboard-or-report).

> [!NOTE]
> Вы должны иметь [лицензию Power BI Pro](/power-bi/service-features-license-type), и люди, с которыми вы делитесь, тоже. Контент должен находиться в рабочей области с [премиум-емкостью](/power-bi/service-premium-what-is). Дополнительные сведения см. в разделе [Способы поделиться своей работой в Power BI](/power-bi/service-how-to-collaborate-distribute-dashboards-reports).

## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Business Central и Power BI](admin-powerbi.md)  
[Создание отчетов Power BI для отображения данных [!INCLUDE [prod_long](includes/prod_long.md)]](across-how-use-financials-data-source-powerbi.md)  
[Обзор компонентов и архитектуры интеграции Power BI для [!INCLUDE[prod_short](includes/prod_short.md)]](admin-powerbi-overview.md)  
[Работа с отчетами Power BI в [!INCLUDE [prod_short](includes/prod_short.md)]](across-working-with-powerbi.md)  
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