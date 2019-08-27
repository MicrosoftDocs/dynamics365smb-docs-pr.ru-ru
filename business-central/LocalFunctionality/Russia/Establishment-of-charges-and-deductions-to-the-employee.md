---
title: Установление начислений и отчислений в России
description: Российские улучшения включают начисления и отчисления.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 99849168f4f29bdbca86057b369924ce401d5e55
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738282"
---
# <a name="establishment-of-charges-and-deductions-to-the-employee"></a>Установление начислений и отчислений работнику

Журнал сотрудников является основным средством внесения изменений в список начислений/отчислений, установленных для сотрудника. Журнал сотрудников также может использоваться для записи приказов по сотрудникам, не связанных с финансами. 

Наиболее часто через журнал записываются: 

- приказы о премировании работника;


- приказы об административном штрафе; 

- приказы о выделении работнику льгот/социальных выплат, установленных законом; 

- заявления об отчислениях с работника, указанных в законе; 

- приказы о выделении работнику материальной помощи, подарка. 

  

> :speech_balloon: **примечание**
>
> Журнал работников не имеет ограничений по регистрации определенных видов начислений и отчислений, но основные условия труда должны быть изменяться путем дополнения трудового договора. Это обеспечивает возможность формирования необходимых печатных форм документов для работника. 

Список полей, которые должны быть заполнены в строке журнала сотрудников, определяется кодом зарплатного элемента. 

### <a name="fill-in-the-journal-lines-which-is-used-to-register-chargesdeductions-with-a-predetermined-amount"></a>Заполните строки журнала, которые используются для регистрации начислений/отчислений с заранее определенной суммой.

| Поле                           | Описание                                                  |
| ------------------------------- | ------------------------------------------------------------ |
| Дата учета                    | Определяет дату учета операции.                          |
| Код периода                     | Период начислений/отчислений. По умолчанию код периода определяется на основе даты учета. При необходимости код периода можно изменить. Код периода определяет, включены ли начислений/отчисления в документ заработной платы. |
| Дата Документа                   | Определяет дату создания связанного документа.    |
| Номер документа                    | Определяет номер связанного документа.                |
| Номер кадрового приказа                    | Номер кадрового приказа, который будет отображен в печатной форме документа. По умолчанию значение поля совпадает с полем "Номер" документа. |
| Дата кадрового приказа                   | Дата кадрового приказа, которая будет отображена в печатной форме документа. По умолчанию значение поля совпадает с полем "Дата" документа. |
| Код сотрудника                    | Определяет номер сотрудника.               |
| Код элемента                    | Определяет код связанного зарплатного элемента для целей налоговой регистрации. |
| Действие при учете                     | Добавить                                                          |
| Описание                     | Текстовое описание начислений/отчислений                 |
| Дата начала                   | Определяет первый день действия.             |
| Дата окончания                     | Определяет последний день действия. Поле не может быть пустым. В этом случае начисление интерпретируется как бессрочное и будет включаться в расчет заработной платы, пока оно не будет отменено. |
| Период начисления до/Период начисления от | Период, на который установлен этот тип начисления. Поле обязательно для элементов зарплаты типа "Премии". |
| Сумма                          | Сумма начислений/отчислений                                 |

Строка журнала должна быть учтена, чтобы начисления/отчисления были применены.

Все начисления и отчисления фиксируются в операциях книги сотрудников. Список начислений и отчислений каждого сотрудника доступен в карточке сотрудника. 

Сгенерированное начисление автоматически включается в расчет заработной платы за период, определенный полями даты начала и окончания. 

### <a name="update-charges"></a>Обновление начислений

Чтобы отменить или изменить ранее сделанное начисление сотрудникам, необходимо создать строку журнала сотрудников, как описано выше, за исключением следующих полей:

| Поле            | Описание                                                  |
| ---------------- | ------------------------------------------------------------ |
| Действие при учете      | **Закрыть** — чтобы остановить включение зарплатного элемента в заработную плату. Дата, с которой зарплатный элемент больше не включается в расчет заработной платы, должна быть указана в поле даты окончания (обычно это последний день месяца). Вы можете оставить поле "Сумма" пустым, так как значение этого поля не изменяется в книге сотрудников.                                                             **Обновить** — изменение суммы для существующего начислений/удержания. Обратите внимание, что поле "Сумма" должно быть заполнено. В противном случае сумма транзакции будет установлена на 0, то есть начисление/отчисление фактически отменяется. |
| Применяемая операция | Номер операции из журнала сотрудников, которую вы хотите закрыть или обновить. |

В процессе учета строки журнала этого типа указанная операция будет изменена в книге сотрудников. Изменение приводит к изменению суммы или даты окончания операции.

## <a name="see-also"></a>См. также

[Персонал](Human-Resources.md)