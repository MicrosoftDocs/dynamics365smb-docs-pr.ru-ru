---
title: Сторнирование учета выхода
description: Бывают случаи, когда учет выхода необходимо сторнировать. В этом разделе описывается процедура сторнирования проводки выхода.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 5510
ms.date: 06/22/2021
ms.author: edupont
ms.openlocfilehash: ed45facfc64dda670d0e1e4d7dd9b396b4c11fae
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "8132789"
---
# <a name="reverse-output-posting"></a>Сторнирование учета выхода

Бывают случаи, когда учет выхода необходимо сторнировать. Например, если произошла ошибка при вводе данных и в производственном заказе учтено неверное количество выхода.  

## <a name="to-reverse-an-output-posting"></a>Сторнирование проводки по выпуску

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Журнал выхода продукции**, а затем выберите связанную ссылку. Выберите пакет.  
2. Заполните соответствующим образом поля. Дополнительные сведения см. разделе [Учет в пакетном режиме выпуска продукции и времени работы](production-how-to-post-output-quantity.md).
3. В поле **Примен. к операции** выберите соответствующую операцию книги товаров. При этом будут сторнированы операции журналов производственных мощностей и товаров.  
4. Учтите сторнирование путем учета журнала.  

Операции журнала выхода продукции учитываются в книге товаров как положительная корректировка.  

## <a name="see-also"></a>См. также

 [Производство](production-manage-manufacturing.md) [Настройка производства](production-configure-production-processes.md)  
 [Планирование](production-planning.md)  
 [Запасы](inventory-manage-inventory.md)  
 [Покупки](purchasing-manage-purchasing.md)  
 [Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]