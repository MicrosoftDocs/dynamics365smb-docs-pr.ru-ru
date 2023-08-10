---
title: Управление работой нескольких компаний в разделе организаций
description: 'Узнайте о разделе организаций в Dynamics 365 Business Central, который вы используете для управления своей работой в нескольких компаниях.'
author: edupont04
ms.topic: conceptual
ms.search.keywords: 'accountant, accounting, financial report'
ms.search.form: '1151, 1154, 1165, 1166'
ms.date: 04/01/2021
ms.author: edupont
---

# <a name="manage-work-across-multiple-companies-in-the-company-hub"></a>Управление работой нескольких компаний в разделе организаций

Некоторые люди работают в нескольких компаниях в [!INCLUDE [prod_short](includes/prod_short.md)], а некоторые также работают в нескольких организациях, например, внешние бухгалтеры или сотрудники и менеджеры корпораций с несколькими дочерними компаниями. Для этих и многих других пользователей Company Hub играет роль домашней страницы, которая позволяет получить финансовый обзор всех организаций и сред. Она служит для управления работой в различных средах, в которых они работают, — в различных организациях, средах и регионах.  

Вы можете получить доступ к разделу организации, переключившись на роль **Раздел организации** в "Мои настройки" или открыв страницу **Раздел организации** напрямую. Вы можете выполнять одну и ту же работу в обоих местах, но действия в меню расположены немного по-разному.  

