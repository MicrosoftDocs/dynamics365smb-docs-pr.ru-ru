---
title: "Включение платежей клиентов через службу платежей | Документы Майкрософт"
description: "Облегчите клиентам оплату счетов, включив службы платежей."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 5853080ef39196e95c293415e9b81502ff03d5ed
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="enable-customer-payments-through-payment-services"></a>Включение платежей клиентов через службу платежей
В качестве альтернативы сбору платежей через банковские переводы или кредитные карты вы можете предложить клиентам оплату через учетную запись в службе платежей, например Microsoft Pay, PayPal или WorldPay.  

После включения службы платежей в [!INCLUDE[d365fin](includes/d365fin_md.md)] станет доступна ссылка на службу в документах продажи, отправляемых по электронной почте клиентам. Клиенты могут использовать эту ссылку для перехода к службе платежей и оплаты счетов непосредственно из документа продажи. Если не требуется включать ссылку, например если клиент платит наличными деньгами, можно удалить службу платежей из счета до учета.  

Расширения Microsoft Pay, PayPal Payments Standard и WorldPay Payments Standard установлены в [!INCLUDE[d365fin](includes/d365fin_md.md)] и готовы к включению.  

## <a name="to-enable-a-payment-service-in-included365finincludesd365finmdmd"></a>Включение службы платежей в [!INCLUDE[d365fin](includes/d365fin_md.md)]
1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Службы платежей**, а затем выберите связанную ссылку.  
2. В окне **Службы платежей** выберите действие **Создать**.  
3. Выберите службу платежей, а затем закройте окно.  
4. В окне **Службы платежей** выберите действие **Настройка**.  
5. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. Закройте данное окно.  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a>Выбор службы платежей в счете продажи
1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Счета продажи**, а затем выберите связанную ссылку.  
2. Откройте счет продажи, который необходимо оплатить с помощью службы платежей.  
3. В поле **Служба платежей** выберите службу платежей.  

    > [!NOTE]  
    > Поле **Служба платежей** доступно, только если включена служба платежей.  

## <a name="see-also"></a>См. также  
[Настройка продаж](sales-setup-sales.md)  
[Продажи](sales-manage-sales.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
