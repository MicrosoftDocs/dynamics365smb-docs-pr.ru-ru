---
title: Методы амортизации для основных средств
description: Узнайте о различных встроенных методах амортизации или списания основных средств в версии Business Central по умолчанию.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: write down
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 9e531a4f304829b0549fbe21e8d671708373ab22
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5774159"
---
# <a name="depreciation-methods-for-fixed-assets"></a>Методы амортизации для основных средств

По умолчанию доступно восемь методов амортизации в версии [!INCLUDE [prod_short](includes/prod_short.md)]:  

* SL  
* DB 1  
* DB 2  
* DB1/SL  
* DB2/SL  
* Пользовательский  

  > [!NOTE]  
  > Укажите собственный метод амортизации, задав таблицы амортизации.
* Ручной  

  > [!NOTE]  
  > Этот метод можно использовать для основных средств, которые не являются объектом амортизации, например земли. Необходимо ввести амортизацию в журнале ГК основных средств. Пакетное задание **Расчет амортизации** пропускает основные средства при использовании этого метода амортизации.  
* Начисление полугодовой нормы износа  

  > [!NOTE]  
  > При использовании этого метода основное средство амортизируется на одну и ту же сумму каждый год.  

## <a name="straight-line-depreciation"></a>Линейная амортизация

При использовании линейного метода необходимо определить один из следующих параметров книги амортизации основных средств:  

* Период амортизации (годы и месяцы) или дата конца амортизации  
* Фиксированный ежегодный процент  
* Фиксированная ежегодная сумма  
* Период амортизации  

### <a name="depreciation-period"></a>Период амортизации

При указании периода амортизации (число лет, месяцев или даты окончания амортизации) используется следующая формула для вычисления суммы амортизации:  

*Сумма амортизации = ((учетная стоимость - ликвидационная стоимость) x число дней амортизации) / оставшиеся дни амортизации*  

Оставшиеся дни амортизации рассчитываются как число дней амортизации минус число дней между датой начала амортизации и последней датой операции основного средства.  

Учетная стоимость может быть снижена по учтенному повышению стоимости, понижению стоимости, суммам метода 1 и метода 2, в зависимости от того, установлен ли флажок напротив поля **Включать в расчет амортизации** или снят флажок **Часть балансовой стоимости** на странице **Настройка типа учета ОС**. Этот расчет обеспечивает полную амортизацию средства к моменту окончания амортизации.  

### <a name="fixed-yearly-percentage"></a>Фиксированный годовой процент

При указании фиксированного годового процента приложение будет использовать следующую формулу для расчета суммы амортизации:  

*Сумма амортизации = (Линейный (%) x базис амортизации x число дней амортизации) / (100 x 360)*  

### <a name="fixed-yearly-amount"></a>Фиксированная ежегодная сумма

При указании фиксированной ежегодной суммы приложение будет использовать следующую формулу для расчета суммы амортизации:  

*Сумма амортизации = (фиксированная сумма амортизации x число дней амортизации)/360*  

### <a name="example---straight-line-depreciation"></a>Пример - линейная амортизация

Основное средство имеет стоимость 100 000 рублей. Оценочный срок службы — восемь лет. Пакетное задание **Расчет амортизации** выполняется дважды в год.  

Для данного примера операция книги основных средств выглядит следующим образом:  

| Дата | Тип учета ОС | Дни | Сумма | Балансовая стоимость |
| --- | --- | --- | --- | --- |
| 01-01-20 |Стоимость приобретения |(Дата начала амортизации) |100,000.00 |100,000.00 |
| 06-30-20 |Амортизация |180 |-6 250,00 |93,750.00 |
| 12-31-20 |Амортизация |180 |-6 250,00 |87,500.00 |
| 06-30-21 |Амортизация |180 |-6 250,00 |81,250.00 |
| 12-31-21 |Амортизация |180 |-6 250,00 |75,000.00 |
| 06-30-27 |Амортизация |180 |-6 250,00 |6,250.00 |
| 12-31-27 |Амортизация |180 |-6 250,00 |0 |

