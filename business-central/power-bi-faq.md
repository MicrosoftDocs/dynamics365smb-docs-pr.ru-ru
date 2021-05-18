---
title: Часто задаваемые вопросы по Power BI
description: Получите ответы на некоторые типичные вопросы о работе с Power BI и Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Power BI, reports, faq, errors
ms.date: 04/22/2021
ms.author: jswymer
ms.openlocfilehash: 939b280e631113d3196f6fbbc90d9bf19b9fc408
ms.sourcegitcommit: a76475f124e79440a5bba20577b335c4d50a2d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2021
ms.locfileid: "6025837"
---
# <a name="power-bi--faq"></a>Часто задаваемые вопросы по Power BI

В этой статье даны ответы на некоторые вопросы, которые могут у вас возникнуть по работе с Power BI и [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="general"></a>[Общие](#tab/general)
<!-- 26 -->
### <a name="ive-selected-a-report-for-my-role-center-in-business-central-if-i-later-make-changes-to-the-reports-visuals-online-will-the-role-center-automatically-update-to-my-changes"></a>Я выбрал отчет для своего ролевого центра в Business Central. Если позже я внесу изменения в визуальные элементы отчета в Интернете, будет ли центр ролей автоматически обновлен в соответствии с моими изменениями?

Да, потому что отчеты встроены из Power BI.

<!-- 3 -->
### <a name="are-the-business-central-apps-for-power-bi-available-in-languages-other-than-english"></a>Приложения Business Central для Power BI доступны на других языках, кроме английского?

Кол-во Эти приложения в настоящее время доступны только на английском языке.

<!-- 24 -->
### <a name="once-a-report-is-published-on-mypowerbicomworkspace-can-i-download-its-pbix"></a>После публикации отчета в моем рабочем пространстве powerbi.com могу ли я загрузить его PBIX? 

Да. Для получения дополнительной информации см. [Загрузка отчета из службы Power BI в Power BI Desktop](/power-bi/create-reports/service-export-to-pbix).  

<!-- 27 -->
### <a name="can-i-download-the-apps-as-pbix-files"></a>Могу ли я загрузить приложения в виде файлов PBIX? 

Кол-во В настоящее время нет возможности скачивать файлы PBIX для официальных приложений Power BI, потому что они опубликованы в AppSource.

## <a name="license"></a>[Лицензия](#tab/license)

<!-- 14 -->
### <a name="do-i-need-a-power-bi-pro-license-to-publish-reports"></a>Нужна ли мне лицензия Power BI Pro для публикации отчетов? 

<!-- todo What does " or for every user that consults the published report" mean? fixed -->
Кол-во Лицензия Pro не нужна для публикации отчетов. Стандартной (бесплатной лицензии) Power BI достаточно. Дополнительные сведения см. в разделе [Лицензирование Power BI](admin-powerbi-setup.md#license).

<!-- 15 -->
### <a name="is-there-anything-i-cant-do-with-the-free-license"></a>Что я не могу делать с бесплатной лицензией?

Вы не можете делиться отчетами или устанавливать приложения Business Central для Power BI. Помимо этого, бесплатная лицензия позволяет создавать практически все варианты диаграмм и отчетов.

<!-- 16 -->
### <a name="if-someone-shares-a-report-with-another-person-then-that-person-needs-a-pro-license-to-see-the-report-are-there-plans-to-make-this-capability-possible-with-the-free-license"></a>Если кто-то поделится отчетом с другим человеком, то ему потребуется лицензия Pro для просмотра отчета. Есть ли планы открыть эту возможность для бесплатной лицензии?

Мы не контролируем это требование. Это требование установлено в Power BI. Для получения дополнительной информации см. [Общий доступ к панелям мониторинга и отчетам Power BI для коллег и других](/power-bi/collaborate-share/service-share-dashboards).  

## <a name="designer"></a>[Конструктор](#tab/designer)

<!-- 7 -->
### <a name="does-the-connector-work-with-api-pages"></a>Соединитель работает со страницами API?

Пока нет. Но начиная с июня 2021 г. соединитель Power BI будет поддерживать как веб-службы Business Central, так и страницы API. Для получения дополнительной информации см. [Разрешить соединителю Power BI работать с API Business Central вместо работы только с веб-службами](/dynamics365-release-plan/2021wave1/smb/dynamics365-business-central/enable-power-bi-connector-work-business-central-apis-instead-web-services-only).

<!-- 11 --> 
### <a name="is-it-possible-to-choose-which-business-central-environment-to-get-data-from-for-power-bi-for-example-like-a-sandbox-or-production-environment"></a>Можно ли выбрать, из какой среды Business Central получать данные для Power BI, например песочницы или рабочей среды? 

Да. Можно легко выбрать. При подключении к Business Central с помощью соединителя необходимо выбрать среду и название компании.

<!-- 6 --> 
### <a name="can-i-merge-data-from-several-production-environments-of-the-same-tenant"></a>Могу ли я объединить данные из нескольких рабочих сред одного клиента?

Да. В Power BI просто запустите операцию получения данных еще раз и выберите нужную среду.

<!-- 25 -->
### <a name="which-pages-in-business-central-have-the-power-bi-report-part"></a>Для каких страниц в Business Central предусмотрена часть отчетов Power BI?  

В настоящее время есть несколько выбранных страниц, на которых есть информационное поле с областью **Отчеты Power BI** для отображения отчета. 

На страницах списков область **Отчеты Power BI** фильтруется для отображения отчетов, относящихся к данным в списке. Вот страницы типа списка, которые содержат область **Отчеты Power BI**:

|ИД страницы|Name|
|-------|----|
|22|Список клиентов|
|27|Список поставщиков|
|31|Список товаров|
|9305|Список заказов на продажу|
|9308|Счета покупки|

Вот другие страницы, которые содержат более крупную, не отфильтрованную область **Отчеты Power BI**:

|ИД страницы|Name|
|-------|----|
|1156|Сведения о компании|
|4013|Аналитика в интеллектуальном облаке |
|9006|Ролевой центр обработчика заказов|
|9008|Склад Базовый ролевой центр|
|9010|Ролевой центр планировщика производства|
|9015|Ролевой центр руководителя проекта задания|
|9016|Ролевой центр диспетчера по сервису|
|9022|Ролевой центр "Бизнес-руководитель"|
|9024|Ролевой центр "Администратор безопасности"|
|9026|Руководитель по продажам и взаимодействию Ролевой центр|
|9027|Ролевой центр бухгалтера|

> [!TIP]
> В настоящее время мы не планируем добавлять его на все страницы списков. Однако вы можете создать простое расширение страницы, которое добавляет область **Отчеты Power BI** на информационную панель. Дополнительные сведения см. в [Добавление областей отчетов Power BI на страницы](/dynamics365/business-central/dev-itpro/developer/devenv-power-bi-report-parts) в справке для разработчиков и ИТ-специалистов.

<!-- 5 -->
### <a name="is-there-any-way-to-filter-a-dataset-from-business-central-before-i-pull-it-into-power-bi-instead-of-applying-filters-afterwards"></a>Есть ли способ отфильтровать набор данных из Business Central *перед* его извлечением в Power BI вместо того, чтобы применять фильтры впоследствии?

Чтобы отфильтровать большие наборы данных, самый простой способ — установить фильтр в вашем отчете Power BI, изменив непосредственно формулу Power Query. Большинство фильтров, которые вы устанавливаете таким образом, будут переданы в Business Central через свертывание запросов. Си. [Пошаговое обновление для наборов данных](/power-bi/admin/service-premium-incremental-refresh).

В настоящее время нет возможности настроить фильтр для данных веб-службы из Business Central. Если вашему приложению необходимо установить фильтр из Business Central, вам нужно будет создать для этой цели собственное приложение Business Central.

<!-- 8 and 9 -->

### <a name="for-embedding-reports-in-business-central-pages-right-now-its-only-possible-to-get-reports-from-my-workspace-in-power-bi-are-there-plans-to-make-it-possible-to-get-them-from-custom-workspaces"></a>Для встраивания отчетов на страницы Business Central прямо сейчас можно получить отчеты только из *Моя рабочая область* в Power BI. Есть ли планы сделать возможным их получение из настраиваемых рабочих пространств?

Да. В наших планах добавить поддержку общих рабочих пространств, но у нас пока нет графика выпуска, который мы можем вам сообщить.  

<!-- 10 -->
### <a name="from-power-bi-besides-using-a-query-is-there-another-way-to-get-data-from-business-central-tables-that-dont-have-an-associated-page-for-example-like-the-item-attributes-value-mapping-table"></a>В Power BI, есть ли другой способ, помимо использования запроса, получить данные из таблиц Business Central, у которых нет связанной страницы? Например, как таблица *Сопоставление значений атрибута товара*.

Кол-во Не сейчас.

<!-- 12 --> 
### <a name="are-published-queries-faster-to-use-than-published-pages"></a>Опубликованные запросы работают быстрее, чем опубликованные страницы?

Когда дело доходит до веб-служб, опубликованные запросы обычно быстрее, чем аналогичные опубликованные страницы. Причина в том, что запросы оптимизированы для чтения данных и не содержат сложных триггеров, таких как OnAfterGetRecord.

Когда новый соединитель будет доступен в июне 2021 года, вам будет предложено использовать страницы API вместо запросов, опубликованных в виде веб-служб.

<!-- 13 --> 
### <a name="is-there-a-way-for-an-end-user-to-create-a-web-service-with-a-column-thats-in-a-business-central-table-but-not-a-page-or-will-developer-have-to-create-a-custom-query"></a>Есть ли способ для конечного пользователя создать веб-службу со столбцом в таблице Business Central, но не на странице? Или разработчику придется создавать собственный запрос? 

Пока нет. Но когда новый соединитель будет доступен в июне 2021 года, разработчик может создать новую страницу API для удовлетворения этого требования. 

<!-- 28 --> 
### <a name="can-i-connect-power-bi-to-a-read-only-database-server-of-business-central-online"></a>Могу ли я подключить Power BI к серверу баз данных с доступом только для чтения Business Central Online? 

Кол-во Но у нас есть эта функция в нашей долгосрочной дорожной карте. 

## <a name="performance"></a>[Производительность](#tab/performance)

<!-- 17 -->

### <a name="is-it-faster-to-get-data-using-api-pages-than-using-web-services"></a>Быстрее ли получать данные с помощью страниц API, чем с помощью веб-служб?

Да. Наши тесты показывают, что страницы API на 25% производительнее веб-служб.

<!-- 18 -->
### <a name="are-there-plans-to-have-a-mirror-on-the-azure-sql-database-instance-which-i-can-connect-to-directly"></a>Планируется ли установка зеркала в экземпляре базы данных SQL Azure, к которому я могу подключиться напрямую?

Кол-во Не сейчас. Вы можете обмениваться данными с Business Central только через API.

<!-- 19 -->
### <a name="loading-data-from-business-central-web-services-seems-slow-is-there-any-way-to-get-data-directly-from-the-sql-database-table"></a>Загрузка данных из веб-служб Business Central кажется медленной. Есть ли способ получить данные прямо из таблицы базы данных SQL?

Кол-во Прямой доступ к базе данных невозможен, но переключение на страницы API (когда будет доступен новый соединитель) очень поможет.

## <a name="advanced"></a>[Дополнительно](#tab/advanced)
<!-- 1 -->

### <a name="are-there-plans-for-the-power-bi-connector-to-support-the-incremental-refresh-features-in-the-power-bi-service"></a>Есть ли планы, чтоб соединитель Power BI поддерживал функции пошагового обновления в службе Power BI?

Да. Это в нашей дорожной карте.

<!-- 2 -->
### <a name="if-a-business-central-on-premises-solution-doesnt-have-internet-access-can-i-still-use-power-bi"></a>Если в локальном решении Business Central нет доступа в Интернет, могу ли я использовать Power BI?
<!-- todo: please explain this one-->

Да. В этом случае вы используете Power BI Desktop локально и подключаетесь к Business Central локально. После подключения вы можете создавать и просматривать отчеты, но вы просто не можете публиковать их в службе Power BI. 
<!-- 20 -->
### <a name="are-there-any-plans-to-make-it-possible-to-replicate-business-central-online-databases-so-theyre-accessible-for-read-only-sql-queries-this-capability-would-support-incremental-refresh-and-be-a-lot-faster-than-apis-or-web-services"></a>Есть ли планы сделать возможным репликацию баз данных Business Central Online, чтобы они были доступны для запросов SQL только для чтения? Эта возможность будет поддерживать пошаговое обновление и будет намного быстрее, чем API или веб-службы.

<!-- todo: what does "BC-Saas-DB-replicated DB accessible" mean? fixe-->
Да. У нас есть эта функция в нашей долгосрочной дорожной карте. 

<!-- 21 -->
### <a name="if-i-use-azure-data-factory-to-get-data-from-business-central-and-consume-it-on-power-bi-will-that-help-in-increase-in-performance"></a>Если я использую фабрику данных Azure для получения данных из Business Central и использования их в Power BI, это поможет повысить производительность? 

Да. Этот расширенный сценарий поможет Business Central оставаться производительным, поскольку доступ к данным будет осуществляться через фабрику данных Azure.

<!-- 22 -->
### <a name="are-there-any-plans-to-support-power-bi-deployment-pipelines-or-a-way-to-build-deployment-pipelines-for-pbi-reports-similar-to-extensions-or-maybe-even-a-simple-api-in-the-business-admin-center"></a>Есть ли планы по поддержке конвейеров развертывания Power BI или способа создания конвейеров развертывания для отчетов PBI, похожих на расширения? Или, может быть, даже простой API в Business Admin Center? 

Мы изучаем эту функцию. Power BI предлагает мощные API-интерфейсы для управления развертыванием отчетов. Для получения дополнительной информации см. [Общие сведения о конвейерах развертывания](/power-bi/create-reports/deployment-pipelines-overview).

### <a name="ive-tried-the-preview-of-the-new-connector-which-will-be-live-in-june-2021-i-see-some-values-like-_x0020_-when-connecting-to-api-v20-what-are-these-values"></a>Я попробовал предварительную версию нового соединителя, который будет доступен в июне 2021 года. Я вижу такие значения, как "_x0020_" при подключении к API v2.0. Что это за значения?

Предстоящая версия соединителя Power BI позволяет подключаться к страницам API Business Central, включая API v2.0. Эти страницы включают несколько полей на основе [объектов AL Enum](/dynamics365/business-central/dev-itpro/developer/devenv-extensible-enums). Поля, основанные на объектах AL Enum, должны иметь согласованные и всегда одинаковые имена, чтобы фильтры в отчете всегда работали &mdash; независимо от того, какой язык или операционную систему вы используете. По этой причине поля, основанные на перечислениях AL Enum, не переводятся и кодируются, чтобы избежать использования специальных символов, включая пробел. В частности, всякий раз, когда в объекте AL Enum есть пустой параметр, он кодируется как "_x0020_". Вы всегда можете применить преобразование к своим данным в Power BI, если вы хотите отобразить другое значение для этих полей, например "Пусто".


---

## <a name="see-also"></a>См. также

[Общие сведения о лицензировании Power BI](admin-powerbi-setup.md#license)
[Business Central и Power BI](admin-powerbi.md)  
[Обзор интеграции Power BI](admin-powerbi-overview.md)  
[Включение Power BI в Business Central](admin-powerbi-setup.md)  
[Работа с отчетами Power BI в Business Central](across-working-with-powerbi.md)  
[Работа с данными Business Central в Power BI](across-working-with-business-central-in-powerbi.md)  
[Создание отчетов Power BI для отображения данных Business Central](across-how-use-financials-data-source-powerbi.md)    
[Документация Power BI](/power-bi/)  


[!INCLUDE[footer-include](includes/footer-banner.md)]