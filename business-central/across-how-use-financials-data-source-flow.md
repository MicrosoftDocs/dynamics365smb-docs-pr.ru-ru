---
title: Использование Business Central в рабочих процессах Power Automate
description: Настройте и используйте рабочие процессы Power Automate, которые создают или изменяют данные Business Central.
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, OData, Power App, SOAP, Entity set not found, workflowWebhookSubscriptions
ms.date: 05/12/2022
ms.author: edupont
author: jswymer
ms.openlocfilehash: 056fe537df2fba23e02cb4e70675937cde724fbf
ms.sourcegitcommit: 3acadf94fa34ca57fc137cb2296e644fbabc1a60
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2022
ms.locfileid: "9533029"
---
# <a name="use-prod_short-in-power-automate-flows"></a>Использование [!INCLUDE[prod_short](includes/prod_short.md)] в рабочих процессах Power Automate

Можно использовать данные [!INCLUDE[prod_short](includes/prod_short.md)] как часть рабочего процесса в Microsoft Power Automate. Создавайте собственные рабочие процессы и подключайтесь к своим данным с помощью соединителя [!INCLUDE [prod_short](includes/prod_short.md)].  

> [!NOTE]  
> Вы должны иметь допустимую учетную запись в [!INCLUDE[prod_short](includes/prod_short.md)] и в Power Automate.  

> [!TIP]
> Кроме Power Automate, в [!INCLUDE[prod_short](includes/prod_short.md)] можно использовать шаблоны рабочего процесса утверждения. Хотя это две отдельные системы для создания рабочих процессов, любой шаблон рабочего процесса утверждения, созданный в Power Automate, добавляется в список рабочих процессов в [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Рабочие процессы](across-workflow.md).  

## <a name="automated-workflows"></a>Автоматизированные рабочие процессы

С помощью Power Automate вы можете создавать бизнес-процессы непосредственно внутри компании и полагаться на разработчиков-любителей. Дополнительные сведения см. в разделе [Настройка автоматизированных рабочих процессов](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) в материалах по администрированию.  

## <a name="manual-instant-flows"></a>Ручные мгновенные рабочие процессы

С мая 2022 года администратор [!INCLUDE [prod_short](includes/prod_short.md)] онлайн может [включить функцию](admin-feature-management.md), чтобы рабочий процесс Power Automate можно было запускать с большинства страниц. Дополнительные сведения см. в разделе [Настройка автоматизированных рабочих процессов](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) в материалах по администрированию.  

После того как администратор подключит [!INCLUDE [prod_short](includes/prod_short.md)] к Power Automate, вы увидите все рабочие процессы, добавленные вашей организацией, выбрав действие **Автоматизировать** на соответствующих страницах. Вы сможете запускать рабочие процессы, не покидая [!INCLUDE [prod_short](includes/prod_short.md)].  

Эти автоматизированные рабочие процессы открываются на панели в [!INCLUDE [prod_short](includes/prod_short.md)] онлайн, чтобы вы оставались в контексте бизнес-процесса, над которым работали. На некоторых страницах действие **Автоматизировать** расположено в меню **Больше параметров**. Найдите его, выберите пункт меню **Power Automate**, а затем нажмите на соответствующую ссылку, чтобы запустить рабочий процесс. Подключение к Power Automate уже настроено.  

Для большинства рабочих процессов требуется заполнить одно или два поля, прежде чем выбирать действие **Запустить процесс**.  

> [!TIP]
> Если вы не видите действие **Автоматизировать**, ваш сервис [!INCLUDE [prod_short](includes/prod_short.md)], вероятно, еще не настроен для использования Power Automate. Для получения дополнительных сведений обратитесь к администратору.

## <a name="add-more-automated-flows-and-manual-instant-flows"></a>Добавьте больше автоматизированных рабочих процессов и ручных мгновенных рабочих процессов

Вы можете создавать рабочие процессы на веб-сайте [powerautomate.microsoft.com](https://powerautomate.microsoft.com). Однако если ваш администратор включил возможность запуска рабочих процессов Power Automate в [!INCLUDE [prod_short](includes/prod_short.md)] онлайн, вы можете начать создавать рабочий процесс с действия **Автоматизировать** на соответствующих страницах. На некоторых страницах действие **Автоматизировать** расположено в меню **Больше параметров**. Найдите его, выберите пункт меню **Power Automate**, а затем нажмите **Создать рабочий процесс**. Power Automate откроется в новой вкладке браузера, и вы автоматически войдете в систему.

## <a name="manage-workflows"></a>Управление рабочими процессами

Вы посмотреть все рабочие процессы, к которым у вас есть доступ, выбрав действие **Управление рабочими процессами** в меню **Power Automate**. Список процессов откроется в новой вкладке браузера, и вы автоматически войдете в Power Automate. Там можно увидеть, когда каждый рабочий процесс запускался в последний раз.  

## <a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/use-power-automate/)

## <a name="see-also"></a>См. также

[Устранение неполадок в автоматизированных рабочих процессах [!INCLUDE[prod_short](includes/prod_short.md)]](across-flow-troubleshoot.md)  
[Подготовка к ведению бизнеса](ui-get-ready-business.md)  
[Рабочие процессы](across-workflow.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Назначение разрешений пользователям и группам](ui-define-granular-permissions.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Финансы](finance.md)  
[Настройка автоматизированных рабочих процессов](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