## <a name="declining-balance-1-depreciation"></a>Амортизация с уменьшаемым остатком DB 1

Это метод ускоренной амортизации, с помощью которого самая большая часть себестоимости актива распределяется на первые годы срока полезного использования. При использовании этого метода необходимо указать фиксированный ежегодный процент.  

Формула для расчета сумм амортизации:  

*Сумма амортизации = (уменьшаемый остаток % x число дней амортизации x базис амортизации) / (100 x 360)*  

Базис амортизации рассчитывается как балансовая стоимость минус учтенная амортизация с момента начала текущего финансового года.  

Учтенная сумма амортизации может содержать операции с различными типами учета (понижение стоимости, метод 1 и метод 2), учтенными с начальной даты текущего финансового года. Эти типы учета включаются в сумму учтенной амортизации, если на странице **Настройки типа ОС учета** установлены флажки напротив полей **Тип амортизации** и **Часть балансовой стоимости**.  

### <a name="example---declining-balance-1-depreciation"></a>Пример - амортизация DB 1

Основное средство имеет стоимость 100 000 рублей. В поле **Уменьш. остатка, %** задано значение 25. Пакетное задание **Расчет амортизации** выполняется дважды в год.  

В следующей таблице показано, как выглядят операции книги основных средств.  

| Дата | Тип учета ОС | Дни | Сумма | Балансовая стоимость |
| --- | --- | --- | --- | --- |
| 01-01-20 |Стоимости приобретения |(Дата начала амортизации) |100,000.00 |100,000.00 |
| 06-30-20 |Амортизация |180 |-12 500,00 |87,500.00 |
| 12-31-20 |Амортизация |180 |-12 500,00 |75,000.00 |
| 06-30-21 |Амортизация |180 |-9 375,00 |65,625.00 |
| 12-31-21 |Амортизация |180 |-9 375,00 |56,250.00 |
| 06-30-22 |Амортизация |180 |-7 031,25 |49,218.75 |
| 12-31-22 |Амортизация |180 |-7 031,25 |42,187.50 |
| 06-30-23 |Амортизация |180 |-5 273,44 |36,914.06 |
| 12-31-23 |Амортизация |180 |-5 273,44 |31,640.62 |
| 06-30-24 |Амортизация |180 |-3 955,08 |27,685.54 |
| 12-31-24 |Амортизация |180 |-3 955,08 |23,730.46 |

Метод расчета:  

* Год 1: *25% от 100 000 = 25 000 = 12 500 + 12 500*

* Год 2: *25% от 75 000 = 18 750 = 9375 + 9375*

* Год 3: *25% от 56 250 = 14 062,50 = 7031,25 + 7031,25*

Расчет выполняется до тех пор, пока учетная стоимость не станет равной окончательной сумме округления или введенной ликвидационной стоимости.  

## <a name="declining-balance-2-depreciation"></a>Амортизация с уменьшаемым остатком DB 2

С помощью методов уменьшаемого остатка 1 и 2 вычисляются общие одинаковые суммы амортизации на каждый год. Однако, если пакетное задание **Расчет амортизации** выполняется чаще одного раза в год, использование метода уменьшаемого остатка 1 дает равные суммы амортизации для каждого периода амортизации. Использование метода уменьшаемого остатка 2 дает в результате суммы амортизации, которые уменьшаются с каждым периодом.  

### <a name="example---declining-balance-2-depreciation"></a>Пример. Амортизация методом уменьшаемого остатка 2

Основное средство имеет стоимость 100 000 рублей. В поле **Уменьш. остатка, %** задано значение 25. Пакетное задание **Расчет амортизации** выполняется дважды в год. Операции книги основных средств выглядят следующим образом:  

