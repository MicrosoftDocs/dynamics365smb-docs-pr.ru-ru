---
title: Связывание данных с Flow | Документация Майкрософт
description: Вы можете сделать данные Business Central доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания автоматического бизнес-процесса.
documentationcenter: ''
author: bmeier90
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 10/01/2019
ms.author: bmeier
ms.openlocfilehash: 86178bafa806fb8cba531d5b78157437c242d432
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2305036"
---
# <a name="using-included365finincludesd365fin_mdmd-in-an-automated-workflow"></a>Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в автоматическом бизнес-процессе
Можно использовать данные [!INCLUDE[d365fin](includes/d365fin_md.md)] как часть рабочего процесса в Microsoft Flow.

> [!NOTE]
> В дополнение к Microsoft Flow, можно использовать функцию рабочего процесса в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Обратите внимание, что хотя это две отдельные системы для создания рабочих процессов, любой шаблон Flow, созданный в Microsoft Flow, добавляется в список рабочих процессов в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Дополнительные сведения см. в разделе [Рабочий процесс](across-workflow.md).  

> [!NOTE]  
> Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в Flow.  

## <a name="to-add-included365finincludesd365fin_mdmd-as-a-data-source-in-flow"></a>Добавление [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных в Flow
1. В браузере перейдите к [flow.microsoft.com](https://flow.microsoft.com/en-us/) и выполните вход.
2. Выберите **Мои Flow** в ленте вверху страницы.
3. Есть три способа создать поток: **Начните с шаблона**, **Начните с пустого** и **Начните с соединителя**. Шаблон представляет собой предопределенный поток Flow, уже созданный для пользователя. Чтобы использовать шаблон, просто выберите его и создайте подключение для каждого сервиса, используемого шаблоном. При использовании вариантов **Начните с пустого** и **Начните с соединителя** можно создать новый поток совершенно с нуля.
4. Чтобы создать поток с нуля, на странице **Мои потоки** выберите **Начните с пустого** и **Автоматизированный поток**.
5. Найдите соединитель **Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]**.
6. Укажите имя и выберите триггер, который вы будете использовать для своего потока.
7. Из списка доступных триггеров выберите один из доступных триггеров [!INCLUDE[d365fin](includes/d365fin_md.md)]:  
    
    *При запросе утверждения поставщика*,    
    *Если запрашивается утверждение строки финансового журнала*    
    *При удалении записи*,    
    *При изменении записи*,    
    *При создании записи*,    
    *Когда запись изменена*    
    *Если запрашивается утверждение раздела финансового журнала*   
    *Если запрашивается утверждение клиента*   
    *Если запрашивается утверждение товара*    
    *При запросе утверждения документа покупки* или     
     *При запросе утверждения документа покупки*.
     
8. Flow предложит выбрать среду и организацию в пределах вашего арендатора [!INCLUDE[d365fin](includes/d365fin_md.md)], а также все условия в ваших данных, которые вам требуется обнаруживать.

> [!NOTE]  
>   Соединитель [!INCLUDE[d365fin](includes/d365fin_md.md)] для Microsoft Flow поддерживает несколько рабочих сред и сред-песочниц. Если вы не создали несколько рабочих сред и сред-песочниц, **Рабочая среда** — единственный доступный для выбора вариант. 

На этом шаге вы успешно подключились с данным Business Central и готовы начать создание потока.

9. Для создания потока на основе шаблона выберите вариант **Начните с шаблона**.
10. Найдите шаблоны **Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]**.
11. Из списка доступных шаблонов выберите один из шаблонов, а затем выберите **Создать**.  

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
    *Запросить утверждение раздела финансового журнала Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]* или    
    *Запросить утверждение строк финансового журнала Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]*.  
12. Flow отобразит список служб, используемых в шаблоне Flow, и попытается автоматически подключиться к этим службам. Если вы ранее не подключались к какой-либо службе, вам будет предложено войти в каждую из служб, к которой нужно подключиться. После успешного установления подключения рядом с каждой из служб появится зеленая галочка. Выберите **Продолжить**.
13. Flow предложит вам выбрать среду и организацию с вашем арендаторе [!INCLUDE[d365fin_md](includes/d365fin_md.md)]. Поскольку каждый этап в потоке не зависит от следующего, при использовании шаблона Flow для [!INCLUDE[d365fin_md](includes/d365fin_md.md)] может потребоваться указать среду и организацию несколько раз.

Дополнительные сведения см. в разделе [Документация Flow](/flow/getting-started).

## <a name="see-also"></a>См. также
[Приступая к работе](product-get-started.md)  
[Рабочий процесс](across-workflow.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Управление пользователями и разрешениями](ui-how-users-permissions.md)   
[Управление рабочими процессами [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](across-use-workflows.md)  
[Настройка пользователя для утверждений](across-how-to-set-up-approval-users.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Финансы](finance.md)  