[![Отображает страницу Company Hub, на которой перечислены все компании.](media/company-hub.png)](media/company-hub.png#lightbox)  

> [!NOTE]
> Вы можете подключить к корпоративному узлу столько компаний, сколько вам нужно. Однако вы можете подключить узел компании только к компаниям, которые размещены в [!INCLUDE [prod_short](includes/prod_short.md)] Online.

## <a name="company-hub-home-page"></a>Домашняя страница раздела организации

Если вы используете роль **Раздел организации**, ваша домашняя страница показывает список компаний, к которым у вас есть доступ, включая информацию о ключевых точках интереса (KPI) и ссылки для открытия каждой компании. <!--You can customize the dashboard to show the data points that you want to see by adding or removing columns. For example, you might want to see taxes that are due, how many open sales documents each company has, or the number of purchase invoices that are due next week. You can configure the view to suit your needs. If you have added many companies, you can use filters to sort your view.--> Выберите действия **Раздел организации**, чтобы открыть раздел организации, где вы можете более тесно сотрудничать с каждой компанией.  

> [!TIP]
> Чтобы получить доступ к конкретной компании в [!INCLUDE [prod_short](includes/prod_short.md)], выберите название компании или выберите пункт меню **Перейти к компании** — вы автоматически авторизуетесь в новой вкладке браузера.

:::image type="content" source="media/company-hub-company-list-actions.png" alt-text="Действия для компании, которая указана в разделе организации.":::

Вы можете добавлять новые компании, например, когда у вас появляется новый клиент или когда ваша корпорация добавляет новую дочернюю компанию. Для получения дополнительной информации см. [Добавление компании в ваш раздел организации](company-hub-add-company.md).  

> [!TIP]
> Чтобы обновить данные в раздел организации, у вас должен быть доступ к данным в компаниях, из которых они поступают.

<!--## Company details

In the **Company Hub** page, you can see more information about each company by choosing the name of the company that you want to learn more about. This opens the **Company Details** pane, where you can see additional information, such as the following:  

* Cash account balances  
* Cash flow forecast  
* Overdue purchase invoices  
* Overdue sales invoices  

> [!TIP]
> You can launch predefined Excel workbooks from the **Reports** tab in the ribbon. These Excel workbooks are designed as ready-to-print key financial statements and reports, but you can also modify them to fit your needs. For more information, see [Analyzing Financial Statements in Microsoft Excel](finance-analyze-excel.md).  

Otherwise, close the details pane and continue to the next company.  -->

## <a name="assigned-tasks"></a>Назначенные задачи

В [!INCLUDE [prod_short](includes/prod_short.md)] вы можете назначать задачи себе и другим пользователям, а другие пользователи могут назначать задачи вам. Раздел организации позволяет получить представление о назначенных задачах по каждой компании; кроме того, вы можете открыть список всех назначенных задач, выбрав **Мои задачи пользователя** на странице **Главная**.  

<!--In the client company, you also have cues that call out tasks assigned to you in this particular client.  -->

### <a name="my-user-tasks"></a>Мои задачи пользователя

Список **Мои задачи пользователя** поможет вам расставить приоритеты и спланировать свой рабочий день: в нем отображается дополнительная информация о задачах, назначенных вам различными вашими компаниями.  

Вы можете сортировать его по сроку выполнения, например, или по любому другому типу данных, чтобы расставить приоритеты для планирования своей работы. По умолчанию в списке отображаются все назначенные вам задачи, однако вы можете настроить фильтры, чтобы в нем отображались только задачи, помеченные как высокоприоритетные, например.  

Чтобы выбрать задачу, выберите ее в списке ожидающих задач пользователя. На ленте ссылка **Перейти к элементу задачи** открывает страницу, на которой можно сделать работу.  

После завершения задачи отметьте ее как выполненную.  

Для получения дополнительной информации о компаниях и средах см. [Ссылки на среды](company-hub-add-company.md#environment-links).  

## <a name="access-the-company-hub"></a>Доступ к разделу организации

[!INCLUDE [2023rw1-sec-group-short](includes/2023rw1-sec-group-short.md)]

Чтобы получить доступ к разделу организации, вы должны иметь доступ группы пользователей *РАЗДЕЛ ОРГАНИЗАЦИИ D365* или набор разрешений *РАЗДЕЛ ОРГАНИЗАЦИИ D365*. У вас также должен быть доступ к компаниям, перечисленным в вашем разделе организации, что означает, что вы должны быть пользователем этих компаний. Для получения дополнительной информации см. раздел [Создание пользователей в соответствии с лицензиями](ui-how-users-permissions.md).  

> [!IMPORTANT]
> Раздел организации — это список масштаба всей компании, поэтому любой пользователь, которому предоставлен доступ к разделу организации, сможет увидеть все компании в своем собственном клиенте [!INCLUDE [prod_short](includes/prod_short.md)] и все KPI компаний, к которым у него есть доступ.

Если вы не можете найти раздел организации и знаете, что вам был предоставлен доступ к нему, уточните у своего администратора, указан ли раздел организации в списке на странице **Управление расширениями**. Дополнительные сведения см. в разделе [Настройка Business Central с помощью расширений](ui-extensions.md).  

## <a name="set-up-the-company-hub"></a>Настройка раздела организации

Чтобы начать использовать раздел организации, вы должны добавить одну или несколько компаний на свою управления мониторинга. Для получения дополнительной информации см. [Добавление компании в ваш раздел организации](company-hub-add-company.md).  

Но чтобы добавить компанию, вам должен быть предоставлен доступ к одному или нескольким экземплярам [!INCLUDE [prod_short](includes/prod_short.md)] в дополнение к компании, в которой вы используете раздел организации.  

Например, если вы бухгалтер, ваши клиенты могут пригласить вас в свои [!INCLUDE [prod_short](includes/prod_short.md)]. Для получения дополнительной информации см. [Приглашение внешнего бухгалтера в ваш Business Central](finance-accounting.md#inviteaccountant).  

Администраторы могут использовать то же руководство по вспомогательной настройке, чтобы добавить вас в свои [!INCLUDE [prod_short](includes/prod_short.md)], или они могут добавить вас в соответствующую учетную запись Azure AD в центре администрирования Microsoft 365. Дополнительные сведения см. в разделе [Управление пользователями и группами](/microsoft-365/admin/add-users/?view=o365-worldwide&preserve-view=true).  

## <a name="see-also"></a>См. также

[Добавьте компании в свой раздел организации](company-hub-add-company.md)  
[Работа бухгалтера в Business Central](finance-accounting.md)  
[Раздел организации для расширения Business Central](ui-extensions-company-hub.md)  
[Изменение базовых настроек](ui-change-basic-settings.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
