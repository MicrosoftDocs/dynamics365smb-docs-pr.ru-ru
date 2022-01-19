---
title: Настройка отслеживания товаров по серийному номеру, номеру партии и номеру упаковки
description: Настройка отслеживания товаров по серийному номеру, номеру партии и номеру упаковки
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 08/31/2021
ms.author: edupont
ms.openlocfilehash: c6bfeeadda01ee82981f40eb49431fc6d40aebbc
ms.sourcegitcommit: 04055135ff13db551dc74a2467a1f79d2953b8ed
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/08/2021
ms.locfileid: "7482514"
---
# <a name="set-up-item-tracking-with-serial-lot-and-package-numbers"></a>Настройка отслеживания товаров по серийному номеру, номеру партии и номеру упаковки

Следите за товарно-материальными запасами даже в сложных складских конфигурациях с номерами, которые специфичны для каждого товара, будь то отдельный объект, партия или упаковка. С помощью отслеживания товаров вы можете отслеживать перемещения товаров на внутреннем складе, а также исходящие и входящие документы.

Товары с серийными номерами и номерами партий можно отслеживать как в прямом, так и в обратном направлении по цепочке поставок. Это полезно для общего обеспечения качества и для отзывов продукции. Дополнительные сведения см. в разделе [Отслеживание товаров, трассируемых по товарам](inventory-how-to-trace-item-tracked-items.md).  

> [!TIP]
> В выпуске волны 1 2021 года и более поздней версии включите обновление функции *использование отслеживания по номеру пакета в системе резервирования и трассировки*, если вы хотите работать с номерами упаковок, а также с серийными номерами и номерами партий. Для получения дополнительной информации см. [Раннее включение новых функций](admin-feature-management.md). После включения этой функции вы можете назначать номера упаковок исходящим и входящим документам аналогично тому, как вы можете работать с номерами партий.  

## <a name="numbers-and-item-tracking"></a>Номера и отслеживание товаров

В рамках складских процессов можно объединить ваши запасы в упаковки, коробки, контейнеры и т. д. Но чтобы отслеживать товары, вы присваиваете уникальные номера для идентификации. Например, вы производите и продаете стул с номенклатурным номером *1900-S*. У каждого отдельного стула есть серийный номер, *1001*, но вы также упаковываете четыре стула в партию, *LOT0001*, и вы отгружаете стулья в контейнере с номером упаковки *CONTAINER010*, который также включает другие товары, такие как *LOT0100* с боковыми столиками и *LOT200* с лампами.  

В зависимости от вашей конфигурации, вы используете эти разные номера для отслеживания запасов в [!INCLUDE [prod_short](includes/prod_short.md)] на разных этапах покупки, продажи, складских операций и т. д.

## <a name="to-set-up-item-tracking-codes"></a>Настройка кодов трассировки товара

Код трассировки товара отражает различные соображения, имеющиеся у организации в отношении использования серийных номеров и номеров партий для товаров, перемещающихся внутри сети складов.  

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Коды трассировки товаров**, а затем выберите связанную ссылку.  
2. Выберите действие **Создать**.
3. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. На экспресс-вкладках **Серийный номер**, **Номер партии** и **Номер упаковки** определите политики трассировки товаров соответственно по серийным номерам, номерам партий и номерам упаковок.  

> [!NOTE]  
> Если вы хотите отслеживать конкретные товары или конкретные партии на протяжении всего их срока службы, необходимо выбрать поля **Трассировка СН** и **Партия - трассировка** соответственно. В результате при обработке исходящей единицы товара с этим кодом отслеживания товара необходимо всегда будет указывать, какой существующий серийный номер или какой существующий номер партии обрабатывать. Это означает, что при продаже единицы товара номер должен применяться в соответствии с конкретным пулом серийных номеров или с конкретным номером партии на складе. Или, иначе говоря, серийный номер или номер партии, присваиваемый товару при вводе на складе, должен соответствовать этому типу товара и после того, как он покинет склад.

