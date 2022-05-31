---
title: Устранение неполадок в автоматизированных рабочих процессах
description: Узнайте, как устранить неполадки соединения между Business Central и Power Automate, когда вы создаете автоматизированный рабочий процесс.
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 05/12/2022
ms.author: edupont
author: jswymer
ms.openlocfilehash: b8fff95ced93e7ee2a3112969f45525532b19445
ms.sourcegitcommit: e86f0bd15604c2fb327e3182929c44a4172790c7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2022
ms.locfileid: "8786200"
---
# <a name="troubleshoot-your-prod_short-automated-workflows"></a>Устранение неполадок в автоматизированных рабочих процессах [!INCLUDE[prod_short](includes/prod_short.md)]

Подключая [!INCLUDE [prod_short](includes/prod_short.md)] к Power Automate для создания автоматизированных рабочих процессов, вы можете увидеть сообщения об ошибках. В этой статье представлены рекомендуемые решения для часто возникающих проблем.

## <a name="flow-doesnt-run-on-all-records-created-or-changed"></a>Рабочий процесс выполняется не для всех созданных или измененных записей

### <a name="problem"></a>Проблема

Если событие создает или изменяет много записей, рабочий процесс не запускается для некоторых или всех из них.

### <a name="possible-cause"></a>Возможная причина

В настоящее время существует ограничение на количество записей, которые может обработать рабочий процесс. Если в течение 30 секунд будет создано или изменено более 100 записей, рабочий процесс не будет запущен.

> [!NOTE]
> Для разработчиков запуск рабочего процесса выполняется с помощью уведомлений веб-перехватчика, и это ограничение связано с тем, как коннектор Business Central обрабатывает уведомления `collection`. Дополнительные сведения см. в разделе [Работа с веб-перехватчиками в Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/api-reference/v2.0/dynamics-subscriptions#notes-for-power-automate-flows) справочных материалов для разработчиков и администраторов.

## <a name="entity-set-not-found-error"></a>Ошибка "Набор сущностей не найден"

### <a name="problem"></a>Проблема

При создании нового рабочего процесса Power Automate с использованием триггера утверждения [!INCLUDE[prod_short](includes/prod_short.md)], например *Если запрашивается утверждение документа покупки*, вы получите сообщение об ошибке, подобное следующему:

`Entity set not found: \<name\>`

Заполнитель `\<name\>` — это название отсутствующей веб-службы, например *workflowWebhookSubscriptions* или *workflowPurchaseDocumentLines*.

### <a name="possible-cause"></a>Возможная причина

Для использования Power Automate с вашими утверждениями требуется, чтобы определенные объекты страницы и модуля codeunit были опубликованы как веб-службы. По умолчанию большинство необходимых объектов публикуются для вас как веб-службы. Но в некоторых случаях ваша среда могла быть настроена так, что эти объекты больше не публикуются.

### <a name="fix"></a>Исправление

Перейдите на страницу **Веб-службы** и убедитесь, что следующие объекты опубликованы как веб-службы. Для каждого объекта в списке должна быть запись с установленным флажком **Опубликовано**.  

|Тип объекта|ИД объекта|Имя объекта|Имя службы|
|-----------|---------|-----------|------------|
|Модуль Codeunit|  1544    |WorkflowWebhookSubscription|WorkflowActionResponse|
|Стр.|  6408|   workflowCustomers|  workflowCustomers|
|Стр.   |6406   |workflowGenJournalBatches| workflowGenJournalBatches|
|Стр.   |6407   |workflowGenJournalLines|workflowGenJournalLines|
|Стр.   |6409   |workflowItems| workflowItems|
|Стр.   |6405   |Объект строки документа покупки|workflowPurchaseDocumentLines|
|Стр.|  6404    |workflowPurchaseDocuments| workflowPurchaseDocuments|
|Стр.|  6403    |Объект строки документа продажи |workflowSalesDocumentLines|
|Стр.|  6402|   workflowSalesDocuments| workflowSalesDocuments|
|Стр.|  6410    |workflowVendors|   workflowVendors|
|Стр.|  831 |workflowWebhookSubscriptions|  workflowWebhookSubscriptions|

> [!NOTE]
> Значение **Имя службы** должно быть точно таким, как показано в таблице. Не меняйте и не переводите название службы.

Дополнительные сведения о публикации веб-служб см. в разделе [Публикация веб-службы](across-how-publish-web-service.md).

## <a name="see-also"></a>См. также

[Использование [!INCLUDE[prod_short](includes/prod_short.md)] в автоматическом рабочем процессе](across-how-use-financials-data-source-flow.md)  
[Рабочий процесс](across-workflow.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]