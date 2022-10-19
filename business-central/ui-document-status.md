---
title: Поле статуса на документах
description: Узнайте о статусе «Открыто» и «Выпущено» в документах с расценками, заказами или кредит-нотами.
author: rubenseishima
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: document, status, quote, order, credit memo, released, open, pending approval, pending prepayment,
ms.search.form: ''
ms.date: 09/19/2022
ms.author: a-reishima
ms.openlocfilehash: c96909b4ee37673ee7b0c752224478a144ad853e
ms.sourcegitcommit: 8ad79e0ec6e625796af298f756a142624f514cf3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2022
ms.locfileid: "9608198"
---
# <a name="status-field-on-documents"></a>Поле статуса на документах

При создании предложения, заказа или кредит-ноты, поле **Статус** в заголовке документа содержит по умолчанию статус **Открыт**.

После заполнения документа его можно выпустить, и тогда приложение [!INCLUDE[prod_short](includes/prod_short.md)] изменит значение в поле **Статус** на **Запущен**. Этот статус указывает, что заказ готов для следующего этапа обработки перед выполнением его учета.

| Состояние | Описанием |
| ------ | ----------- |
| Открытый   | В данный документ можно внести изменения. |
| Выпущенный | Документ выпущен на следующий этап обработки, и в строки типа *Товар* и *Основное средство* изменения вносить нельзя.<br /><br />Если в содержимое выпущенного документа нужно внести изменения, его можно открыть повторно. Для переноса скорректированного документа на следующий этап обработки его следует выпустить еще раз. |
| Ожидает утверждения   | Документ ожидает утверждения. |
| Ожидает предоплаты | Для документа был учтен счет на предоплату. |

## <a name="releasing"></a>Выпуск

Процесс выпуска можно использовать по-разному в целях облегчения обычных рабочих процедур, например, для обеспечения следования установленным в организации правилам одобрения или запуска складских процессов.

### <a name="approval-procedures"></a>Процедуры утверждения

Процедура выпуска может использоваться организацией для указания того, что документ одобрен другим пользователем, или внешний контракт удовлетворяет спецификациям в документе, как показано в следующих примерах:

* Заказ покупки можно выпустить только после сообщения поставщика о готовности его выполнить.
* До получения разрешения на выпуск создаваемого заказа, возможно, требуется одобрение второго пользователя, например, по соображениям безопасности.
* Созданная кредит-нота должна быть выпущена лицом, ответственным за одобрение всех компенсаций.

Узнайте больше о рабочих процессах утверждения в разделе [Использование рабочих процессов](across-use-workflows.md).

### <a name="warehouse-activities"></a>Складские задания

При статусе заказа **Открыт**, склад не начнет подготовку к отгрузке и не предполагает получения товаров по заказу покупки. При выпуске заказа указывается, что заказ завершен, и что он может быть включен в операции данного склада.

## <a name="reopening-a-released-order"></a>Повторное открытие выпущенного заказа

В выпущенный заказ можно внести изменения, повторно его открыв. Однако можно увеличить только количество строк, уже обработанных складом.

После внесения изменений и повторного выпуска заказа налог на добавленную стоимость (НДС) и скидка счета пересчитываются.

При внесении изменений в выпущенный заказ необходимо уведомить об этом склад.

> [!NOTE]
> Если требуется учесть единичный открытый заказ или кредит-ноту без предшествующего выпуска, программа автоматически выпустит данный документ при выполнении его учета. При выполнении учета заказов или кредит-нот с помощью функции **Пакетный учет**, можно выбрать учет только уже выпущенных заказов или кредит-нот.

## <a name="see-also"></a>См. также

[Продажа товара с заказом продажи клиента](sales-how-sell-products.md)  
[Регистрация покупок со счетами покупок](purchasing-how-record-purchases.md)  
[Отгрузка товаров](warehouse-how-ship-items.md)  
[Приемка товаров](warehouse-how-receive-items.md)  
[Использование рабочего процесса утверждения](across-how-use-approval-workflows.md)  
[Сортировка, поиск и фильтрация списков](ui-enter-criteria-filters.md)  
[Архивирование документов](across-how-to-archive-documents.md)  
[Общие бизнес-функции](ui-across-business-areas.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]