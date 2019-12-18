---
title: Включение бизнес-данных для Power BI | Документация Майкрософт
description: Анализ данных, бизнес-аналитика и КПЭ на основе данных Business Central становятся проще благодаря приложениям Business Central для Power BI.
author: bmeier90
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.reviewer: edupont
ms.date: 10/01/2019
ms.author: bmeier
ms.openlocfilehash: 0750f1724260eb7767757d947f30dcb074ef1aeb
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2879110"
---
# <a name="enabling-your-business-data-for-power-bi"></a>Включение бизнес-данных для Power BI

Анализ данных [!INCLUDE[prodshort](includes/prodshort.md)] становится проще благодаря приложениям [!INCLUDE[prodshort](includes/prodshort.md)] для Power BI. Power BI извлекает ваши данные и строит готовую панель мониторинга и отчеты на основе этих данных.  

Вы должны иметь допустимую учетную запись в [!INCLUDE[prodshort](includes/prodshort.md)] и в Power BI. Кроме того, необходимо скачать [Power BI Desktop](https://powerbi.microsoft.com/desktop/), если вы хотите создавать собственные отчеты Power BI. Для приложений Power BI требуются разрешения к таблицам, из которых извлекаются данные. Дополнительные сведения о требованиях см. ниже.  

> [!IMPORTANT]
> Приложения Power BI, которые описаны в этой статье, предназначены для использования Azure Active Directory в качестве механизма аутентификации, если не указано иное. Чтобы установить приложение Power BI ,вы также должны иметь лицензию Power BI Pro.  После установки приложения Power BI оно может быть передано пользователям с любым типом лицензии.

Корпорация [!INCLUDE [prodlong](includes/prodlong.md)] опубликовывала следующие приложения для Power BI:

- [!INCLUDE [prodlong](includes/prodlong.md)] — CRM  
- [!INCLUDE [prodlong](includes/prodlong.md)] — Finance  
- [!INCLUDE [prodlong](includes/prodlong.md)] — Sales  
- [!INCLUDE [prodlong](includes/prodlong.md)](локальная версия) — CRM  
- [!INCLUDE [prodlong](includes/prodlong.md)](локальная версия) — Finance  
- [!INCLUDE [prodlong](includes/prodlong.md)](локальная версия) — Sales  

## <a name="using-the-include-prodshortincludesprodshortmd-dashboards-in-power-bi"></a>Использование панелей мониторинга [!INCLUDE [prodshort](includes/prodshort.md)] в Power BI

Каждое приложение предоставляет отчеты, которые можно подробно изучать:

- Выберите любой из визуальных элементов панели мониторинга, чтобы открыть один из отчетов.  
- Отфильтруйте отчет или добавьте поля, которые вы хотите отслеживать.  
- Прикрепите настроенное представление к панели мониторинга для дальнейшего отслеживания.  
  Можно обновить данные вручную, а также можно настроить график обновления. Дополнительные сведения см. в разделе [Настройка графика обновления](/power-bi/refresh-scheduled-refresh).  

Приложения предназначены для работы с данными любой компании, которая есть в вашем [!INCLUDE[prodshort](includes/prodshort.md)]. Когда вы устанавливаете приложение Power BI, вы указываете один или несколько параметров для подключения к вашему [!INCLUDE [prodshort](includes/prodshort.md)].  

> [!NOTE]
> Также можно создать собственные отчеты и панели мониторинга в Power BI на основании данных [!INCLUDE[d365fin](includes/d365fin_md.md)]. Дополнительные сведения см. в разделе [Подключение ваших бизнес-данных к Power BI](across-how-use-financials-data-source-powerbi.md).  

### <a name="to-connect-your-data-in-power-bi"></a>Чтобы подключить ваши данные в Power BI

1. Откройте браузер, перейдите по адресу https://powerbi.microsoft.com и войдите в свою учетную запись.
2. Выберите **Получить данные** в нижней части левой панели навигации.  

    ![Переход к разделу "Получить данные"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)

    Можно также начать из [!INCLUDE [prodshort](includes/prodshort.md)]. Находясь на домашней странице, перейдите к пункту **Выбор отчета** в разделе Power BI. Выберите на ленте **Сервис** или **Моя организация**. Когда выбрано одно из этих действий, производится переход к галерее "Организация" в Power BI или в Microsoft AppSource, которые также будут отфильтрованы для отображения только приложений, имеющих отношение к [!INCLUDE[prodshort](includes/prodshort.md)].

3. В поле **Службы** выберите **Получить**. Откроется страница, на которой отображаются **AppSource** и **Приложения для Power BI**.  

<!--    ![Choose apps from online services that you use.](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)-->
4. Выберите **Приложения** на вкладке **Приложения для Power BI**, выберите требуемое приложение **Microsoft Dynamics 365 Business Central** и выберите **Получить сейчас**.  
<!--    ![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packspowerbi-dynamics365-for-financials-get-it-now.png)/-->
5. При появлении запроса введите название среды и организации в приложении [!INCLUDE[prodshort](includes/prodshort.md)], к которому вы хотите подключиться. Если вы не создали несколько сред, введите **Рабочая среда**. Что касается параметра организации, убедитесь, что вы вводите имя, а не отображаемое имя. Название организации можно найти на странице **Организации** в вашем экземпляре [!INCLUDE[prodshort](includes/prodshort.md)].  

    > [!NOTE]
    > Если вы подключитесь к [!INCLUDE [prodshort](includes/prodshort.md)] on-premises, вы должны указать параметр *URL-адрес веб-службы*. Его можно найти на странице **Веб-службы** в [!INCLUDE [prodshort](includes/prodshort.md)]. Ваш экземпляр [!INCLUDE [server](includes/server.md)] должен быть настроен для базовой аутентификации, и вы должны указать пользователя и ключ веб-доступа этого пользователя в качестве пароля. В следующем примере замените *myserver:7048* вашим именем [!INCLUDE [server](includes/server.md)], а *CRONUS%20US* — с названием вашей организации.  
    > ```https://myserver:7048/BC140/ODataV4/Company('CRONUS%20US')/```

6. После подключения панель мониторинга и отчеты добавляются в вашу рабочую область Power BI. По завершении плитки отображают данные из вашей организации [!INCLUDE[prodshort](includes/prodshort.md)].

    ![Выберите Dynamics 365 Business Central и выберите "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)

### <a name="what-now"></a>Что теперь?

- Попробуйте [задать вопрос в поле "Вопросы и ответы"](/power-bi/service-q-and-a-tips) вверху панели мониторинга.
- [Измените плитки](/power-bi/service-dashboard-edit-tile) на панели мониторинга.  
- [Выберите плитку](/power-bi/service-dashboard-tiles), чтобы открыть основной отчет.  
- По умолчанию ваш набор данных не запланирован для обновления. Вы можете изменить расписание обновления или попробовать обновить его по требованию, используя **Обновить сейчас**. Дополнительные сведения см. в разделе [Настройка графика обновления](/power-bi/refresh-scheduled-refresh).

## <a name="power-bi-in-include-prodshortincludesprodshortmd"></a>Power BI в [!INCLUDE [prodshort](includes/prodshort.md)]

Ваша домашняя страница в [!INCLUDE [prodshort](includes/prodshort.md)] может включать в себя элемент управления Power BI, который можно настроить для отображения отчетов Power BI на вашей домашней странице.

> [!IMPORTANT]
> Вы должны иметь допустимую учетную запись в [!INCLUDE [prodshort](includes/prodshort.md)] и в Power BI. Кроме того, если вы хотите изменить какие-либо отчет, вы должны загрузить Power BI Desktop. Дополнительные сведения см. в разделе [Использование Business Central как источника данных Power BI](across-how-use-financials-data-source-powerbi.md).  

### <a name="on-first-login"></a>При первом входе

При первом входе в [!INCLUDE [prodshort](includes/prodshort.md)] вы заметите пустую часть Power BI на вашей домашней странице. Для просмотра отчетов сначала необходимо подключиться к Power BI, выбрав ссылку *Начало работы с Power BI*.

[!INCLUDE [prodshort](includes/prodshort.md)] затем общается к службе Power BI, чтобы определить, если у вас есть действительная учетная запись Power BI. Как только ваша лицензия будет подтверждена, отчеты Power BI по умолчанию отображаются на домашней странице.

### <a name="selecting-power-bi-reports"></a>Выбор отчетов Power BI

Элемент управления Power BI на вашей домашней странице может отображать любой отчет Power BI. Чтобы просмотреть существующий отчет, выберите действие **Выбрать отчет** из раскрывающегося списка команд Power BI.  

Страница выбора отчетов показывает список всех отчетов Power BI, к которым у вас есть доступ. Этот список получается из вашей рабочей области Power BI. Включите каждый отчет, который вы хотите отобразить на домашней странице, затем нажмите OK. Вы вернетесь на свою домашнюю страницу, и появится последний включенный отчет. Используя раскрывающийся список команд, используйте команду "предыдущий" и "следующий" для перехода между отчетами.  

### <a name="get-reports"></a>Получение отчетов

Если вы не видите никаких отчетов на странице "Выбрать отчеты" или не видите нужный отчет. Вы можете получать отчеты из раздела *Моя организация* или из раздела *Службы*.
Выберите *Моя организация*, чтобы перейти в службы Power BI, где вы можете просматривать отчеты в вашей организации, которые вы имеете право просматривать, и добавлять их в свою рабочую область. Выберите *Службы*, чтобы перейти в Microsoft AppSource, где вы можете установить приложения Power BI.  

Вы также можете создавать новые отчеты Power BI. Как только эти отчеты будут опубликованы в вашей рабочей области Power BI, они появятся на этой странице.  

### <a name="managing-reports"></a>Управление отчетами

В разделе Power BI на домашней странице вы можете выбрать действие **Управление отчетом** из выпадающего списка команд, чтобы вы могли изменить отчет, который был в фокусе в ролевом центре.  

Изменения могут быть внесены в отчет и сохранены.  Любые изменения, внесенные в отчет, будут изменены для любого пользователя, которому предоставлен доступ к этому отчету, поскольку вы изменяете отчет, хранящийся в службе Power BI.  

После внесения изменений выберите "Сохранить". Если это общий отчет, вы можете выбрать "Сохранить как", чтобы не вносить изменения для всех пользователей.
Вернитесь в ролевой центр, в нем появится обновленный отчет. Если вы выполнили команду "Сохранить как", вам нужно будет открыть страницу выбора отчета и включить новый отчет.

### <a name="uploading-reports"></a>Отправка отчетов

Вы можете отправить новые отчеты Power BI и поделиться ими со всеми пользователями вашего [!INCLUDE [prodshort](includes/prodshort.md)]. Отчеты становятся общими внутри каждой организации в [!INCLUDE [prodshort](includes/prodshort.md)].  

Чтобы отправить отчет, выберите действие **Отправить отчет** из раскрывающегося списка команд. Затем вы можете отправить файл .pbix, который определяет отчеты, которыми вы хотите поделиться. Можно изменить имя по умолчанию для файла.  

После того как отчет был отправлен в вашу рабочую область Power BI, он автоматически отправляется в рабочие области Power BI всех других пользователей в этой организации при следующем входе в [!INCLUDE [prodshort](includes/prodshort.md)].

## <a name="system-requirements"></a>Требования к системе

Чтобы импортировать данные [!INCLUDE[prodshort](includes/prodshort.md)] в Power BI, необходимо иметь разрешения на доступ к веб-службам, используемым для извлечения данных. Веб-службы, необходимые для каждого приложения Power BI:

### <a name="microsoft-dynamics-365-business-central--crm"></a>Microsoft Dynamics 365 Business Central — CRM

- Возможности продаж
- Шаблон Excel для просмотра сведений об организации
- Метки отчета Power BI

### <a name="microsoft-dynamics-365-business-central--finance"></a>Microsoft Dynamics 365 Business Central — Finance

- PowerBIFinance
- Шаблон Excel для просмотра сведений об организации
- Метки отчета Power BI

### <a name="microsoft-dynamics-365-business-central---sales"></a>Microsoft Dynamics 365 Business Central — Sales

- Продажа товаров по клиенту
- Панель мониторинга продажи
- Организация для просмотра шаблона Excel
- Метки отчета Power BI

> [!NOTE]
> [!INCLUDE [prodshort](includes/prodshort.md)] on-premises использует те же конечные точки веб-служб, что и [!INCLUDE [prodshort](includes/prodshort.md)] online.

## <a name="web-services"></a>Веб-службы

Простой способ найти веб-службы — найти *веб-службы* в [!INCLUDE[prodshort](includes/prodshort.md)]. На странице **Веб-службы** убедитесь, что поле **Опубликовать** выбрано для веб-служб, перечисленных выше.

## <a name="troubleshooting"></a>Устранение неполадок

Панель мониторинга Power BI основана на опубликованных веб-службах, которые перечислены выше, и содержит данные демонстрационной организации или вашей организации, если вы импортировали данные из текущего финансового решения. Однако если что-то работает некорректно, в этом разделе предложено обходное решение для типичных проблем.  

### <a name="you-do-not-have-a-power-bi-account"></a>У вас нет учетной записи Power BI

Учетная запись Power BI не была настроена. Для того, чтобы иметь действительную учетную запись Power BI, у вас должна быть лицензия, и вы должны были предварительно войти в Power BI, чтобы ваше рабочая область Power BI была создана.  

### <a name="message-there-are-no-enabled-reports-choose-select-report-to-see-a-list-of-reports-that-you-can-display"></a>Сообщение: "Включенные отчеты отсутствуют. Нажмите кнопку "Выбрать отчет", чтобы увидеть список отчетов, которые можно открыть."

Это сообщение появляется, если стандартный отчет не удалось развернуть в вашей рабочей области Power BI или если отчет был развернут, но его не удалось обновить. В этом случае перейдите к отчету в своей рабочей области Power BI, выберите **Набор данных**, **Настройки**, а затем вручную обновите учетные данные. После успешного обновления набора данных вернитесь в Business Central и вручную выберите отчет на странице **Выбрать отчеты**. 

### <a name="you-need-a-power-bi-pro-license-to-install-the-include-prodshortincludesprodshortmd-app-in-power-bi"></a>Вам необходима лицензия Power BI Pro для установки приложения [!INCLUDE [prodshort](includes/prodshort.md)] в Power BI

Приложения Power BI могут быть установлены только пользователями, которые имеют лицензию Power BI Pro. После того как приложение Power BI установлено, вы можете поделиться им с пользователями, которые не имеют лицензии Power BI Pro.  

### <a name="parameter-validation-failed-please-make-sure-all-parameters-are-valid"></a>"Ошибка при проверке параметра. Убедитесь, что все параметры допустимы"

Эта ошибка указывает на то, что еще один из параметров недействителен.

- Указанный параметр среды не соответствует ни одной из существующих рабочих сред или песочниц [!INCLUDE [prodshort](includes/prodshort.md)]. 
- Указанный параметр организации не соответствует ни одной из существующих организаций [!INCLUDE [prodshort](includes/prodshort.md)]. Проверьте название компании на странице **Организации** в [!INCLUDE [prodshort](includes/prodshort.md)].
- При подключении к [!INCLUDE [prodshort](includes/prodshort.md)] on-premises. вы ввели неверный URL-адрес. Вы можете проверить URL-адрес на странице **Веб-службы** в [!INCLUDE [prodshort](includes/prodshort.md)]  
- Порт не открыт, чтобы позволить запросу пройти через ваш брандмауэр.

### <a name="login-failed"></a>Сбой при входе

Если при попытке войти с использованием учетных данных [!INCLUDE [prodshort](includes/prodshort.md)] появляется ошибка "Сбой при входе", это может быть вызвано одной из следующих причин:

- У используемой учетной записи нет разрешений на извлечение данных [!INCLUDE [prodshort](includes/prodshort.md)] для вашей учетной записи. Убедитесь, что у вас есть разрешения на необходимые данные в [!INCLUDE [prodshort](includes/prodshort.md)] и попробуй еще раз.
- При подключении к [!INCLUDE [prodshort](includes/prodshort.md)] on-premises был выбран тип проверки подлинности, отличный от базового.
- Вы не ввели действительное имя пользователя или пароль.

### <a name="incorrect-company-name"></a>Неверное название организации

Распространенной ошибкой является ввод отображаемого имени организации вместо названия организации. Чтобы найти название организации, найдите **Организации**. Затем в поле **Название** введите название организации.

### <a name="the-key-didnt-match-any-rows-in-the-table"></a>Ключ не соответствует ни одной из строк в таблице

Если ввести недействительное имя организации в процессе подключения, можно получить сообщение об ошибке "Ключ не соответствует ни одной из строк в таблице". Укажите правильное название организации и попробуйте подключиться снова.

### <a name="historical-data-appears-to-be-missing"></a>Исторические данные отсутствуют

После того как приложение Power BI установлено, и ваши данные появились в Power BI, вы можете заметить, что отображаются не все ваши данные. Наборы данных фильтруются, чтобы возвращать только данные за предыдущие 365 дней. Это значение по умолчанию используется для ускорения создания отчетов.  

### <a name="i-only-see-data-for-a-single-company"></a>Я вижу данные только для одной организации

Приложение Power BI будет отображать только данные из организации [!INCLUDE [prodshort](includes/prodshort.md)], которая была определена, когда приложение Power BI было установлено. Данные из других организаций можно добавлять в отчеты, добавляя новые запросы, которые используют другие организации в качестве источника данных.  

## <a name="see-also"></a>См. также

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