| Дата | Тип учета ОС | Дни | Сумма | Балансовая стоимость |
| --- | --- | --- | --- | --- |
| 01-01-20 |Стоимости приобретения |(Дата начала амортизации)|100,000.00 |100,000.00 |
| 06-30-20 |Амортизация |180 |-13 397,46 |86,602.54 |
| 12-31-20 |Амортизация |180 |-11 602,54 |75,000.00 |
| 06-30-21 |Амортизация |180 |-10 048,09 |64,951.91 |
| 12-31-21 |Амортизация |180 |-8 701,91 |56,250.00 |

Метод расчета:  

* *BV* = Учетная стоимость  
* *ND* = число дней амортизации  
* *DBP* = процент уменьшаемого остатка  
* *P* = *DBP*/100  
* *D* = *ND*/360  

Формула для расчета амортизационных отчислений:  

*DA* = *BV* x (1 – (1 –P)<sup>D</sup>)

Значениями амортизации являются:  

| Дата | Расчет |
| --- | --- |
| 06-30-20 |DA = 100 000,00 x (1 -(1 - 0,25)<sup>0,5</sup>) = 13 397,46 |
| 12-31-20 |DA = 86 602,54 x (1 - (1 - 0,25)<sup>0,5</sup>) = 11 602,54 |
| 06-30-21 |DA = 75 000,00 x (1 - (1 - 0,25)<sup>0,5</sup>) = 10 048,09 |
| 12-31-21 |DA = 64 951,91 x (1 - (1 - 0,25)<sup>0,5</sup>) = 8 701,91 |

## <a name="db1sl-depreciation"></a>Амортизация DB1/SL

DB1/SL — это сокращение, обозначающее сочетание уменьшаемого остатка 1 и линейного. Расчет выполняется до тех пор, пока учетная стоимость не станет равной окончательной сумме округления или введенной ликвидационной стоимости.  

С помощью пакетного задания **Расчет амортизации** вычисляется сумма амортизации линейным методом и методом уменьшаемого остатка, но в журнал переносится только большая из этих сумм.  

Можно использовать различные проценты для расчета уменьшаемого остатка.  

При использовании данного метода необходимо указать предполагаемый срок полезного использования и процент уменьшающегося остатка на странице **Книга амортизации ОС**.  

### <a name="example---db1-sl-depreciation"></a>Пример. Амортизация DB1-SL

Основное средство имеет стоимость 100 000 рублей. На странице **ОС - книги амортизации**, в поле **Уменьш. остатка, %**, задано значение 25, а в поле **Число лет амортизации** задано значение 8. Пакетное задание **Расчет амортизации** выполняется дважды в год.  

Операции книги основных средств выглядят следующим образом:  

| Дата | Тип учета ОС | Дни | Сумма | Балансовая стоимость |
| --- | --- | --- | --- | --- |
| 01-01-20 |Стоимости приобретения |(Дата начала амортизации) |100,000.00 |100,000.00 |
| 06-30-20 |Амортизация |180 |-12 500,00 |87,500.00 |
| 12-31-20 |Амортизация |180 |-12 500,00 |75,000.00 |
| 06-30-21 |Амортизация |180 |-9 375,00 |65,625.00 |
| 12-31-21 |Амортизация |180 |-9 375,00 |56,250.00 |
| 06-30-22 |Амортизация |180 |-7 031,25 |49,218.75 |
| 12-31-22 |Амортизация |180 |-7 031,25 |42,187.50 |
| 06-30-23 |Амортизация |180 |-5 273,44 |36,914.06 |
| 12-31-23 |Амортизация |180 |-5 273,44 |31,640.62 |
| 06-30-24 |Амортизация |180 |-3 955,08 |27,685.54 |
| 12-31-24 |Амортизация |180 |-3 955,08 |23,730.46 |
| 06-30-25 |Амортизация |180 |-3 955,08 |19 775,38 SL |
| 12-31-25 |Амортизация |180 |-3 955,08 |15 820,30 SL |
| 06-30-26 |Амортизация |180 |-3 955,08 |11 865,22 SL |
| 12-31-26 |Амортизация |180 |-3 955,07 |7 910,15 SL |
| 06-30-27 |Амортизация |180 |-3 955,08 |3 955,07 SL |
| 12-31-27 |Амортизация |180 |-3 955,07 |0,00 SL |

