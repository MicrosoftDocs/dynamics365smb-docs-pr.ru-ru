---
title: Практическое руководство. Настройка экспедиторов | Документация Майкрософт
description: Для каждого экспедитора можно задать код и указать соответствующую информацию.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: fbd27caed8be1e7231f98964890fafed66c7bbbb
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4748222"
---
# <a name="set-up-shipping-agents"></a>Настройка экспедиторов
Для каждого экспедитора можно задать код и указать соответствующую информацию.  

Если для экспедитора указывается адрес Интернет и экспедитор предоставляет пакет услуг, связанных с трассировкой товара при помощи Интернет, можно использовать функцию автоматической трассировки посылок. Дополнительные сведения см. в разделе [Трассировка посылок](sales-how-track-packages.md).

При настройке в заказах продажи экспедиторов можно также указать услуги, предоставляемые каждым экспедитором.  
Для каждого экспедитора можно настроить неограниченное количество услуг и по каждой услуге указать время отгрузки.  

После того, как для строки продажи задана услуга экспедитора, время отгрузки для услуги будет включаться в расчет сроков по заказу для данной строки. Дополнительные сведения см. в разделе [Расчет сроков планирования заказов](sales-how-to-calculate-order-promising-dates.md).

## <a name="to-set-up-a-shipping-agent"></a>Настройка экспедитора  
1.  Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Экспедиторы**, затем выберите соответствующую ссылку.  
2.  Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].  
3.  Выберите действие **Услуги экспедитора**.
4. В поле **Услуги экспедитора** заполните требуемые поля.

> [!NOTE]  
>  Если удалить экспедитора из строки заказа, код услуги экспедитора для данной строки также будет удален. Производится пересчет содержимого полей, которые были частично связаны с данной услугой экспедитора.  

## <a name="see-also"></a>См. также
[Настройка методов отгрузки](sales-how-set-up-shipment-methods.md)  
[Трассировка посылок](sales-how-track-packages.md)    
[Управление складом](warehouse-manage-warehouse.md)  
[Запасы](inventory-manage-inventory.md)  
[Настройка управления складом](warehouse-setup-warehouse.md)     
[Управление сборкой](assembly-assemble-items.md)    
[Сведения о проектировании: управление складом](design-details-warehouse-management.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]