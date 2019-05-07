---
title: Включение платежей клиентов через службу платежей | Документы Майкрософт
description: Облегчите клиентам оплату счетов, включив службы платежей.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: e5d4d9fd0c6857c22f2b4c929a6e6ed528cadf26
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "931680"
---
# <a name="enable-customer-payments-through-payment-services"></a>Включение платежей клиентов через службу платежей
В качестве альтернативы сбору платежей через банковские переводы или кредитные карты вы можете предложить клиентам оплату через учетную запись в службе платежей, например Microsoft Pay, PayPal или WorldPay.  

После включения службы платежей в [!INCLUDE[d365fin](includes/d365fin_md.md)] станет доступна ссылка на службу в документах продажи, отправляемых по электронной почте клиентам. Клиенты могут использовать эту ссылку для перехода к службе платежей и оплаты счетов непосредственно из документа продажи. Если не требуется включать ссылку, например если клиент платит наличными деньгами, можно удалить службу платежей из счета до учета.  

Расширения Microsoft Pay, PayPal Payments Standard и WorldPay Payments Standard установлены в [!INCLUDE[d365fin](includes/d365fin_md.md)] и готовы к включению.  

## <a name="to-enable-a-payment-service-in-included365finincludesd365finmdmd"></a>Включение службы платежей в [!INCLUDE[d365fin](includes/d365fin_md.md)]
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Службы платежей**, затем выберите связанную ссылку.  
2. На странице **Службы платежей** выберите действие **Создать**.  
3. Выберите службу платежей, затем закройте страницу.  
4. На странице **Службы платежей** выберите действие **Настройка**.  
5. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. Закройте страницу.  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a>Выбор службы платежей в счете продажи
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета продажи**, затем выберите связанную ссылку.  
2. Откройте счет продажи, который необходимо оплатить с помощью службы платежей.  
3. В поле **Служба платежей** выберите службу платежей.  

    > [!NOTE]  
    > Поле **Служба платежей** доступно, только если включена служба платежей.  

## <a name="see-also"></a>См. также  
[Настройка продаж](sales-setup-sales.md)  
[Продажи](sales-manage-sales.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
