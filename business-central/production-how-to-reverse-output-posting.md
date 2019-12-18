---
title: Практическое руководство. Сторнирование учета выхода | Документация Майкрософт
description: Бывают случаи, когда учет выхода необходимо сторнировать. Например, если произошла ошибка при вводе данных и в производственном заказе учтено неверное количество выхода.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 2cdda8a01d6391f97bfae5600ce35d2ab989ae54
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2877852"
---
# <a name="reverse-output-posting"></a>Сторнирование учета выхода
Бывают случаи, когда учет выхода необходимо сторнировать. Например, если произошла ошибка при вводе данных и в производственном заказе учтено неверное количество выхода.  

## <a name="to-reverse-an-output-posting"></a>Сторнирование проводки по выпуску  
1.  Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал выхода продукции**, затем выберите соответствующую ссылку. Выберите пакет.  
2. Заполните соответствующим образом поля. Дополнительные сведения см. разделе [Учет в пакетном режиме выпуска продукции и времени работы](production-how-to-post-output-quantity.md).
3.  В поле **Примен. к операции** выберите соответствующую операцию книги товаров. При этом будут сторнированы операции журналов производственных мощностей и товаров.  
4. Учтите сторнирование путем учета журнала.  

Операции журнала выхода продукции учитываются в книге товаров как положительная корректировка.  

## <a name="see-also"></a>См. также  
 [Производство](production-manage-manufacturing.md)    
 [Настройка производства](production-configure-production-processes.md)  
 [Планирование](production-planning.md)      
 [Запасы](inventory-manage-inventory.md)  
 [Покупки](purchasing-manage-purchasing.md)  
 [Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
