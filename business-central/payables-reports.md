---
title: Отчеты о кредиторской задолженности и аналитика
description: Посмотрите, какие отчеты и аналитика доступны в стандартной версии Business Central, чтобы вы могли отслеживать свою кредиторскую задолженность.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: reporting
ms.date: 07/13/2021
ms.author: edupont
ms.openlocfilehash: 774fd24bc15cb4cefb56991289d9c72c0909a319
ms.sourcegitcommit: a486aa1760519c380b8cdc8fdf614bed306b65ea
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "6543366"
---
# <a name="accounts-payable-reports-and-analytics-in-business-central"></a>Отчеты и аналитика по кредиторской задолженности в Business Central

Чтобы помочь вам управлять своей кредиторской задолженностью в [!INCLUDE [prod_short](includes/prod_short.md)], встроены стандартные отчеты и аналитика. Функция выходит за рамки традиционных ограничений отчетности, чтобы помочь вам эффективно разрабатывать различные типы отчетов.  

## <a name="reports"></a>Отчеты

В следующей таблице описаны некоторые ключевые отчеты в отчетности по кредиторской задолженности.

| Отчет | ИД объекта | Описание |
|--|--|--|
| **Кредиторская задолженность по срокам давности** | 322|Показывает просроченные остатки по поставщикам в просроченные промежутки времени. Просроченные суммы могут быть показаны по сроку, дате проводки или по дате документа, если необходимо. Вы можете выбрать отображение сумм в местной валюте (МВ) и распечатать сведения просроченных документов. Временные интервалы могут иметь заголовки с датами или с количеством просроченных дат относительно указанного срока хранения по типу.<br>Этот отчет является основным отчетом для выверки книги поставщика с главной книгой. Предполагается, что вы не разрешили прямую проводку по счетам, используемым в счете кредиторской задолженности группы разноски поставщиков, этот отчет представляет собой спецификацию сумм, которые вы найдете в главной книге.|
| **Поставщик - баланс на дату** | 321 | Показывает баланс поставщика на дату окончания указанного диапазона дат. Вы можете выбрать отображение сальдо поставщика в местной валюте (МВ). Выберите поле **Включить отмененные операции**, чтобы показать операции, которые были закрыты к дате окончания, но были не применены (открыты) позже. Выберите **Показать операции с нулевым сальдо** для отображения поставщиков с нулевым сальдо на дату окончания фильтра даты. Фильтр по дате применяется к подробным операциям книги поставщиков для операций в отчете. Если у вас есть платежи позже даты окончания, которые были применены к счетам в пределах диапазона дат, счета-фактуры появятся в отчете, поскольку они не были закрыты по состоянию на дату окончания. |
| **Поставщик – пробный баланс** | 329 | Показывает чистые изменения для поставщиков за период, указанный в фильтре дат, а также чистое изменение с начала года до даты финансового года, соответствующего выбранному периоду. Отчет сгруппирован по группам разноски поставщиков и дает иное представление о книге поставщиков, чем в отчете **Кредиторская задолженность по срокам давности**. **Примечание**. Если вы не настроили никакой отчетный период, система не будет знать, какой финансовый год использовать, и будет либо отображать текущий год с самого последнего определенного финансового года, либо просто выберет период, который может или не может быть с начала года.|
| **Поставщик – подробный пробный баланс** | 304 | Показывает все операции книги поставщиков в пределах указанного фильтра даты. Отчет показывает начальные балансы поставщика относительно фильтра даты. |
| **Статистика покупок** |312 |[!INCLUDE [reports-purchase-statistics](includes/reports-purchase-statistics.md)]<br>Этот отчет также можно использовать для работы с кредиторской задолженностью, так как проще быстро найти разнесенные платежи, скидки и другие транзакции для данного поставщика.|
|**Поставщик - сводка задолженности с распределением по срокам**|305| Устаревший отчет кредиторской задолженности по срокам давности. Мы рекомендуем вам вместо этого использовать отчет **Кредиторская задолженность по срокам давности**. Вы можете выбрать продолжительность периода и дату, которые будут использоваться как дата *просрочено на*.|
|**Удерживаемые платежи**|319|Показывает операции книги поставщиков, где поле **На удержании** не пустое.|
|**Журнал предоплат поставщика**|317|Показывает журнал платежей с информацией о скидках и допусках. Отчет можно использовать для проверки платежей перед созданием файлов платежей и разноской журнала. **Примечание**. В отчете будут неправильно отображаться скидки при оплате, если в приложении использовалось несколько кредит-нот. В этом случае скидка на оплату дополнительных кредит-нот будет показана как непримененная сумма.|
|**Список поставщиков**|301|Показывает различные виды базовой информации по поставщикам, такие как учетная группа поставщика, информация о скидках и оплате, приоритетный уровень и валюта поставщика по умолчанию, а также баланс поставщика в текущей валюте (МВ). Отчет может быть использован, для того, чтобы представлять информацию в таблице «Поставщик».|

## <a name="see-also"></a>См. также

[Анализ финансовых отчетов в Microsoft Excel](finance-analyze-excel.md)  
[Работа с измерениями](finance-dimensions.md)  
[Управление основными средствами](fa-manage.md)  
[Обзор локальных функциональных возможностей](about-localization.md)  
[Работа бухгалтера в [!INCLUDE[prod_long](includes/prod_long.md)]](finance-accounting.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]