---
title: Учет налоговых разниц в России
description: Российские улучшения включают учет налоговых разниц.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 4a312fcf142f2ca6cdac0e26e6e4726da1bdc4c1
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738258"
---
# <a name="how-to-post-tax-differences"></a>Практическое руководство. Учет налоговых разниц

**Журнал налоговых разниц** используется для создания и учета транзакций для налоговых разниц. Налоговые разницы представляют собой расхождения сумм налога, вызванные различиями в правилах признания доходов и расходов в бухгалтерском и налоговом учете.

С помощью окна **Журнал налоговых разниц** можно вручную создавать операции налоговых разниц и изменять имеющиеся операции, созданные периодическими процедурами расчета налоговых разниц. При учете окна **Журнал налоговых разниц** соответствующие операции учитываются в выбранных учетных группах.

## <a name="to-post-tax-differences"></a>Учет налоговых разниц

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы налоговых разниц**, затем выберите связанную ссылку.

2. Введите значения в поля, как описано в следующей таблице.

   | Поле                    | Описание                                                  |
   | :----------------------- | :----------------------------------------------------------- |
   | **Дата учета**         | Введите дату транзакции.                                  |
   | **Номер документа**         | Введите номер документа из исходной транзакции.       |
   | **Описание**          | Введите описание транзакции.                     |
   | **Тип налог. разницы**       | Укажите, является налоговая разница **постоянной** или **временной**. |
   | **Код налог. разницы**       | Выберите идентификационный код дохода или расхода, определяющий источник налоговой разницы. |
   | **Тип источника**          | Выберите источник налоговой разницы. Возможные варианты: **Расходы будущих периодов**, **Основное средство** и **Нематериальный актив**. |
   | **Номер источника**           | Если поле **Тип источника** имеет значение **Расходы будущих периодов**, введите код расходов будущих периодов.  В противном случае это поле следует оставить пустым. |
   | **Код юрисдикции**    | Выберите код юрисдикции, который используется для расчета налогооблагаемых прибыли и убытков для налоговых разниц. |
   | **Код нормы**            | Выберите код юрисдикции нормы, который используется для расчета налогооблагаемых прибыли и убытков для налоговых разниц. |
   | **Ставка налога**           | Введите ставку налога на прибыль, которая используется для расчета налоговых разниц. |
   | **Сумма (БУ)**        | Введите сумму расходов на основании данных бухгалтерского учета. Эта информация используется, если настроен расчет налоговых разниц для периода времени. |
   | **Сумма (НУ)**         | Введите сумму расходов на основании транзакций налогового учета. Эта информация используется, если настроен расчет налоговых разниц для периода времени. |
   | **Разница**           | Введите значение разницы между транзакциями бухгалтерского и налогового учета. |
   | **Сумма с начала года (БУ)**    | Введите значение расходов и доходов по данным бухгалтерского учета с начала года. |
   | **Сумма с начала года (НУ)**     | Введите значение расходов и доходов по данным налогового учета с начала года. |
   | **Разница с начала года**       | Введите значение разницы между транзакциями бухгалтерского и налогового учета с начала года. |
   | **Налоговая разница - режим расчета** | Определяет разницу режима расчета. Если выбрано значение **Баланс**, разница будет рассчитываться нарастающим итогом с начала года. Если это поле не выбрано, разница будет создана для текущего периода. |
   | **Сумма налога**           | Определяет результат расчета. Значение этого поля корректирует налог на прибыль в транзакциях бухгалтерского учета. |
   | **Сумма налогового актива**     | Определяет рассчитанную сумму налогового актива.                   |
   | **Сумма налог. обязательства** | Определяет рассчитанную сумму налогового обязательства.               |
   | **Сумма реализации ОНО/ОНА**  | Определяет сумму налога, которая списывается при реализации товара. |
   | **ОНА - начальное сальдо** | Определяет начальную сумму реализации ОНО/ОНА перед расчетом.  |
   | **ОНО - начальное сальдо** | Определяет обязательства по начальной сумме реализации ОНО/ОНА перед расчетом. |
   | **ОНА - конечное сальдо**   | Определяет сумму реализации ОНО/ОНА после расчета.            |
   | **ОНО - конечное сальдо**   | Определяет обязательства по сумме реализации ОНО/ОНА после расчета.  |
   | **Метод реализации**        | Выберите, требуется ли записать налоговую разницу или преобразовать ее в постоянную разницу. |
   | **Дата реализации**        | Введите дату реализации товара.                       |
   | **Частичная реализация**     | Выберите, если требуется реализовать товар, который приводит к расхождениям в коде расходов или доходов. Если данное поле не выбрано, налоговые разницы списываются. |

3. Выберите действие **Учет**. Транзакции журнала налоговых разниц будут учтены.

4. Выберите действие **Книга операций**, чтобы открыть окно **Книга операций по налоговым разницам** и проверить учтенные операции.

## <a name="see-also"></a>См. также

[Налоговые разницы](Tax-Differences.md)  
[Настройка расчета налоговых разниц](Setting-up-Tax-Difference-Calculation.md)  
[Налоговый учет](Tax-Accounting.md)  
[Налоговые регистры](Tax-Registers.md)  
[Практическое руководство. Создание налоговых регистров](How-to-Create-Tax-Registers.md)  