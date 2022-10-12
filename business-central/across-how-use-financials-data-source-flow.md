---
title: Использование потоков Power Automate в Business Central
description: Настройте и используйте потоки Power Automate для создания и изменения данных Business Central.
author: jswymer
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, OData, Power App, SOAP, Power Automate,
ms.search.form: 1500,
ms.date: 09/13/2022
ms.author: edupont
ms.openlocfilehash: 5fe089c0330a8d2b7a71f4907212665722d27d38
ms.sourcegitcommit: 8ad79e0ec6e625796af298f756a142624f514cf3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2022
ms.locfileid: "9606526"
---
# <a name="use-power-automate-flows-in-prod_short"></a>Использование потоков Power Automate в [!INCLUDE[prod_short](includes/prod_short.md)]

Можно использовать данные [!INCLUDE[prod_short](includes/prod_short.md)] как часть рабочего процесса в Microsoft Power Automate. Создавайте собственные потоки и подключайтесь к своим данным из внутренних и внешних источников с помощью соединителя [!INCLUDE [prod_short](includes/prod_short.md)].

> [!NOTE]
> Вы должны иметь допустимую учетную запись как в [!INCLUDE[prod_short](includes/prod_short.md)], так и в Power Automate.  

> [!TIP]
> Кроме Power Automate, в [!INCLUDE[prod_short](includes/prod_short.md)] можно использовать шаблоны рабочего процесса утверждения. Хотя это две отдельные системы для создания рабочих процессов, любой шаблон рабочего процесса утверждения, созданный в Power Automate, добавляется в список рабочих процессов в [!INCLUDE[prod_short](includes/prod_short.md)]. Подробнее см. в разделе [Рабочие процессы](across-workflow.md).

Потоки Power Automate запускаются такими событиями, как создание, изменение или удаление записей и документов (автоматические потоки). Потоки также могут запускаться по заданному пользователем расписанию (запланированные потоки) или по запросу (мгновенные потоки).

## <a name="power-automate-features-in-prod_short"></a>Возможности Power Automate в [!INCLUDE[prod_short](includes/prod_short.md)]

Потоки расширяют встроенные функции рабочих процессов утверждения, доступные в [!INCLUDE[prod_short](includes/prod_short.md)], не требуя знаний в области программирования, и могут быть связаны с широким спектром событий и ответов, таких как изменения записей, обновления внешних файлов, проводка документов, а также с различными службами Microsoft и сторонних поставщиков, такими как Microsoft Outlook, Microsoft Excel, Microsoft Dataverse, Microsoft Teams, Microsoft SharePoint, Microsoft Power Apps и более.

Так, например, новый счет продажи может инициировать рабочий процесс для запроса утверждения, для которого могут быть установлены разные события в зависимости от ответа утверждающего. При отрицательном ответе отправителю запроса на утверждение отправляется уведомление и электронное письмо. Положительный ответ одновременно обновляет электронную таблицу Excel, расположенную в папке SharePoint, и отправляет обновление в чат Teams.

Мгновенные потоки работают аналогично пакетным ярлыкам, выполняя несколько длительных шагов с помощью нескольких нажатий кнопок и запуская их с определенных страниц или таблиц. Например, поток может добавить кнопку в меню действий на странице **Поставщики**, чтобы блокировать платежи поставщику и, в то же время, отправлять настраиваемые электронные письма контактному лицу поставщика и закупщикам вашей компании, а также обновлять контакт в Outlook.

## <a name="automated-workflows"></a>Автоматизированные рабочие процессы

С помощью Power Automate вы можете создавать бизнес-процессы непосредственно внутри компании и полагаться на разработчиков-любителей. Автоматизированные рабочие процессы могут быть запущены как внутренними, так и внешними событиями в [!INCLUDE[prod_short](includes/prod_short.md)], а также можно настроить периодический запуск. Узнайте больше и получите инструкции о том, как создавать рабочие процессы, в статье [Настройка автоматизированных рабочих процессов](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) в материалах по администрированию.

## <a name="instant-flows"></a>Мгновенные потоки

