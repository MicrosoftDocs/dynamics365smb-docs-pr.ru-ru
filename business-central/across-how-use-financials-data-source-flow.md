---
title: "Связывание данных с Flow | Документы Майкрософт"
description: "Данные Financials можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания автоматического бизнес-процесса."
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 01/25/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 23e9ebbb75d23595d568d022526e551bf590a979
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

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
    *Если запрашивается утверждение клиента*  
    *Если запрашивается утверждение раздела финансового журнала*  
    *Если запрашивается утверждение строки финансового журнала*  
    *Если запрашивается утверждение товара*  
    *Если запрашивается утверждение документа покупки*  
    *Если запрашивается утверждение документа продажи*, или  
    *Если запрашивается утверждение поставщика*
5. Поток предложит вам выбрать организацию с вашем арендаторе [!INCLUDE[d365fin](includes/d365fin_md.md)]. Поскольку каждый этап во Flow не зависит от следующего, может потребоваться определить организацию несколько раз при использовании шаблона [!INCLUDE[d365fin](includes/d365fin_md.md)].

На этом шаге вы успешно подключились с данным Business Central и готовы начать создание потока. Дополнительные сведения см. в разделе [Документация Flow](https://flow.microsoft.com/documentation/getting-started/).

При устранении неполадок с Microsoft Flow см. раздел [Устранение неполадок при интеграции с Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).

## <a name="see-also"></a>См. также
[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Импорт бизнес-данных из других финансовых систем](upload-data.md)  
[Управление пользователями и разрешениями](ui-how-users-permissions.md)    
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Финансы](finance.md)  

