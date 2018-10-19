---
title: "Business Central и пакеты содержимого Power BI | Документы Майкрософт"
description: "Анализ данных, бизнес-аналитика и КПЭ на основе данных Business Central становятся проще благодаря пакетам содержимого Power BI и Business Central."
author: edupont04
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: eae7e97ec122b91a479ad956176a0b34b269bcb6
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="enabling-your-business-data-for-power-bi"></a>Включение бизнес-данных для Power BI
Анализ данных [!INCLUDE[d365fin](includes/d365fin_md.md)] становится проще благодаря Power BI и пакетам содержимого [!INCLUDE[d365fin](includes/d365fin_md.md)]. Power BI извлекает ваши данные и строки готовую панель мониторинга и отчеты на основе этих данных.  

Вы должны иметь допустимую учетную запись в Dynamics 365 и Power BI. Кроме того, необходимо загрузить [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/), если вы хотите создавать свои собственные отчеты Power BI. Для пакетов содержимого Power BI требуются разрешения к таблицам, из которых извлекаются данные. Дополнительные сведения о требованиях см. ниже.  

Майкрософт опубликовывала следующие пакеты содержимого:

| Приложение | Описанием |
| --- | --- |
| Microsoft Business Central | Обеспечивает панель мониторинга с ключевыми финансовыми данными в зависимости от времени, такими как прибыль и расходы, текущая прибыль и наличный цикл.|
| Microsoft Business Central - CRM | Предоставляет панель мониторинга с ключевыми данными о возможных сделках по продажам и контактах.  |
| Microsoft Business Central - Sales | Предоставляет панель мониторинга с ключевыми данными о продажах и запасах. |

## <a name="using-the-dashboards"></a>Использование панелей мониторинга
Каждый пакет содержимого предоставляет отчеты, которые можно подробно изучать:

* Выберите любой из визуальных элементов панели мониторинга, чтобы открыть один из отчетов.  
* Отфильтруйте отчет или добавьте поля, которые вы хотите отслеживать.  
* Прикрепите настроенное представление к панели мониторинга для дальнейшего отслеживания.  
  Можно обновить данные вручную, а также можно настроить график обновления. Дополнительные сведения см. в разделе [Настройка графика обновления](https://powerbi.microsoft.com/en-us/documentation/powerbi-refresh-scheduled-refresh/).  

Пакеты содержимого предварительно настроены для работы с данными из демонстрационной организации, которую вы получаете при регистрации в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Когда вы устанавливайте приложения в Power BI и подключаетесь к своим собственным данным, некоторые отчеты могут не работать, так как в них используются данные, которые отсутствуют в вашей организации. В таких случаях можно просто удалить этот отчет с панели мониторинга.  

> [!NOTE]  
>   Также можно создать собственные отчеты и панели мониторинга в Power BI на основании данных [!INCLUDE[d365fin](includes/d365fin_md.md)]. Дополнительные сведения см. в разделе [Подключение ваших бизнес-данных к Power BI](across-how-use-financials-data-source-powerbi.md).  

## <a name="how-to-connect"></a>Подключение
1. Выберите **Получить данные** в нижней части левой панели навигации.  
![Переход к разделу "Получить данные"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)

Можно также начать работать из Dynamics 365 Business Edition. Из ролевого центра перейдите к пункту **Выбор отчета** части ролевого центра Power BI. Выберите на ленте **Сервис** или **Моя организация**. Когда выбрано одно из этих действий, производится переход к галерее "Организация" в Power BI или к библиотеке сервисов в Power BI, которые также будут отфильтрованы для отображения только соответствующих пакетов, имеющих отношение к [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].

2. В поле **Службы** выберите **Получить**. Откроется окно **AppSource** и **Приложения для приложений Power BI**.  
![Выбор пакетов содержимого из веб-служб](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)
3. Выберите **Приложения** на вкладке **Приложения для приложений Power BI**, выберите требуемый пакет содержимого **Microsoft Dynamics 365 Business Central** и щелкните **Получить сейчас**.  
![Выберите Dynamics 365 Business Central и выберите "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)
4. При появлении запроса ведите имя *вашей организации* в [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)]. Это не отображаемое имя. Название организации можно найти на странице "Организации" в вашем экземпляре [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].  
![Выберите Dynamics 365 Business Central и выберите "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)
5. После подключения панель мониторинга, отчет и набор данных будут автоматически отправлены в рабочую область Power BI. По завершении плитки обновятся для отображения данных из вашей организации [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].
![Выберите Dynamics 365 Business Central и выберите "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)

## <a name="what-now"></a>Что теперь?

- Попробуйте [задать вопрос в поле "Вопросы и ответы"](https://docs.microsoft.com/en-us/power-bi/service-q-and-a-tips) вверху панели мониторинга.
- [Измените плитки](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) на панели мониторинга.  
- [Выберите плитку](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles), чтобы открыть основной отчет.  
- Хотя набор данных будет обновляться ежедневно, можно изменить график обновлений или попытаться обновить его по требованию с помощью функции **Обновить сейчас**.

## <a name="system-requirements"></a>Требования к системе
Чтобы импортировать данные [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] в Power BI, необходимо иметь разрешения на доступ к веб-службам, используемым для извлечения данных. Веб-службы, необходимые для каждого пакета содержимого:

## <a name="role-center-reports"></a>Отчеты ролевого центра

**Microsoft Dynamics 365 Business Central – CRM**
- Возможности продаж
- Организация для просмотра шаблона Excel
- Метки отчетов Power BI

**Microsoft Dynamics 365 Business Central – Finance**
- PowerBIFinance
- Организация для просмотра шаблона Excel
- Метки отчетов Power BI

**Microsoft Dynamics 365 Business Central – Jobs**
- Список работ
- Строки планирования работ
- Строки рабочего задания
- Метки отчетов Power BI
- Организация для просмотра шаблона Excel

**Microsoft Dynamics 365 Business Central - Sales**
- Панель мониторинга продажи
- Организация для просмотра шаблона Excel
- Метки отчетов Power BI

## <a name="list-page-reports"></a>Список отчетов страниц

**Microsoft Dynamics 365 Business Central – Customers List**
- Продажа товаров по клиенту
- Список покупок товаров Power BI
- Список продаж товаров Power BI
- Панель мониторинга продажи
- Список клиентов Power BI
- ExcelTemplateViewCompany
- Метки отчетов Power BI

**Microsoft Dynamics 365 Business Central - General Ledger Entries List**
- Список сумм ГК Power BI
- Сумма бюджета ГК Power BI
- ExcelTemplateViewCompany
- Метки отчетов Power BI

**Microsoft Dynamics 365 Business Central – Items List**
- Продажа товаров по клиенту
- Список покупок товаров Power BI
- Список продаж товаров Power BI
- Панель мониторинга продажи
- ExcelTemplateViewCompany
- Метки отчетов Power BI

**Microsoft Dynamics 365 Business Central – Jobs List**
- Список работ Power BI
- ExcelTemplateViewCompany
- Метки отчетов Power BI

**Microsoft Dynamics 365 Business Central – Purchase Invoices List**
- Список покупок Power BI
- ExcelTemplateViewCompany
- Метки отчетов Power BI

**Microsoft Dynamics 365 Business Central – Sales Orders List**
- Список продаж Power BI
- ExcelTemplateViewCompany
- Метки отчетов Power BI


**Microsoft Dynamics 365 Business Central – Vendors List**
- Список покупок товаров Power BI
- Список продаж товаров Power BI
- Список поставщиков Power BI
- ExcelTemplateViewCompany
- Метки отчетов Power BI

## <a name="web-services"></a>Веб-службы
Простой способ найти веб-службы — найти веб-службы в [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]. В списке проверьте, что установлен флажок "Опубликовать" для веб-служб, перечисленных выше.

## <a name="troubleshooting"></a>Устранение неполадок
Панель мониторинга Power BI основана на опубликованных веб-службах, которые перечислены выше, и содержит данные демонстрационной организации или вашей организации, если вы импортировали данные из текущего финансового решения. Однако если что-то работает некорректно, в этом разделе предложено обходное решение для типичных проблем.

### <a name="incorrect-company-name"></a>Неверное название организации  
Распространенной ошибкой является ввод отображаемого имени организации вместо названия организации. Чтобы найти название организации, найдите **Организации**. Затем в поле **Название** введите название организации.

### <a name="incorrect-user-name-and-password"></a>Неверные имя пользователя и пароль  
Имя пользователя и пароль, используемые для подключения, аналогичны используемым для подключения к учетной записи Microsoft Office 365.  

Также для пакетов содержимого требуется наличие учетной записи Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]. После ввода учетных данных будут автоматически обнаружены все арендаторы Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)], к которым у вас есть доступ. Если у вас нет лицензированной или пробной учетной записи Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)], вы получите сообщение об ошибке.

### <a name="the-key-didnt-match-any-rows-in-the-table"></a>Ключ не соответствует ни одной из строк в таблице
Если ввести недействительное имя организации в процессе подключения, можно получить сообщение об ошибке "Ключ не соответствует ни одной из строк в таблице". Укажите правильное название организации и попробуйте подключиться снова.

## <a name="see-also"></a>См. также
[Начало работы с Power BI](https://docs.microsoft.com/en-us/power-bi/service-get-started)  
[Power BI — основные понятия](https://docs.microsoft.com/en-us/power-bi/service-basic-concepts)  
[Бизнес-аналитика](bi.md)  
[Приступая к работе](product-get-started.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных Power BI](across-how-use-financials-data-source-powerbi.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных PowerApps](across-how-use-financials-data-source-powerapps.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в Microsoft Flow](across-how-use-financials-data-source-flow.md)   

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  