`SL` после значения учетной стоимости означает, что был использован линейный метод.  

Метод расчета:  

* Год 1 (2020):  

    *Сумма уменьшаемого остатка: 25% от 100 000 = 25 000 = 12 500+12 500*  

    *Сумма SL = 100 000/8=12 500= 6 250+6 250*  

    Используется сумма уменьшаемого остатка, поскольку она является более высокой.  

* Год 5 (2025):  

    *Сумма уменьшаемого остатка: 25% от 23 730,46 = 4 943,85= 2 471,92+2 471,92*  

    *Сумма SL = 23 730,46/3 = 7 910,15=3 995,07+3 995,08*  

    Используется линейная (SL) сумма, поскольку она является более высокой.  

## <a name="user-defined-depreciation"></a>Определенная пользователем амортизация

В приложении существует средство, позволяющее настраивать определенные пользователем методы амортизации.  

В определяемом пользователем методе используется страница **Таблицы амортизации**, в котором необходимо указать процент амортизации для каждого периода (месяца, квартала, года или учетного периода). Затем, когда вы назначаете книгу амортизации с помощью пользовательского метода для основных средств, вы должны задать поля **Первая польз. дата аморт.** и **Дата начала амортизации** на странице **Книга амортизации ОС** для конкретного основного средства.  

Формула для расчета амортизационных отчислений:  

*Сумма амортизации = (амортизация % x число дней амортизации x базис амортизации) / (100 x 360)*  

### <a name="depreciation-based-on-number-of-units"></a>Амортизация на основании числа единиц

Этот определяемый пользователем метод также можно использовать для амортизации на основании единиц товара, например при учете производственных машин с известным сроком службы. На странице **Таблицы амортизации** можно ввести число единиц, которые могут производиться в каждый период (месяц, квартал, год и учетный период).  

### <a name="to-set-up-user-defined-depreciation-methods"></a>Настройка пользовательских методов амортизации

На странице **Таблица амортизации** можно задать определяемые пользователем методы амортизации. Например, можно настроить амортизацию на основе количества единиц.  

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Таблицы амортизации**, затем выберите соответствующую ссылку.  
2. На странице **Список таблиц амортизации** выберите действие **Создать**.  
3. На странице **Карточка таблицы амортизации** заполните поля по мере необходимости. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

> [!TIP]
> Используйте функцию **Создание табличной части** для определения таблицы амортизации на основе метода *Сумма цифр*.

При методе *Сумма цифр*: если основные средства амортизируются в течение 4 лет, то амортизация за каждый год рассчитывается следующим образом:

Сумма цифр = 1 + 2 + 3 + 4 = 10 Амортизация:

* Год 1 = 4/10  
* Год 2 = 3/10  
* Год 3 = 2/10  
* Год 4 = 1/10  

### <a name="example---user-defined-depreciation"></a>Пример. Определенная пользователем амортизация

Используется метод амортизации, который позволяет амортизировать средства ускоренным путем с целью снижения налогов.  

В целях снижения налогов необходимо использовать следующие нормы амортизации основных средств с трехгодичным сроком:  

* Год 1: 25%  
* Год 2: 38%  
* Год 3: 37%  

Стоимость приобретения — 100 000 рублей, а срок амортизации — пять лет. Амортизация вычисляется ежегодно.  

| Дата | Тип учета ОС | Дни | Сумма | Балансовая стоимость |
| --- | --- | --- | --- | --- |
| 01-01-20 |Стоимость приобретения |(Дата начала амортизации) |100,000.00 |100,000.00 |
| 12-31-20 |Амортизация |360 |-25 000,00 |75,000.00 |
| 12-31-21 |Амортизация |360 |-38 000,00 |37,000.00 |
| 12-31-22 |Амортизация |360 |-37 000,00 |0 |
| 12-31-23 |Амортизация |Нет |Нет |0 |
| 12-31-24 |Амортизация |Нет |Нет |0 |

