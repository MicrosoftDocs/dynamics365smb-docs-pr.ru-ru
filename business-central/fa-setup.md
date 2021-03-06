---
title: Настройка основных средств | Документация Майкрософт
description: Узнайте оп последовательности задач, которые следует выполнить для настройки основных средств, например машин или оборудования.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: machinery, buildings
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: a35bd9a83ec05a25bc087722fb2009ca27bbfa2f
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5770420"
---
# <a name="setting-up-fixed-assets"></a>Настройка основных средств
До начала работы с основными средствами необходимо определить несколько вещей.  

* Способ страхования, ведения и амортизации основных средств.  
* Способ регистрации записей и других значений в главной книге.  

Таблица ниже содержит ссылки на дополнительную информацию. После настройки этих вещей можно приступить к различным действиям. Дополнительные сведения см. в разделе [Основные средства](fa-manage.md).  

> [!NOTE]  
>   Вы можете записывать транзакции по основным средствам на странице **Журнал ГК учета основных средств** или на странице **Журнал ОС** в зависимости от назначения транзакций: для финансовой отчетности или для внутреннего управления. В справке для основных средств описывается только использование страницы **Журнал ГК учета основных средств**.  

Если вы включаете действие основного средства в разделе **Интеграция С ГК** на странице **Карточка книги амортизации**, страница **Журнал ГК учета основных средств** будет использоваться для учета транзакций для соответствующего действия.

В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.  

| Действие | Ссылка |
| --- | --- |
| Настройте счета ГК по умолчанию, ключи распределения, шаблоны и разделы журналов для учета основных средств, а также настройте классы и подклассы основных средств, такие как материальные и нематериальные основные средства. |[Настройка общих данных основных средств](fa-how-setup-general.md) |
| Создайте книги амортизации, определите различные методы амортизации, выполните интеграцию с главной книгой и включите дублирование операций в нескольких книгах амортизации. |[Настройка амортизации основных средств](fa-how-setup-depreciation.md) |
| Включите страхование основных средств, настройте общие сведения о страховании, страховую карточку для каждого полиса, а также подготовьте журналы для учета затрат на страхование. |[Настройка страхования основного средства](fa-how-setup-insurance.md) |
| Включите обслуживание основных средств, настройте общие сведения об обслуживании, настройте счета учета обслуживания и определите типы работ по техническому обслуживанию. |[Настройка обслуживания основного средства](fa-how-setup-maintenance.md) |
| Изучите различные методы расчета амортизации основных средств. |[Методы амортизации](fa-depreciation-methods.md) |

## <a name="see-also"></a>См. также
[Основные Средства](fa-manage.md)  
[Финансы](finance.md)  
[Подготовьтесь к ведению бизнеса](ui-get-ready-business.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]