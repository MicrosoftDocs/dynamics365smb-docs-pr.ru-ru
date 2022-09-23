---
title: Использование приложений Business Central в Power BI
description: Анализ данных, бизнес-аналитика и КПЭ на основе данных Business Central становятся проще благодаря приложениям Business Central для Power BI.
author: jswymer
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: a0ea051ec39b290706b30da455fce518cd7bdcd0
ms.sourcegitcommit: 3acadf94fa34ca57fc137cb2296e644fbabc1a60
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2022
ms.locfileid: "9533380"
---
# <a name="use-the-prod_short-apps-in-power-bi"></a>Использование приложений [!INCLUDE [prod_short](includes/prod_short.md)] в Power BI

> **ОТНОСИТСЯ К:** [!INCLUDE [prod_long](includes/prod_long.md)] Online 

[!INCLUDE [prod_long](includes/prod_long.md)] публикует следующие приложения Power BI, которые предоставляют подробные панели мониторинга для просмотра данных:

- [!INCLUDE [prod_long](includes/prod_long.md)] — CRM  
- [!INCLUDE [prod_long](includes/prod_long.md)] — Finance  
- [!INCLUDE [prod_long](includes/prod_long.md)] — Sales

## <a name="overview"></a>Обзор

Каждое приложение включает в себя несколько отчетов, в которых вы можете детализировать данные, включая следующие функции:

- Выберите любой из визуальных элементов панели мониторинга, чтобы открыть один из отчетов.  
- Отфильтруйте отчет или добавьте поля, которые вы хотите отслеживать.  
- Закрепите настроенное представление к панели мониторинга для дальнейшего отслеживания.  
  Можно обновить данные вручную, а также можно настроить график обновления. Дополнительные сведения см. в разделе [Настройка графика обновления](/power-bi/refresh-scheduled-refresh).  

Приложения предназначены для работы с данными из любой компании в [!INCLUDE[prod_short](includes/prod_short.md)]. Когда вы устанавливаете приложение Power BI, вы указываете один или несколько параметров для подключения к вашему [!INCLUDE [prod_short](includes/prod_short.md)].  

> [!NOTE]
> Также можно создать собственные отчеты и панели мониторинга в Power BI на основании данных [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Подключение ваших бизнес-данных к Power BI](across-how-use-financials-data-source-powerbi.md). 

## <a name="prerequisites"></a>Предварительные требования

Приложениям Power BI требуются разрешения для таблиц, из которых извлекаются данные, и веб-служб, используемых для извлечения данных. В следующей таблице перечислены веб-службы, необходимые для каждого приложения Power BI:
    
|Приложение | Веб-службы|
|----|-------------|
|[!INCLUDE[prod_short](includes/prod_short.md)] — CRM| <ul><li>Возможности продаж</li><li>Шаблон Excel для просмотра сведений об организации</li><li>Метки отчета Power BI</li></ul>|
|[!INCLUDE[prod_short](includes/prod_short.md)] — Finance| <ul><li>PowerBIFinance</li><li>Шаблон Excel для просмотра сведений об организации</li><li>Метки отчета Power BI</li></ul>|
|[!INCLUDE[prod_short](includes/prod_short.md)] — Sales| <ul><li>Продажа товаров по клиенту</li><li>Панель мониторинга продажи</li><li>Шаблон Excel для просмотра сведений об организации</li><li>Метки отчета Power BI</li></ul>|

> [!TIP]
> Простой способ найти веб-службы — найти *веб-службы* в [!INCLUDE[prod_short](includes/prod_short.md)]. На странице **Веб-службы** убедитесь, что поле **Опубликовать** выбрано для веб-служб, перечисленных выше. Дополнительные сведения см. в разделе [Публикация веб-службы](across-how-publish-web-service.md).

## <a name="get-ready"></a>Подготовка