Если используется метод, определенный пользователем, то поля **Первая польз. дата аморт.** и **Дата начала амортизации** должны заполняться на странице **Книги амортизации ОС** для конкретного основного средства. Поле **Первая польз. дата аморт.** и содержимое поля **Длина периода** на странице **Таблицы амортизации** используются для определения интервалов времени, которые будут использоваться для расчета амортизации. Это гарантирует, что приложение начнет использовать указанный процент в один день для всех основных средств. Поле **Дата начала амортизации** используется для определения количества дней амортизации.  

В предыдущем примере оба поля **Первая польз. дата аморт.** и **Дата начала амортизации** будут заданы как 01-01-20 на странице **Книга амортизации ОС** для конкретного основного средства. Однако, если бы в поле **Первая польз. дата аморт.** было задано значение 01.01.20, а в поле **Дата начала амортизации** — значение 01.04.20, то в результате получилось бы следующее:  

| Дата | Тип учета ОС | Дни | Сумма | Балансовая стоимость |
| --- | --- | --- | --- | --- |
| 01-01-20 |Стоимость приобретения |(Дата начала амортизации) |100,000.00 |100,000.00 |
| 12-31-20 |Амортизация |270 |-18 750,00 |81,250.00 |
| 12-31-21 |Амортизация |360 |-38 000,00 |42,250.00 |
| 12-31-22 |Амортизация |360 |-37 000,00 |6,250.00 |
| 12-31-23 |Амортизация |90 |-6 250,00 |0 |
| 12-31-24 |Амортизация |Нет |Нет |0 |

## <a name="half-year-convention-depreciation"></a>Амортизация с полугодовой нормой износа

Метод амортизации путем начисления полугодовой нормы износа будет применяться только, если установлен флажок в поле **Использ. начисл. полугод. нормы износа** на фиксированной странице **Книга амортизации ОС**.  

Этот метод амортизации можно использовать в сочетании со следующими методами амортизации в приложении:  

* SL  
* DB 1  
* DB1/SL  

При применении полугодового соглашения основное средство имеет шестимесячную амортизацию в первый финансовый год вне зависимости от содержимого поля **Дата начала амортизации**.  

> [!NOTE]  
> При использовании метода полугодового соглашения оценочное время жизни основного средства, оставшееся после первого финансового года, всегда включает в себя полгода. Поэтому для правильного применения метода полугодового соглашения в поле **Дата окончания амортизации** на странице **Книга амортизации ОС** всегда должна быть указана дата, после которой остается ровно шесть месяцев до конечной даты финансового года, когда основное средство становится полностью амортизированным.  

### <a name="example---half-year-convention-depreciation"></a>Пример. Амортизация с полугодовой нормой износа

Основное средство имеет стоимость 100 000 рублей. Дата в поле **Дата начала амортизации** — 01.03.20. Оценочный срок службы составляет пять лет, таким образом, **Дата окончания амортизации** должна быть 30.06.25. Таким образом, **Дата окончания амортизации** должна быть. Этот пример основан на календарном финансовом году.  

Операции книги основных средств выглядят следующим образом:  

| Дата | Тип учета ОС | Дни | Сумма | Балансовая стоимость |
| --- | --- | --- | --- | --- |
| 03-01-20 |Стоимость приобретения |(Дата начала амортизации) |100,000.00 |100,000.00 |
| 12-31-20 |Амортизация |270 |-10 000,00 |90,000.00 |
| 12-31-21 |Амортизация |360 |-20 000,00 |70,000.00 |
| 12-31-22 |Амортизация |360 |-20 000,00 |50,000.00 |
| 12-31-23 |Амортизация |360 |-20 000,00 |30,000.00 |
| 12-31-24 |Амортизация |360 |-20 000,00 |10,000.00 |
| 12-31-25 |Амортизация |180 |-10 000,00 |0.00 |

