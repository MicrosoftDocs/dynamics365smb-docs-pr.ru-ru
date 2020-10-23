---
title: Как корректировать предоплаты | Документация Майкрософт
description: Можно скорректировать заказ после учета счета на предоплату по данному заказу. Можно добавить новые строки в заказ после выставления счета на предоплату, после чего можно учесть другой счет на предоплату, но невозможно удалить строку из заказа после того, как по этой строке был выставлен счет на предоплату.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 3dd124807d3d6ce3a775d18dcd88a8251b0feb30
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3924182"
---
# <a name="correct-prepayments"></a><span data-ttu-id="95472-104">Корректировка предоплат</span><span class="sxs-lookup"><span data-stu-id="95472-104">Correct Prepayments</span></span>

<span data-ttu-id="95472-105">Можно скорректировать заказ после учета счета на предоплату по данному заказу.</span><span class="sxs-lookup"><span data-stu-id="95472-105">You can make a correction to an order after you have posted a prepayment invoice for the order.</span></span> <span data-ttu-id="95472-106">Можно добавить новые строки в заказ после выставления счета на предоплату, после чего можно учесть другой счет на предоплату, но невозможно удалить строку из заказа после того, как по этой строке был выставлен счет на предоплату.</span><span class="sxs-lookup"><span data-stu-id="95472-106">You can add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice, but you cannot delete a line from an order after a prepayment has been invoiced for the line.</span></span>  

> [!TIP]
> <span data-ttu-id="95472-107">Если вы учли счет на предоплату для счета продажи, который затем корректируете или отменяете, вы также должны исправить или отменить предоплату.</span><span class="sxs-lookup"><span data-stu-id="95472-107">If you have posted a prepayment invoice for a sales invoice that you then correct or cancel, you must correct or cancel the prepayment as well.</span></span>

## <a name="to-correct-a-prepayment"></a><span data-ttu-id="95472-108">Корректировка предоплаты</span><span class="sxs-lookup"><span data-stu-id="95472-108">To correct a prepayment</span></span>

<span data-ttu-id="95472-109">Приведенная ниже процедура показывает, как создать кредит-ноту предоплаты, чтобы отменить все предоплаты, по которым выставлены счета, для заказа на продажу.</span><span class="sxs-lookup"><span data-stu-id="95472-109">The following procedure shows how to issue a prepayment credit memo to cancel all invoiced prepayments for a sales order.</span></span>  

1. <span data-ttu-id="95472-110">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="95472-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="95472-111">Откройте соответствующий заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="95472-111">Open the relevant sales order.</span></span>
3. <span data-ttu-id="95472-112">Выберите действие **Предоплата**, затем выберите **Учет кредит-ноты на предоплату** или **Учет и печать кредит-ноты на предоплату**.</span><span class="sxs-lookup"><span data-stu-id="95472-112">Choose the **Prepayment** action, and then choose the **Post Prepayment Credit Memo** action or the **Post and Print Prepmt. Cr. Memo** action.</span></span>  
4. <span data-ttu-id="95472-113">На странице **Кредит-нота продажи** исправьте соответствующие операции, как и для любой кредит-ноты продажи.</span><span class="sxs-lookup"><span data-stu-id="95472-113">On the **Sales Credit Memo** page, proceed to correct the relevant entries, as for any sales credit memo.</span></span> <span data-ttu-id="95472-114">Дополнительные сведения см. в разделе [Обработка возвратов продажи или отмен](sales-how-process-sales-returns-cancellations.md)</span><span class="sxs-lookup"><span data-stu-id="95472-114">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span></span>  

    > [!NOTE]  
    > <span data-ttu-id="95472-115">Чтобы уменьшить сумму в поле **Сумма строки**, сначала необходимо увеличить процент предоплаты в данной строке, чтобы значение в поле **Сумма в строке предоплаты** не становилась меньше значения в поле **Сумм. предопл. для выст. счета**.</span><span class="sxs-lookup"><span data-stu-id="95472-115">To reduce the amount in the **Line Amount** field, you must first increase the prepayment percentage on the line so that the value in the **Prepmt. Line Amount** field is not decreased below the value in the **Prepmt. Amt. Inv.** field.</span></span>

5. <span data-ttu-id="95472-116">Чтобы создать счет на предоплату для любых новых строк в кредит-ноте продажи, выберите действие **Предоплата**, затем выберите действие **Учет счета на предоплату** или **Учет и печать счета на предоплату**.</span><span class="sxs-lookup"><span data-stu-id="95472-116">To make a prepayment invoice for any new lines in the sales credit memo, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action or the **Post and Print Prepmt. Invoice** action.</span></span>  
6. <span data-ttu-id="95472-117">Чтобы создать дополнительный счет на предоплату, увеличьте сумму предоплаты в одной или нескольких строках и выполните учет счета на предоплату.</span><span class="sxs-lookup"><span data-stu-id="95472-117">To issue an additional prepayment invoice, increase the prepayment amount on one or more lines and post the prepayment invoice.</span></span> <span data-ttu-id="95472-118">Новый счет будет создан на сумму разницы между суммами предоплаты, уже включенными в счет, и новыми суммами предоплаты.</span><span class="sxs-lookup"><span data-stu-id="95472-118">A new invoice will be created for the difference between the prepayment amounts invoiced and the new prepayment amounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="95472-119">См. также</span><span class="sxs-lookup"><span data-stu-id="95472-119">See Also</span></span>

[<span data-ttu-id="95472-120">Выставление счетов на предоплату</span><span class="sxs-lookup"><span data-stu-id="95472-120">Invoicing Prepayments</span></span>](finance-invoice-prepayments.md)  
[<span data-ttu-id="95472-121">Пошаговое руководство. Настройка и выставление счетов на продажу</span><span class="sxs-lookup"><span data-stu-id="95472-121">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[<span data-ttu-id="95472-122">Финансы</span><span class="sxs-lookup"><span data-stu-id="95472-122">Finance</span></span>](finance.md)  
<span data-ttu-id="95472-123">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="95472-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
