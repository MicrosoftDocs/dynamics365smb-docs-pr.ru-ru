---
title: "Связывание данных с Flow | Документы Майкрософт"
description: "Данные Financials можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания автоматического бизнес-процесса."
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 01/25/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: ef4d841723b6bb0af37695a8c3ed1d805319be78
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="using-included365finincludesd365finmdmd-in-an-automated-workflow"></a>Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в автоматическом бизнес-процессе
Можно использовать данные [!INCLUDE[d365fin](includes/d365fin_md.md)] как часть рабочего процесса в Microsoft Flow.  

> [!NOTE]  
>   Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в Flow.  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-flow"></a>Добавление [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных в Flow
1. В браузере перейдите к [flow.microsoft.com](https://flow.microsoft.com/en-us/) и выполните вход.
2. Выберите **Мои Flow** в ленте вверху страницы.
3. В окне **Мои Flow** выберите параметр **Создать новый**.
4. Из списка доступных триггеров выберите один из доступных триггеров [!INCLUDE[d365fin](includes/d365fin_md.md)]:  
    *При создании записи*  
    *При удалении записи*  
    *При изменении записи*  
    *Если запрашивается утверждение клиента*  
    *Если запрашивается утверждение раздела финансового журнала*  
    *Если запрашивается утверждение строки финансового журнала*  
    *Если запрашивается утверждение товара*  
    *Если запрашивается утверждение документа покупки*  
    *Если запрашивается утверждение документа продажи*, или  
    *Если запрашивается утверждение поставщика*
5. Flow отобразит запрос на ввод информации, необходимой для подключения к данным [!INCLUDE[d365fin](includes/d365fin_md.md)]. При выборе одного из следующих триггеров *При создании записи*, *При изменении записи* или *При удалении записи* необходимо выбрать название организации или имя таблицы. В случае любого другого триггера для подключения требуется только название организации.

   Flow отобразит список организаций и таблиц, доступных для [!INCLUDE[d365fin](includes/d365fin_md.md)]. Эти таблицы или конечные точки представляют все веб-службы, которые вы опубликовали из [!INCLUDE[d365fin](includes/d365fin_md.md)].

   Либо создайте новый URL-адрес веб-службы в [!INCLUDE[d365fin](includes/d365fin_md.md)], используя действие **Создать набор данных** на странице **Веб-службы** с помощью руководства по сопровождаемой настройке **Настройка отчетов** либо используя действие **Изменить в Excel** в любом списке.

На этом шаге вы успешно подключились с данным Finance and Operations, Business edition и готовы начать создание потока. Дополнительные сведения см. в разделе [Документация Flow](https://flow.microsoft.com/documentation/getting-started/).

При устранении неполадок с Microsoft Flow см. раздел [Устранение неполадок при интеграции с Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).

## <a name="see-also"></a>См. также
[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Импорт бизнес-данных из других финансовых систем](upload-data.md)  
[Управление пользователями и разрешениями](ui-how-users-permissions.md)    
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Финансы](finance.md)  