[!INCLUDE [prod_short](includes/prod_short.md)] может запускать потоки Power Automate с большинства страниц со списками, карточек и страниц документов. После того как администратор подключит [!INCLUDE [prod_short](includes/prod_short.md)] к Power Automate, вы увидите все потоки, добавленные вашей организацией, выбрав действие **Автоматизировать** на соответствующих страницах. Мгновенные потоки выполняются, не покидая [!INCLUDE [prod_short](includes/prod_short.md)]. Узнайте больше в статье [Настройка автоматизированных рабочих процессов](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) в материалах по администрированию.

Эти мгновенные рабочие процессы открываются на странице в [!INCLUDE [prod_short](includes/prod_short.md)] Online, чтобы вы оставались в контексте бизнес-процесса, над которым работали. Выберите действие **Автоматизировать** (на некоторых страницах оно расположено в меню **Больше параметров**), выберите пункт меню **Power Automate**, затем выберите соответствующую ссылку, чтобы запустить рабочий процесс. Подключение к Power Automate уже настроено.

Для большинства рабочих процессов требуется заполнить одно или два поля, прежде чем выбирать действие **Запустить поток**.

> [!TIP]
> Если вы не видите действие **Автоматизировать**, ваш сервис [!INCLUDE [prod_short](includes/prod_short.md)], вероятно, еще не настроен для использования Power Automate. Узнайте больше у администратора.

## <a name="add-more-automated-flows-and-instant-flows"></a>Добавление дополнительных автоматизированных потоков и мгновенных потоков

Вы можете создавать потоки с помощью веб-сайта [powerautomate.microsoft.com](https://powerautomate.microsoft.com). Однако если ваш администратор включил возможность запуска потоков Power Automate изнутри [!INCLUDE [prod_short](includes/prod_short.md)] Online, вы можете начать процесс построения потока с действия **Автоматизировать** на соответствующих страницах, которое можно найти в разделе меню **Дополнительные параметры** в зависимости от страницы. Затем выберите пункт меню **Power Automate**, затем выберите действие **Создать поток**. Power Automate откроется в новой вкладке браузера, и вы автоматически войдете в систему.

Вы можете найти образцы шаблонов для адаптации к вашей компании и всем доступным триггерным событиям, используя [!INCLUDE [prod_short](includes/prod_short.md)] и внешние инструменты, выбрав меню **Соединители** на веб-сайте Power Automate. Узнайте больше о доступных шаблонах и триггерах в статье [Настройка автоматизированных рабочих процессов](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) в материалах по администрированию.

## <a name="manage-automated-workflows"></a>Управление автоматизированными рабочими процессами

Вы можете создавать новые потоки или управлять существующими потоками Power Automate в [!INCLUDE [prod_short](includes/prod_short.md)] на странице **Управление потоками Power Automate**. Узнайте больше в статье [Управление потоками Power Automate](/dynamics365/business-central/dev-itpro/powerplatform/manage-power-automate-flows) в материалах по администрированию.

Вы также можете управлять доступными рабочими процессами Power Automate на странице **Рабочие процессы** в [!INCLUDE[prod_short](includes/prod_short.md)]. На этой странице перечислены как встроенные утверждения, так и рабочие процессы Power Automate с возможностью последующего включения/отключения, удаления и просмотра рабочего процесса на веб-сайте Power Automate.

## <a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/use-power-automate/)

## <a name="see-also"></a>См. также

[Устранение неполадок в автоматизированных рабочих процессах [!INCLUDE[prod_short](includes/prod_short.md)]](across-flow-troubleshoot.md)  
[Подготовка к ведению бизнеса](ui-get-ready-business.md)  
[Рабочие процессы](across-workflow.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Назначение разрешений пользователям и группам](ui-define-granular-permissions.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Финансы](finance.md)  
[Управление потоками Power Automate](/dynamics365/business-central/dev-itpro/powerplatform/manage-power-automate-flows)  
[Настройка автоматизированных рабочих процессов](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows)  
[Включение мгновенных потоков](/dynamics365/business-central/dev-itpro/powerplatform/instant-flows)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
