---
title: Часто задаваемые вопросы по Power BI
description: Получите ответы на некоторые типичные вопросы о работе с Power BI и Business Central.
author: jswymer
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'Power BI, reports, faq, errors'
ms.date: 04/22/2021
ms.author: jswymer
---
# <a name="power-bi--faq" />Часто задаваемые вопросы по Power BI

В этой статье даны ответы на некоторые вопросы, которые могут у вас возникнуть по работе с Power BI и [!INCLUDE [prod_short](includes/prod_short.md)].

## [Общие](#tab/general)
<!-- 26 -->
### <a name="ive-selected-a-report-for-my-role-center-in-business-central-if-i-later-make-changes-to-the-reports-visuals-online-will-the-role-center-automatically-update-to-my-changes" />Я выбрал отчет для своего ролевого центра в Business Central. Если позже я внесу изменения в визуальные элементы отчета в Интернете, будет ли центр ролей автоматически обновлен в соответствии с моими изменениями?

Да, потому что отчеты встроены из Power BI.

<!-- 3 -->
### <a name="are-the-business-central-apps-for-power-bi-available-in-languages-other-than-english" />Приложения Business Central для Power BI доступны на других языках, кроме английского?

Кол-во Эти приложения в настоящее время доступны только на английском языке.

<!-- 24 -->
### <a name="once-a-report-is-published-on-mypowerbicomworkspace-can-i-download-its-pbix" />После публикации отчета в моем рабочем пространстве powerbi.com могу ли я загрузить его PBIX?

Да. Для получения дополнительной информации см. [Загрузка отчета из службы Power BI в Power BI Desktop](/power-bi/create-reports/service-export-to-pbix).  

<!-- 27 -->
### <a name="can-i-download-the-apps-as-pbix-files" />Могу ли я загрузить приложения в виде файлов PBIX?

Кол-во В настоящее время нет возможности скачивать файлы PBIX для официальных приложений Power BI, потому что они опубликованы в AppSource.

## [Лицензия](#tab/license)

<!-- 14 -->
### <a name="do-i-need-a-power-bi-pro-license-to-publish-reports" />Нужна ли мне лицензия Power BI Pro для публикации отчетов?

