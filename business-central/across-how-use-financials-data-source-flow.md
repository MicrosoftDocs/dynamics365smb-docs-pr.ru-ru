---
title: "Связывание данных с Flow | Документы Майкрософт"
description: "Вы можете сделать данные Business Central доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания автоматического бизнес-процесса."
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 05/09/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: e3917573a912a4e51416c4e926443c87513728fe
ms.openlocfilehash: 4dd987ee51cd2b5d8575d6d97ad21d00ec85739a
ms.contentlocale: ru-ru
ms.lasthandoff: 06/01/2018

---
# <a name="using-included365finincludesd365finmdmd-in-an-automated-workflow"></a>Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в автоматическом бизнес-процессе
Можно использовать данные [!INCLUDE[d365fin](includes/d365fin_md.md)] как часть рабочего процесса в Microsoft Flow.  

> [!NOTE]  
>   Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в Flow.  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-flow"></a>Добавление [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных в Flow
1. В браузере перейдите к [flow.microsoft.com](https://flow.microsoft.com/en-us/) и выполните вход.
2. Выберите **Мои Flow** в ленте вверху страницы.
3. Предусмотрено 2 способа создания потока Flow; **Создать из шаблона** и **Создать новый**. Шаблон представляет собой предопределенный поток Flow, уже созданный для пользователя.  Чтобы использовать шаблон, просто выберите его и создайте подключение для каждого сервиса, используемого шаблоном. Пустой шаблон позволяет создать полностью новый поток Flow.
4. Чтобы создать полностью новый поток, в окне **Мои Flow** выберите вариант **Создать новый**.
5. Найдите соединитель **Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]**.
6. Из списка доступных триггеров выберите один из доступных триггеров [!INCLUDE[d365fin](includes/d365fin_md.md)]:  
    *Если запрашивается утверждение клиента*  
    *Если запрашивается утверждение раздела финансового журнала*  
    *Если запрашивается утверждение строки финансового журнала*  
    *Если запрашивается утверждение товара*  
    *Если запрашивается утверждение документа покупки*  
    *Если запрашивается утверждение документа продажи*, или  
    *Если запрашивается утверждение поставщика*.
7. Поток Flow предлагает выбрать организацию в пределах вашего арендатора [!INCLUDE[d365fin](includes/d365fin_md.md)], а также все условия в ваших данных, которые вам требуется обнаруживать.

На этом шаге вы успешно подключились с данным Business Central и готовы начать создание потока.

8. Для создания из шаблона выберите вариант **Создать из шаблона**.
9. Найдите шаблоны **Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]**.
10. Из списка доступных шаблонов выберите один из шаблонов.  
    *Запросить утверждение для заказа на продажу Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*,  
    *Запросить утверждение для предложения по продаже Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*,  
    *Запросить утверждение для счета на продажу Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*,  
    *Запросить утверждение для кредит-ноты продажи Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*,  
    *Запросить утверждение для клиента Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*,  
    *Запросить утверждение для заказа на покупку Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*,  
    *Запросить утверждение для счета на покупку Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*,  
    *Запросить утверждение для кредит-ноты покупки Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*,  
    *Запросить утверждение для товара Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*,  
    *Запросить утверждение для поставщика Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*,  
    *Запросить утверждение раздела финансового журнала Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*.  
    *Запросить утверждение строк финансового журнала Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*.  
11. Поток предложит вам выбрать организацию с вашем арендаторе [!INCLUDE[d365fin_md](includes/d365fin_md.md)]. Поскольку каждый этап в потоке не зависит от следующего, при использовании шаблона Flow [!INCLUDE[d365fin_md](includes/d365fin_md.md)] может потребоваться определить организацию несколько раз.

> [!NOTE]  
> Шаблон Flow [!INCLUDE[d365fin_md](includes/d365fin_md.md)] интегрируется с базовым механизмом обработки бизнес-процессов [!INCLUDE[d365fin_md](includes/d365fin_md.md)]. Это означает, что каждый раз, когда вы используете один из шаблонов для создания потока, создается соответствующий бизнес-процесс в [!INCLUDE[d365fin_md](includes/d365fin_md.md)]. Дополнительные сведения см. в разделе [Рабочий процесс](across-workflow.md).

Дополнительные сведения см. в разделе [Документация Flow](https://docs.microsoft.com/en-us/flow/getting-started).

При устранении неполадок с Microsoft Flow см. раздел [Устранение неполадок при интеграции с Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).

## <a name="see-also"></a>См. также
[Приступая к работе](product-get-started.md)  
[Рабочий процесс](across-workflow.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Управление пользователями и разрешениями](ui-how-users-permissions.md)   
[Управление рабочими процессами [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](across-use-workflows.md)  
[Настройка пользователя для утверждений](across-how-to-set-up-approval-users.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Финансы](finance.md)  

