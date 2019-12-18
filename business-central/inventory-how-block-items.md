---
title: Блокировка товаров для продажи или покупки
description: В Business Central товар можно пометить как заблокированный для продажи, покупки или всех целей.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 12/04/2019
ms.author: sgroespe
ms.openlocfilehash: 0218cf1b4982b9e8c5b5c2817590bc5ebd8f1941
ms.sourcegitcommit: b6e506a45a1cd632294bafa1c959746cc3a144f6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/06/2019
ms.locfileid: "2896065"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="7bcd7-103">Блокировка товаров для продажи или покупки</span><span class="sxs-lookup"><span data-stu-id="7bcd7-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="7bcd7-104">Можно заблокировать товар для ввода в строки продажи или покупки либо учета в любой транзакции.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span></span>  

<span data-ttu-id="7bcd7-105">В следующей таблице показано, что происходит при блокировке товаров.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="7bcd7-106">Параметр</span><span class="sxs-lookup"><span data-stu-id="7bcd7-106">Option</span></span>|<span data-ttu-id="7bcd7-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7bcd7-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="7bcd7-108">**Продажи заблокированы**</span><span class="sxs-lookup"><span data-stu-id="7bcd7-108">**Sales Blocked**</span></span>|<span data-ttu-id="7bcd7-109">Невозможно ввести товар в документ продажи или в журнал товаров продажи.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-109">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="7bcd7-110">**Покупки заблокированы**</span><span class="sxs-lookup"><span data-stu-id="7bcd7-110">**Purchasing Blocked**</span></span>|<span data-ttu-id="7bcd7-111">Невозможно ввести товар в документ покупки, в журнал товаров покупки или в процессы планирования покупки.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="7bcd7-112">**Заблокировано**</span><span class="sxs-lookup"><span data-stu-id="7bcd7-112">**Blocked**</span></span>|<span data-ttu-id="7bcd7-113">Невозможно использовать товар для товарной транзакции.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-113">You cannot use the item for any item transaction.</span></span>|  

> [!NOTE]
> <span data-ttu-id="7bcd7-114">Заблокированные товары могут быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-114">Blocked items can be returned.</span></span> <span data-ttu-id="7bcd7-115">Это означает, что ни одна из вышеприведенных настроек не применяется, если товар используется в возвратах и кредит-нотах.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-115">This means that none of the above settings apply when the item is used on return orders and credit memos.</span></span>

<span data-ttu-id="7bcd7-116">Когда вы используете функцию **Копировать документ** для создания новых документов на основе существующих документов, вы получаете уведомление, если какие-либо элементы в строках исходного документа заблокированы.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-116">When you use the **Copy Document** function to create new documents based on existing documents, you are notified if any items on the source document lines are blocked.</span></span> <span data-ttu-id="7bcd7-117">Заблокированные строки документа исключаются из нового документа, а уведомление показывает обзор всех строк документа, которые заблокированы в исходном документе.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-117">The blocked document lines are excluded from the new document, and a notification shows an overview of all document lines that are blocked in the source document.</span></span>

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="7bcd7-118">Блокировка ввода товара в строки продажи</span><span class="sxs-lookup"><span data-stu-id="7bcd7-118">To block an item from being entered on sales lines</span></span>  

1.  <span data-ttu-id="7bcd7-119">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7bcd7-120">Выберите товар, который необходимо заблокировать, а затем установите флажок **Продажи заблокированы**.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-120">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

<span data-ttu-id="7bcd7-121">При попытке ввода товара в строку документа продажи или журнала отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-121">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="7bcd7-122">Блокировка ввода товара в строки покупки</span><span class="sxs-lookup"><span data-stu-id="7bcd7-122">To block an item from being entered on purchase lines</span></span>  

1.  <span data-ttu-id="7bcd7-123">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7bcd7-124">Выберите товар, который необходимо заблокировать, а затем установите флажок **Покупки заблокированы**.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-124">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

<span data-ttu-id="7bcd7-125">При попытке ввода товара в строку документа покупки или журнала отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-125">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="7bcd7-126">Блокировка товара для учета</span><span class="sxs-lookup"><span data-stu-id="7bcd7-126">To block an item from being posted</span></span>
1. <span data-ttu-id="7bcd7-127">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="7bcd7-128">Выберите товар, который необходимо заблокировать, а затем установите флажок **Заблокировано**.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-128">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

<span data-ttu-id="7bcd7-129">При попытке учесть любой тип транзакции для товара отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="7bcd7-129">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span></span>

## <a name="see-also"></a><span data-ttu-id="7bcd7-130">См. также</span><span class="sxs-lookup"><span data-stu-id="7bcd7-130">See Also</span></span>  
[<span data-ttu-id="7bcd7-131">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="7bcd7-131">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="7bcd7-132">Запасы</span><span class="sxs-lookup"><span data-stu-id="7bcd7-132">Inventory</span></span>](inventory-manage-inventory.md)  
