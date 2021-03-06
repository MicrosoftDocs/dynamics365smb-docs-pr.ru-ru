---
title: Как архивировать документы о продажах и покупке | Документация Майкрософт
description: Можно архивировать заказы продажи и покупки, предложения, заказы на возврат и общие заказы, и можно использовать архивный документ для восстановления документа, из которого он был архивирован.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 209ef492bf5620921ce371a17227653576dcae8a
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775901"
---
# <a name="archive-documents"></a>Архивирование документов
Можно поместить в архив заказы на продажу и покупку, предложения с расценками, заказы на возврат и общие заказы, например, если хотите сохранить копию документа для повторного пользования позднее. Можно поместить в архив документ по продаже или покупке несколько раз, каждый раз сохраняя другую архивную версию.

Для архивных документов, для которых оригинал все еще существует и не учтен, можно использовать функцию **Восстановить**, чтобы перезаписать оригинал архивной версией документа. Это целесообразно, если необходимо восстановить содержимое документа на более раннем этапе.

Для архивных документов, для которых оригинал удален, содержимое можно использовать только путем копирования данных, например с помощью функции **Копировать из документа**.   

## <a name="to-set-up-automatic-document-archiving"></a>Настройка автоматического архивирования документов  
Можно настроить автоматическое архивирование заказов продаж и покупки, предложений, общих заказов и заказов на возврат перед удалением документов.

Следующая процедура описывает, как настроить автоматическое архивирование документов продажи. Действия для документов на покупку аналогичны.
1.  Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Продажи и дебитор. задолж."**, затем выберите соответствующую ссылку.
2. На странице **Настройка модуля "Продажи"** заполните поля, как указано ниже.

|Поле|Описание|
|-----|-----------|
|**Архивирование предложений по продаже**|**Никогда**, чтобы никогда не архивировать предложения по продаже при их удалении. **Вопрос**, чтобы предлагать пользователю выбрать, требуется ли архивировать предложения по продаже перед их удалением. **Всегда**, чтобы автоматически архивировать предложения по продаже при их удалении.|
|**Архивирование общих заказов на продажу**|Выберите для автоматического архивирования общих заказов на продажу каждый раз при их удалении.|
|**Архивировать заказы и заказы на возврат**|Выберите для автоматического архивирования заказов на продажу каждый раз при их удалении.|

## <a name="to-archive-a-sales-order"></a>Архивирование заказа на продажу
Следующая процедура описывает, как архивировать заказ на продажу. Эти шаги аналогичны для всех заказов, общих заказов, заказов на возврат и предложений.

1.  Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.  
2.  Откройте заказ на продажу, который требуется архивировать.  
3.  Выберите действие **Архивировать документ**.

Заказ на продажу архивирован. Его можно просмотреть на странице **Архивные заказы на продажу**.

## <a name="to-restore-a-non-posted-sales-order-from-the-archive"></a>Восстановление неучтенного заказа на продажу из архива
Далее описывается процедура переноса содержимого архивного заказа на продажу назад в оригинальный заказ на продажу. Это возможно только в том случае, если исходный документ не был учтен. Эти шаги аналогичны для всех заказов, общих заказов, заказов на возврат и предложений.

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Архивные заказы на продажу**, затем выберите соответствующую ссылку.
2. Выберите архивированный заказ на продажу или ту его версию, которую требуется восстановить, затем выберите действие **Восстановить**.  

Содержимое оригинального заказа на продажу заменяется содержимым выбранной архивной версии.

## <a name="to-delete-archived-sales-orders"></a>Удаление архивных заказов продажу
Следующая процедура описывает, как удалить архивные заказы на продажу. Шаги аналогичны для всех остальных архивных документов продажи и покупки.

1.  Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Удалить архивные версии заказов продажи**, затем выберите соответствующую ссылку.  
2.  На странице **Удалить архивные версии заказов продажи** выберите соответствующие фильтры.  
3.  Нажмите кнопку **ОК**.

## <a name="see-also"></a>См. также
[Отслеживание строк документа](across-how-to-track-document-lines.md)  
[Продажи](sales-manage-sales.md)  
[Общие бизнес-функции](ui-across-business-areas.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]