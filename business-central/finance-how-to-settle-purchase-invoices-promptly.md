---
title: Немедленное создание счетов покупки
description: В случае потребности в оплате поставщику наличными или чеком, необходимый учет можно производить при учете самого счета.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/06/2020
ms.author: bholtorf
ms.openlocfilehash: bac023393d95623a2731ef1b2ada7d30b135063b
ms.sourcegitcommit: 0fb6952376d853a878ed33257e73aadc03b95572
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "3968363"
---
# <a name="settle-purchase-invoices-promptly"></a><span data-ttu-id="7917a-103">Немедленное создание счетов покупки</span><span class="sxs-lookup"><span data-stu-id="7917a-103">Settle Purchase Invoices Promptly</span></span>

<span data-ttu-id="7917a-104">В случае потребности в оплате поставщику наличными или чеком, платеж можно учесть при учете счета.</span><span class="sxs-lookup"><span data-stu-id="7917a-104">If you need to pay the vendor by cash or check, you can post the payment when you post the invoice.</span></span>  

> [!NOTE]  
> <span data-ttu-id="7917a-105">Если оплата счетов наличными, чеком или банковским переводом производится часто, то можно рекомендовать установить специальный метод оплаты с использованием балансирующего счета и ввода этого метода в поле **Способ платежа** на карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="7917a-105">If you frequently pay purchase invoices in cash, check, or bank transfer, it is a good idea to set up a specific payment method with a balancing account and enter this method in the **Payment Method** field on the vendor card.</span></span> <span data-ttu-id="7917a-106">Номер балансирующего счета вставляется автоматически в заголовок счета при создании нового счета.</span><span class="sxs-lookup"><span data-stu-id="7917a-106">The balancing account number is inserted automatically on the invoice header every time you create a new invoice.</span></span> <span data-ttu-id="7917a-107">Дополнительные сведения см. в разделе [Определение способов оплаты](finance-payment-methods.md).</span><span class="sxs-lookup"><span data-stu-id="7917a-107">For more information, see [Defining Payment Methods](finance-payment-methods.md).</span></span>  

## <a name="to-settle-purchase-invoices-promptly"></a><span data-ttu-id="7917a-108">Немедленное создание счетов покупки</span><span class="sxs-lookup"><span data-stu-id="7917a-108">To settle purchase invoices promptly</span></span>

1. <span data-ttu-id="7917a-109">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета покупки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7917a-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="7917a-110">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="7917a-110">Choose the **New** action.</span></span>  
3. <span data-ttu-id="7917a-111">Для того чтобы произвести оплату наличными или с помощью банковского трансферта, следует ввести номер счета ГК или банковского счета в поле **Номер баланс. счета**.</span><span class="sxs-lookup"><span data-stu-id="7917a-111">To pay either in cash or by bank transfer, enter the number of the general ledger cash account or the bank account in the **Bal. Account No.** field.</span></span>  

> [!IMPORTANT]  
> <span data-ttu-id="7917a-112">Поля **Тип баланс. счета** и **Номер баланс. счета** не включены в стандартную схему заголовка счета.</span><span class="sxs-lookup"><span data-stu-id="7917a-112">The **Bal. Account Type** and **Bal. Account No.** fields are not included in the standard layout of the invoice header.</span></span> <span data-ttu-id="7917a-113">Чтобы разнести оплату счета, вы должны связаться с партнером Microsoft, который может добавить поля с помощью кода.</span><span class="sxs-lookup"><span data-stu-id="7917a-113">In order to post the payment of an invoice, you must contact a Microsoft partner who can add the fields through code.</span></span>  
>
> <span data-ttu-id="7917a-114">Эта настройка требуется только в том случае, если вы не укажете балансирующие счета в способах оплаты, как описано выше.</span><span class="sxs-lookup"><span data-stu-id="7917a-114">This customization is only required if you do not specify balancing accounts on the payment methods as describe above.</span></span>

## <a name="see-also"></a><span data-ttu-id="7917a-115">См. также</span><span class="sxs-lookup"><span data-stu-id="7917a-115">See Also</span></span>

[<span data-ttu-id="7917a-116">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="7917a-116">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="7917a-117">Покупки</span><span class="sxs-lookup"><span data-stu-id="7917a-117">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="7917a-118">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7917a-118">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
