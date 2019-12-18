---
title: Настройка способов оплаты | Документация Майкрософт
description: Способы оплаты, например, чеки, банковские переводы, наличные или PayPal используются для того, чтобы определять, как именно должны оплачиваться счета на продажу и покупку.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, bank transfer, cash, PayPal
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: 753b9f30648059a68c22b524008e21c6c866d19c
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2882546"
---
# <a name="defining-payment-methods"></a><span data-ttu-id="94c55-103">Определение способов оплаты</span><span class="sxs-lookup"><span data-stu-id="94c55-103">Defining Payment Methods</span></span>
<span data-ttu-id="94c55-104">Методы оплаты определяют предпочтительный способ, которым клиенты осуществляют платежи вам, и способ, которым вы хотите платить поставщикам.</span><span class="sxs-lookup"><span data-stu-id="94c55-104">Payment methods define the way you prefer for customers to pay you, and how you like to pay your vendors.</span></span> <span data-ttu-id="94c55-105">Метод может меняться для каждого клиента или поставщика.</span><span class="sxs-lookup"><span data-stu-id="94c55-105">The method can vary for each customer or vendor.</span></span> <span data-ttu-id="94c55-106">Типичными примерами методов оплаты являются **банк**, **касса**, **чек** или **счет**.</span><span class="sxs-lookup"><span data-stu-id="94c55-106">Examples of typical payment methods are **bank**, **cash**, **check**, or **account**.</span></span>

<span data-ttu-id="94c55-107">Можно назначить метод оплаты клиентам и поставщикам, чтобы один и тот же метод всегда использовался в документах продаж и покупки, создаваемых для них.</span><span class="sxs-lookup"><span data-stu-id="94c55-107">You can assign a payment method to customers and vendors so that the same method is always used on the sales and purchase documents you create for them.</span></span> <span data-ttu-id="94c55-108">При необходимости можно изменить метод в документе продажи или покупки.</span><span class="sxs-lookup"><span data-stu-id="94c55-108">If needed, you can change the method on the sales or purchase document.</span></span> <span data-ttu-id="94c55-109">Например, если требуется оплатить конкретный счет на покупку наличными, а не чеком.</span><span class="sxs-lookup"><span data-stu-id="94c55-109">For example, if you want to pay a particular purchase invoice in cash rather than by check.</span></span> <span data-ttu-id="94c55-110">Это не изменяет метод оплаты по умолчанию, назначенный поставщику.</span><span class="sxs-lookup"><span data-stu-id="94c55-110">This does not change the default payment method assigned to the vendor.</span></span>

<span data-ttu-id="94c55-111">Эти же способы платежа используются для документов покупки и продажи.</span><span class="sxs-lookup"><span data-stu-id="94c55-111">The same payment methods are used for sales and purchase documents.</span></span> <span data-ttu-id="94c55-112">Например, способ платежа _касса_ используется как при осуществлении платежей, так и при получении платежей.</span><span class="sxs-lookup"><span data-stu-id="94c55-112">For example, a _cash_ payment method is used both when you make payments and when you receive them.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="94c55-113">знает, что при создании счета продажи ожидается получение платежа, и оплата наоброт для счетов покупки.</span><span class="sxs-lookup"><span data-stu-id="94c55-113">knows that when you are creating a sales invoice you expect to receive payment, and the opposite for purchase invoices.</span></span>

<span data-ttu-id="94c55-114">Кредит-ноты для возвратов, однако, являются исключениями, поскольку денежные средства передаются в противоположных направлениях, от вас клиенты и от вашего поставщика вам.</span><span class="sxs-lookup"><span data-stu-id="94c55-114">Credit memos for returns, however, are exceptions because money is flowing in the opposite directions, from you to your customer and from your vendor to you.</span></span> <span data-ttu-id="94c55-115">Поэтому способ платежа по умолчанию не назначается кредит-нотам.</span><span class="sxs-lookup"><span data-stu-id="94c55-115">Therefore, a default payment method is not assigned to credit memos.</span></span> <span data-ttu-id="94c55-116">Имеется, однако, обходной способ, если вы указали условия платежа для клиента или поставщика.</span><span class="sxs-lookup"><span data-stu-id="94c55-116">There is, however, a workaround if you have specified terms of payment for the customer or vendor.</span></span> <span data-ttu-id="94c55-117">Хотя поле **Расчет скидки оплаты по кредит-нотам** не предназначено для этого, если установить флажок **Условия платежа**, метод оплаты по умолчанию будет добавлен при создании кредит-ноты.</span><span class="sxs-lookup"><span data-stu-id="94c55-117">Though the **Calc. Pmt. Disc. on Cr. Memos** field is not intended for this, if you choose the check box on the **Payment Terms** page a default payment method will be added when you create a credit memo.</span></span> <br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE476Ys]

## <a name="to-set-up-a-payment-method"></a><span data-ttu-id="94c55-118">Настройка метода оплаты</span><span class="sxs-lookup"><span data-stu-id="94c55-118">To set up a payment method</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="94c55-119">обеспечивает несколько способов платежа, которые часто используются организациями.</span><span class="sxs-lookup"><span data-stu-id="94c55-119">provides a few payment methods that businesses often use.</span></span> <span data-ttu-id="94c55-120">Можно, однако, добавить любое необходимое число.</span><span class="sxs-lookup"><span data-stu-id="94c55-120">You can, however, add as many as you need.</span></span>

1. <span data-ttu-id="94c55-121">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Методы оплаты**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="94c55-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Methods**, and then choose the related link.</span></span>
2. <span data-ttu-id="94c55-122">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="94c55-122">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-assign-a-payment-method-to-a-customer-or-vendor"></a><span data-ttu-id="94c55-123">Присвоение метода платежа клиенту или поставщику</span><span class="sxs-lookup"><span data-stu-id="94c55-123">To assign a payment method to a customer or vendor</span></span>
1. <span data-ttu-id="94c55-124">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиент** или **Поставщик**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="94c55-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer** or **Vendor**, and then choose the related link.</span></span>
2. <span data-ttu-id="94c55-125">В поле **Код способа оплаты** выберите метод, который будет использоваться по умолчанию для клиента или поставщика.</span><span class="sxs-lookup"><span data-stu-id="94c55-125">In the **Payment Method Code** field, choose the method to use by default for the customer or vendor.</span></span>

## <a name="see-also"></a><span data-ttu-id="94c55-126">См. также</span><span class="sxs-lookup"><span data-stu-id="94c55-126">See Also</span></span>
[<span data-ttu-id="94c55-127">Регистрация новых клиентов</span><span class="sxs-lookup"><span data-stu-id="94c55-127">Register New Customers</span></span>](sales-how-register-new-customers.md)  
[<span data-ttu-id="94c55-128">Финансы</span><span class="sxs-lookup"><span data-stu-id="94c55-128">Finance</span></span>](finance.md)  
<span data-ttu-id="94c55-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="94c55-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
