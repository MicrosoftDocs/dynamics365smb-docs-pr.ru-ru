---
title: Блокировка товаров для продажи или покупки
description: В Business Central товар можно пометить как заблокированный для продажи, покупки или всех целей.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: e13d59e939e71a252e08afc26d2fb1ec76b247c9
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1238536"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="563d9-103">Блокировка товаров для продажи или покупки</span><span class="sxs-lookup"><span data-stu-id="563d9-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="563d9-104">Можно заблокировать товар для ввода в строки продажи или покупки либо учета в любой транзакции.</span><span class="sxs-lookup"><span data-stu-id="563d9-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span></span>  

<span data-ttu-id="563d9-105">В следующей таблице показано, что происходит при блокировке товаров.</span><span class="sxs-lookup"><span data-stu-id="563d9-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="563d9-106">Параметр</span><span class="sxs-lookup"><span data-stu-id="563d9-106">Option</span></span>|<span data-ttu-id="563d9-107">Описанием</span><span class="sxs-lookup"><span data-stu-id="563d9-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="563d9-108">**Продажи заблокированы**</span><span class="sxs-lookup"><span data-stu-id="563d9-108">**Sales Blocked**</span></span>|<span data-ttu-id="563d9-109">Невозможно ввести товар в документ продажи или в журнал товаров продажи.</span><span class="sxs-lookup"><span data-stu-id="563d9-109">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="563d9-110">**Покупки заблокированы**</span><span class="sxs-lookup"><span data-stu-id="563d9-110">**Purchasing Blocked**</span></span>|<span data-ttu-id="563d9-111">Невозможно ввести товар в документ покупки, в журнал товаров покупки или в процессы планирования покупки.</span><span class="sxs-lookup"><span data-stu-id="563d9-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="563d9-112">**Заблокировано**</span><span class="sxs-lookup"><span data-stu-id="563d9-112">**Blocked**</span></span>|<span data-ttu-id="563d9-113">Невозможно использовать товар для товарной транзакции.</span><span class="sxs-lookup"><span data-stu-id="563d9-113">You cannot use the item for any item transaction.</span></span> <span data-ttu-id="563d9-114">Дополнительные сведения о блокировке товара для всех целей см. в карточке товара.</span><span class="sxs-lookup"><span data-stu-id="563d9-114">For more information about blocking an item for all purposes, see Item Card.</span></span>|  

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="563d9-115">Блокировка ввода товара в строки продажи</span><span class="sxs-lookup"><span data-stu-id="563d9-115">To block an item from being entered on sales lines</span></span>  

1.  <span data-ttu-id="563d9-116">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="563d9-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="563d9-117">Выберите товар, который необходимо заблокировать, а затем установите флажок **Продажи заблокированы**.</span><span class="sxs-lookup"><span data-stu-id="563d9-117">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

<span data-ttu-id="563d9-118">При попытке ввода товара в строку документа продажи или журнала отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="563d9-118">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="563d9-119">Блокировка ввода товара в строки покупки</span><span class="sxs-lookup"><span data-stu-id="563d9-119">To block an item from being entered on purchase lines</span></span>  

1.  <span data-ttu-id="563d9-120">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="563d9-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="563d9-121">Выберите товар, который необходимо заблокировать, а затем установите флажок **Покупки заблокированы**.</span><span class="sxs-lookup"><span data-stu-id="563d9-121">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

<span data-ttu-id="563d9-122">При попытке ввода товара в строку документа покупки или журнала отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="563d9-122">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="563d9-123">Блокировка товара для учета</span><span class="sxs-lookup"><span data-stu-id="563d9-123">To block an item from being posted</span></span>
1. <span data-ttu-id="563d9-124">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="563d9-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="563d9-125">Выберите товар, который необходимо заблокировать, а затем установите флажок **Заблокировано**.</span><span class="sxs-lookup"><span data-stu-id="563d9-125">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

<span data-ttu-id="563d9-126">При попытке учесть любой тип транзакции для товара отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="563d9-126">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span></span>

## <a name="see-also"></a><span data-ttu-id="563d9-127">См. также</span><span class="sxs-lookup"><span data-stu-id="563d9-127">See Also</span></span>  
[<span data-ttu-id="563d9-128">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="563d9-128">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="563d9-129">Наличие</span><span class="sxs-lookup"><span data-stu-id="563d9-129">Inventory</span></span>](inventory-manage-inventory.md)  
