---
title: Работа со сборочными спецификациями
description: Сборочная спецификация создается для указания компонентов, требуемых для создания товара, который представляет спецификация.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: assembly bom, bills of material,
ms.search.form: 36, 5870, 5872, 5874
ms.date: 09/26/2022
ms.author: edupont
ms.openlocfilehash: 87379ca23e914cf29ebff0d4cfc13639ce6d0d54
ms.sourcegitcommit: 8ad79e0ec6e625796af298f756a142624f514cf3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2022
ms.locfileid: "9608257"
---
# <a name="work-with-assembly-boms"></a>Работа со сборочными спецификациями

Сборочные спецификации используются для структурирования родительских товаров, которые должны быть собраны из компонентов с минимальным использованием ресурсов или вовсе без него. Сборочная спецификация также может использоваться, например, для продажи родительского товара как комплекта, состоящего из товаров-компонентов.

Сборочные заказы используются для производства конечных элементов из компонентов в простом процессе, который может быть выполнен с помощью одного или нескольких ресурсов, которые не являются машинами или рабочими центрами, а также без использования ресурсов. Например, сборочный процесс может выбирать две бутылки вина и один мешок кофе, а затем упаковать их как подарочный набор.  

Сборочная спецификация — это основные данные, которые определяют, какие товары-компоненты попадают в собранный конечный товар и какие ресурсы используются для сборки сборочного элемента. При вводе сборочного элемента и количества в заголовке нового сборочного заказа, строки сборочного заказа автоматически заполняются в соответствии со сборочной спецификацией с одной строкой сборочного заказа на каждый компонент или ресурс. Подробнее см. в статье [Управление сборкой](assembly-assemble-items.md).

[!INCLUDE[prod_short](includes/prod_short.md)] также поддерживает производственные спецификации. Производственные спецификации отличаются от сборочных спецификаций тем, что включают более сложные процедуры, включая использование ресурсов, производственную маршрутизацию и рабочие или машинные центры. Подробнее о различиях см. в статьях [Работа со спецификациямиl](inventory-how-work-BOMs.md) и [Создание производственных спецификаций](production-how-to-create-production-boms.md).

## <a name="to-create-an-assembly-bom"></a>Создание сборочной спецификации

Для определения родительского товара, который состоит из других товаров и, возможно, ресурсов, необходимых для создания родительского элемента, следует создать сборочную спецификацию.  

Сборочные спецификации обычно содержат товары, но могут также содержать один или несколько ресурсов, которые необходимы для создания сборочного элемента.

Сборочные спецификации могут быть многоуровневыми, что означает, что компонент сборочной спецификации может сам быть сборочным элементом. В этом случае поле **Сборочная спецификация** в строке сборочной спецификации содержит значение **Да**.

Особые требования применяются к товарам в сборочных спецификациях в отношении доступности. Подробнее см. в статье [Просмотр доступности товара по использованию в сборочных спецификациях](inventory-how-availability-overview.md#to-view-the-availability-of-an-item-by-its-use-in-assembly-or-production-boms).

Создание новой сборочной спецификации выполняется в два этапа:

- Настройка нового товара
- Определение структуры спецификации сборочного элемента.

1. Настройте новый товар. Подробнее в разделе [Регистрация новых товаров](inventory-how-register-new-items.md).

   Введите компоненты или ресурсы в сборочной спецификации.  
2. На странице **Карточка товара** для сборочного элемента выберите действие **Сборка**, а затем выберите действие **Сборочная спецификация**.
3. На странице **Сборочная спецификация** заполните поля по мере необходимости. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!TIP]
> Сборочные элементы могут иметь разные варианты, заданные в [!INCLUDE[prod_short](includes/prod_short.md)] — точно так же, как и любой другой товар; это помогает сократить список доступных продуктов. Подробнее об этой функции см. в статье [Управление вариантами продукта](inventory-item-variants.md).

## <a name="to-edit-assembly-boms"></a>Редактирование сборочных спецификаций

Вы можете редактировать строки в сборочной спецификации в любое время. Но имейте в виду, что спецификация может использоваться в текущих продажах или сборках родительского узла, на которые может повлиять это изменение. Выберите действие **Применимость**, чтобы увидеть, в каких позициях она используется и могут ли быть затронуты заказы на продажу или сборку.

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок, введите **Товары**, а затем выберите соответствующую ссылку.
2. Выберите значение **Да** в столбце **Сборочная спецификация**.
3. На странице **Сборочная спецификация** выберите действие **Изменить список**, а затем измените любое поле, как вам нужно.

## <a name="to-view-components-and-resources-indented-according-to-the-bom-structure"></a>Просмотр компонентов и ресурсов с отступом согласно структуре спецификации

