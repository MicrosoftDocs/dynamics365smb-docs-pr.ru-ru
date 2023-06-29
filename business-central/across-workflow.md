---
title: Рабочие процессы в Dynamics 365 Business Central
description: 'Используйте встроенные возможности рабочего процесса, чтобы настроить рабочие процессы утверждения в дополнение к автоматизированным рабочим процессам на основе Power Automate. Вы можете настроить этапы назначения задач разным людям в рамках разных задач бизнес-процесса.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.date: 10/10/2022
ms.custom: bap-template
---
# <a name="workflows-in-dynamics-365-business-central"></a><a name="workflows-in-dynamics-365-business-central"></a>Рабочие процессы в Dynamics 365 Business Central

Можно настроить и использовать рабочие процессы для связи задач бизнес-процесса, выполняемых различными пользователями. Системные задачи, такие как автоматическая публикация, могут включаться в рабочие процессы в качестве шагов. Перед системными задачами или после них могут выполняться пользовательские задачи. Типичные шаги рабочего процесса — запрос и выдача разрешения на создание новых записей.

Версия [!INCLUDE [prod_short](includes/prod_short.md)] по умолчанию поддерживает три типа рабочих процессов:
  
* Рабочие процессы Power Automate

  * Автоматизированные потоки, запускаемые событиями (такими как создание, изменение или удаление записей и документов) в [!INCLUDE[prod_short](includes/prod_short.md)]. Также включаются создаваемые в Power Automate потоки утверждения, которые запускаются при запросе утверждения в [!INCLUDE[prod_short](includes/prod_short.md)].
  * Мгновенные потоки, запускаемые вручную с помощью действия **Автоматизация** из списков, карточек и страниц документов.

    Создайте и вручную запустите поток Power Automate для записи [!INCLUDE[prod_short](includes/prod_short.md)], такой как клиент, товар или заказ на продажу, с возможностью управления информацией как внутри, так и снаружи (с использованием встроенных инструментов).

* Рабочие процессы утверждения на основе встроенных шаблонов рабочих процессов

  На странице **Шаблоны рабочих процессов** вы можете увидеть все доступные рабочие процессы. Пробная версия [!INCLUDE[prod_short](includes/prod_short.md)] содержит множество заранее настроенных рабочих процессов, представленных шаблонами, которые можно скопировать для создания новых. Когда вы открываете шаблон со страницы **Шаблоны рабочего процесса** и название рабочего процесса начинается с *MS-*, тогда этот шаблон был добавлен Microsoft.

## <a name="power-automate-flows"></a><a name="power-automate-flows"></a>Рабочие процессы Power Automate

Используя [!INCLUDE [prod_short](includes/prod_short.md)] Online, вы можете зарегистрироваться в Power Automate для создания мощных автоматизированных рабочих процессов. Эти рабочие процессы будут запускаться из [!INCLUDE [prod_short](includes/prod_short.md)]. Эти потоки могут соединять внутренние и внешние источники данных и инструменты — без знания программирования.

|**Задача** |**Раздел**|
|-------|-------|
|Начало работы с Power Automate и создание потоков, запуск мгновенных потоков|[Использование потоков Power Automate в [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-financials-data-source-flow.md)|
|Узнайте как создавать потоки, редактировать их и управлять ими|[Настройка автоматизированных потоков](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) и [Настройка мгновенных потоков](/dynamics365/business-central/dev-itpro/powerplatform/instant-flows)|
|Настройка интеграции Power Automate с [!INCLUDE[prod_short](includes/prod_short.md)] для пользователей в качестве администратора|[Настройка интеграции с Power Automate](/dynamics365/business-central/dev-itpro/powerplatform/power-automate-setup)|

## <a name="approval-workflows"></a><a name="approval-workflows"></a>Рабочие процессы утверждения

Создайте рабочий процесс утверждения, указав что запускает рабочий процесс и что происходит дальше, следующим образом:

* Событие рабочего процесса, которое модерируется условиями события.
* Ответ рабочего процесса, который модерируется вариантами ответа.

Для определения шагов рабочего процесса необходимо заполнить поля в строках рабочего процесса, используя значения событий и ответов, представляющих поддерживаемые сценарии.

Примеры событий рабочих процессов утверждения включают, среди прочего, создание заказов на продажу или покупку/предложений/счетов, изменение цен, редактирование поставщика или клиента и др.

[!INCLUDE[workflow](includes/workflow.md)]

| **Задача** | **Раздел** |
|--|--|
| Настройте пользователей рабочего процесса утверждения, определите, как пользователи будут получать уведомления, и создайте новые рабочие процессы. (Для создания новых рабочих процессов для неподдерживаемых сценариев реализуйте необходимые элементы рабочего процесса путем настройки кода приложения.) | [Настройка рабочих процессов утверждения](across-set-up-workflows.md) |
| Включите рабочие процессы утверждения, выполните действия над уведомлениями рабочего процесса, включая запрос утверждения и утверждение шага рабочего процесса. Архивируйте и удалите рабочие процессы. | [Использование рабочих процессов утверждения](across-use-workflows.md) |

<!--
| Integrate company data with Power Automate workflows, using both internal and external sources and events to create and automate tasks or workflows. | [Use Power Automate Flows in [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-financials-data-source-flow.md) |-->

## <a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/create-workflows/)

## <a name="see-also"></a><a name="see-also"></a>См. также

[Продажи](sales-manage-sales.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Управление проектами](projects-manage-projects.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Устранение неполадок в автоматизированных рабочих процессах [!INCLUDE[prod_short](includes/prod_short.md)]](across-flow-troubleshoot.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
