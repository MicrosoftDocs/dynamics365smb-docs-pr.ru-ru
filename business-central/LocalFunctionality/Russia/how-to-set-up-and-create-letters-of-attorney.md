---
title: Настройка и создание доверенностей в России
description: Российские усовершенствования включают создание и печать доверенностей.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: cc4cc21751f4c53d58aaac6e537a5f8bfc1208c7
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5770617"
---
# <a name="set-up-and-create-letters-of-attorney"></a>Создание и настройка доверенности

Функция доверенностей позволяет создавать и печатать доверенности, а также печатать журнал доверенностей.  

Настройте нумерацию для открытых и выпущенных доверенностей. Номера для открытых документов генерируются после создания нового документа. Номера для выпущенных документов генерируются после печати документа. Этот номер заносится в форму печати документа и в журнал доверенностей.  

Ниже показано, как настроить нумерацию для доверенностей.

## <a name="to-set-up-a-letter-of-attorney"></a>Настройка доверенности 

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Покупки и кредиторская задолженность"**, затем выберите соответствующую ссылку.
2. На экспресс-вкладке **Фоновая разноска** заполните поля **Серия номеров доверенностей** и **Серия номеров выпущенных доверенностей**.
3. Нажмите кнопку **ОК**.

Ниже показано, как создать доверенность.

## <a name="to-create-a-letter-of-attorney"></a>Создание доверенности 

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Доверенности**, затем выберите соответствующую ссылку.

2. Создайте новый документ и заполните поля в следующей таблице.

   | Поле                      | Описание                                                  |
   | :------------------------- | :----------------------------------------------------------- |
   | **Номер доверенности** | Введите номер напечатанного документа. Этот номер заносится в форму печати документа и в журнал доверенностей. Это поле заполняется автоматически из серии номеров. |
   | **Код сотрудника**           | Введите номер сотрудника.                                   |
   | **ФИО сотрудника**     | Определяет имя сотрудника. Это поле заполняется автоматически из **карточки сотрудника**. |
   | **Должность сотрудника**     | Определяет должность сотрудника. Это поле заполняется автоматически из **карточки сотрудника**. |
   | **Тип исходного документа**   | Введите тип исходного документа. Доверенность (заголовок и строки) можно создать на основе существующего еще неучтенного документа покупки. |
   | **Номер исходного документа**    | Введите номер исходного документа.                            |
   | **Код поставщика**    | Определяет номер поставщика. Оно заполняется автоматически в соответствии с документом покупки, когда выбран исходный документ. Выбрать поставщика можно вручную. |
   | **Название поставщика**   | Определяет имя поставщика. Это поле заполняется автоматически из **карточки поставщика**. |
   | **Описание документа**   | Определяет сведения об исходном документе. Это поле заполняется автоматически, но можно ввести описание документа и вручную. |
   | **Отметка о выполнении**      | Определяет документ, который выполнен.                     |
   | **Дата Документа**          | Введите дату доверенности. По умолчанию в этом поле указана рабочая дата. При необходимости введите дату документа вручную. |
   | **Срок действия**          | Введите дату окончания срока действия для документа. По умолчанию в этом поле указана дата на 15 дней позже даты документа. При необходимости введите дату окончания срока действия вручную. |
   | **Статус**                 | Определяет статус документа.                        |
   | **Номер**                    | Введите номер открытого документа. Это поле заполняется автоматически из серии номеров. |

3. Нажмите кнопку **ОК**.

## <a name="see-also"></a>См. также

[Настройка материально-ответственных сотрудников и авансовых отчетов](How-to-Set-Up-Responsible-Employees-and-Advance-Statements.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]