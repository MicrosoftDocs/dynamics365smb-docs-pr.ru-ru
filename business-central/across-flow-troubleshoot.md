---
title: Устранение неполадок в автоматизированных рабочих процессах
description: 'Узнайте, как устранить неполадки соединения между Business Central и Power Automate, когда вы создаете автоматизированный рабочий процесс.'
author: jswymer
ms.topic: conceptual
ms.search.keywords: 'workflow, OData, Power App, SOAP, Entity set not found, workflowWebhookSubscriptions, Power Automate,'
ms.date: 07/03/2023
ms.author: jswymer
ms.reviewer: jswymer
---

# <a name="troubleshoot-your--automated-workflows"></a>Устранение неполадок в автоматизированных рабочих процессах [!INCLUDE[prod_short](includes/prod_short.md)]

Подключая [!INCLUDE [prod_short](includes/prod_short.md)] к Power Automate для создания автоматизированных рабочих процессов, вы можете увидеть сообщения об ошибках. В этой статье представлены рекомендуемые решения для постоянно возникающих проблем.

## <a name="flow-doesnt-run-on-all-records-created-or-changed"></a>Рабочий процесс выполняется не для всех созданных или измененных записей

### <a name="problem"></a>Проблема

Если событие создает или изменяет много записей, рабочий процесс не запускается для некоторых или всех из них.

### <a name="possible-cause"></a>Возможная причина

В настоящее время существует ограничение на количество записей, которые может обработать рабочий процесс. Если в течение 30 секунд будет создано или изменено более 1000 записей, поток не запускается.

> [!NOTE]
> Для разработчиков запуск рабочего процесса выполняется с помощью уведомлений веб-перехватчика, и это ограничение связано с тем, как коннектор Business Central обрабатывает уведомления `collection`. Подробнее см. в разделе [Работа с веб-перехватчиками в Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/api-reference/v2.0/dynamics-subscriptions#notes-for-power-automate-flows) справочных материалов для разработчиков и администраторов.

## <a name="the-response-from-the-business-central-service-is-too-large-error"></a>Ошибка «Ответ от службы Business Central слишком велик»

### <a name="problem-1"></a>Проблема

При использовании действия, взаимодействующего с записями (например, *Создать запись (версия 3)* и *Получить запись (версия 3)*), Power Automate может отобразить ошибку, подобную следующей:

`The response from the Business Central service is too large`

### <a name="possible-cause-1"></a>Возможная причина

Несмотря на то что в Business Central нет установленных ограничений на размер записей, возвращаемых API, соединитель Dynamics 365 Business Central для Power Automate может обрабатывать только записи размером до 8 МБ.

Все API-интерфейсы Business Central, предоставляемые Майкрософт, возвращают записи в рамках этого ограничения, однако в случае API-интерфейсов, предоставляемых партнерами, оно может не соблюдаться. Если вы видите сообщение об ошибке «Ответ от службы Business Central слишком велик», обратитесь к партнеру, который создал используемый вами API.

## <a name="entity-set-not-found-error"></a>Ошибка "Набор сущностей не найден"

### <a name="problem-2"></a>Проблема

При создании нового рабочего процесса Power Automate с использованием триггера утверждения [!INCLUDE[prod_short](includes/prod_short.md)], например *Если запрашивается утверждение документа покупки*, вы получите сообщение об ошибке, подобное следующему:

`Entity set not found: \<name\>`

Заполнитель `\<name\>` — это название отсутствующей веб-службы, например *workflowWebhookSubscriptions* или *workflowPurchaseDocumentLines*.

### <a name="possible-cause-2"></a>Возможная причина

Для использования Power Automate с утверждениями требуется, чтобы определенные объекты страницы и модуля codeunit были опубликованы как веб-службы. По умолчанию большинство необходимых объектов публикуются как веб-службы. Но в некоторых случаях ваша среда могла быть настроена так, что эти объекты больше не публикуются.

### <a name="fix"></a>Исправить

Перейдите на страницу **Веб-службы** и убедитесь, что следующие объекты опубликованы как веб-службы. Для каждого объекта в списке должна быть запись с установленным флажком **Опубликовано**.  

| Тип объекта | ИД объекта | Имя объекта | Имя службы |
|--|--|--|--|
| Модуль Codeunit | 1544 | WorkflowWebhookSubscription | WorkflowActionResponse |
| Стр. | 6408 | workflowCustomers | workflowCustomers |
| Стр. | 6406 | workflowGenJournalBatches | workflowGenJournalBatches |
| Стр. | 6407 | workflowGenJournalLines | workflowGenJournalLines |
| Стр. | 6409 | workflowItems | workflowItems |
| Стр. | 6405 | Объект строки документа покупки | workflowPurchaseDocumentLines |
| Стр. | 6404 | workflowPurchaseDocuments | workflowPurchaseDocuments |
| Стр. | 6403 | Объект строки документа продажи | workflowSalesDocumentLines |
| Стр. | 6402 | workflowSalesDocuments | workflowSalesDocuments |
| Стр. | 6410 | workflowVendors | workflowVendors |
| Стр. | 831 | workflowWebhookSubscriptions | workflowWebhookSubscriptions |

> [!NOTE]
> Значение **Имя службы** должно быть точно таким, как показано в таблице. Не меняйте и не переводите название службы.

Подробнее о публикации веб-служб см. в разделе [Публикация веб-службы](across-how-publish-web-service.md).

## <a name="see-also"></a>См. также

[Использование потоков Power Automate в [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-financials-data-source-flow.md)  
[Рабочий процесс](across-workflow.md)  
[Настройка автоматизированных рабочих процессов](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows)  
[Включение мгновенных потоков](/dynamics365/business-central/dev-itpro/powerplatform/instant-flows)  
[Управление потоками Power Automate](/dynamics365/business-central/dev-itpro/powerplatform/manage-power-automate-flows)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
