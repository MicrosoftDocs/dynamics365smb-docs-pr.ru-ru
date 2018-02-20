---
title: "Настройка отчетов для Finance and Operations, Business edition в Power BI | Microsoft Docs"
description: "Можно сделать данные Financials доступными в качестве источника данных в Power BI и создать мощные отчеты о состоянии вашего бизнеса."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 12/21/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 056761b398737bd052b68488756198051f0cdb9a
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="using-included365finincludesd365finmdmd-as-power-bi-data-source-for-building-reports"></a>Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных Power BI для создания отчетов
Можно сделать данные [!INCLUDE[d365fin](includes/d365fin_md.md)] доступными в качестве источника данных в Power BI и создать мощные отчеты о состоянии вашего бизнеса.  

> [!NOTE]  
> Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в Power BI. Кроме того, необходимо загрузить [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-power-bi-desktop"></a>Добавление [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных в Power BI Desktop
1. В Power BI Desktop в левой области навигации выберите **Получить данные**.
2. В окне **Получить данные** выберите **Веб-службы**, выберите **Dynamics 365 for Finance and Operations, Business edition**, а затем нажмите кнопку **Подключиться**.
3. Power BI отобразит мастер с руководством по [процессу подключения](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md). Первый шаг — вход в службу. Выберите **Войти** и выберите учетную запись для входа. Это должна быть та же учетная запись, которая использовалась для входа в [!INCLUDE[d365fin](includes/d365fin_md.md)].
4. Нажмите кнопку **Подключиться**, чтобы продолжить. Мастер Power BI отобразит список организаций и источников данных [!INCLUDE[d365fin](includes/d365fin_md.md)]. Эти источники данных представляют все веб-службы, которые вы опубликовали из каждой организации в [!INCLUDE[d365fin](includes/d365fin_md.md)].
5. Либо создайте новый URL-адрес веб-службы в [!INCLUDE[d365fin](includes/d365fin_md.md)], используя действие **Создать набор данных** на странице **Веб-службы** с помощью руководства по сопровождаемой настройке **Настройка отчетов** либо используя действие **Изменить в Excel** в любом списке.
6. Укажите данные, которые требуется добавить в модель данных, а затем нажмите кнопку **Загрузить**.
7. Повторите предыдущие шаги для добавления дополнительных данных [!INCLUDE[d365fin](includes/d365fin_md.md)] в модель данных Power BI.

> [!NOTE]  
> После успешного подключения к [!INCLUDE[d365fin](includes/d365fin_md.md)] выполнять повторный вход не требуется.

После загрузки данные отобразятся в правой области навигации на странице. На этом шаге вы успешно подключились с данным Finance and Operations, Business edition и готовы начать создание отчета Power BI. Дополнительные сведения см. в разделе [Документация Power BI](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).

## <a name="see-also"></a>См. также
[Бизнес-аналитика](bi.md)  
[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Импорт бизнес-данных из других финансовых систем](upload-data.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)   
[Финансы](finance.md)  
[Подключение Power BI к [!INCLUDE[d365fin](includes/d365fin_md.md)]](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md)  

