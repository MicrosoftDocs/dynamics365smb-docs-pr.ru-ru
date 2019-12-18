---
title: Изменение или отмена неоплаченных счетов покупки | Документация Майкрософт
description: Описывается, как исправлять и отменять учтенные счета покупки и автоматически создавать кредит-ноты покупки.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: undo, credit memo, return
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 81b2ab1956e1468bfcce2f438edbed934f4de703
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2883122"
---
# <a name="correct-or-cancel-unpaid-purchase-invoices"></a><span data-ttu-id="8dd1a-103">Исправление или отмена неоплаченных счетов покупки</span><span class="sxs-lookup"><span data-stu-id="8dd1a-103">Correct or Cancel Unpaid Purchase Invoices</span></span>
<span data-ttu-id="8dd1a-104">Можно исправить или отменить учтенный счет покупки.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-104">You can correct or cancel a posted purchase invoice.</span></span> <span data-ttu-id="8dd1a-105">Это используется, если нужно исправить опечатку либо внести изменение в покупку на раннем этапе обработки заказа.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-105">This is useful if you want to correct a typing mistake, or if you want to change the purchase early in the order process.</span></span>

<span data-ttu-id="8dd1a-106">Если продукты в учтенном счете покупки уже оплачены, его невозможно откорректировать или отменить из учтенного счета покупки.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-106">If you have already paid for products on the posted purchase invoice, you cannot correct or cancel it from the posted purchase invoice itself.</span></span> <span data-ttu-id="8dd1a-107">Вместо этого необходимо вручную создать кредит-ноту покупки для сторнирования покупки, при необходимости управляемую заказом на возврат покупки.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-107">Instead, you must manually create a purchase credit memo to reverse the purchase, optionally managed with a purchase return order.</span></span> <span data-ttu-id="8dd1a-108">Дополнительные сведения см. в разделе [Обработка возвратов покупки или отмен](purchasing-how-process-purchase-returns-cancellations.md)</span><span class="sxs-lookup"><span data-stu-id="8dd1a-108">For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).</span></span>

<span data-ttu-id="8dd1a-109">На странице **Учтенный счет покупки** можно нажать кнопку **Исправить** или **Отмена**.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-109">On the **Posted Purchase Invoice** page, you can choose the **Correct** button or the **Cancel** button.</span></span> <span data-ttu-id="8dd1a-110">При корректировке или отмене учтенного счета покупки корректирующая кредит-нота покупки применяется ко всем операциям ГК и журнала товаров, созданным при учете первоначального счета покупки.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-110">When you correct or cancel a posted purchase invoice, the corrective purchase credit memo is applied to all general ledger and inventory ledger entries that were created when the initial purchase invoice was posted.</span></span> <span data-ttu-id="8dd1a-111">При этом сторнируется учтенный счет покупки в финансовых записях и оставляется корректирующая учтенная кредит-нота покупки для аудиторского следа.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-111">This reverses the posted purchase invoice in your financial records and leaves the corrective posted purchase credit memo for your audit trail.</span></span> <span data-ttu-id="8dd1a-112">Ниже описано использование кнопок **Исправить** и **Отмена**.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-112">In the following the use of **Correct** and **Cancel** is described.</span></span>
<br><br>
> [!Video https://www.microsoft.com/videoplayer/embed/RE4dhoc]

## <a name="to-correct-a-posted-purchase-invoice"></a><span data-ttu-id="8dd1a-113">Коррекция учтенного счета покупки</span><span class="sxs-lookup"><span data-stu-id="8dd1a-113">To correct a posted purchase invoice</span></span>
1. <span data-ttu-id="8dd1a-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенные счета покупки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8dd1a-115">Выберите учтенный счет покупки, который требуется откорректировать.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-115">Select the posted purchase invoice that you want to correct.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="8dd1a-116">Если установлен флажок **Отменено**, невозможно откорректировать учтенный счет покупки, поскольку он уже откорректирован или отменен.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-116">If the **Canceled** check box is selected, then you cannot correct the posted purchase invoice because it has already been corrected or canceled.</span></span>
3. <span data-ttu-id="8dd1a-117">На странице **Учтенный счет покупки** выберите **Исправить**.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-117">On the **Posted Purchase Invoice** page, choose **Correct**.</span></span>

    <span data-ttu-id="8dd1a-118">Создается новый счет покупки с теми же сведениями, в который можно внести изменения.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-118">A new purchase invoice with the same information is created where you can make the correction.</span></span> <span data-ttu-id="8dd1a-119">Дополнительные сведения см. в разделе [Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="8dd1a-119">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span> <span data-ttu-id="8dd1a-120">Значение в поле **Отменено** в исходном учтенном счете покупки изменится на **Да**.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-120">The **Canceled** field on the initial posted purchase invoice is changed to **Yes**.</span></span>

    <span data-ttu-id="8dd1a-121">Автоматически создается кредит-нота покупки, которая учитывается для аннулирования исходного учтенного счета покупки.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-121">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span></span>
4. <span data-ttu-id="8dd1a-122">Выберите **Показать корректирующую кредит-ноту**, чтобы просмотреть учтенную кредит-ноту покупки, которая аннулирует исходный учтенный счет покупки.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-122">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span></span>

## <a name="to-cancel-a-posted-purchase-invoice"></a><span data-ttu-id="8dd1a-123">Отмена учтенного счета покупки</span><span class="sxs-lookup"><span data-stu-id="8dd1a-123">To cancel a posted purchase invoice</span></span>
1. <span data-ttu-id="8dd1a-124">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенные счета покупки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8dd1a-125">Выберите учтенный счет покупки, который требуется отменить.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-125">Select the posted purchase invoice that you want to cancel.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="8dd1a-126">Если установлен флажок **Отменено**, невозможно отменить учтенный счет покупки, поскольку он уже отмене или скорректирован.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-126">If the **Canceled** check box is selected, then you cannot cancel the posted purchase invoice because it has already been canceled or corrected.</span></span>
3. <span data-ttu-id="8dd1a-127">На странице **Учтенный счет покупки** выберите **Отмена**.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-127">On the **Posted Purchase Invoice** page, choose **Cancel**.</span></span>

    <span data-ttu-id="8dd1a-128">Автоматически создается кредит-нота покупки, которая учитывается для аннулирования исходного учтенного счета покупки.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-128">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span></span> <span data-ttu-id="8dd1a-129">Значение в поле **Отменено** в исходном учтенном счете покупки изменится на **Да**.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-129">The **Canceled** field on the initial posted purchase invoice is changed to **Yes**.</span></span>
4. <span data-ttu-id="8dd1a-130">Выберите **Показать корректирующую кредит-ноту**, чтобы просмотреть учтенную кредит-ноту покупки, которая аннулирует исходный учтенный счет покупки.</span><span class="sxs-lookup"><span data-stu-id="8dd1a-130">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span></span>

## <a name="see-also"></a><span data-ttu-id="8dd1a-131">См. также</span><span class="sxs-lookup"><span data-stu-id="8dd1a-131">See Also</span></span>
[<span data-ttu-id="8dd1a-132">Покупки</span><span class="sxs-lookup"><span data-stu-id="8dd1a-132">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="8dd1a-133">Регистрация покупок</span><span class="sxs-lookup"><span data-stu-id="8dd1a-133">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
<span data-ttu-id="8dd1a-134">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8dd1a-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
