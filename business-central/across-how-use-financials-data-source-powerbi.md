---
title: Создание отчетов в Power BI Desktop для отображения данных Business Central | Документация Майкрософт
description: Можно сделать данные доступными в качестве источника данных в Power BI и создать мощные отчеты о состоянии вашего бизнеса.
author: jswymer
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'business intelligence, KPI, Odata, Power App, SOAP, analysis'
ms.date: 09/07/2022
ms.author: jswymer
---

# <a name="building-power-bi-reports-to-display-include-prodlongincludesprodlongmd-data" />Создание отчетов Power BI для отображения данных [!INCLUDE [prod_long](includes/prod_long.md)]

Можно сделать данные [!INCLUDE[prod_long](includes/prod_long.md)] доступными в качестве источника данных в Power BI Desktop и создать мощные отчеты о состоянии вашего бизнеса.

В этой статье рассказывается, как начать использовать Power BI Desktop для создания отчетов, отображающих данные [!INCLUDE[prod_long](includes/prod_long.md)].  После создания отчетов вы можете опубликовать их в своей службе Power BI или поделиться ими со всеми пользователями в вашей организации. Как только эти отчеты будут в службе Power BI, пользователи, которые настроены для нее, могут затем просматривать отчеты в [!INCLUDE[prod_long](includes/prod_long.md)].

## <a name="get-ready" />Подготовка

