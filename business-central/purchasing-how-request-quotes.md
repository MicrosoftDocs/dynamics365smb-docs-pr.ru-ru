---
title: Создание предложения по покупке для запроса предложения
description: Описывается процесс создание предложения по продаже или запроса предложения (RFQ) для записи вашего предложения клиенту для продажи продуктов на определенных условиях.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: rfq
ms.date: 06/23/2021
ms.author: edupont
ms.openlocfilehash: 3872a996149404e15349dd85221289bc819ad5cc
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "6443270"
---
# <a name="request-quotes"></a>Запрос предложений
Предложение по покупке может использоваться в качестве предварительного предложения по заказу на покупку, а заказ затем может быть преобразован в счет или заказ на покупку.


## <a name="to-create-a-purchase-quote"></a>Создание предложения по покупке
1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Предложения по покупке**, а затем выберите связанную ссылку.
2. Создайте новый документ, так же, как это делается для заказа на покупку. Дополнительные сведения см. в разделе [Регистрация покупок](purchasing-how-record-purchases.md).

## <a name="to-convert-a-purchase-quote-to-a-purchase-order"></a>Преобразование предложения по покупке в заказ на покупку
Когда вы приняли предложение поставщика, можно преобразовать его в счет или заказ покупки для обработки покупки.

1. Откройте предложение по покупке, которое готово к преобразованию, затем выберите действие **Сделать заказ**.

Предложение по покупке удаляется из базы данных. Создается счет покупки или заказ на покупку на основе сведений в предложении по покупке, в котором можно обработать покупку. В поле **Номер предложения** в счете покупке или заказе покупки отображается номер предложения по покупки, из которого он создан.

## <a name="see-also"></a>См. также
[Покупки](purchasing-manage-purchasing.md)  
[Настройка покупки](purchasing-setup-purchasing.md)  
[Отправка документов по электронной почте](ui-how-send-documents-email.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]