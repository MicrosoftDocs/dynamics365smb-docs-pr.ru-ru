---
title: Создание предложения по покупке для запроса предложения
description: Описывается процесс создание предложения по продаже или запроса коммерческого предложения (RFQ) для записи вашего предложения клиенту для продажи продуктов на определенных условиях.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: rfq
ms.search.form: '49, 97, 9306, 9346'
ms.date: 08/08/2022
ms.author: edupont
---
# <a name="request-quotes"></a><a name="request-quotes"></a><a name="request-quotes"></a>Запрос предложений

Предложение по покупке может использоваться в качестве предварительного предложения по заказу на покупку, которое затем может быть преобразовано в счет покупки.

## <a name="create-a-purchase-quote"></a><a name="create-a-purchase-quote"></a><a name="create-a-purchase-quote"></a>Создание предложения по покупке

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок, введите **Предложения по покупке**, затем выберите связанную ссылку.
2. Создайте новый документ, так же, как это делается для заказа на покупку. Подробнее в разделе [Регистрация покупок](purchasing-how-record-purchases.md).

## <a name="convert-a-purchase-quote-to-a-purchase-order"></a><a name="convert-a-purchase-quote-to-a-purchase-order"></a><a name="convert-a-purchase-quote-to-a-purchase-order"></a>Преобразование предложения по покупке в заказ на покупку

Когда вы приняли предложение поставщика, можно преобразовать его в заказ покупки для обработки покупки.

1. Откройте предложение по покупке, которое необходимо преобразовать, затем выберите действие **Сделать заказ**.

Предложение по покупке удаляется из базы данных. Создается заказ на покупку на основе сведений в предложении по покупке, которое можно использовать для обработки покупки и затем учесть счет покупки. В поле **Номер предложения** в счете покупки и заказе покупки отображается номер предложения по покупки, из которого они созданы.

> [!NOTE]
> Невозможно напрямую преобразовать предложение по покупке в счет покупки, как это можно сделать с предложениями по продаже. Подробнее о том, как создать счет покупки, см. в разделе [Регистрация покупок с помощью счетов покупок](purchasing-how-record-purchases.md).

## <a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/create-purchase-documents-dynamics-365-business-central/).

## <a name="see-also"></a><a name="see-also"></a><a name="see-also"></a>См. также

[Покупки](purchasing-manage-purchasing.md)  
[Настройка покупки](purchasing-setup-purchasing.md)  
[Отправка документов по электронной почте](ui-how-send-documents-email.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