<!-- todo What does " or for every user that consults the published report" mean? fixed -->
Кол-во Лицензия Pro не нужна для публикации отчетов. Стандартной (бесплатной лицензии) Power BI достаточно. Дополнительные сведения см. в разделе [Лицензирование Power BI](admin-powerbi-setup.md#license).

<!-- 15 -->
### <a name="is-there-anything-i-cant-do-with-the-free-license" />Что я не могу делать с бесплатной лицензией?

Вы не можете делиться отчетами или устанавливать приложения Business Central для Power BI. Помимо этого, бесплатная лицензия позволяет создавать практически все варианты диаграмм и отчетов.

<!-- 16 -->
### <a name="if-someone-shares-a-report-with-another-person-then-that-person-needs-a-pro-license-to-see-the-report-are-there-plans-to-make-this-capability-possible-with-the-free-license" />Если кто-то поделится отчетом с другим человеком, то ему потребуется лицензия Pro для просмотра отчета. Есть ли планы открыть эту возможность для бесплатной лицензии?

Мы не контролируем это требование. Это требование установлено в Power BI. Для получения дополнительной информации см. [Общий доступ к панелям мониторинга и отчетам Power BI для коллег и других](/power-bi/collaborate-share/service-share-dashboards).  

## [Конструктор](#tab/designer)

<!-- 7 -->
### <a name="does-the-connector-work-with-api-pages" />Соединитель работает со страницами API?

Да. Начиная с июня 2021 г. соединитель Power BI поддерживает как веб-службы Business Central, так и страницы API. Для получения дополнительной информации см. [Разрешить соединителю Power BI работать с API Business Central вместо работы только с веб-службами](/dynamics365-release-plan/2021wave1/smb/dynamics365-business-central/enable-power-bi-connector-work-business-central-apis-instead-web-services-only).

### <a name="can-i-build-a-power-bi-report-using-the-sales-invoice-lines-or-journal-lines-apis" />Могу ли я создать отчет Power BI с помощью API-интерфейсов строк счетов-фактур продажи или строк журнала?

Наиболее часто используемые записи строк доступны в [API Business Central v2.0](/dynamics365/business-central/dev-itpro/api-reference/v2.0/). Таким образом, вы можете использовать их для создания отчетов в Power BI, выбрав их в соединителе **Dynamics 365 Business Central**. Тем не менее API **Строки** предназначены для использования только с некоторыми очень специфическими фильтрами и могут не работать в вашем сценарии. Вы можете получить сообщение об ошибке, подобное «Вы должны указать код или код документа, чтобы получить строки». Чтобы решить эту проблему, выполните следующие действия при получении данных из Business Central для отчета в Power BI Desktop:

1. Вместо включения источника данных для сущности строк добавьте родительский источник данных. Например, добавьте **Счет-фактура продажи** вместо **Строки счета-фактуры продажи**.
2. Выберите **Преобразовать данные** на панели действий Power BI Desktop.
3. Выберите только что добавленный запрос, например **Счета-фактуры продажи**.
4. Примените любую необходимую фильтрацию к записям, чтобы уменьшить количество записей, загружаемых в отчет.
5. Прокрутите вправо, пока не найдете столбец, названный строками, например **SalesInvoiceLines**.
6. Нажмите кнопку «Развернуть» в заголовке столбца рядом с именем столбца.

   :::image type="content" source="media/saleinvoicelines.png" alt-text="Показывает столбец SalesInvoiceLines в Power BI Desktop.":::
<!-- 11 --> 
### <a name="is-it-possible-to-choose-which-business-central-environment-to-get-data-from-for-power-bi-for-example-like-a-sandbox-or-production-environment" />Можно ли выбрать, из какой среды Business Central получать данные для Power BI, например песочницы или рабочей среды?

Да. Можно легко выбрать. При подключении к Business Central с помощью соединителя необходимо выбрать среду и название компании.

<!-- 6 --> 
### <a name="can-i-merge-data-from-several-production-environments-of-the-same-tenant" />Могу ли я объединить данные из нескольких рабочих сред одного клиента?

Да. В Power BI просто запустите операцию получения данных еще раз и выберите нужную среду.

<!-- 25 -->
### <a name="which-pages-in-business-central-have-the-power-bi-report-part" />Для каких страниц в Business Central предусмотрена часть отчетов Power BI?

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
### <a name="is-there-any-way-to-filter-a-dataset-from-business-central-before-i-pull-it-into-power-bi-instead-of-applying-filters-afterwards" />Есть ли способ отфильтровать набор данных из Business Central *перед* его извлечением в Power BI вместо того, чтобы применять фильтры впоследствии?

Чтобы отфильтровать большие наборы данных, самый простой способ — установить фильтр в вашем отчете Power BI, изменив непосредственно формулу Power Query. Большинство фильтров, которые вы устанавливаете таким образом, будут переданы в Business Central через свертывание запросов. Си. [Пошаговое обновление для наборов данных](/power-bi/admin/service-premium-incremental-refresh).

В настоящее время нет возможности настроить фильтр для данных веб-службы из Business Central. Если вашему приложению необходимо установить фильтр из Business Central, вам нужно будет создать для этой цели собственное приложение Business Central.

<!-- 10 -->
### <a name="from-power-bi-besides-using-a-query-is-there-another-way-to-get-data-from-business-central-tables-that-dont-have-an-associated-page-for-example-like-the-item-attributes-value-mapping-table" />В Power BI, есть ли другой способ, помимо использования запроса, получить данные из таблиц Business Central, у которых нет связанной страницы? Например, как таблица *Сопоставление значений атрибута товара*.

Кол-во Не сейчас.

<!-- 12 --> 
### <a name="are-published-queries-faster-to-use-than-published-pages" />Опубликованные запросы работают быстрее, чем опубликованные страницы?

Когда дело доходит до веб-служб, опубликованные запросы обычно быстрее, чем аналогичные опубликованные страницы. Причина в том, что запросы оптимизированы для чтения данных и не содержат сложных триггеров, таких как OnAfterGetRecord.

Веб-службы основаны на страницах или запросах, созданных для доступа из Интернета и обычно не оптимизированных для доступа из внешних служб. Несмотря на то, что соединитель Business Central по-прежнему поддерживает получение данных из веб-служб, мы рекомендуем вам по возможности использовать страницы API вместо веб-служб.

<!-- 13 --> 
### <a name="is-there-a-way-for-an-end-user-to-create-a-web-service-with-a-column-thats-in-a-business-central-table-but-not-a-page-or-will-the-developer-have-to-create-a-custom-query" />Есть ли способ для конечного пользователя создать веб-службу со столбцом в таблице Business Central, но не на странице? Или разработчику придется создавать собственный запрос?

В настоящее время нет способа добавить новое поле в веб-службу. Страницы API обеспечивают полную гибкость структуры страницы, поэтому разработчик может создать новую страницу API, соответствующую этому требованию. 

<!-- 28 --> 
### <a name="can-i-connect-power-bi-to-a-read-only-database-server-of-business-central-online" />Могу ли я подключить Power BI к серверу баз данных с доступом только для чтения Business Central Online?

Эта функция будет доступна в ближайшее время. С февраля 2022 г. новые отчеты, которые вы создаете на основе данных Business Central Online, будут автоматически пытаться подключиться к реплике базы данных, доступной только для чтения. Это ускорит обновление ваших отчетов и окажет меньшее влияние на производительность, если вы используете Business Central во время обновления отчета. Мы по-прежнему рекомендуем, когда это возможно, планировать обновление отчетов на нерабочее время.

Если у вас есть старые отчеты, основанные на данных Business Central, они не будут подключаться к доступной только для чтения реплике базы данных.

### <a name="a-namedatabasemodsaive-tried-the-preview-of-the-new-connector-for-the-february--update-when-i-connect-to-my-custom-business-central-api-page-i-get-the-error-cannot-insert-a-record-current-connection-intent-is-read-only-how-can-i-fix-it" /><a name="databasemods"></a>Мы попробовали предварительную версию нового соединителя для обновления за февраль 2022 года. При подключении к своей настраиваемой странице API Business Central, я получаю сообщение об ошибке "Невозможно вставить запись. Назначение текущего подключения — только чтение". Как это исправить?

С новым соединителем новые отчеты, использующие данные Business Central, по умолчанию будут подключаться к доступной только для чтения реплике базы данных Business Central. Это изменение принесет улучшение производительности. Однако в редких случаях это может вызвать ошибку. Эта ошибка обычно возникает из-за того, что ваш пользовательский API вносит изменения в записи Business Central, пока Power BI пытается получить данные. В частности, это происходит при работе триггеров AL: OnInit, OnOpenPage, OnFindRecord, OnNextRecord, OnAfterGetRecord и OnAfterGetCurrRecord.

Чтобы устранить эту проблему, заставив соединитель Business Central разрешить такое поведение, см. [Создание отчетов Power BI для отображения данных Business Central — устранение проблем](across-how-use-financials-data-source-powerbi.md#fixing-problems).

<!--
In general, we recommend avoiding any database modifications in API pages when they're opening or loading records, because they cause performance issues and might cause your report refresh to fail. In some cases, you might still need to make a database modification when your custom API page opens or loads records. You can force the Business Central connector to allow this behavior. Do the following steps when getting data from Business Central for the report in Power BI Desktop:

1. Start Power BI Desktop.
2. In the ribbon, select **Get Data** > **Online Services**.
3. In the **Online Services** pane, select **Dynamics 365 Business Central**, then **Connect**.
4. In the **Navigator** window, select the API endpoint that you want to load data from.
5. In the preview pane on the right, you'll see the following error:

   *Dynamics365BusinessCentral: Request failed: The remote server returned an error: (400) Bad Request. (Cannot insert a record. Current connection intent is Read-Only. CorrelationId: [...])".*

6.  Select **Transform Data** instead of **Load** as you might normally do.
7. In **Power Query Editor**, select **Advanced Editor** from the ribbon.
8.  Replace the following line:

   ```
   Source = Dynamics365BusinessCentral.ApiContentsWithOptions(null, null, null, null),
   ```

   with the line:

   ```
   Source = Dynamics365BusinessCentral.ApiContentsWithOptions(null, null, null, [UseReadOnlyReplica = false]),
   ```

9.  Select **Done**.
10. Select **Close & Apply** from the ribbon to save the changes and close Power Query Editor.

-->
### <a name="a-namepermsahow-do-i-change-or-clear-the-user-account-im-currently-using-to-connect-to-business-central-from-power-bi-desktop" /><a name="perms"></a>Как изменить или удалить учетную запись пользователя, которую я сейчас использую для подключения к Business Central из Power BI Desktop?

В Power BI Desktop выполните один из следующих шагов:

1. В меню Файл выберите **Параметры и настройки** > **Параметры источника данных**.
2. Выберите **Dynamics Business Central** из списка, затем выберите **Удалить разрешения** > **Удалить**.

Затем, когда вы в следующий раз подключитесь к Business Central для получения данных, вам будет предложено войти в систему.

## [Производительность](#tab/performance)

<!-- 17 -->

### <a name="is-it-faster-to-get-data-using-api-pages-than-using-web-services" />Быстрее ли получать данные с помощью страниц API, чем с помощью веб-служб?

Да. Наши тесты показывают, что страницы API на 25% производительнее веб-служб.

<!-- 18 -->
### <a name="are-there-plans-to-have-a-mirror-on-the-azure-sql-database-instance-which-i-can-connect-to-directly" />Планируется ли установка зеркала в экземпляре базы данных SQL Azure, к которому я могу подключиться напрямую?

Кол-во Не сейчас. Вы можете обмениваться данными с Business Central только через API.

<!-- 19 -->
### <a name="loading-data-from-business-central-web-services-seems-slow-is-there-any-way-to-get-data-directly-from-the-sql-database-table" />Загрузка данных из веб-служб Business Central кажется медленной. Есть ли способ получить данные прямо из таблицы базы данных SQL?

Кол-во Прямой доступ к базе данных невозможен, но переключение на страницы API (когда будет доступен новый соединитель) очень поможет.

## [Дополнительно](#tab/advanced)
<!-- 1 -->

### <a name="are-there-plans-for-the-power-bi-connector-to-support-the-incremental-refresh-features-in-the-power-bi-service" />Есть ли планы, чтоб соединитель Power BI поддерживал функции пошагового обновления в службе Power BI?

Да. Это в нашей дорожной карте.

<!-- 2 -->
### <a name="if-a-business-central-on-premises-solution-doesnt-have-internet-access-can-i-still-use-power-bi" />Если в локальном решении Business Central нет доступа в Интернет, могу ли я использовать Power BI?
<!-- todo: please explain this one-->

Да. В этом случае вы используете Power BI Desktop локально и подключаетесь к Business Central локально. После подключения вы можете создавать и просматривать отчеты, но вы просто не можете публиковать их в службе Power BI. 
<!-- 20 -->
### <a name="are-there-any-plans-to-make-it-possible-to-replicate-business-central-online-databases-so-theyre-accessible-for-read-only-sql-queries-this-capability-would-support-incremental-refresh-and-be-a-lot-faster-than-apis-or-web-services" />Есть ли планы сделать возможным репликацию баз данных Business Central Online, чтобы они были доступны для запросов SQL только для чтения? Эта возможность будет поддерживать пошаговое обновление и будет намного быстрее, чем API или веб-службы.

<!-- todo: what does "BC-Saas-DB-replicated DB accessible" mean? fixe-->
Да. У нас есть эта функция в нашей долгосрочной дорожной карте. 

<!-- 21 -->
### <a name="if-i-use-azure-data-factory-to-get-data-from-business-central-and-consume-it-on-power-bi-will-that-help-in-increase-in-performance" />Если я использую фабрику данных Azure для получения данных из Business Central и использования их в Power BI, это поможет повысить производительность?

Да. Этот расширенный сценарий поможет Business Central оставаться производительным, поскольку доступ к данным будет осуществляться через фабрику данных Azure.

<!-- 22 -->
### <a name="are-there-any-plans-to-support-power-bi-deployment-pipelines-or-a-way-to-build-deployment-pipelines-for-pbi-reports-similar-to-extensions-or-maybe-even-a-simple-api-in-the-business-admin-center" />Есть ли планы по поддержке конвейеров развертывания Power BI или способа создания конвейеров развертывания для отчетов PBI, похожих на расширения? Или, может быть, даже простой API в Business Admin Center?

Мы изучаем эту функцию. Power BI предлагает мощные API-интерфейсы для управления развертыванием отчетов. Для получения дополнительной информации см. [Общие сведения о конвейерах развертывания](/power-bi/create-reports/deployment-pipelines-overview).

### <a name="when-i-get-data-from-business-central-to-use-in-my-power-bi-reports-i-see-some-values-like-x-what-are-these-values" />Когда я получаю данные из Business Central для использования в моих отчетах Power BI, я вижу некоторые значения, такие как "_х0020_". Что это за значения?

На некоторых страницах API, включая большинство страниц API версии 2.0, есть поля, основанные на [объектах AL Enum](/dynamics365/business-central/dev-itpro/developer/devenv-extensible-enums). Поля, основанные на объектах AL Enum, должны иметь согласованные и всегда одинаковые имена, чтобы фильтры в отчете всегда работали &mdash; независимо от того, какой язык или операционную систему вы используете. По этой причине поля, основанные на перечислениях AL Enum, не переводятся и кодируются, чтобы избежать использования специальных символов, включая пробел. В частности, всякий раз, когда в объекте AL Enum есть пустой параметр, он кодируется как "_x0020_". Вы всегда можете применить преобразование к своим данным в Power BI, если вы хотите отобразить другое значение для этих полей, например "Пусто".


---

## <a name="see-related-microsoft-trainingtrainingmoduleschange-documents-dynamics--business-central" />См. соответствующее [обучение Microsoft](/training/modules/change-documents-dynamics-365-business-central/)

## <a name="see-also" />См. также

[Лицензирование Power BI](admin-powerbi-setup.md#license)  
[Введение в Business Central и Power BI](admin-powerbi.md)  
[Обзор интеграции Power BI](admin-powerbi-overview.md)  
[Включение Power BI в Business Central](admin-powerbi-setup.md)  
[Работа с отчетами Power BI в Business Central](across-working-with-powerbi.md)  
[Работа с данными Business Central в Power BI](across-working-with-business-central-in-powerbi.md)  
[Создание отчетов Power BI для отображения данных Business Central](across-how-use-financials-data-source-powerbi.md)  
[Документация Power BI](/power-bi/)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