Подпишитесь на службу Power BI. Если вы еще не зарегистрировались, перейдите на [https://powerbi.microsoft.com](https://powerbi.microsoft.com). При регистрации используйте рабочий адрес электронной почты и пароль.

## <a name="install-a-prod_short-app-in-power-bi"></a>Установка приложения [!INCLUDE[prod_short](includes/prod_short.md)] в Power BI

1. Откройте браузер, перейдите по адресу [https://powerbi.microsoft.com](https://powerbi.microsoft.com) и войдите в свою учетную запись.
2. Выберите **Получить данные** в нижней части левой панели навигации.  

    ![Переход к разделу "Получить данные".](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)

    Можно также начать из [!INCLUDE [prod_short](includes/prod_short.md)]. Находясь на домашней странице, перейдите к пункту **Выбор отчета** в разделе Power BI. Выберите на ленте **Сервис** или **Моя организация**. Галерея организации в Power BI или Microsoft AppSource открывается, отфильтрованная, чтобы отображать только приложения, связанные с [!INCLUDE[prod_short](includes/prod_short.md)].

3. В поле **Службы** выберите **Получить**.

    Этот шаг открывает страницу **Приложения Power BI**, которая позволяет просматривать приложение Power BI, доступное в **AppSource**.  

4. В поле **Поиск** введите **Dynamics 365 Business Central**.
5. Выберите приложение, которое вы хотите использовать, выберите **Получить сейчас**, затем **Установить**.  

    По завершении приложение будет доступно в пункте **Приложения** в меню навигации в Power BI.

## <a name="connect-the-prod_short-app-to-your-data"></a>Подключение приложения [!INCLUDE[prod_short](includes/prod_short.md)] к вашим данным

1. В пункте **Приложения** выберите приложение Business Central, затем **Подключить**.
2. При появлении запроса заполните поля **Название компании** и **Среда** сведениями об экземпляре [!INCLUDE[prod_short](includes/prod_short.md)], к которому хотите подключиться.

    - В поле **Название компании** обязательно используйте полное имя, а не отображаемое имя. Название организации можно найти на странице **Организации** в [!INCLUDE[prod_short](includes/prod_short.md)]. 
    - В поле **Среда**, если вы не создали несколько сред, введите **Производственная**.

3. Выберите **Далее**.
4. Выберите **Войти**.
5. При появлении запроса введите имя пользователя и пароль для входа в [!INCLUDE[prod_short](includes/prod_short.md)].
6. После подключения панель мониторинга и отчеты добавляются в вашу рабочую область Power BI. По завершении плитки отображают данные из вашей организации [!INCLUDE[prod_short](includes/prod_short.md)].

    ![Выберите Dynamics 365 Business Central и выберите "Получить сейчас".](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)

## <a name="fixing-problems"></a>Устранение проблем

Панель мониторинга Power BI полагается на опубликованные веб-службы, перечисленные выше. Она показывает данные демонстрационной компании или вашей собственной компании, если вы импортируете данные из своего текущего финансового решения. Однако если что-то работает некорректно, в этом разделе предложено обходное решение для типичных проблем.  

### <a name="you-dont-have-a-power-bi-account"></a>У вас нет учетной записи Power BI

Учетная запись Power BI не была настроена. У вас должна быть лицензия, чтобы получить действующую учетную запись Power BI. Кроме того, вы должны предварительно войти в Power BI, чтобы создать свою рабочую область Power BI.  

### <a name="message-there-are-no-enabled-reports-choose-select-report-to-see-a-list-of-reports-that-you-can-display"></a>Сообщение: "Включенные отчеты отсутствуют. Нажмите кнопку "Выбрать отчет", чтобы увидеть список отчетов, которые можно открыть."

Это сообщение появляется, если отчет по умолчанию не удалось развернуть на вашей рабочей области Power BI. Или отчет развернут, но не был успешно обновлен. В случае этой проблемы перейдите к отчету в своей рабочей области Power BI, выберите **Набор данных**, **Настройки**, а затем вручную обновите учетные данные. После успешного обновления набора данных вернитесь в [!INCLUDE[prod_short](includes/prod_short.md)] и вручную выберите отчет на странице **Выбрать отчеты**.

### <a name="you-need-a-power-bi-pro-license-to-install-the-prod_short-app-in-power-bi"></a>Вам необходима лицензия Power BI Pro для установки приложения [!INCLUDE[prod_short](includes/prod_short.md)] в Power BI

Вам требуется [лицензия Power BI Pro](/power-bi/service-features-license-type), чтобы делиться своим контентом, и людям, с которыми вы им делитесь, тоже. Контент должен находиться в рабочей области с [премиум-емкостью](/power-bi/service-premium-what-is). Дополнительные сведения см. в разделе [Способы поделиться своей работой в Power BI](/power-bi/service-how-to-collaborate-distribute-dashboards-reports).  

### <a name="parameter-validation-failed-please-make-sure-all-parameters-are-valid"></a>"Ошибка при проверке параметра. Убедитесь, что все параметры допустимы"

Эта ошибка указывает на то, что еще один из параметров недействителен.

- Указанный параметр среды не соответствует ни одной из существующих рабочих сред или песочниц [!INCLUDE[prod_short](includes/prod_short.md)].
- Указанный параметр организации не соответствует ни одной из существующих организаций [!INCLUDE[prod_short](includes/prod_short.md)]. Проверьте название компании на странице **Организации** в [!INCLUDE[prod_short](includes/prod_short.md)].
- При подключении к [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises вы ввели недопустимый URL-адрес. Вы можете проверить URL-адрес на странице **Веб-службы** в [!INCLUDE[prod_short](includes/prod_short.md)]  
- Порт не открыт, чтобы позволить запросу пройти через ваш брандмауэр.

### <a name="cant-sign-in"></a>Не удается войти

Если при попытке войти с использованием учетных данных [!INCLUDE[prod_short](includes/prod_short.md)] появляется ошибка "Сбой при входе", это может быть вызвано одной из следующих причин:

- У используемой учетной записи нет разрешений на извлечение данных [!INCLUDE[prod_short](includes/prod_short.md)] для вашей учетной записи. Убедитесь, что у вас есть разрешения на необходимые данные в [!INCLUDE[prod_short](includes/prod_short.md)] и попробуй еще раз.
- При подключении к [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises был выбран тип проверки подлинности, отличный от базового.
- Вы не ввели действительное имя пользователя или пароль.

### <a name="message-your-data-source-cant-be-refreshed-because-the-credentials-are-invalid-please-update-your-credentials-and-try-again"></a>Сообщение: ваш источник данных не может быть обновлен, потому что учетные данные недействительны. Обновите свои учетные данные и попробуйте еще раз

Для [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises проблема может заключаться в том, что URL-адрес OData доступен только в локальной сети.

### <a name="incorrect-company-name"></a>Неверное название организации

Распространенной ошибкой является ввод отображаемого имени организации вместо названия организации. Чтобы найти название организации, найдите **Организации**. Затем в поле **Название** введите название организации.

### <a name="the-key-didnt-match-any-rows-in-the-table"></a>Ключ не соответствует ни одной из строк в таблице

Если ввести недействительное имя организации в процессе подключения, можно получить сообщение об ошибке "Ключ не соответствует ни одной из строк в таблице". Укажите правильное название организации и попробуйте подключиться снова.

### <a name="historical-data-appears-to-be-missing"></a>Исторические данные отсутствуют

После того как приложение Power BI установлено, и ваши данные появились в Power BI, вы можете заметить, что отображаются не все ваши данные. Наборы данных фильтруются, чтобы возвращать только данные за предыдущие 365 дней. Это значение по умолчанию используется для ускорения создания отчетов.  

### <a name="i-only-see-data-for-a-single-company"></a>Я вижу данные только для одной организации

Приложение Power BI будет отображать только данные из организации [!INCLUDE[prod_short](includes/prod_short.md)], которая была определена, когда приложение Power BI было установлено. Данные из других организаций можно добавлять в отчеты, добавляя новые запросы, которые используют другие организации в качестве источника данных.  

### <a name="what-now"></a>Что теперь?

- Попробуйте [задать вопрос в поле "Вопросы и ответы"](/power-bi/service-q-and-a-tips) вверху панели мониторинга.
- [Измените плитки](/power-bi/service-dashboard-edit-tile) на панели мониторинга.  
- [Выберите плитку](/power-bi/service-dashboard-tiles), чтобы открыть основной отчет.  
- По умолчанию ваш набор данных не запланирован для обновления. Вы можете изменить расписание обновления или попробовать обновить его по требованию, используя **Обновить сейчас**. Дополнительные сведения см. в разделе [Настройка графика обновления](/power-bi/refresh-scheduled-refresh).

## <a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Business Central и Power BI](admin-powerbi.md)  
[Обзор компонентов и архитектуры интеграции Power BI для [!INCLUDE[prod_short](includes/prod_short.md)]](admin-powerbi-overview.md)  
[Работа с данными [!INCLUDE [prod_short](includes/prod_short.md)] в Power BI](across-working-with-business-central-in-powerbi.md)  
[Создание отчетов Power BI для отображения данных [!INCLUDE [prod_long](includes/prod_long.md)]](across-how-use-financials-data-source-powerbi.md)  
[Бизнес-аналитика](bi.md)  
[Подготовка к ведению бизнеса](ui-get-ready-business.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
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
