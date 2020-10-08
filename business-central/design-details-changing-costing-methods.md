---
title: Сведения о проектировании — изменение методов учета себестоимости для товаров
description: Узнайте, как назначить товару другой метод учета себестоимости, хотя вы уже использовали этот товар в транзакциях.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: costing methods, costing, item cost
ms.date: 07/23/2020
ms.author: bholtorf
ms.openlocfilehash: 0560e2bf900af4b49d0ce299dfa751a5c41ea54e
ms.sourcegitcommit: 7b5c927ea9a59329daf1b60633b8290b552d6531
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "3617735"
---
# <a name="design-details-change-the-costing-method-for-items"></a>Сведения о проектировании: изменение методов учета себестоимости для товаров

В [!INCLUDE[d365fin](includes/d365fin_md.md)] нельзя изменить метод учета себестоимости для товара после того, как вы включили товар в транзакцию. Например, после того, как вы купили или продали товар. Если для товара или товаров был назначен неправильный метод учета себестоимости, вы можете не обнаружить проблему, пока не создадите финансовую отчетность.

В этом разделе описывается, как разрешить эту ситуацию. Рекомендуемый подход заключается в замене товара с неправильным методом учета себестоимости новым товаром и использовании заказа на сборку для переноса запаса из старого товара в новый.

> [!NOTE]
> Использование заказов на сборку позволяет расходам оставаться в потоке, хотя есть неоплаченные счета покупки или расходы по отгрузке для учета. Кроме того, он позволяет отменить преобразование и вернуть количество исходных товаров, если это необходимо.

> [!TIP]
> Чтобы ознакомиться с процессом, мы рекомендуем начать процесс преобразования с одного товара или небольшого набора товаров.

## <a name="about-costing-methods"></a>О методах расчета себестоимости

Методы расчета себестоимости контролируют расчеты себестоимости, когда товары приобретаются, поступают в запасы и продаются. Методы расчета себестоимости влияют на сроки сумм, записанных в COGS, которые влияют на общую прибыль. Именно этот поток вычисляет COGS. Стоимость проданных товаров (COGS) и доход используются для определения общей прибыли следующим образом:

*валовая прибыль* = *выручка – COGS*

Когда вы настраиваете товарные запасы, вы должны назначить метод расчета себестоимости. Метод может варьироваться от бизнеса к бизнесу и от товара к товару, поэтому важно выбрать правильный. Следующие методы учета себестоимости поддерживаются в [!INCLUDE[d365fin](includes/d365fin_md.md)]:

* Среднее
* Обслуживание в порядке поступления
* LIFO
* Стандартная
* Определенный

Дополнительные сведения см. в разделе [Сведения о проектировании: методы учета себестоимости](design-details-costing-methods.md).

## <a name="using-assembly-orders-to-change-costing-method-assignments"></a>Использование заказов на сборку для изменения назначений метода учета себестоимости

В этом разделе описываются следующие шаги для изменения метода учета себестоимости, назначенного товару:

1. Определите метод учета себестоимости по умолчанию.
2. Определите товары, для которых необходимо изменить метод учета себестоимости, и перенумеруйте их.
3. Создайте новые товары со старой схемой нумерации и скопируйте основные данные в пакете.
4. Вручную скопируйте связанные основные данные из существующего товара в новый товар.
5. Определите количество запасов для преобразования из исходного товара в новый.
6. Перенести запас на новый товар.
7. Обработка количества запасов, которые распределены по требованию.
8. Заблокируйте исходный товар от дальнейшего использования.  

### <a name="define-a-default-costing-method"></a>Определите метод учета себестоимости по умолчанию

Чтобы избежать ошибок в будущем, вы можете указать метод учета себестоимости для новых товаров по умолчанию. Всякий раз, когда кто-то создает новый товар, [!INCLUDE[d365fin](includes/d365fin_md.md)] предложит метод учета себестоимости по умолчанию. Вы указываете метод по умолчанию в поле **Метод учета себестоимости по умолчанию** на странице **Настройка запасов**. 

