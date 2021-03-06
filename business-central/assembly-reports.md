---
title: Отчеты по сборке и аналитика в Business Central
description: Посмотрите, какие отчеты по сборке и аналитика доступны в стандартной версии Business Central, чтобы вы могли отслеживать свой бизнес.
author: AndreiPanko
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: reporting
ms.date: 06/01/2021
ms.author: andreipa
ms.openlocfilehash: 91234cd02736d425116be40137efd9d068b5bd97
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "6216391"
---
# <a name="assembly-reports-and-analytics-in-business-central"></a>Отчеты по сборке и аналитика в Business Central

Отчетность по сборке в [!INCLUDE [prod_short](includes/prod_short.md)] позволяет профессионалам производства и бизнеса получать информацию и статистические данные о текущей и прошлой деятельности по сборке.  

## <a name="reports"></a>Отчеты

В следующей таблице описаны некоторые ключевые отчеты отчетности по сборке.

|Отчет |ИД объекта|Описание  |
|---------|---------|---------|
|**Сборочные спецификации**|801|Отображает список "Спецификации": имя, номер спецификации, компоненты спецификации и любые другие спецификации, которые в свою очередь являются частью спецификаций. Компоненты комплекта определены в таблице "Компонент спецификации". Здесь вы также увидите единицу измерения и необходимое количество каждого компонента на базовую единицу измерения. |
|**Товар - возможно сделать (время)**|5871|Отображает, как пять различных ключевых показателей доступности изменяются с течением времени для товара в спецификации. Эти цифры изменяются в соответствии с ожидаемыми событиями спроса и предложения и с поставками, основанными на наличии компонентов, которые можно собрать или произвести.<br>Этот отчет можно использовать для просмотра, можно ли выполнить заказ на продажу товара в указанную дату. Для этого просмотрите текущее наличие товара и потенциальное количество, которое можно получить при выполнении сборочного заказа. В отчете указывается, когда и сколько единиц сборочных элементов и изготавливаемого товара можно сделать, на основании доступности компонентов и текущего наличия товара. Это отображается как общее количество.<br>Информация отображается на графике, где каждый показатель наличия представлен в виде строки, которая идет вдоль графика времени и поднимается и опускается по мере изменения количества. Значения количества поступают из того же источника, который предоставляет информацию в окно **Доступность товаров по уровню спецификации**. |
|**Долевое распределение затрат на спецификацию**|5872|Графически отображает, как себестоимость собранного или произведенного товара распределяется посредством его спецификации.<br>Такая информация может быть полезна при принятии решения, например, о том, следует ли заменить поставщиков компонентов, заменить внутреннее использование производственных мощностей внешними или наоборот, или при просмотре и изменении спецификации материала.<br>Первая диаграмма в отчете показывает общую себестоимость единицы компонентов и трудовых ресурсов родительского товара с разбивкой по пяти разным долям себестоимости, что представлено графически разными цветами.<br>Круговая диаграмма с заголовком *По материалам/трудозатратам* показывает пропорциональное распределение между затратами на материал и трудовыми затратами родительского товара, а также его собственные производственные накладные расходы. Доля себестоимости материала включает себестоимость материала товара. Доля затрат на труд включает производственные мощности, накладные расходы по производственной мощности и затраты на субподряд. Доли себестоимости отображаются по-разному в зависимости от параметра, выбранного в поле **Показать только**.<br>Круговая диаграмма с заголовком *По прямым/косвенным* показывает пропорциональное распределение между прямыми и косвенными затратами родительского товара. Доля прямой себестоимости включает материал товара, производственные мощности и затраты на субподряд. Доля косвенных затрат включает накладные расходы по производственной мощности и производственные накладные расходы.<br>Таблица в нижней части отчета включена при установке флажка "Включить подробности". Это показывает выбранные значения в окне "Структура затрат спецификации" на одном уровне или свернутыми в зависимости от параметра, который вы выбираете в поле "Показать доли себестоимости как".|
|**Список использования**|809|Отображает список спецификаций, компонентами которых являются выбранные товары. Полезный обзор на случай, если вам нужно изменить компонент в спецификации, которая вставляется в сборочный элемент. Например, если ваш поставщик больше не может поставить конкретный элемент, который вы использовали для сборки или производства. В таких сценариях этот отчет предоставляет простой обзор того, в какие спецификации включен компонент. Вы можете установить фильтр по номеру компонента.|
|**Спецификация — сырье**|810|Этот отчет может дать вам обзор необходимых компонентов как для сборки, так и для производства. Вы увидите инвентарь, базовую единицу измерения, основного поставщика, если поставщик нет. прописано в самой карточке товара, а также в расчете времени выполнения заказа.|
|**Спецификация — сборочные узлы**|811|Если вы производите и/или собираете подузлы, используйте этот отчет, чтобы получить обзор этого типа компонента. В этом отчете показаны базовая единица измерения, запасы, удельные затраты и альтернативный номенклатурный номер. |
|**Сборочная спецификация — конечные товары**|812|Показывает список товаров и спецификаций, которые не являются компонентами "Спецификации". **Примечание**. Этот отчет не ограничивается только спецификацией, поэтому не забудьте установить фильтр в поле **Сборочная спецификация** или поле **Система пополнения**.|
|**Сборка для заказа — продажи**|915|Отображает ключевые показатели продаж товаров для сборочного компонента, которые могут быть проданы как часть комплекта при сборке на заказ и как отдельный товар непосредственно со склада.<br>Этот отчет позволяет проанализировать количество, себестоимость, продажи и прибыль от компонентов сборки для поддержания решений, например стоит ли установить другую цену на набор или исключить некий товар из сборки.<br>В строке **В сборке** показаны показатели продаж для общего количества, проданного в виде отдельных товаров. Продажи конкретного сборочного элемента, которые суммируются для получения этого итогового значения, отображаются, если выбрано поле **Показать сведения о сборке**.<br>Основное внимание сосредоточено на сборочных компонентах, однако показатели вычисляются на основе размера прибыли родительского сборочного элемента. Соответственно, сумма продажи каждого компонента рассчитывается из сего себестоимости и размера прибыли родительского элемента по следующей формуле.<br>В отчете приводится информация по товарам, которые отвечают одному или обоим из следующих критериев:<br>- Существует в сборочной спецификации товара, который использует политику сборки Сборка на заказ.<br>- Продано как часть продажи сборки на заказ.|

## <a name="tasks"></a>Задачи

В следующих статьях описываются некоторые ключевые задачи анализа состояния вашего бизнеса:

* [Просмотр наличия товара](inventory-how-availability-overview.md)

## <a name="see-also"></a>См. также

[Управление сборкой](assembly-assemble-items.md)  
[Работа со спецификациями](inventory-how-work-boms.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
