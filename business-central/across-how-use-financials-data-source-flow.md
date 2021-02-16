---
title: Связывание данных с Power Automate | Microsoft Docs
description: Вы можете сделать данные Business Central доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания автоматического бизнес-процесса.
author: bmeier90
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.search.keywords: workflow, OData, Power App, SOAP
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: f44b727a353208d1b2b8f5d918400de1687acc52
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4754546"
---
# <a name="using-prod_short-in-an-automated-workflow"></a>Использование [!INCLUDE[prod_short](includes/prod_short.md)] в автоматическом бизнес-процессе

Можно использовать данные [!INCLUDE[prod_short](includes/prod_short.md)] как часть рабочего процесса в Microsoft Power Automate.

> [!NOTE]
> В дополнение к Power Automate, можно использовать функцию рабочего процесса в [!INCLUDE[prod_short](includes/prod_short.md)]. Обратите внимание, что хотя это две отдельные системы для создания рабочих процессов, любой шаблон рабочего процесса, созданный в Power Automate, добавляется в список рабочих процессов в [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Рабочий процесс](across-workflow.md).  

> [!NOTE]  
> Вы должны иметь допустимую учетную запись в [!INCLUDE[prod_short](includes/prod_short.md)] и в Power Automate.  

## <a name="to-add-prod_short-as-a-data-source-in-power-automate"></a>Добавление [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных в Power Automate

1. В браузере перейдите к [flow.microsoft.com](https://flow.microsoft.com) и выполните вход.
2. Выберите **Мои потоки** в ленте вверху страницы.
3. Есть три способа создать поток: **Начните с шаблона**, **Начните с пустого** и **Начните с соединителя**. Шаблон представляет собой предопределенный поток, уже созданный для пользователя. Чтобы использовать шаблон, просто выберите его и создайте подключение для каждого сервиса, используемого шаблоном. При использовании вариантов **Начните с пустого** и **Начните с соединителя** можно создать новый поток совершенно с нуля.
4. Чтобы создать поток с нуля, на странице **Мои потоки** выберите **Начните с пустого** и **Автоматизированный поток**.
5. Найдите соединитель **Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]**.
6. Укажите имя и выберите триггер, который вы будете использовать для своего потока.
7. Из списка доступных триггеров выберите один из доступных триггеров [!INCLUDE[prod_short](includes/prod_short.md)]:  

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

8. Power Automate предложит выбрать среду и организацию в пределах вашего арендатора [!INCLUDE[prod_short](includes/prod_short.md)], а также все условия в ваших данных, которые вам требуется обнаруживать.

    > [!NOTE]
    > Соединитель [!INCLUDE[prod_short](includes/prod_short.md)] для Power Automate поддерживает несколько рабочих сред и сред-песочниц. Если вы не создали несколько рабочих сред и сред-песочниц, **Рабочая среда** — единственный доступный для выбора вариант.  

    На этом шаге вы успешно подключились к данным Business Central[!INCLUDE[prod_short](includes/prod_short.md)] и готовы начать создание потока.

9. Для создания потока на основе шаблона выберите вариант **Начните с шаблона**.
10. Найдите шаблоны **Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]**.
11. Из списка доступных шаблонов выберите один из шаблонов, а затем выберите **Создать**.  

    *Запросить утверждение для заказа на продажу Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]*,  
    *Запросить утверждение для предложения по продаже Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]*,  
    *Запросить утверждение для счета на продажу Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]*,  
    *Запросить утверждение для кредит-ноты продажи Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]*,  
    *Запросить утверждение для клиента Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]*,  
    *Запросить утверждение для заказа на покупку Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]*,  
    *Запросить утверждение для счета на покупку Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]*,  
    *Запросить утверждение для кредит-ноты покупки Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]*,  
    *Запросить утверждение для товара Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]*,  
    *Запросить утверждение для поставщика Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]*,  
    *Запросить утверждение раздела финансового журнала Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]* или    
    *Запросить утверждение строк финансового журнала Microsoft [!INCLUDE[prod_long](includes/prod_long.md)]*.  
12. Power Automate отобразит список служб, используемых в шаблоне потока, и попытается автоматически подключиться к этим службам. Если вы ранее не подключались к какой-либо службе, вам будет предложено войти в каждую из служб, к которой нужно подключиться. После успешного установления подключения рядом с каждой из служб появится зеленая галочка. Выберите **Продолжить**.
13. Power Automate предложит вам выбрать среду и организацию в вашем арендаторе [!INCLUDE[prod_short](includes/prod_short.md)]. Поскольку каждый этап в потоке не зависит от следующего, при использовании шаблона [!INCLUDE[prod_short](includes/prod_short.md)] Power Automate может потребоваться указать среду и организацию несколько раз.

Дополнительные сведения см. в разделе [Документация по Power Automate](/power-automate/getting-started).

## <a name="see-also"></a>См. также

[Приступая к работе](product-get-started.md)  
[Рабочий процесс](across-workflow.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Назначение разрешений пользователям и группам](ui-define-granular-permissions.md)  
[Управление рабочими процессами [!INCLUDE[prod_long](includes/prod_long.md)]](across-use-workflows.md)  
[Настройка пользователя для утверждений](across-how-to-set-up-approval-users.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Финансы](finance.md)  