### <a name="identify-the-items-to-change-the-costing-method-for-and-renumber-them"></a>Определите товары, для которых необходимо изменить метод учета себестоимости, и перенумеруйте их

Возможно, вы захотите дать вашим новым товарам те же номера, что и заменяемым. Для этого измените номера существующих товаров. Например, если существующий номер товара — «P1000», вы можете изменить его на «X-P1000». Это изменение вручную, которое вы должны сделать для каждого товара.

### <a name="create-new-items-with-the-old-numbering-scheme-and-copy-the-master-data-in-a-batch"></a>Создайте новые товары со старой схемой нумерации и скопируйте основные данные в пакете

Создайте новые товары, используя текущую схему номеров. За исключением поля **Метод учета себестоимости** новые товары должны содержать те же основные данные, что и существующие товары. Для переноса основных данных для товара и связанных данных из других функций используйте действие **Копировать товар** на странице **Карточка товара**. Дополнительные сведения см. в разделе [Копирование существующих товаров для создания новых товаров](inventory-how-copy-items.md),

После создания новых товаров и переноса основных данных назначьте правильный метод расчета себестоимости.

### <a name="manually-copy-related-master-data-from-the-original-item-to-the-new-item"></a>Вручную скопируйте связанные основные данные из исходного товара в новый товар

Чтобы сделать новые товары полностью полезными, необходимо вручную скопировать некоторые основные данные из других областей, как описано в следующей таблице.

|Регион  |Что копировать  |Как это копировать  |
|---------|---------|---------|
|Запасы     |Единицы хранения (SKU)         |Проверьте, указана ли SKU для исходного товара. Если параметры планирования были введены для каждой карточки SKU, необходимо вручную создать SKU для нового товара. Если параметры не указаны, вы можете использовать пакетное задание **Создать единицу хранения** на странице **Карточка товара** для создания данных.        |
|     |Замены товара         |Проверьте, определены ли какие-либо замены товара для исходного товара. Если есть, перенесите эти данные в новый товар. Для просмотра заменяющих товаров используйте действие **Замены** на странице **Карточка товара**.         |
|     |Аналитические отчеты         |Просмотрите отчеты «Анализ товаров», «Анализ продаж» и «Анализ покупок». Для тех, которые ссылаются на исходные товары, вы можете либо создать новый отчет об анализе со ссылкой на новый товар (оставив исходный отчет об анализе для использования в качестве истории), либо настроить отчеты так, чтобы они ссылались на новый товар.         |
|     |Стандартные журналы         |Проверьте, ссылаются ли стандартные журналы на исходный товар, и перенесите эти данные в новый товар, когда это необходимо. Эта информация находится в стандартных журналах, которые доступны в журнале товаров.          |
|Продажи     |Проценты предоплаты при продаже         | Проверьте, определены ли какие-либо проценты предоплаты при продаже для исходного товара и перенесите эти данные в новый товар. Чтобы просмотреть проценты предоплаты, на странице **Карточка товара** выберите **Продажи**, а потом **Процент предоплаты**.        |
|Покупка     |Проценты предоплаты при покупке         |Проверьте, определены ли какие-либо проценты предоплаты при покупке для исходного товара и перенесите эти данные в новый товар. Чтобы просмотреть проценты предоплаты, на странице **Карточка товара** выберите **Покупки**, а потом **Процент предоплаты**.                 |
|Склад     |Содержимое ячейки         |Просмотрите содержимое ячейки, определенное для исходного товара. Если столбцы, такие как Мин. кол-во, Макс. кол-во, По умолчанию и Специальный были введены индивидуально, после чего вы должны вручную создать содержимое ячейки для нового товара. Если это не так, никаких действий не требуется. [!INCLUDE[d365fin](includes/d365fin_md.md)] будет вести записи при регистрации складских документов и журналов.|
|Работа     |Цена работы         |Проверьте, определены ли цены работ для исходного товара и перенесите эти данные в новый товар. Эта информация доступна на страница **Карточка работы** в части **Сведения о работе — Количество цен** на **информационной панели**.         |
|Сервис     |Квалификация сервисного ресурса         |Проверьте, определены ли квалификации сервисного ресурса для исходного товара и перенесите эти данные в новый товар. Для просмотра квалификации ресурсов используйте действие **Квалификация ресурсов** на странице **Карточка товара**.          |
|     |Компоненты сервисного товара         |Проверьте, определены ли компоненты для исходного сервисного товара и перенесите эти данные в новый товар. Для просмотра компонентов сервисного товара на страница **Карточка товара** использовать действие **Сервисный товар**, чтобы открыть список связанных сервисных товаров, а затем выберите действие **Компоненты**.          |
|Зона производства     |Производственные спецификации         |Проверьте, содержат ли какие-либо производственные спецификации исходный товар, и замените его новым. Чтобы заменить исходный товар, на странице **Производственные спецификации** выберите действие **Заменить товар в спецификации**.         |
|Сборка     |Сборочные спецификации         |Проверьте, содержат ли какие-либо сборочные спецификации исходный товар, и вручную замените его новым.         |

