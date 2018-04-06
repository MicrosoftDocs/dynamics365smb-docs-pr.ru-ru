---
title: "Практическое руководство. Сторнирование учета выхода | Документы Майкрософт"
description: "Бывают случаи, когда учет выхода необходимо сторнировать. Например, если произошла ошибка при вводе данных и в производственном заказе учтено неверное количество выхода."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f2430dcf45303e04baad406880783ab0f74dd4f2
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="reverse-output-posting"></a>Сторнирование учета выхода
Бывают случаи, когда учет выхода необходимо сторнировать. Например, если произошла ошибка при вводе данных и в производственном заказе учтено неверное количество выхода.  

## <a name="to-reverse-an-output-posting"></a>Сторнирование проводки по выпуску  
1.  Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журнал выхода продукции**, затем выберите связанную ссылку. Выберите пакет.  
2. Заполните соответствующим образом поля. Дополнительные сведения см. разделе [Учет в пакетном режиме выпуска продукции и времени работы](production-how-to-post-output-quantity.md).
3.  В поле **Примен. к операции** выберите соответствующую операцию книги товаров. При этом будут сторнированы операции журналов производственных мощностей и товаров.  
4. Учтите сторнирование путем учета журнала.  

Операции журнала выхода продукции учитываются в книге товаров как положительная корректировка.  

## <a name="see-also"></a>См. также  
 [Производство](production-manage-manufacturing.md)    
 [Настройка производства](production-configure-production-processes.md)  
 [Планирование](production-planning.md)      
 [Наличие](inventory-manage-inventory.md)  
 [Покупки](purchasing-manage-purchasing.md)  
 [Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

