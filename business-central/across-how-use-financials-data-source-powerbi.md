---
title: Создание отчетов в Power BI Desktop для отображения данных Business Central
description: Можно сделать данные доступными в качестве источника данных в Power BI и создать мощные отчеты о состоянии вашего бизнеса.
author: jswymer
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'business intelligence, KPI, Odata, Power App, SOAP, analysis'
ms.date: 06/12/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---

# <a name="building-power-bi-reports-to-display--data"></a>Создание отчетов Power BI для отображения данных [!INCLUDE [prod_long](includes/prod_long.md)]

Вы можете сделать свои данные [!INCLUDE[prod_long](includes/prod_long.md)] доступными в качестве источника данных в Power BI Desktop и создавать мощные отчеты о состоянии вашего бизнеса.

В этой статье рассказывается, как начать использовать Power BI Desktop для создания отчетов, отображающих данные [!INCLUDE[prod_long](includes/prod_long.md)]. После создания отчетов вы можете опубликовать их в своей службе Power BI или поделиться ими со всеми пользователями в вашей организации. Как только эти отчеты будут в службе Power BI, пользователи, которые имеют к ней доступ, смогут просматривать отчеты в [!INCLUDE[prod_long](includes/prod_long.md)].

## <a name="get-ready"></a>Подготовка