Поскольку настройка конкретного поля охватывает все возможные транзакции с данным товаром, в индивидуальных входящих/исходящих полях также будут установлены флажки. Однако, индивидуальные входящие/исходящие поля не применимы ко всему складу — они только определяют рабочий процесс вашей компании в части времени присвоения номеров для трассировки товара.  

> [!NOTE]  
>  Чтобы присвоить номера трассировки товаров в складских операциях, необходимо установить поля **Трассировка по СН склада** и **Склад партии - трассировка** в карточке "Код трассировки товара".  

## <a name="to-set-up-expiration-rules-for-serial-or-lot-numbers"></a>Настройка правил срока действия для серийных номеров или номеров партий

Для некоторых товаров может потребоваться настроить особые даты срока действия в коде трассировки товара. Это позволит постоянно отслеживать моменты истечения срока действия конкретных серийных номеров и номеров партий.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Коды трассировки товаров**, а затем выберите связанную ссылку.
2. Выберите имеющийся код трассировки товара, затем выберите действие **Правка**.  
3. На экспресс-вкладке **Прочее** установите следующие поля:  

    |Поле|Описание|  
    |---------------------------------|---------------------------------------|  
    |**Строгий учет срока годности**|Указывает, что дату истечения срока годности, установленную для номеру трассировки товара при его поступлении на склад, необходимо соблюдать при его выходе со склада.|  
    |**Требуется ввод даты истечения срока годности**|Указывает, что необходимо ввести дату истечения срока годности в строке трассировки товара.|  
    |**Использовать сроки годности**|Укажите, что нужно вычислять сроки годности. |  

## <a name="to-set-up-warranties-for-serial-or-lot-numbers"></a>Настройка гарантий для серийных номеров или номеров партий

Для некоторых товаров может потребоваться настроить особые гарантии в коде трассировки товара. Это позволит постоянно отслеживать моменты истечения гарантий по конкретным серийным номерам или номерам партий в складском запасе.  

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Коды трассировки товаров**, а затем выберите связанную ссылку.  
2. Выберите имеющийся код трассировки товара, затем выберите действие **Правка**.  
3. На экспресс-вкладке **Прочее** заполните поле **Формула даты гарантии**, затем установите поля следующим образом:  

    |Поле|Описание|  
    |---------------------------------|---------------------------------------|  
    |**Формула даты гарантии**|Определяет дату истечения строка гарантии для данного товара.|  
    |**Требуется ввод даты гарантии**|Определяет, что необходимо вручную ввести дату гарантии в строке трассировки товара.|  


## <a name="to-set-up-items-for-tracking-with-the-correct-item-tracking-codes"></a>Чтобы настроить товары для отслеживания с использованием правильных кодов отслеживания товаров

Чтобы включить отслеживание товара, сначала необходимо присвоить товару коды отслеживания товара. Есть два способа добавить коды отслеживания товаров: выбрав код из предварительно определенного списка или назначив новый уникальный код. Наведите указатель на поля, чтобы увидеть короткое описание.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Товар**, а затем выберите связанную ссылку.
2. Выберите существующий товар из списка и откройте страницу **Карточка товара**.  
3. На экспресс-вкладке **Отслеживание товара** назначьте соответствующие коды отслеживания товаров и выберите **Код отслеживания товара**, **Серийные номера** и **Номера партий**.
    1. В качестве альтернативы вы также можете создать новый код отслеживания товара, выбрав действие **Создать**.

## <a name="see-also"></a>См. также

[Работа с серийными номерами и номерами партий](inventory-how-work-item-tracking.md)
[Трассировка товаров, трассируемых по товарам](inventory-how-to-trace-item-tracked-items.md)  
[Запасы](inventory-manage-inventory.md)  
[Сведения о проектировании: трассировка товара](design-details-item-tracking.md)  
[Сведения о проектировании. Трассировка и резервирование товара](design-details-item-tracking-and-reservations.md)  
[Резервирование товаров](inventory-how-to-reserve-items.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]