- Подпишитесь на службу Power BI.

  Если вы еще не зарегистрировались, перейдите на [https://powerbi.microsoft.com](https://powerbi.microsoft.com). При регистрации используйте рабочий адрес электронной почты и пароль.

- Скачайте [Power BI Desktop](https://powerbi.microsoft.com/desktop/).

  Power BI Desktop — это бесплатное приложение, которое вы устанавливаете на свой локальный компьютер. Для получения дополнительной информации см. раздел [Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data),

- Убедитесь, что данные, которые вы хотите включить в отчет, доступны как страница API или опубликованы в виде веб-службы.

  Для получения дополнительной информации прочитайте [Предоставлять данные через страницы API или веб-службы OData](admin-powerbi-setup.md#exposedata).

- Для [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises получите следующую информацию:

  - URL-адрес OData для [!INCLUDE[prod_short](includes/prod_short.md)].
  
    Обычно этот URL-адрес имеет формат `http[s]://[computer]:[port]/[serverinstance]/ODataV4`, например `https://localhost:7048/BC190/ODataV4`. Если у вас есть развертывание в нескольких клиентах, включите клиент в URL-адрес, например `https://localhost:7048/BC190/ODataV4?tenant=tenant1`.
  - Имя пользователя и ключ доступа к веб-сервису учетной записи [!INCLUDE[prod_short](includes/prod_short.md)].

    Чтобы получить данные из [!INCLUDE[prod_short](includes/prod_short.md)], Power BI использует базовую аутентификацию. Итак, для подключения вам понадобятся имя пользователя и ключ доступа к веб-службе. Учетная запись может быть вашей собственной учетной записью пользователя, или ваша организация может иметь специальную учетную запись для этой цели.

- Загрузите тему отчета [!INCLUDE [prod_short](includes/prod_short.md)] (необязательно).

  Дополнительные сведения см. в разделе [Использование темы отчета [!INCLUDE [prod_short](includes/prod_short.md)]](#theme) в этой статье.

[!INCLUDE[note-multicompany-reports](includes/note-multicompany-reports.md)]

## <a name="a-namegetdataaadd-includeprodshortincludesprodshortmd-as-a-data-source-in-power-bi-desktop" /><a name="getdata"></a>Добавление [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных в Power BI Desktop

Первая задача при создании отчетов — добавить [!INCLUDE[prod_short](includes/prod_short.md)] как источник данных в Power BI Desktop. После подключения вы можете приступить к созданию отчета.

1. Запустите Power BI Desktop.
2. Выберите **Получить данные**.

    Если вы не видите пункт **Получить данные**, выберите меню **Файл**, затем **Получить данные**.
3. На странице **Получить данные** выберите **Веб-службы**.
4. В области **Веб-службы** выполните одно из следующих действий:

    - Чтобы подключиться к [!INCLUDE [prod_short](includes/prod_short.md)] онлайн, выберите **Dynamics 365 Business Central**, затем **Подключить**.
    - Чтобы подключиться к [!INCLUDE [prod_short](includes/prod_short.md)] локально, выберите **Dynamics 365 Business Central (локальная версия)**, затем **Подключить**.

5. Войдите в [!INCLUDE [prod_short](includes/prod_short.md)] (только один раз).

    Если вы еще не вошли в [!INCLUDE [prod_short](includes/prod_short.md)] из Power BI Desktop, вам будет предложено войти в систему.

    - Для сетевой версии [!INCLUDE [prod_short](includes/prod_short.md)] выберите **Войти**, затем выберите соответствующую учетную запись. Используйте ту же учетную запись, которая используется для входа в [!INCLUDE [prod_short](includes/prod_short.md)]. Когда готово, выберите **Подключить**.

    - Для локальной версии [!INCLUDE [prod_short](includes/prod_short.md)] сначала введите URL-адрес OData для [!INCLUDE[prod_short](includes/prod_short.md)], затем выберите **ОК**. Когда будет предложено, введите имя пользователя и пароль учетной записи, которая будет использоваться для подключения к [!INCLUDE[prod_short](includes/prod_short.md)]. В поле **Пароль** введите ключ доступа к веб-службе. Когда готово, выберите **Подключить**.

    > [!NOTE]  
    > После успешного подключения к [!INCLUDE[prod_short](includes/prod_short.md)] выполнять повторный вход не требуется. [Как изменить или удалить учетную запись, которую я сейчас использую для подключения к Business Central из Power BI Desktop?](/dynamics365/business-central/power-bi-faq?tabs=designer#perms)

6. После подключения Power BI связывается со службой Business Central. Появляется окно **Навигатор**, в котором отображаются доступные источники данных для построения отчетов. Выберите папку, чтобы развернуть ее и просмотреть доступные источники данных. 

   Эти источники данных представляют все веб-службы и страницы API, которые опубликованы для [!INCLUDE [prod_short](includes/prod_short.md)]. Источники данных сгруппированы по средам Business Central и компаниям. С Business Central Online **Навигатор** имеет следующую структуру:

    - **Имя среды**
      - **Название организации**
        - **Расширенные API**

          В этой папке перечислены расширенные страницы API, опубликованные Microsoft, например [API автоматизации Business Central](/dynamics365/business-central/dev-itpro/administration/itpro-introduction-to-automation-apis) и [Настраиваемые страницы API для Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-develop-custom-api). Страницы пользовательского API далее сгруппированы по папкам по свойствам [APIPublisher](/dynamics365/business-central/dev-itpro/developer/properties/devenv-apipublisher-property)/[APIGroup](/dynamics365/business-central/dev-itpro/developer/properties/devenv-apigroup-property) исходного кода страницы API.

        - **Стандартные API v2.0**

          В этой папке перечислены страницы API, представленные [Business Central API V2.0](/dynamics365/business-central/dev-itpro/api-reference/v2.0/).

        - **Веб-службы \(устаревшие версии)**

          В этой папке перечислены страницы, модули codeunit и запросы, опубликованные как веб-службы в Business Central.

    > [!NOTE]
    > Структура локальной версии Business Central отличается, поскольку она не поддерживает страницы API.

7. Выберите источник данных или источники, которые требуется добавить в модель данных, а затем нажмите кнопку **Загрузить**.
8. Если позже вы захотите добавить дополнительные данные Business Central, вы можете повторить предыдущие шаги.

После загрузки данных они отображаются в правой области навигации на странице. На этом шаге вы успешно подключились с данным [!INCLUDE[prod_short](includes/prod_short.md)] и можете начать создание отчета Power BI.  

> [!TIP]
> Дополнительные сведения об использовании Power BI Desktop см. в разделе [Приступая к работе с Power BI Desktop](/power-bi/fundamentals/desktop-getting-started).

## <a name="creating-accessible-reports" />Создание доступных отчетов

Важно, чтобы ваши отчеты были доступны как можно большему количеству людей. Постарайтесь создавать отчеты так, чтобы они не требовали специальной адаптации для удовлетворения конкретных потребностей разных пользователей. Убедитесь, что дизайн позволяет пользователям использовать стандартные технологии специальных возможностей, например программы чтения с экрана. Power BI включает различные специальные возможности, инструменты и рекомендации, которые помогут вам в достижении этой цели. Для дополнительной информации см. [Разработка отчетов Power BI с учетом специальных возможностей](/power-bi/create-reports/desktop-accessibility-creating-reports) в документации Power BI.

## <a name="creating-reports-to-display-data-associated-with-a-list" />Создание отчетов для отображения данных, связанных со списком

Вы можете создавать отчеты, которые отображаются на информационной панели страницы списка [!INCLUDE [prod_short](includes/prod_short.md)]. Отчеты могут содержать данные о записи, выбранной в списке. Создание этих отчетов аналогично созданию других отчетов, за исключением того, что вам нужно сделать несколько вещей, чтобы убедиться, что отчеты отображаются должным образом. Для получения дополнительной информации см. раздел [Создание отчетов Power BI для отображения данных списка в [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-powerbi-reports-factbox.md).

## <a name="a-namethemeausing-the-include-prodshortincludesprodshortmd-report-theme-optional" /><a name="theme"></a>Использование темы отчетов [!INCLUDE [prod_short](includes/prod_short.md)] (необязательно)

Перед построением отчета рекомендуется скачать и импортировать файл темы [!INCLUDE [prod_short](includes/prod_short.md)]. Файл темы создает цветовую палитру, чтобы можно было создавать отчеты с таким же цветовым стилем, что и приложения [!INCLUDE [prod_short](includes/prod_short.md)] без необходимости определения настраиваемых цветов для каждого визуального элемента.

> [!NOTE]
> Эта задача является необязательной. Вы всегда можете создать свои отчеты, затем скачать и применить шаблон стиля позже.

### <a name="download-the-theme" />Скачивание темы

Файл темы доступен как файл json в коллекции тем сообщества Microsoft Power BI. Чтобы скачать файл темы, выполните следующие действия:

1. Перейдите в [Коллекцию тем сообщества Microsoft Power BI для Microsoft Dynamics 365 Business Central](https://community.powerbi.com/t5/Themes-Gallery/Microsoft-Dynamics-365-Business-Central/m-p/385875).
2. Выберите скачивание вложения **Microsoft Dynamics Business Central.json**.

### <a name="import-the-theme-on-a-report" />Импорт темы в отчет

После того, как вы скачали тему отчета [!INCLUDE [prod_short](includes/prod_short.md)], вы можете импортировать ее в свои отчеты. Чтобы импортировать тему, выберите **Представление** > **Темы** > **Поиск тем**. Дополнительные сведения см. в разделе [Power BI Desktop — импорт пользовательских тем отчетов](/power-bi/create-reports/desktop-report-themes#import-custom-report-theme-files).

## <a name="publish-reports" />Публикация отчетов

После того как вы создали или изменили отчет, вы можете опубликовать его в своей службе Power BI, а также поделиться им с другими в вашей организации. После публикации вы увидите отчет в Power BI. Отчет также становится доступным для выбора в [!INCLUDE[prod_short](includes/prod_short.md)].

Чтобы опубликовать отчет, выберите **Опубликовать** на вкладке **Главная** на ленте или из меню **файл**. Если вы вошли в службу Power BI, отчет публикуется в этой службе. В противном случае вам будет предложено войти в систему. 

## <a name="distribute-or-share-a-report" />Распространение отчета или предоставление доступа к нему

Есть несколько способов отправить отчеты своим коллегам и другим людям:

- Распространяйте отчеты в виде файлов .pbix.

    Отчеты хранятся на вашем компьютере в виде файлов .pbix. Вы можете распространять файл отчета .pbix среди пользователей, как и любой другой файл. Затем пользователи могут отправить этот файл в свою службу Power BI. См. раздел [Отправить отчеты из файлов](across-working-with-business-central-in-powerbi.md#upload).

    > [!NOTE]
    > Распространение отчетов таким образом означает, что обновление данных для отчетов будет выполняться каждым пользователем индивидуально. Эта ситуация может повлиять на производительность [!INCLUDE[prod_short](includes/prod_short.md)].

- Предоставление доступа к отчету из вашей службы Power BI

    Если у вас есть лицензия Power BI Pro, вы можете поделиться отчетом с другими прямо из своей службы Power BI. Дополнительные сведения см. в разделе [Power BI — предоставление доступа к панели мониторинга или отчету](/power-bi/collaborate-share/service-share-dashboards#share-a-dashboard-or-report).

## <a name="fixing-problems" />Устранение проблем

### <a name="cannot-insert-a-record-current-connection-intent-is-read-only-error-connecting-to-custom-api-page" />"Невозможно вставить запись. Назначение текущего подключения — только чтение". ошибка при подключении к странице пользовательского API

> **ПРИМЕНЯЕТСЯ К:** Business Central Online

С февраля 2022 г. новые отчеты, использующие данные Business Central, по умолчанию будут подключаться к доступной только для чтения реплике базы данных Business Central. В редких случаях, в зависимости от дизайна страницы, вы получите сообщение об ошибке при попытке подключения и получения данных со страницы.

1. Запустите Power BI Desktop.
2. На ленте выберите **Получить данные** > **Веб-службы**.
3. В области **Веб-службы** выберите **Dynamics 365 Business Central**, затем **Подключить**.
4. В окне **Навигатор** выберите конечную точку API, из которой вы хотите загрузить данные.
5. На панели предварительного просмотра справа вы увидите следующую ошибку:

   *Dynamics365BusinessCentral: ошибка запроса. Удаленный сервер вернул ошибку: (400) неверный запрос. (Невозможно вставить запись. Текущее намерение подключения доступно только для чтения. CorrelationId: [...])".*

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

## <a name="see-related-microsoft-trainingtrainingmodulesconfigure-powerbi-excel-dynamics--business-centralindex" />См. соответствующее [обучение Microsoft](/training/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also" />См. также

[Включение бизнес-данных для Power BI](admin-powerbi.md)  
[Бизнес-аналитика](bi.md)  
[Подготовьтесь к ведению бизнеса](ui-get-ready-business.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Финансы](finance.md)  
[Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
