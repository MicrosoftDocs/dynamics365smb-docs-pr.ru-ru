---
title: Включение платежей клиентов через службу платежей | Документация Майкрософт
description: Облегчите клиентам оплату счетов, включив службы платежей.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 753a9ae7b6b47113107bb9f9bdf439323cff615a
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3781739"
---
# <a name="enable-customer-payments-through-payment-services"></a><span data-ttu-id="e9d71-103">Включение платежей клиентов через службу платежей</span><span class="sxs-lookup"><span data-stu-id="e9d71-103">Enable Customer Payments Through Payment Services</span></span>
<span data-ttu-id="e9d71-104">В качестве альтернативы сбору платежей через банковские переводы или кредитные карты вы можете предложить клиентам оплату через учетную запись в службе платежей, например Microsoft Pay, PayPal или WorldPay.</span><span class="sxs-lookup"><span data-stu-id="e9d71-104">As an alternative to collecting payments through bank transfer or credit cards, your customers can pay you through their account with payment services, such as Microsoft Pay, PayPal, or WorldPay.</span></span>  

<span data-ttu-id="e9d71-105">После включения службы платежей в [!INCLUDE[d365fin](includes/d365fin_md.md)] станет доступна ссылка на службу в документах продажи, отправляемых по электронной почте клиентам.</span><span class="sxs-lookup"><span data-stu-id="e9d71-105">After you enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)], a link to the service is available on sales documents that you send by email to your customers.</span></span> <span data-ttu-id="e9d71-106">Клиенты могут использовать эту ссылку для перехода к службе платежей и оплаты счетов непосредственно из документа продажи.</span><span class="sxs-lookup"><span data-stu-id="e9d71-106">Customers can use the link to go to the payment service and pay the bill, directly from the sales document.</span></span> <span data-ttu-id="e9d71-107">Если не требуется включать ссылку, например если клиент платит наличными деньгами, можно удалить службу платежей из счета до учета.</span><span class="sxs-lookup"><span data-stu-id="e9d71-107">If you don't want to include the link, for example, if a customer will pay with cash, you can remove the payment service from the invoice before posting.</span></span>  

<span data-ttu-id="e9d71-108">Расширения Microsoft Pay, PayPal Payments Standard и WorldPay Payments Standard установлены в [!INCLUDE[d365fin](includes/d365fin_md.md)] и готовы к включению.</span><span class="sxs-lookup"><span data-stu-id="e9d71-108">The Microsoft Pay, PayPal Payments Standard, and WorldPay Payments Standard extensions are installed in [!INCLUDE[d365fin](includes/d365fin_md.md)], and are ready for you to enable.</span></span>  

## <a name="to-enable-a-payment-service-in-d365fin"></a><span data-ttu-id="e9d71-109">Включение службы платежей в [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="e9d71-109">To enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
1. <span data-ttu-id="e9d71-110">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Службы платежей**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e9d71-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e9d71-111">На странице **Службы платежей** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="e9d71-111">On the **Payment Services** page, choose the **New** action.</span></span>  
3. <span data-ttu-id="e9d71-112">Выберите службу платежей, затем закройте страницу.</span><span class="sxs-lookup"><span data-stu-id="e9d71-112">Select the payment service, and then close the page.</span></span>  
4. <span data-ttu-id="e9d71-113">На странице **Службы платежей** выберите действие **Настройка**.</span><span class="sxs-lookup"><span data-stu-id="e9d71-113">On the **Payment Services** page, choose the **Setup** action.</span></span>  
5. <span data-ttu-id="e9d71-114">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="e9d71-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. <span data-ttu-id="e9d71-115">Закройте страницу.</span><span class="sxs-lookup"><span data-stu-id="e9d71-115">Close the page.</span></span>  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a><span data-ttu-id="e9d71-116">Выбор службы платежей в счете продажи</span><span class="sxs-lookup"><span data-stu-id="e9d71-116">To select a payment service on a sales invoice</span></span>
1. <span data-ttu-id="e9d71-117">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета продажи**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e9d71-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e9d71-118">Откройте счет продажи, который необходимо оплатить с помощью службы платежей.</span><span class="sxs-lookup"><span data-stu-id="e9d71-118">Open the sales invoice that you want to pay by using the payment service.</span></span>  
3. <span data-ttu-id="e9d71-119">В поле **Служба платежей** выберите службу платежей.</span><span class="sxs-lookup"><span data-stu-id="e9d71-119">In the **Payment Service** field, choose the payment service.</span></span>  

    > [!NOTE]  
    > <span data-ttu-id="e9d71-120">Поле **Служба платежей** доступно, только если включена служба платежей.</span><span class="sxs-lookup"><span data-stu-id="e9d71-120">The **Payment Service** field is available only if you've enabled the payment service.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e9d71-121">См. также</span><span class="sxs-lookup"><span data-stu-id="e9d71-121">See Also</span></span>  
[<span data-ttu-id="e9d71-122">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="e9d71-122">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="e9d71-123">Продажи</span><span class="sxs-lookup"><span data-stu-id="e9d71-123">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="e9d71-124">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="e9d71-124">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="e9d71-125">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e9d71-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
