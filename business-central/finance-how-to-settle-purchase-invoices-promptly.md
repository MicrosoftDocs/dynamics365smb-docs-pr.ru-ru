---
title: Немедленное создание счетов покупки
description: В случае потребности в оплате поставщику наличными или чеком, необходимый учет можно производить при учете самого счета.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/06/2020
ms.author: bholtorf
ms.openlocfilehash: fb442c7b1e9e7bdcb727ca6de157657e370e254f
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4746845"
---
# <a name="settle-purchase-invoices-promptly"></a><span data-ttu-id="7c826-103">Немедленное создание счетов покупки</span><span class="sxs-lookup"><span data-stu-id="7c826-103">Settle Purchase Invoices Promptly</span></span>

<span data-ttu-id="7c826-104">В случае потребности в оплате поставщику наличными или чеком, платеж можно учесть при учете счета.</span><span class="sxs-lookup"><span data-stu-id="7c826-104">If you need to pay the vendor by cash or check, you can post the payment when you post the invoice.</span></span>  

> [!NOTE]  
> <span data-ttu-id="7c826-105">Если оплата счетов наличными, чеком или банковским переводом производится часто, то можно рекомендовать установить специальный метод оплаты с использованием балансирующего счета и ввода этого метода в поле **Способ платежа** на карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="7c826-105">If you frequently pay purchase invoices in cash, check, or bank transfer, it is a good idea to set up a specific payment method with a balancing account and enter this method in the **Payment Method** field on the vendor card.</span></span> <span data-ttu-id="7c826-106">Номер балансирующего счета вставляется автоматически в заголовок счета при создании нового счета.</span><span class="sxs-lookup"><span data-stu-id="7c826-106">The balancing account number is inserted automatically on the invoice header every time you create a new invoice.</span></span> <span data-ttu-id="7c826-107">Дополнительные сведения см. в разделе [Определение способов оплаты](finance-payment-methods.md).</span><span class="sxs-lookup"><span data-stu-id="7c826-107">For more information, see [Defining Payment Methods](finance-payment-methods.md).</span></span>  

## <a name="to-settle-purchase-invoices-promptly"></a><span data-ttu-id="7c826-108">Немедленное создание счетов покупки</span><span class="sxs-lookup"><span data-stu-id="7c826-108">To settle purchase invoices promptly</span></span>

1. <span data-ttu-id="7c826-109">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета покупки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7c826-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="7c826-110">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="7c826-110">Choose the **New** action.</span></span>  
3. <span data-ttu-id="7c826-111">Для того чтобы произвести оплату наличными или с помощью банковского трансферта, следует ввести номер счета ГК или банковского счета в поле **Номер баланс. счета**.</span><span class="sxs-lookup"><span data-stu-id="7c826-111">To pay either in cash or by bank transfer, enter the number of the general ledger cash account or the bank account in the **Bal. Account No.** field.</span></span>  

> [!IMPORTANT]  
> <span data-ttu-id="7c826-112">Поля **Тип баланс. счета** и **Номер баланс. счета** не включены в стандартную схему заголовка счета.</span><span class="sxs-lookup"><span data-stu-id="7c826-112">The **Bal. Account Type** and **Bal. Account No.** fields are not included in the standard layout of the invoice header.</span></span> <span data-ttu-id="7c826-113">Чтобы разнести оплату счета, вы должны связаться с партнером Microsoft, который может добавить поля с помощью кода.</span><span class="sxs-lookup"><span data-stu-id="7c826-113">In order to post the payment of an invoice, you must contact a Microsoft partner who can add the fields through code.</span></span>  
>
> <span data-ttu-id="7c826-114">Эта настройка требуется только в том случае, если вы не укажете балансирующие счета в способах оплаты, как описано выше.</span><span class="sxs-lookup"><span data-stu-id="7c826-114">This customization is only required if you do not specify balancing accounts on the payment methods as describe above.</span></span>

## <a name="see-also"></a><span data-ttu-id="7c826-115">См. также</span><span class="sxs-lookup"><span data-stu-id="7c826-115">See Also</span></span>

[<span data-ttu-id="7c826-116">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="7c826-116">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="7c826-117">Покупки</span><span class="sxs-lookup"><span data-stu-id="7c826-117">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="7c826-118">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7c826-118">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