> [!IMPORTANT]
> Если новый метод расчета себестоимости является стандартным, вы должны ввести значение в поле **Стандартная себестоимость** на странице **Карточка товара**. Вы можете использовать страница **Журнал стандартной себестоимости**, чтобы установить доли себестоимости соответственно. Дополнительные сведения см. в разделе [Обновление стандартных себестоимостей](finance-how-to-update-standard-costs.md).

### <a name="determine-the-inventory-quantity-to-convert-from-the-original-item-to-the-new-item"></a>Определите количество запасов для преобразования из исходного товара в новый

> [!NOTE]
> Этот шаг не учитывает количества, включенные в неотгруженные заказы. Дополнительные сведения см. в [Обработка количества запасов, которые распределены по требованию](design-details-changing-costing-methods.md#handle-inventory-quantities-that-are-allocated-to-demand). 

Используйте журнал инвентаризации для составления списка количеств в запасах. В зависимости от настройки местоположения склада, используйте одно из следующего:

* Журналы инвентаризации
* Склад Журналы инвентаризации

Оба журнала могут рассчитать количество товара, включая местоположение, вариант, ячейку и расположение хранилища. Дополнительные сведения см. в разделе [Подсчет, корректировка и повторная классификация запасов с помощью журналов](inventory-how-count-adjust-reclassify.md).

### <a name="transfer-the-inventory-to-the-new-item"></a>Перенести запас на новый товар

Создание и учет заказов на сборку для переноса стоимости и количества запаса из исходного товара в новый. Заказы на сборку могут преобразовывать один товар в другой, сохраняя при этом затраты. Это помогает гарантировать, что чистые итоги для товарного счета и COGS не будут затронуты (за исключением случая, когда новый метод расчета себестоимости является стандартным, и в этом случае затраты могут быть распределены по вариациям счетов). Дополнительные сведения см. в разделе [Управление сборкой](assembly-assemble-items.md).

При создании заказов на сборку используйте информацию из журнала инвентаризации или склада. Журнал инвентаризации. В следующих таблицах описывается информация в отчетах, вводимая в заголовок и строки заказа на сборку.

#### <a name="header"></a>Заголовок

|Поле  |Значение для ввода  |
|---------|---------|
|Код товара     |Номер нового товара.         |
|количество;     |Количество в журнале инвентаризации.<br> **ПРИМЕЧАНИЕ:** Количества, рассчитанные в журналах инвентаризации, не включают количества в заказах, которые еще не были отгружены.          |
|Код варианта     |Так же, как в журнале инвентаризации.          |
|Код Склада     |Так же, как в журнале инвентаризации.         |
|Код единицы измерения     |Так же, как в журнале инвентаризации.         |
|Код ячейки     |Так же, как в журнале инвентаризации.         |

#### <a name="lines"></a>Строки

|Поле  |Значение для ввода  |
|---------|---------|
|Тип     |Товар         |
|Кол-во     |Номер нового исходного товара.         |
|Кол-во в     |1         |
|Код варианта     |Так же, как в журнале инвентаризации.         |
|Код Склада     |Так же, как в журнале инвентаризации.         |
|Код единицы измерения     |Так же, как в журнале инвентаризации.         |

> [!NOTE]
> Заказ на сборку может обрабатывать только один единицу хранения товара за раз. Необходимо создать заказ на сборку для каждой комбинации SKU, имеющей количество в запасе.

> [!NOTE]
> Для местоположения склада вам, возможно, придется создать подборы, прежде чем вы сможете учесть заказ на сборку. Чтобы выяснить это, просмотрите настройки подбора на странице **Карточка склада**. Дополнительные сведения см. в [Настройка товаров и складов для использования расширенного подбора и размещения](warehouse-how-to-set-up-items-for-directed-put-away-and-pick.md).

### <a name="handle-inventory-quantities-that-are-allocated-to-demand"></a>Обработка количества запасов, которые распределены по требованию

В идеале, запас для исходного товара должен обнуляться после переноса количества запаса. Однако могут быть невыполненные заказы, таблицы и журналы (см. Таблицу ниже), для которых по-прежнему требуется количество исходного товара. Количество также может быть заблокировано резервированием или отслеживанием товара.

**Пример** Есть 1000 шт. в инвентаре и 20 шт. зарезервированы для заказа на продажу, который еще не отгружен. В этом случае вы можете решить оставить 20 шт. в старом товаре, чтобы вы могли выполнить невыполненный заказ.

> [!NOTE]
> Есть функциональные области, которые могут влиять на количество, как указано в таблице ниже, поэтому может быть сложно найти правильное количество. В целях безопасности, используя приведенный выше пример, вы можете оставить 100 шт. и передать оставшиеся 900 шт. вместо. Еще один способ сделать это — обработать документы и журналы так, чтобы осталось только несколько управляемых. Еще одна альтернатива — перенести все количество на новый товар, а затем перенести часть ее обратно на исходный товар, используя заказ на сборку.

В следующей таблице перечислены функциональные области, в которых могут быть неоплаченные количества.

|Регион  |Где искать невыполненные количества  |
|---------|---------|
|Продажи     |Документы продажи, включая заказы, заказы на возврат, счета, предложения, общие заказы и кредит-ноты         |
|Запасы     |Журналы товаров, резервирования, отслеживание товаров и журнал стандартной себестоимости         |
|Покупка     |Документы покупки, включая заказы, заказы на возврат, счета, предложения, общие заказы и кредит-ноты         |
|Планирование     |Журнал заявки, журнал планирования и планирование заказов         |
|Склад     |Заказы на перемещение, складские отгрузки, складские журналы и складские подборы, размещения и перемещения, внутренние отборы и размещения и журналы создания ячеек         |
|Сборка     |Документы сборки, включая заказы, заказы на возврат и общие заказы         |
|Работы     |Строки планирования работ и строки журнала работ         |
|Сервис     |Сервисные документы и сервисные контракты         |
|Зона производства     |Производственные заказы (запланированные, утвержденные производственные и выпущенные)         |

### <a name="block-the-original-item-from-further-use"></a>Заблокируйте исходный товар от дальнейшего использования

Когда запас для исходного товара равен нулю, вы можете заблокировать товар, чтобы предотвратить его использование в новых транзакциях. Чтобы заблокировать товар, на странице **Карточка товара** включите **Заблокировано**. Дополнительные сведения см. в [Блокировка товаров для продажи или покупки](inventory-how-block-items.md).

## <a name="summary"></a>Сводка

Изменение метода расчета себестоимости для товаров, которые использовались в транзакциях, является процессом, а не стандартным действием в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Вы можете использовать шаги, описанные в этом разделе, в качестве шаблона для процесса.

Процесс может занять много времени, потому что есть несколько шагов вручную. Однако если вы потратите время на его выполнение, это сведет к минимуму влияние ошибок на вашу главную книгу.

Мы рекомендуем следующее:

1. Оцените выполнимость процесса, взяв один или, возможно, несколько представительных товаров в течение всего процесса.
2. Подумайте о том, чтобы связаться с опытным партнером, который может помочь вам в этом процессе.

## <a name="see-also"></a>См. также

[Сведения о проектировании: методы учета себестоимости](design-details-costing-methods.md)  
[Обзор](design-details-inventory-costing.md)