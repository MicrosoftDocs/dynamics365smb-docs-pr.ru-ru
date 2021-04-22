---
title: Блокировка товаров для продажи или покупки
description: Вы можете запретить использование элемента, например, в документах продажи или покупки.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 4bc130d6982d969084f7fcbf3618893978317f36
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5786052"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="4f096-103">Блокировка товаров для продажи или покупки</span><span class="sxs-lookup"><span data-stu-id="4f096-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="4f096-104">Можно заблокировать товар для ввода в строки документов продажи или покупки либо учета в любой транзакции.</span><span class="sxs-lookup"><span data-stu-id="4f096-104">You can block an item from being entered on lines in sales or purchase documents, and you can block it from being posted in any transaction.</span></span> <span data-ttu-id="4f096-105">Например, это удобно, если товар имеет известный дефект.</span><span class="sxs-lookup"><span data-stu-id="4f096-105">For example, this is useful when an item has a known defect.</span></span> <span data-ttu-id="4f096-106">Если кто-то выберет заблокированный товар в документе продажи или покупки, он получит сообщение о том, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="4f096-106">If someone chooses a blocked item on a sales or purchase document a message will inform them that the item is blocked.</span></span>

<span data-ttu-id="4f096-107">В следующей таблице показано, что происходит при блокировке товаров.</span><span class="sxs-lookup"><span data-stu-id="4f096-107">The following table describes what occurs when items are blocked.</span></span>  

|<span data-ttu-id="4f096-108">Параметр</span><span class="sxs-lookup"><span data-stu-id="4f096-108">Option</span></span>|<span data-ttu-id="4f096-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4f096-109">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="4f096-110">**Продажи заблокированы**</span><span class="sxs-lookup"><span data-stu-id="4f096-110">**Sales Blocked**</span></span>|<span data-ttu-id="4f096-111">Невозможно ввести товар в документ продажи или в журнал товаров продажи.</span><span class="sxs-lookup"><span data-stu-id="4f096-111">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="4f096-112">**Покупки заблокированы**</span><span class="sxs-lookup"><span data-stu-id="4f096-112">**Purchasing Blocked**</span></span>|<span data-ttu-id="4f096-113">Невозможно ввести товар в документ покупки, в журнал товаров покупки или в процессы планирования покупки.</span><span class="sxs-lookup"><span data-stu-id="4f096-113">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="4f096-114">**Заблокировано**</span><span class="sxs-lookup"><span data-stu-id="4f096-114">**Blocked**</span></span>|<span data-ttu-id="4f096-115">Невозможно использовать товар для товарной транзакции.</span><span class="sxs-lookup"><span data-stu-id="4f096-115">You cannot use the item for any item transaction.</span></span>|  

> [!NOTE]
> <span data-ttu-id="4f096-116">Заблокированные товары могут быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="4f096-116">Blocked items can be returned.</span></span> <span data-ttu-id="4f096-117">Это означает, что ни одна из вышеприведенных настроек не применяется, если товар используется в возвратах и кредит-нотах.</span><span class="sxs-lookup"><span data-stu-id="4f096-117">This means that none of the above settings apply when the item is used on return orders and credit memos.</span></span>

<span data-ttu-id="4f096-118">Когда вы используете функцию **Копировать из документа** для создания новых документов на основе существующих документов, вы получаете уведомление, если какие-либо элементы в строках исходного документа заблокированы.</span><span class="sxs-lookup"><span data-stu-id="4f096-118">When you use the **Copy from Document** function to create new documents based on existing documents, you are notified if any items on the source document lines are blocked.</span></span> <span data-ttu-id="4f096-119">Заблокированные строки документа исключаются из нового документа, а уведомление показывает обзор всех строк документа, которые заблокированы в исходном документе.</span><span class="sxs-lookup"><span data-stu-id="4f096-119">The blocked document lines are excluded from the new document, and a notification shows an overview of all document lines that are blocked in the source document.</span></span>

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="4f096-120">Блокировка ввода товара в строки продажи</span><span class="sxs-lookup"><span data-stu-id="4f096-120">To block an item from being entered on sales lines</span></span>  
1.  <span data-ttu-id="4f096-121">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="4f096-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4f096-122">Выберите товар, который необходимо заблокировать, а затем установите флажок **Продажи заблокированы**.</span><span class="sxs-lookup"><span data-stu-id="4f096-122">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="4f096-123">Блокировка ввода товара в строки покупки</span><span class="sxs-lookup"><span data-stu-id="4f096-123">To block an item from being entered on purchase lines</span></span>  
1.  <span data-ttu-id="4f096-124">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="4f096-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4f096-125">Выберите товар, который необходимо заблокировать, а затем установите флажок **Покупки заблокированы**.</span><span class="sxs-lookup"><span data-stu-id="4f096-125">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="4f096-126">Блокировка товара для учета</span><span class="sxs-lookup"><span data-stu-id="4f096-126">To block an item from being posted</span></span>
1. <span data-ttu-id="4f096-127">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="4f096-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="4f096-128">Выберите товар, который необходимо заблокировать, а затем установите флажок **Заблокировано**.</span><span class="sxs-lookup"><span data-stu-id="4f096-128">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

## <a name="see-also"></a><span data-ttu-id="4f096-129">См. также</span><span class="sxs-lookup"><span data-stu-id="4f096-129">See Also</span></span>  
[<span data-ttu-id="4f096-130">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="4f096-130">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="4f096-131">Запасы</span><span class="sxs-lookup"><span data-stu-id="4f096-131">Inventory</span></span>](inventory-manage-inventory.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]