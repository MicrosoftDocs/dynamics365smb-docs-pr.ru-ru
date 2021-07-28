---
title: Настройка методов отгрузки
description: Для предлагаемого метода отгрузки можно задать код и указать соответствующую информацию.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: incoterms
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 9ee6cdceb716331e2d8338e178def4b8b1e5cfe8
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "6436705"
---
# <a name="set-up-shipment-methods"></a>Настройка методов отгрузки

Часто методы отгрузки зависят от товаров, клиентов и поставщиков. Например, если клиент живет на острове, то товары могут быть ему отправлены или по воздуху, или морем. Некоторым клиентам может потребоваться доставка на следующий день. Другие могут захотеть забрать заказ. В карточках клиента и поставщика определяется требуемый тип доставки.

Описание и код каждого метода отгрузки настраивается на странице **Методы отгрузки**. Например, можно настроить код ФОБ и ввести "Франко-борт" в поле **Описание**. Затем код можно ввести в поля **Код метода отгрузки** по всей программе, например, в карточку клиента. После этого при создании заказов, счетов, кредит-нот и т. д. программа будет вводить описание, представленное данным кодом. При необходимости его можно изменить в документе.

## <a name="to-set-up-a-shipment-method"></a>Настройка метода отгрузки

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Методы отгрузки**, а затем выберите связанную ссылку.
2. На странице **Методы отгрузки** выберите действие **Создать**.
3. В новой строке определите код и описание для метода отгрузки.

> [!TIP]
> Если вы используете Инкотермс, настройте способы отгрузки для соответствующих правил Инкотермс.  

## <a name="see-also"></a>См. также

[Настройка экспедиторов](sales-how-to-set-up-shipping-agents.md)  
[Трассировка посылок](sales-how-track-packages.md)  
[Управление складом](warehouse-manage-warehouse.md)  
[Запасы](inventory-manage-inventory.md)  
[Настройка управления складом](warehouse-setup-warehouse.md)  
[Управление сборкой](assembly-assemble-items.md)  
[Сведения о проектировании: управление складом](design-details-warehouse-management.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Инкотермс на iccwbo.org](https://iccwbo.org/resources-for-business/incoterms-rules)  

[!INCLUDE[footer-include](includes/footer-banner.md)]