- Подпишитесь на службу Power BI.

  Если вы еще не зарегистрировались, перейдите на [https://powerbi.microsoft.com](https://powerbi.microsoft.com). При регистрации используйте рабочий адрес электронной почты и пароль.

- Скачайте [Power BI Desktop](https://powerbi.microsoft.com/desktop/).

  Power BI Desktop — это бесплатное приложение, которое вы устанавливаете на свой локальный компьютер. Для получения дополнительной информации см. раздел [Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data),

- Убедитесь, что данные, которые вы хотите включить в отчет, доступны как страница API или опубликованы в виде веб-службы. Для получения дополнительной информации прочитайте [Предоставлять данные через страницы API или веб-службы OData](admin-powerbi-setup.md#exposedata).

<!--- For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, get the following information:

  - The OData URL for [!INCLUDE[prod_short](includes/prod_short.md)].
  
    Typically, this URL has the format `http[s]://[computer]:[port]/[serverinstance]/ODataV4`, for example, `https://localhost:7048/BC190/ODataV4`. If you have a multi-tenant deployment, include the tenant in the URL, for example, `https://localhost:7048/BC190/ODataV4?tenant=tenant1`.
  - A user name and web service access key of a [!INCLUDE[prod_short](includes/prod_short.md)] account.

    To get data from [!INCLUDE[prod_short](includes/prod_short.md)], Power BI uses basic authentication. So, you'll need a user name and web service access key to connect. The account might be your own user account, or your organization may have specific account for this purpose.-->

- Загрузите тему отчета [!INCLUDE [prod_short](includes/prod_short.md)] (необязательно).

  Дополнительные сведения см. в разделе [Использование темы отчета [!INCLUDE [prod_short](includes/prod_short.md)]](#theme) в этой статье.

[!INCLUDE[note-multicompany-reports](includes/note-multicompany-reports.md)]

## <a name="add--as-a-data-source-in-power-bi-desktop"></a><a name="getdata"></a>Добавление [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных в Power BI Desktop

Первая задача при создании отчетов — добавить [!INCLUDE[prod_short](includes/prod_short.md)] как источник данных в Power BI Desktop. После подключения вы можете приступить к созданию отчета.

1. Запустите Power BI Desktop.
2. Выберите **Получить данные**.

    Если вы не видите пункт **Получить данные**, выберите меню **Файл**, затем **Получить данные**.
3. На странице **Получить данные** выберите **Веб-службы**.
4. В области **Веб-службы** выполните одно из следующих действий:

    - Чтобы подключиться к [!INCLUDE [prod_short](includes/prod_short.md)] онлайн, выберите **Dynamics 365 Business Central**, затем **Подключить**.
    <!--- To connect to  [!INCLUDE [prod_short](includes/prod_short.md)] on-premises, select **Dynamics 365 Business Central (on-premises)**, then **Connect**.-->

5. Войдите в [!INCLUDE [prod_short](includes/prod_short.md)] (только один раз).

    Если вы еще не вошли в [!INCLUDE [prod_short](includes/prod_short.md)] из Power BI Desktop, вам будет предложено войти в систему.

    - Для сетевой версии [!INCLUDE [prod_short](includes/prod_short.md)] выберите **Войти**, затем выберите соответствующую учетную запись. Используйте ту же учетную запись, которая используется для входа в [!INCLUDE [prod_short](includes/prod_short.md)]. Когда готово, выберите **Подключить**.

    <!--- For [!INCLUDE [prod_short](includes/prod_short.md)] on-premises, first enter the OData URL for [!INCLUDE[prod_short](includes/prod_short.md)], then select **OK**. When prompted, enter the user name and password of the account to use for connecting to [!INCLUDE[prod_short](includes/prod_short.md)]. In the **Password** box, enter the web service access key. When done, select **Connect**.-->

    > [!NOTE]  
    > После подключения к [!INCLUDE[prod_short](includes/prod_short.md)] входить в систему больше будет не нужно. [Как изменить или удалить учетную запись, которую я сейчас использую для подключения к Business Central из Power BI Desktop?](/dynamics365/business-central/power-bi-faq?tabs=designer#perms)

6. После подключения Power BI связывается со службой [!INCLUDE [prod_short](includes/prod_short.md)]. Появляется окно **Навигатор**, в котором отображаются доступные источники данных для построения отчетов. Выберите какую-либо папку, чтобы развернуть ее и просмотреть доступные источники данных.

   Эти источники данных представляют все веб-службы и страницы API, которые опубликованы для [!INCLUDE [prod_short](includes/prod_short.md)], сгруппированные по средам и организациям. С [!INCLUDE [prod_short](includes/prod_short.md)] Online окно **Навигатор** имеет следующую структуру:

    - **Имя среды**
      - **Название организации**
        - **Расширенные API**

          В этой папке перечислены расширенные страницы API, опубликованные Microsoft, например [API автоматизации Business Central](/dynamics365/business-central/dev-itpro/administration/itpro-introduction-to-automation-apis) и [Настраиваемые страницы API для Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-develop-custom-api). Страницы пользовательских API далее сгруппированы по папкам по свойствам [APIPublisher](/dynamics365/business-central/dev-itpro/developer/properties/devenv-apipublisher-property)/[APIGroup](/dynamics365/business-central/dev-itpro/developer/properties/devenv-apigroup-property) исходного кода страницы API.

        - **Стандартные API v2.0**

          В этой папке перечислены страницы API, представленные [Business Central API V2.0](/dynamics365/business-central/dev-itpro/api-reference/v2.0/).

        - **Веб-службы \(устаревшие версии)**

          В этой папке перечислены страницы, модули codeunit и запросы, опубликованные как веб-службы в Business Central.

    <!--
    > [!NOTE]
    > The structure for Business Central on-premises is different because it doesn't support API pages.-->

7. Выберите источник данных или источники, которые требуется добавить в модель данных, а затем нажмите кнопку **Загрузить**.
8. Если позже вы захотите добавить дополнительные данные Business Central, вы можете повторить предыдущие шаги.

После загрузки данных они отображаются в правой области навигации на странице. На этом шаге вы успешно подключились к данным [!INCLUDE[prod_short](includes/prod_short.md)] и можете приступать к созданию отчета Power BI.  

> [!TIP]
> Дополнительные сведения об использовании Power BI Desktop см. в разделе [Приступая к работе с Power BI Desktop](/power-bi/fundamentals/desktop-getting-started).

## <a name="creating-accessible-reports"></a>Создание доступных отчетов

Важно, чтобы ваши отчеты были доступны как можно большему количеству людей. Постарайтесь создавать отчеты так, чтобы они не требовали специальной адаптации для удовлетворения конкретных потребностей разных пользователей. Убедитесь, что дизайн позволяет пользователям использовать стандартные технологии специальных возможностей, например программы чтения с экрана. Power BI включает различные специальные возможности, инструменты и рекомендации, которые помогут вам в достижении этой цели. Для дополнительной информации см. [Разработка отчетов Power BI с учетом специальных возможностей](/power-bi/create-reports/desktop-accessibility-creating-reports) в документации Power BI.

## <a name="creating-reports-to-display-data-associated-with-a-list"></a>Создание отчетов для отображения данных, связанных со списком

Вы можете создавать отчеты, которые отображаются на информационной панели страницы списка [!INCLUDE [prod_short](includes/prod_short.md)]. Отчеты могут содержать данные о записи, выбранной в списке. Создание этих отчетов аналогично созданию других отчетов, за исключением того, что нужно выполнить определенные действия, чтобы убедиться, что отчеты отображаются должным образом. Для получения дополнительной информации см. раздел [Создание отчетов Power BI для отображения данных списка в [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-powerbi-reports-factbox.md).

## <a name="using-the--report-theme-optional"></a><a name="theme"></a>Использование темы отчетов [!INCLUDE [prod_short](includes/prod_short.md)] (необязательно)

Перед построением отчета рекомендуется скачать и импортировать файл темы [!INCLUDE [prod_short](includes/prod_short.md)]. Файл темы создает цветовую палитру, чтобы можно было создавать отчеты с таким же цветовым стилем, что и приложения [!INCLUDE [prod_short](includes/prod_short.md)] без необходимости определения настраиваемых цветов для каждого визуального элемента.

> [!NOTE]
> Эта задача является необязательной. Вы всегда можете создать свои отчеты, затем скачать и применить шаблон стиля позже.

### <a name="download-the-theme"></a>Скачивание темы

Файл темы доступен как файл json в коллекции тем сообщества Microsoft Power BI. Чтобы скачать файл темы, выполните следующие действия:

1. Перейдите в [Коллекцию тем сообщества Microsoft Power BI для Microsoft Dynamics 365 Business Central](https://community.powerbi.com/t5/Themes-Gallery/Microsoft-Dynamics-365-Business-Central/m-p/385875).
2. Выберите скачивание вложения **Microsoft Dynamics Business Central.json**.

### <a name="import-the-theme-on-a-report"></a>Импорт темы в отчет

Загрузив тему отчета [!INCLUDE [prod_short](includes/prod_short.md)], вы сможете импортировать ее в свои отчеты. Чтобы импортировать тему, выберите **Представление** > **Темы** > **Поиск тем**. Дополнительные сведения см. в разделе [Power BI Desktop — импорт пользовательских тем отчетов](/power-bi/create-reports/desktop-report-themes#import-custom-report-theme-files).

## <a name="publish-reports"></a>Публикация отчетов

После того как вы создали или изменили отчет, вы можете опубликовать его в своей службе Power BI, а также передать его другим пользователям в своей организации. После публикации отчет становится доступен в Power BI. Отчет также становится доступным для выбора в [!INCLUDE[prod_short](includes/prod_short.md)].

Чтобы опубликовать отчет, выберите **Опубликовать** на вкладке **Главная** на ленте или из меню **файл**. Если вы вошли в службу Power BI, отчет публикуется в этой службе. В противном случае вам будет предложено войти в систему. 

## <a name="distribute-or-share-a-report"></a>Распространение отчета или предоставление доступа к нему

Есть несколько способов отправить отчеты своим коллегам и другим людям:

- Распространяйте отчеты в виде файлов .pbix.

    Отчеты хранятся на вашем компьютере в виде файлов .pbix. Вы можете распространять файл отчета .pbix среди пользователей, как и любой другой файл. Затем пользователи могут отправить этот файл в свою службу Power BI. См. раздел [Отправить отчеты из файлов](across-working-with-powerbi.md#upload).

    > [!NOTE]
    > Распространение отчетов таким образом означает, что обновление данных для отчетов будет выполняться каждым пользователем индивидуально. Эта ситуация может повлиять на производительность [!INCLUDE[prod_short](includes/prod_short.md)].

- Предоставление доступа к отчету из вашей службы Power BI

    Если у вас есть лицензия Power BI Pro, вы можете поделиться отчетом с другими прямо из своей службы Power BI. Дополнительные сведения см. в разделе [Power BI — предоставление доступа к панели мониторинга или отчету](/power-bi/collaborate-share/service-share-dashboards#share-a-dashboard-or-report).

## <a name="how-to-develop-cross-company-or-cross-environment-power-bi-reports"></a>Как разрабатывать отчеты Power BI, охватывающие несколько организаций или сред

Конечные точки API [!INCLUDE[prod_short](includes/prod_short.md)] имеют префикс `https://api.businesscentral.dynamics.com/v2.0/<environment_name>/api/v2.0`, после которого идет `/companies({company_id})/accounts({id})` (здесь мы используем API `accounts` в качестве иллюстрации). Вы можете использовать эту структуру для создания запросов PowerQuery, которые загружают данные для нескольких организаций или нескольких сред, если у пользователя, читающего данные, есть к ним доступ.

Чтобы создать запрос для загрузки данных для нескольких организаций, выполните следующие действия:

1. Возьмите запрос PowerQuery, который загружает данные для одной организации. Преобразуйте его в пользовательскую функцию Power Query, которая принимает идентификатор организации (или, возможно, имя среды) в качестве параметров. Подробнее см. в статье [Использование пользовательских функций Power Query](/power-query/custom-function).
1. Теперь используйте эту новую пользовательскую функцию в запросе PowerQuery, где вам нужно будет сопоставить эту функцию со списком компаний, а затем объединить наборы данных с помощью функции Power Query [Table.Combine](/powerquery-m/table-combine).

## <a name="fixing-problems"></a>Устранение проблем

### <a name="cant-insert-a-record-current-connection-intent-is-read-only-error-connecting-to-custom-api-page"></a>«Невозможно вставить запись. Назначение текущего подключения — только чтение". ошибка при подключении к странице пользовательского API

> **ПРИМЕНЯЕТСЯ К:** Business Central Online

С февраля 2022 г. новые отчеты, в которых используются данные [!INCLUDE [prod_short](includes/prod_short.md)], по умолчанию будут подключаться к доступной только для чтения реплике базы данных [!INCLUDE [prod_short](includes/prod_short.md)]. В редких случаях, в зависимости от дизайна страницы, вы будете видеть сообщение об ошибке при попытке подключения и получения данных со страницы.

1. Запустите Power BI Desktop.
2. На ленте выберите **Получить данные** > **Веб-службы**.
3. В области **Веб-службы** выберите **Dynamics 365 Business Central**, затем **Подключить**.
4. В окне **Навигатор** выберите конечную точку API, из которой вы хотите загрузить данные.
5. На панели предварительного просмотра отображается следующая ошибка:

   *Dynamics365BusinessCentral: ошибка запроса. Удаленный сервер вернул ошибку: (400) неверный запрос. (Невозможно вставить запись. Текущее намерение подключения доступно только для чтения. CorrelationId: [...])».*

6. Выберите **Преобразовать данные** вместо **Загрузить**, как вы обычно делаете.
7. В **редакторе Power Query** выберите **Расширенный редактор** на ленте.
8. В строке, начинающейся с **Источник =**, замените следующий текст:

   ```
   Dynamics365BusinessCentral.ApiContentsWithOptions(null, null, null, null)
   ```

   на:

   ```
   Dynamics365BusinessCentral.ApiContentsWithOptions(null, null, null, [UseReadOnlyReplica = false])
   ```

9. Нажмите **Готово**.
10. Выберите **Закрыть и применить** на ленте, чтобы сохранить изменения и закрыть редактор Power Query.

## <a name="see-also"></a>См. также

[Включение бизнес-данных для Power BI](admin-powerbi-setup.md)  
[Бизнес-аналитика](bi.md)  
[Подготовьтесь к ведению бизнеса](ui-get-ready-business.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Финансы](finance.md)  
[Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
