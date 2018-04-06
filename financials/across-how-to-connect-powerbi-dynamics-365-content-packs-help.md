---
title: "Подключение Power BI к Finance and Operations, Business edition | Microsoft Docs"
description: "Анализ данных, бизнес-аналитика и КПЭ на основе данных Finance and Operations, Business edition становятся проще благодаря пакетам содержимого Power BI и Finance and Operations, Business edition."
author: SusanneWindfeldPedersen
ms.service: dynamics365-financials
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 02/05/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: b4e2e7bc1c2622d329c73ae5bf47b4accff10aa8
ms.openlocfilehash: aff8d95b13f795fa12d3146e5613712fb3baf9b4
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="connecting-power-bi-to-finance-and-operations-business-edition-content-packs"></a>Подключение Power BI к пакетам содержимого Finance and Operations, Business edition
Анализ данных Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] становится проще благодаря Power BI и пакетам содержимого Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]. Power BI извлекает ваши данные, а затем создает готовую панель мониторинга и отчеты на основе этих данных.

> [!NOTE]  
>  Вы должны иметь допустимую учетную запись в Dynamics 365 и Power BI. Кроме того, необходимо загрузить [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).  
>  Для пакетов содержимого Power BI требуются разрешения к таблицам, из которых извлекаются данные. Дополнительные сведения о требованиях см. ниже.  

## <a name="how-to-connect"></a>Подключение
1. Выберите **Получить данные** в нижней части левой панели навигации.  
![Переход к разделу "Получить данные"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)
2. В поле **Службы** выберите **Получить**. Откроется окно **AppSource** и **Приложения для приложений Power BI**.  
![Выбор пакетов содержимого из веб-служб](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)
3. Выберите **Приложения** на вкладке **Приложения для приложений Power BI**, выберите требуемый пакет содержимого **Microsoft Dynamics 365 for Finance and Operations** и щелкните **Получить сейчас**.  
![Выбор Dynamics 365 for Finance and Operations, Business edition и выбор "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)
4. При появлении запроса ведите имя *вашей организации* в [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)]. Это не отображаемое имя.  
![Выбор Dynamics 365 for Finance and Operations, Business edition и выбор "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)
5. После подключения панель мониторинга, отчет и набор данных будут автоматически отправлены в рабочую область Power BI. По завершении плитки обновятся для отображения данных из учетной записи.
![Выбор Dynamics 365 for Finance and Operations, Business edition и выбор "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)

## <a name="what-now"></a>Что теперь?

- Попробуйте [задать вопрос в поле "Вопросы и ответы"](https://docs.microsoft.com/en-us/power-bi/service-q-and-a) вверху панели мониторинга.  
- [Измените плитки](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) на панели мониторинга.  
- [Выберите плитку](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles), чтобы открыть основной отчет.  
- Хотя набор данных будет обновляться ежедневно, можно изменить график обновлений или попытаться обновить его по требованию с помощью функции **Обновить сейчас**.

## <a name="system-requirements"></a>Требования к системе
Чтобы импортировать данные [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] в Power BI, необходимо иметь разрешения на доступ к веб-службам, используемым для извлечения данных. Веб-службы, необходимые для каждого пакета содержимого:

**Microsoft Dynamics 365 for Finance and Operations, Business edition – CRM**
- SalesOpportunities
- ExcelTemplateViewCompany

**Microsoft Dynamics 365 for Finance and Operations, Business edition – Sales**
- ItemSalesbyCustomer
- SalesDashboard
- ExcelTemplateViewCompany

**Microsoft Dynamics 365 for Finance and Operations, Business edition – Finance**
- PowerBIFinance
- ExcelTemplateViewCompany

**Microsoft Dynamics 365 for Finance and Operations, Business edition – Jobs**
- Список работ
- Строки планирования работ
- Строки рабочего задания

**Microsoft Dynamics 365 for Finance and Operations, Business edition – Список клиентов**
- ItemSalesbyCustomer
- Power_BI_Item_Purchase_List
- Power_BI_Item_Sales_List
- SalesDashboard
- Power_BI_Customer_List
- ExcelTemplateViewCompany

**Microsoft Dynamics 365 for Finance and Operations, Business edition – Список товаров**
- ItemSalesbyCustomer
- Power_BI_Item_Purchase_List
- Power_BI_Item_Sales_List
- Товаров
- SalesDashboard
- ExcelTemplateViewCompany

**Microsoft Dynamics 365 for Finance and Operations, Business edition – Список поставщиков**
- ItemSalesbyCustomer
- Power_BI_Item_Purchase_List
- Power_BI_Item_Sales_List
- Товаров
- SalesDashboard
- Power_BI_Customer_List
- ItemSalesbyCustomer
- Power_BI_Vendor_List
- ExcelTemplateViewCompany

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
[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Импорт бизнес-данных из других финансовых систем](upload-data.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Финансы](finance.md)  
[Настройка отчетов для [!INCLUDE[d365fin](includes/d365fin_md.md)] в Power BI](across-how-use-financials-data-source-powerbi.md)  

