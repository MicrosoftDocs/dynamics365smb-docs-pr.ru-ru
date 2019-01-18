---
title: "Использование пакетного задания \"Предлож. оплаты поставщикам\" | Документы Майкрософт"
description: "Вы можете задать настройки оплаты поставщикам для получения предложений по оплатам, которые быть произведены в ближайшее время или по которым доступны скидки."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: vendor payment, creditor, debt, balance due, AP
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 5e13b28e2cf75f061246dab56a9f4b3d4a16e1ce
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="suggest-vendor-payments"></a><span data-ttu-id="1dfd6-103">Предлож. оплаты поставщикам</span><span class="sxs-lookup"><span data-stu-id="1dfd6-103">Suggest Vendor Payments</span></span>
<span data-ttu-id="1dfd6-104">На странице **Журнал платежей** можно использовать пакетное задание **Предлож. оплаты поставщикам** для предложения строк платежей.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-104">On the **Payment Journal** page, you can use the **Suggest Vendor Payments** batch job to suggest payment lines.</span></span> <span data-ttu-id="1dfd6-105">Строки для платежей, для которых скоро наступает крайний срок, или платежей, для которых доступна скидка, предлагаются на основании ваших настроек.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-105">Lines for payments that are due soon or payments where a payment discount is available are suggested based on your settings.</span></span>

<span data-ttu-id="1dfd6-106">Чтобы максимально эффективно использовать предложения по оплате, необходимо сначала назначить приоритеты поставщикам.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-106">To benefit fully from payment suggestions, you must first prioritize your vendors.</span></span> <span data-ttu-id="1dfd6-107">Дополнительные сведения см. в разделе [Назначение приоритетов поставщикам](purchasing-how-prioritize-vendors.md).</span><span class="sxs-lookup"><span data-stu-id="1dfd6-107">For more information, see [Prioritize Vendors](purchasing-how-prioritize-vendors.md).</span></span>  

> [!NOTE]  
> <span data-ttu-id="1dfd6-108">Операции в книге поставщиков, для которых установлена отметка **На удержании**, в пакетное задание не включается.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-108">Vendor ledger entries that are **On Hold** are not included in the batch job.</span></span>  

> [!IMPORTANT]  
>   <span data-ttu-id="1dfd6-109">Если вы хотите воспользоваться скидками оплаты и ввели доступную сумму, сумма будет использоваться для:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-109">If you want to take advantage of payment discounts, and have entered an available amount, the amount will be used for:</span></span>  
    * <span data-ttu-id="1dfd6-110">Сначала по просроченным операциям поставщиков с назначенными приоритетами.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-110">Prioritized overdue vendor entries first in order of priority.</span></span>   
    * <span data-ttu-id="1dfd6-111">По просроченным операциям поставщиков, которым не назначены приоритеты.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-111">Overdue vendor entries that are not prioritized.</span></span>  
    * <span data-ttu-id="1dfd6-112">Для открытых операций поставщиков, которые квалифицируются по скидкам оплаты в порядке номеров поставщиков.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-112">Open vendor entries that qualify for payment discounts, arranged by vendor number.</span></span>  

## <a name="to-use-the-suggest-vendor-payments-function"></a><span data-ttu-id="1dfd6-113">Использование функции предложения оплаты поставщикам</span><span class="sxs-lookup"><span data-stu-id="1dfd6-113">To use the Suggest Vendor Payments function</span></span>
1. <span data-ttu-id="1dfd6-114">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы платежей**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1dfd6-115">Откройте соответствующий журнал, а затем выберите действие **Предлож. оплаты поставщикам**.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-115">Open the relevant journal, and then choose the **Suggest Vendor Payments** action.</span></span>  
3. <span data-ttu-id="1dfd6-116">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-116">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. <span data-ttu-id="1dfd6-117">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-117">Choose the **OK** button.</span></span>  

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a><span data-ttu-id="1dfd6-118">Вставка срока оплаты в качестве даты учета в строках журнала платежей</span><span class="sxs-lookup"><span data-stu-id="1dfd6-118">To insert the due date as posting date on payment journal lines</span></span>
<span data-ttu-id="1dfd6-119">При использовании пакетного задания **Предлож. оплаты поставщикам** для создания строк платежей для поставщиков можно также заполнить два специальных поля, чтобы убедиться, что в созданных строках используется дата оплаты для вычисления даты учета.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-119">When you use the **Suggest Vendor Payments** batch job to create payment lines for your vendors, you can fill two special fields to make sure that the generated lines use the due date to calculate the posting date.</span></span> <span data-ttu-id="1dfd6-120">Это поля **Рассчитать дату учета на основе срока оплаты примен. документа** и **Примен. смещения срока оплаты документа**.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-120">These fields are **Calculate Posting Date from Applies-to-Doc Due Date** and **Applies-to-Doc Due Date Offset**.</span></span>  

> [!IMPORTANT]  
>   <span data-ttu-id="1dfd6-121">Невозможно использовать поле **Рассчитать дату учета на основе срока оплаты примен. документа** вместе с полем **Найти скидки оплаты** или **Суммировать по поставщикам**.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-121">You cannot use the **Calculate Posting Date from Applies-to-Doc Due Date** field together with the **Find Payment Discounts** field or the **Summarize per Vendor** field.</span></span> <span data-ttu-id="1dfd6-122">Если дата учета основана на дате оплаты, некоторые скидки по оплате могут вычисляться неверно, поскольку дата учета следует после даты скидки по оплате.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-122">If the posting date is based on the due date, some payment discounts may not calculate correctly because the posting date is after the payment discount date.</span></span>  

<span data-ttu-id="1dfd6-123">Кроме того, если расчетная дата учета уже прошла, дата учета будет изменена на рабочую дату и отобразится предупреждение.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-123">Also, if the calculated posting date is in the past, then the posting date is moved up to the work date, and a warning is displayed.</span></span>  

<span data-ttu-id="1dfd6-124">Либо можно вручную создать строки платежа с использованием срока оплаты для вычисления даты учета.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-124">Alternatively, you can manually create payment lines using the due date to calculate the posting date.</span></span> <span data-ttu-id="1dfd6-125">После применения операций книги поставщиков можно использовать действие **Расчет даты учета** для обновления даты учета в строку журнала сроком оплаты связанного счета покупки.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-125">After you apply vendor ledger entries, you can use the **Calculate Posting Date** action to update the posting date on the journal line with the due date of the related purchase invoice.</span></span> <span data-ttu-id="1dfd6-126">Дополнительные сведения см. в разделе [Применение транзакций платежей вручную](payables-how-apply-purchase-transactions-manually.md).</span><span class="sxs-lookup"><span data-stu-id="1dfd6-126">For more information, see [Apply Purchase Transactions Manually](payables-how-apply-purchase-transactions-manually.md).</span></span>  

> [!NOTE]  
>   <span data-ttu-id="1dfd6-127">Если счет покупки просрочен, в качестве даты учета устанавливается рабочая дата и цвет шрифта в строке меняется на красный.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-127">If the purchase invoice is overdue, the posting date is set to the work date, and the font on the line becomes red.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1dfd6-128">См. также</span><span class="sxs-lookup"><span data-stu-id="1dfd6-128">See Also</span></span>
[<span data-ttu-id="1dfd6-129">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="1dfd6-129">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="1dfd6-130">Осуществление платежей</span><span class="sxs-lookup"><span data-stu-id="1dfd6-130">Making Payments</span></span>](payables-make-payments.md)  
[<span data-ttu-id="1dfd6-131">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="1dfd6-131">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="1dfd6-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