## <a name="example---db1sl-depreciation-using-half-year-convention"></a>Пример. Амортизация DB1/SL с использованием полугодовой нормы износа

Основное средство имеет стоимость 100 000 рублей. Дата в поле **Дата начала амортизации** — 01.11.20. Оценочный срок службы составляет пять лет, таким образом, **Дата окончания амортизации** должна быть 30.06.25. На странице **Книга амортизации ОС** поле **Уменьш. остатка, %** содержит значение 40. Таким образом, **Дата окончания амортизации** должна быть 30.06.05. Этот пример основан на календарном финансовом году.  

Операции книги основных средств выглядят следующим образом:  

| Дата | Тип учета ОС | Дни | Сумма | Балансовая стоимость |
| --- | --- | --- | --- | --- |
| 11-01-20 |Стоимость приобретения |(Дата начала амортизации) |100,000.00 |100,000.00 |
| 12-31-20 |Амортизация |60 |-20 000,00 |80,000.00 |
| 12-31-21 |Амортизация |360 |-32 000,00 |48,000.00 |
| 12-31-22 |Амортизация |360 |-19 200,00 |28,800.00 |
| 12-31-23 |Амортизация |360 |-11 520,00 |17,280.00 |
| 12-31-24 |Амортизация |360 |-11 520,00 |5 760,00 SL |
| 12-31-25 |Амортизация |180 |-5 760,00 |0,00 SL |

`SL` после значения учетной стоимости означает, что был использован линейный метод.  

Метод расчета:  

* Год 1:  

    *Сумма уменьшаемого остатка = Полная годовая сумма = 40% от 100 000 = 40 000.* Таким образом, за полугодие 40 000 / 2 = 20 000  

    *Сумма SL = Полная годовая сумма = 100 000 / 5 = 20 000.* Таким образом, за полугодие = 20 000 / 2 = 10 000  

    Используется сумма уменьшаемого остатка, поскольку она является более высокой.  

* Год 5 (2024):  

    *Сумма уменьшаемого остатка = 40% от 17 280,00 = 6 912,00*  

    *Сумма SL = 28 800 / 1,5 = 11 520,00*  

    Используется линейная (SL) сумма, поскольку она является более высокой.  

## <a name="duplicating-entries-to-more-depreciation-books"></a>Дублирование операций в дополнительные книги амортизации

При наличии трех книг амортизации B1, B2 и B3 и необходимости копирования операций из B1 в B2 и B3 можно установить флажок в поле **Часть списка дубликатов** в карточках книг амортизации B2 и B3. Это может быть полезно, если книга B1 объединена с главной книгой и использует журнал ГК финансового учета основных средств, а книги амортизации B2 и B3 не объединены с главной книгой и используют журнал основных средств.  

Если при вводе операции в книге B1 журнала ГК учета основных средств установлен флажок в поле **Использ. список дублирования**, программа копирует операцию в книги B2 и B3 журнала основных средств после учета операции.  

> [!NOTE]  
> Невозможно дублировать операцию одновременно в журнал и раздел журнала, из которого производится дублирование. Если бухгалтерские операции учитываются в журнале ГК учета основных средств, то их можно дублировать в другом разделе журнала основных средств или журнала финансового учета.  

> [!NOTE]  
> Невозможно использовать одну и ту же серию номеров в журнале ГК основных средств и в журнале основных средств. При учете операций в ГК журнала ОС необходимо оставить поле **Номер документа** незаполненным. При вводе номера в поле номер дублируется в журнале основных средств. Необходимо вручную изменить номер документа перед учетом журнала.  

## <a name="see-also"></a>См. также

[Основные Средства](fa-manage.md)  
[Настройка основных средств](fa-setup.md)  
[Финансы](finance.md)  
[Подготовьтесь к ведению бизнеса](ui-get-ready-business.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]