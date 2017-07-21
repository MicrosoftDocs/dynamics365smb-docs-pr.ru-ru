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
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 277dda7c954380138af1ecabc02d77121f35aac7
ms.contentlocale: ru-ru
ms.lasthandoff: 07/07/2017


---
# <a name="using-included365finincludesd365finmdmd-in-an-automated-workflow"></a>Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в автоматическом бизнес-процессе
Можно использовать данные [!INCLUDE[d365fin](includes/d365fin_md.md)] как часть рабочего процесса в Microsoft Flow.  

> [!NOTE]  
>   Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в Flow.  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-flow"></a>Добавление [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных в Flow
1. В браузере перейдите к [flow.microsoft.com](https://flow.microsoft.com/en-us/) и выполните вход.
2. Выберите **Мои Flow** в ленте вверху страницы.
3. В окне **Мои Flow** выберите параметр **Создать новый**.
4. Из списка доступных триггеров выберите один из двух доступных триггеров [!INCLUDE[d365fin](includes/d365fin_md.md)]: *При создании записи* или *При изменении записи*.
5. Flow отобразит страницу подключения с запросом на ввод информации, необходимой для подключения к данным [!INCLUDE[d365fin](includes/d365fin_md.md)]. Чтобы выполнить подключение, необходимо указать имя подключения, URL-адрес OData, имя пользователя, пароль и название организации.

   Для параметра *URL-адрес OData* можно скопировать URL-адрес OData V4 любой из веб-служб, перечисленных на странице **Веб-службы** в [!INCLUDE[d365fin](includes/d365fin_md.md)], например `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.  

   Для параметра *Название организации* используйте название, которое отображается в поле **Имя** в окне **Информация об организации** в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Если [!INCLUDE[d365fin](includes/d365fin_md.md)] содержит несколько организаций, выберите соответствующее название организации из списка в окне **Организации**. В обоих случаях убедитесь, что название, указываемое в мастере PowerApps точно соответствует тексту, отображаемому в [!INCLUDE[d365fin](includes/d365fin_md.md)], например `My Company`.

   В качестве имени пользователя и пароля используйте имя и ключ доступа веб-службы, определенные для учетной записи в окне **Пользователи** в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Например, ваше имя пользователя — *ADMIN*, а ключ доступа веб-службы, который используется как пароль, — *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*. Дополнительные сведения см. в разделе [Практическое руководство. Управление пользователями и разрешениями](ui-how-users-permissions.md).
6. Нажмите кнопку **Создать** внизу страницы, чтобы продолжить.

   Flow отобразит список таблиц, доступных для [!INCLUDE[d365fin](includes/d365fin_md.md)]. Эти таблицы или конечные точки представляют все веб-службы, которые вы опубликовали из [!INCLUDE[d365fin](includes/d365fin_md.md)].

   Либо создайте новый URL-адрес веб-службы в [!INCLUDE[d365fin](includes/d365fin_md.md)], используя действие **Создать набор данных** на странице **Веб-службы** с помощью руководства по сопровождаемой настройке **Настройка отчетов** либо используя действие **Изменить в Excel** в любом списке.
7. Выберите данные, которые будут использоваться в Flow.

На этом шаге вы успешно подключились с данным Dynamics 365 и готовы начать создание потока. Дополнительные сведения см. в разделе [Документация Flow](https://flow.microsoft.com/documentation/getting-started/).

## <a name="see-also"></a>См. также
[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Импорт бизнес-данных из других финансовых систем](upload-data.md)  
[Практическое руководство. Управление пользователями и разрешениями](ui-how-users-permissions.md)    
[Установка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Финансы](finance.md)  

