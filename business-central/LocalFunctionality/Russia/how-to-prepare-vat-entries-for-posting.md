---
title: Подготовка операций НДС к учету в России
description: Российские улучшения включают возможность периодически предоставлять в налоговые органы данные о чистой сумме НДС покупок или продаж.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: b140fa7b2e2c8015d5fe8d7b1686812200b2f8dc
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738208"
---
# <a name="how-to-prepare-vat-entries-for-posting"></a>Практическое руководство. Подготовка операций НДС к учету

Необходимо периодически предоставлять в налоговые органы данные о чистой сумме НДС. Можно использовать **Журнал НДС** для подготовки транзакций с открытыми суммами НДС к учету и для копирования операций в соответствующий журнал НДС. Обычно это нужно перед запуском пакетного задания **Вычисление и учет зачета НДС** для учета и закрытия операций НДС.

## <a name="to-prepare-vat-entries-for-posting"></a>Подготовка операций НДС к учету

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал НДС**, затем выберите связанную ссылку.

2. Выберите фильтры, которые определяют связанные с НДС транзакции, которые требуется включить в зачет НДС.

   | Поле       | Описание                                                  |
   | :---------- | :----------------------------------------------------------- |
   | **Тип**    | Выберите типы транзакций, которые требуется включить в зачет НДС. |
   | **Просмотр по** | Выберите период времени для зачета НДС.               |
   | **Просмотр как** | Выберите способ просмотра чистой суммы НДС. Возможные варианты: **Оборот** и **Сальдо на дату**. |

3. Выберите **Предложить документы**. Будут показаны транзакции с открытыми операциями НДС, которые соответствуют выбранным фильтрам.

4. Проверьте выбранные транзакции. При необходимости скорректируйте фильтр.

5. Выберите **Копировать строки в журнал**.

Операции копируется в соответствующие журналы НДС. Теперь можно запустить пакетное задание **Вычисление и учет зачета НДС**, чтобы закрыть операции НДС.

## <a name="see-also"></a>См. также

[Практическое руководство. Подача отчета об НДС в налоговые органы](../../finance-how-report-vat.md)  