---
title: "Создание карточек товаров для товаров или услуги | Документы Майкрософт"
description: "Карточки товаров создаются для услуг, которые вы продаете по часам, а также для физических продуктов, например для сборочных элементов, готовой продукции, сырья или компонентов, которые вы продаете из складских запасов."
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: item, finished good, component, raw material, assembly item
ms.date: 08/31/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: ea9b4a6310df319df06d02c53b9d6156caaee24f
ms.openlocfilehash: ac7664480d5a2db4642ecc2cb830c4d7022fb53b
ms.contentlocale: ru-ru
ms.lasthandoff: 03/28/2018

---
# <a name="register-new-items"></a>Регистрация новых товаров
Товары, наряду с другими продуктами, лежат в основе вашего бизнеса; это услуги или продукты, которыми вы торгуете. Каждый товар должен быть зарегистрирован в виде карточки товара.

В карточках товаров содержатся сведения, необходимые для покупки, хранения, продажи, доставки и учета товаров.

Карточка товара может иметь тип **Запасы** или **Услуга**, чтобы указать, является ли товар физической единицей или трудовой единицей измерения времени. Помимо некоторых полей, связанных с физическими аспектами товара, все поля в карточке товара функционируют одинаково для товаров в запасах и услуг. Дополнительные сведения о продаже товара см. в разделах [Продажа продукции](sales-how-sell-products.md) и [Выставление счетов продажи](sales-how-invoice-sales.md).

Товар может быть структурирован как родительский товар с основными дочерними товарами в спецификации. В [!INCLUDE[d365fin](includes/d365fin_md.md)] спецификация может быть или сборочной спецификацией, или производственной спецификацией, в зависимости от ее использования. Дополнительные сведения см. в разделе [Работа со спецификациями](inventory-how-work-BOMs.md).

> [!NOTE]  
>   Если существуют шаблоны товаров для различных типов товаров, при создании новой карточки товара отобразится окно, из которого можно выбрать подходящий шаблон. Если существует только один шаблон товара, для создания новых карточек товаров всегда используется этот шаблон.

Если вы приобретаете один и тот же товар у нескольких поставщиков, можно связать этих поставщиков с карточкой товара. Поставщики тогда будут отображаться в окне **Каталог поставщиков товаров**, чтобы вы могли легко выбирать другого поставщика.

## <a name="to-create-a-new-item-card"></a>Создание новой карточки товара
1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Товары**, а затем выберите связанную ссылку.  
2. В окне **Товары** выберите действие **Создать**.

    Если существует только один шаблон товара, откроется новая карточка товара, в которой некоторые поля будут заполнены сведениями из шаблона.
3. В окне **Выбор шаблона для нового товара** выберите шаблон, который требуется использовать для новой карточки товара.
4. Нажмите кнопку **ОК**. Откроется новая карточка товара, в которой некоторые поля будут заполнены сведениями из шаблона.
5. Заполните или измените поля в карточке товара по мере необходимости. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]
> В поле **Метод учета себестоимости** вы настраиваете способ, при помощи которого вычисляется себестоимость единицы товара, делая допущения относительно физического движения товара через организацию. Предусмотрено пять методов учета себестоимости, в зависимости от типа товара. Дополнительные сведения см. в разделе [Сведения о проектировании: методы учета себестоимости](design-details-costing-methods.md).
>
> Если выбран вариант **Среднее**, себестоимость единицы товара рассчитывается как средняя себестоимость единицы в каждый момент времени после покупки. Запасы переоцениваются из допущения, что все запасы продаются одновременно. При этой настройте можно выбрать поле **Себестоимость единицы** для просмотра в окне **Обзор расчета средней себестоимости** истории транзакций, на основе которых рассчитана средняя себестоимость.

На экспресс-вкладке **Цена и учет** вы можете увидеть специальные цены или скидки, предоставляемые по товару при соблюдении определенных критериев, например по клиенту, минимальному количеству заказа или дате окончания. Каждая строка представляет специальную цену или скидку строки. В каждом столбце представлен критерий, который необходимо применить, чтобы гарантировать специальную цену, введенную в поле **Цена за единицу**, или скидку строки, вводимую в поле **Скидка строки %**. Дополнительные сведения см. в разделе [Регистрация соглашений о цене продажи, скидках и платежах](sales-how-record-sales-price-discount-payment-agreements.md).

Теперь товар зарегистрирован, и карточка товара готова к использованию в документах покупки и продажи.

Если эту карточку товара требуется использовать в качестве шаблона при создании новых карточек товаров, ее можно сохранить в качестве шаблона. Дополнительные сведения см. в следующем разделе.

## <a name="to-save-the-item-card-as-a-template"></a>Сохранение карточки товара в качестве шаблона
1. В окне **Карточка товара** выберите действие **Сохранить как шаблон**. Открывается окно **Шаблон товаров** с отображаемой карточкой товара в виде шаблона.
2. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Для повторного использования измерений в шаблонах, выберите действие **Измерения**. Открывается окно **Шаблоны измерений** с отображением кодов измерений, настроенных для этого товара.
4. Измените или введите коды измерений, которые будут применяться к новым карточкам товаров, созданным с помощью шаблона.
5. Заполнив шаблон нового товара, нажмите кнопку **ОК**.

Шаблон товара добавляется в список шаблонов товаров, чтобы можно было использовать его для создания новых карточек товаров.

## <a name="to-set-up-multiple-vendors-for-an-item"></a>Настройка нескольких поставщиков для товара  
В случае покупки одного и того же товара у нескольких поставщиков, следует ввести информацию о каждом поставщике этого товара, такую как, цены, время ожидания, скидки и т.п.  

1.  Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Товары**, а затем выберите связанную ссылку.  
2.  Выберите соответствующий товар, затем выберите действие **Изменить**.  
3.  Выберите действие **Поставщики**.  
4.  Выберите поле **Код поставщика**, после чего укажите поставщика, которого нужно установить для товара.  
5.  Заполнение оставшихся полей необязательно.  
6.  Повторите шаги со 2 по 5 для каждого поставщика, у которого вы хотите приобретать товар.

Поставщики теперь будут отображаться в окне **Каталог поставщиков товаров**, которое открывается с карточки товара, чтобы можно было легко выбрать другого поставщика.

## <a name="see-also"></a>См. также
[Создание серий номеров](ui-create-number-series.md)  
[Наличие](inventory-manage-inventory.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Продажи](sales-manage-sales.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