Со страницы **Сборочная спецификация** можно открыть отдельную страницу, на которой отображаются компоненты и все ресурсы с отступом согласно позиции спецификации в сборочном элементе.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") введите **Товары**, а затем выберите соответствующую ссылку.
2. Откройте карточку сборочного элемента. (Поле **Сборочная спецификация** на странице **Товары** содержит значение **Да**).
3. На странице **Карточка товара** выберите действие **Сборка**, а затем выберите действие **Сборочная спецификация**.
4. На странице **Сборочная спецификация** выберите действие **Показать спецификацию**.

## <a name="to-replace-the-assembly-item-with-its-components-on-document-lines"></a>Замена сборочного элемента его компонентами в строках документа

Из любого документа покупки и продажи, который содержит сборочный элемент, можно использовать специфическую функцию для замены строки для сборочного элемента новыми строками для его компонентов. Эта функция полезна, например, если требуется продавать компоненты как комплект, который представляет сборочный элемент.

Действие **Раскрыть спецификацию** также доступно на странице **Сборочная спецификация** как способ просмотра вложенных сборочных элементов в сборочной спецификации.

> [!CAUTION]  
> После использования функции **Раскрыть спецификацию** простых способов отмены этого действия не существует. Необходимо удалить строки заказа на продажу, которые представляют компоненты, а затем снова ввести строку заказа на продажу для сборочного элемента.

Следующая процедура основана на счете на продажу. Эти же действия применяются к другим документам на продажу и ко всем документам на покупку.

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок, введите **Счета продажи**, затем выберите связанную ссылку.
2. Откройте счет продажи, содержащий строку для сборочного элемента.
3. Выберите строку для сборочного элемента, затем выберите действие строки **Раскрыть спецификацию**.

Все поля в строке счета продажи для сборочного элемента очищаются, за исключением полей **Товар** и **Описание**. Заполненные строки счета продажи вставляются для компонентов и возможных ресурсов, составляющих сборочный элемент.

> [!NOTE]
> Отчет **Сборочный лист по заказу** также изменяется и отображает только компоненты. Это означает, что работник склада, который подбирает родительский элемент — сборочный элемент — не будет видеть его в сборочном листе. Подробнее см. в статье [Печать сборочного листа](sales-how-print-picking-list.md).

## <a name="to-calculate-the-standard-cost-of-an-assembly-item"></a>Вычисление стандартной себестоимости сборочного элемента

При расчете себестоимости единицы себестоимость каждого сборочного элемента сводится с себестоимостью каждого компонента и каждого ресурса в производственной спецификации товара.

Можно также рассчитать и обновить стандартную себестоимость для одного или нескольких товаров на странице **Журнал станд. себестоимостей**. Подробнее см. в статье [Обновление стандартных себестоимостей](finance-how-to-update-standard-costs.md).  

Себестоимость единицы в сборочной спецификации всегда равняется сумме себестоимостей ее компонентов, включая другие сборочные спецификации, и всех ресурсов.  

> [!NOTE]
> [!INCLUDE [bom-standard-cost](includes/bom-standard-cost.md)]

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, а затем выберите соответствующую ссылку.
2. Откройте карточку сборочного элемента. (Поле **Сборочная спецификация** на странице **Товары** содержит значение **Да**).
3. На странице **Карточка товара** выберите действие **Сборка**, а затем выберите действие **Сборочная спецификация**.
4. На странице **Сборочная спецификация** выберите действие **Расчет станд. себестоимости**.
5. Выберите один из следующих параметров, затем нажмите кнопку **ОК**.

|Параметр |Описание |
|-------|------------|
|**Верхний уровень**|Вычисляет стандартную себестоимость сборочного элемента как общую себестоимость всех приобретенных или собранных товаров по данной сборочной спецификации, независимо от возможных базовых сборочных спецификаций.|
|**Все уровни**|Рассчитывает стандартную себестоимость товара сборки как сумму: 1) Себестоимость всех базовых сборочных спецификаций для сборочной спецификации. 2) Себестоимость всех приобретенных товаров в сборочной спецификации.|

Себестоимости товаров, которые составляют сборочную спецификацию, копируются из карточек товара компонента. Себестоимость каждого товара умножается на количество, и общая себестоимость отображается в поле **Себестоимость единицы** в карточке товара.

## <a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/set-up-assembly-items-dynamics-365-business-central/).

## <a name="see-also"></a>См. также

[Регистрация новых товаров](inventory-how-register-new-items.md)  
[Управление вариантами продукта](inventory-item-variants.md)  
[Просмотр наличия товара](inventory-how-availability-overview.md)  
[Запасы](inventory-manage-inventory.md)  
[Работа со спецификациями](inventory-how-work-BOMs.md)  
[Создание производственных спецификаций](production-how-to-create-production-boms.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]