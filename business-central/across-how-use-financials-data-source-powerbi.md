---
title: Создание отчетов в Power BI Desktop для отображения данных Business Central | Документация Майкрософт
description: Можно сделать данные доступными в качестве источника данных в Power BI и создать мощные отчеты о состоянии вашего бизнеса.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: a19d2bbff275ea4401943b588a68cdd2e6740e12
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3924807"
---
# <a name="building-power-bi-reports-to-display-prodlong-data"></a>Создание отчетов Power BI для отображения данных [!INCLUDE [prodlong](includes/prodlong.md)]

Можно сделать данные [!INCLUDE[prodlong](includes/prodlong.md)] доступными в качестве источника данных в Power BI Desktop и создать мощные отчеты о состоянии вашего бизнеса.

В этой статье рассказывается, как начать использовать Power BI Desktop для создания отчетов, отображающих данные [!INCLUDE[prodlong](includes/prodlong.md)].  После создания отчетов вы можете опубликовать их в своей службе Power BI или поделиться ими со всеми пользователями в вашей организации. Как только эти отчеты будут в службе Power BI, пользователи, которые настроены для нее, могут затем просматривать отчеты в [!INCLUDE[prodlong](includes/prodlong.md)].

## <a name="get-ready"></a>Подготовка

- Подпишитесь на службу Power BI.

    Если вы еще не зарегистрировались, перейдите на [https://powerbi.microsoft.com](https://powerbi.microsoft.com). При регистрации используйте рабочий адрес электронной почты и пароль.

- Скачайте [Power BI Desktop](https://powerbi.microsoft.com/desktop/).

   Power BI Desktop — это бесплатное приложение, которое вы устанавливаете на свой локальный компьютер. Для получения дополнительной информации см. раздел [Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data),

- Убедитесь, что данные, которые вы хотите включить в отчет, опубликованы в виде веб-службы.
    
    По умолчанию опубликовано множество веб-служб. Простой способ найти веб-службы — найти *веб-службы* в [!INCLUDE[prodshort](includes/prodshort.md)]. На странице **Веб-службы** убедитесь, что выбрано поле **Опубликовать**. Эту задачу обычно является административной задачей.
    
    Дополнительные сведения о публикации веб-служб см. в разделе [Публикация веб-службы](across-how-publish-web-service.md).

- Для [!INCLUDE[prodshort](includes/prodshort.md)] On-Premises получите следующую информацию:

    - URL-адрес OData для [!INCLUDE[prodshort](includes/prodshort.md)]. Обычно этот URL-адрес имеет формат `http[s]://[computer]:[port]/[serverinstance]/ODataV4`, например `https://localhost:7048/BC160/ODataV4`. Если у вас есть развертывание в нескольких клиентах, включите клиент в URL-адрес, например `https://localhost:7048/BC160/ODataV4?tenant=tenant1`.
    - Имя пользователя и ключ доступа к веб-сервису учетной записи [!INCLUDE[prodshort](includes/prodshort.md)].

      Чтобы получить данные из [!INCLUDE[prodshort](includes/prodshort.md)], Power BI использует базовую аутентификацию. Итак, для подключения вам понадобятся имя пользователя и ключ доступа к веб-службе. Учетная запись может быть вашей собственной учетной записью пользователя, или ваша организация может иметь специальную учетную запись для этой цели.

- Загрузите тему отчета [!INCLUDE [prodshort](includes/prodshort.md)] (необязательно).

    Дополнительные сведения см. в разделе [Использование темы отчета [!INCLUDE [prodshort](includes/prodshort.md)]](#theme) в этой статье.

## <a name="add-prodshort-as-a-data-source-in-power-bi-desktop"></a>Добавление [!INCLUDE[prodshort](includes/prodshort.md)] как источника данных в Power BI Desktop

Первая задача при создании отчетов — добавить [!INCLUDE[prodshort](includes/prodshort.md)] как источник данных в Power BI Desktop. После подключения вы можете приступить к созданию отчета.

1. Запустите Power BI Desktop.
2. Выберите **Получить данные**.

    Если вы не видите пункт **Получить данные**, выберите меню **Файл**, затем **Получить данные**.
2. На странице **Получить данные** выберите **Веб-службы**.
3. В области **Веб-службы** выполните одно из следующих действий:

    1. Если вы подключаетесь к [!INCLUDE [prodshort](includes/prodshort.md)] Online, выберите **Dynamics 365 Business Central**, затем **Подключить**.
    2. Если вы подключаетесь к [!INCLUDE [prodshort](includes/prodshort.md)] On-Premises, выберите **Dynamics 365 Business Central (on-premises)**, затем **Подключить**.

4. Power BI отобразит мастер с руководством по процессу подключения, включая вход в [!INCLUDE [prodshort](includes/prodshort.md)].

    Для сетевой версии выберите **Войти**, затем выберите соответствующую учетную запись. Используйте ту же учетную запись, которая используется для входа в [!INCLUDE [prodshort](includes/prodshort.md)].
    
    Для локальной версии введите URL-адрес OData для [!INCLUDE[prodshort](includes/prodshort.md)], и, необязательно, название компании. Затем, когда будет предложено, введите имя пользователя и пароль учетной записи, которая будет использоваться для подключения к [!INCLUDE[prodshort](includes/prodshort.md)]. В поле **Пароль** введите ключ доступа к веб-службе.

    > [!NOTE]  
    > После успешного подключения к [!INCLUDE[prodshort](includes/prodshort.md)] выполнять повторный вход не требуется.
    
5. Выберите **Подключить** для продолжения.

    Мастер Power BI отобразит список сред, компаний и источников данных Microsoft [!INCLUDE[d365fin](includes/d365fin_md.md)]. Эти источники данных представляют все веб-службы, которые вы опубликовали из [!INCLUDE [prodshort](includes/prodshort.md)].
6. Укажите данные, которые требуется добавить в модель данных, а затем нажмите кнопку **Загрузить**.
7. Повторите предыдущие шаги для добавления дополнительных данных [!INCLUDE [prodshort](includes/prodshort.md)] или других данных в модель данных Power BI.

После загрузки данных они отображаются в правой области навигации на странице. На этом шаге вы успешно подключились с данным [!INCLUDE[prodshort](includes/prodshort.md)] и можете начать создание отчета Power BI.  

> [!TIP]
> Дополнительные сведения об использовании Power BI Desktop см. в разделе [Приступая к работе с Power BI Desktop](/power-bi/fundamentals/desktop-getting-started).

## <a name="creating-reports-to-display-data-associated-with-a-list"></a>Создание отчетов для отображения данных, связанных со списком

Вы можете создавать отчеты, которые отображаются на информационной панели страницы списка [!INCLUDE [prodshort](includes/prodshort.md)]. Отчеты могут содержать данные о записи, выбранной в списке. Создание этих отчетов аналогично созданию других отчетов, за исключением того, что вам нужно сделать несколько вещей, чтобы убедиться, что отчеты отображаются должным образом. Для получения дополнительной информации см. раздел [Создание отчетов Power BI для отображения данных списка в [!INCLUDE[prodshort](includes/prodshort.md)]](across-how-use-powerbi-reports-factbox.md).

## <a name="using-the-prodshort-report-theme-optional"></a><a name="theme"></a>Использование темы отчетов [!INCLUDE [prodshort](includes/prodshort.md)] (необязательно)

Перед построением отчета рекомендуется скачать и импортировать файл темы [!INCLUDE [prodshort](includes/prodshort.md)]. Файл темы создает цветовую палитру, чтобы можно было создавать отчеты с таким же цветовым стилем, что и приложения [!INCLUDE [prodshort](includes/prodshort.md)] без необходимости определения настраиваемых цветов для каждого визуального элемента.

> [!NOTE]
> Эта задача является необязательной. Вы всегда можете создать свои отчеты, затем скачать и применить шаблон стиля позже.

### <a name="download-the-theme"></a>Скачивание темы

Файл темы доступен как файл json в коллекции тем сообщества Microsoft Power BI. Чтобы скачать файл темы, выполните следующие действия:

1. Перейдите в [Коллекцию тем сообщества Microsoft Power BI для Microsoft Dynamics 365 Business Central](https://community.powerbi.com/t5/Themes-Gallery/Microsoft-Dynamics-365-Business-Central/m-p/385875).
2. Выберите скачивание вложения **Microsoft Dynamics Business Central.json**.

### <a name="import-the-theme-on-a-report"></a>Импорт темы в отчет

После того, как вы скачали тему отчета [!INCLUDE [prodshort](includes/prodshort.md)], вы можете импортировать ее в свои отчеты. Чтобы импортировать тему, выберите **Представление** > **Темы** > **Поиск тем**. Дополнительные сведения см. в разделе [Power BI Desktop — импорт пользовательских тем отчетов](/power-bi/create-reports/desktop-report-themes#import-custom-report-theme-files).

## <a name="publish-reports"></a>Публикация отчетов

После того как вы создали или изменили отчет, вы можете опубликовать его в своей службе Power BI, а также поделиться им с другими в вашей организации. После публикации вы увидите отчет в Power BI. Отчет также становится доступным для выбора в [!INCLUDE[prodshort](includes/prodshort.md)].

Чтобы опубликовать отчет, выберите **Опубликовать** на вкладке **Главная** на ленте или из меню **файл**. Если вы вошли в службу Power BI, отчет публикуется в этой службе. В противном случае вам будет предложено войти в систему. 

## <a name="distribute-or-share-a-report"></a>Распространение отчета или предоставление доступа к нему

Есть несколько способов отправить отчеты своим коллегам и другим людям:

- Распространяйте отчеты в виде файлов .pbix.

    Отчеты хранятся на вашем компьютере в виде файлов .pbix. Вы можете распространять файл отчета .pbix среди пользователей, как и любой другой файл. Затем пользователи могут отправить этот файл в свою службу Power BI. См. раздел [Отправить отчеты из файлов](across-working-with-business-central-in-powerbi.md#upload).

    > [!NOTE]
    > Распространение отчетов таким образом означает, что обновление данных для отчетов будет выполняться каждым пользователем индивидуально. Эта ситуация может повлиять на производительность [!INCLUDE[prodshort](includes/prodshort.md)].

- Предоставление доступа к отчету из вашей службы Power BI

    Если у вас есть лицензия Power BI Pro, вы можете поделиться отчетом с другими прямо из своей службы Power BI. Дополнительные сведения см. в разделе [Power BI — предоставление доступа к панели мониторинга или отчету](/power-bi/collaborate-share/service-share-dashboards#share-a-dashboard-or-report).

## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Включение бизнес-данных для Power BI](admin-powerbi.md)  
[Бизнес-аналитика](bi.md)  
[Приступая к работе](product-get-started.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Финансы](finance.md)  
[Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
