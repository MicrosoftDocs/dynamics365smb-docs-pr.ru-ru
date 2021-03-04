---
title: Практическое руководство. Настройка методов отгрузки | Документация Майкрософт
description: Для предлагаемого метода отгрузки можно задать код и указать соответствующую информацию.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: incoterms
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: f1916724c995f875d15b931e919d07d2253dcdb1
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4748298"
---
# <a name="set-up-shipment-methods"></a>Настройка методов отгрузки
Зачастую методы отгрузки, называемые также ИНКОТЕРМС, зависят от товаров, клиентов и поставщиков. Например, если клиент живет на острове, то товары могут быть ему отправлены или по воздуху, или морем. Некоторым клиентам может потребоваться доставка на следующий день. Другие могут захотеть забрать заказ. В карточках клиента и поставщика определяется требуемый тип доставки.

Описание и код каждого метода отгрузки настраивается на странице **Методы отгрузки**. Например, можно настроить код ФОБ и ввести "Франко-борт" в поле **Описание**. Затем код можно ввести в поля **Код метода отгрузки** по всей программе, например, в карточку клиента. После этого при создании заказов, счетов, кредит-нот и т. д. программа будет вводить описание, представленное данным кодом. При необходимости его можно изменить в документе.

## <a name="to-set-up-a-shipment-code"></a>Настройка кода отгрузки
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Методы отгрузки**, затем выберите соответствующую ссылку.
2. На странице **Методы отгрузки** выберите действие **Создать**.
3. В новой строке определите код и описание для метода отгрузки.

## <a name="see-also"></a>См. также
[Инкотермс](https://iccwbo.org/resources-for-business/incoterms-rules)  
[Настройка экспедиторов](sales-how-to-set-up-shipping-agents.md)  
[Трассировка посылок](sales-how-track-packages.md)    
[Управление складом](warehouse-manage-warehouse.md)  
[Запасы](inventory-manage-inventory.md)  
[Настройка управления складом](warehouse-setup-warehouse.md)     
[Управление сборкой](assembly-assemble-items.md)    
[Сведения о проектировании: управление складом](design-details-warehouse-management.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]