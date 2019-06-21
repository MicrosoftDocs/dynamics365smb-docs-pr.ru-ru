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
ms.openlocfilehash: 8c98e4b893783c795a49e05ab04dc70b03161c6a
ms.sourcegitcommit: bf5f89dfaf5ad9f8f9902941cf3dac3e9f3553e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2019
ms.locfileid: "1594258"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="5988b-103">Блокировка товаров для продажи или покупки</span><span class="sxs-lookup"><span data-stu-id="5988b-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="5988b-104">Можно заблокировать товар для ввода в строки продажи или покупки либо учета в любой транзакции.</span><span class="sxs-lookup"><span data-stu-id="5988b-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span></span>  

<span data-ttu-id="5988b-105">В следующей таблице показано, что происходит при блокировке товаров.</span><span class="sxs-lookup"><span data-stu-id="5988b-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="5988b-106">Параметр</span><span class="sxs-lookup"><span data-stu-id="5988b-106">Option</span></span>|<span data-ttu-id="5988b-107">Описанием</span><span class="sxs-lookup"><span data-stu-id="5988b-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="5988b-108">**Продажи заблокированы**</span><span class="sxs-lookup"><span data-stu-id="5988b-108">**Sales Blocked**</span></span>|<span data-ttu-id="5988b-109">Невозможно ввести товар в документ продажи или в журнал товаров продажи.</span><span class="sxs-lookup"><span data-stu-id="5988b-109">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="5988b-110">**Покупки заблокированы**</span><span class="sxs-lookup"><span data-stu-id="5988b-110">**Purchasing Blocked**</span></span>|<span data-ttu-id="5988b-111">Невозможно ввести товар в документ покупки, в журнал товаров покупки или в процессы планирования покупки.</span><span class="sxs-lookup"><span data-stu-id="5988b-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="5988b-112">**Заблокировано**</span><span class="sxs-lookup"><span data-stu-id="5988b-112">**Blocked**</span></span>|<span data-ttu-id="5988b-113">Невозможно использовать товар для товарной транзакции.</span><span class="sxs-lookup"><span data-stu-id="5988b-113">You cannot use the item for any item transaction.</span></span>|  

> [!NOTE]
> <span data-ttu-id="5988b-114">Заблокированные товары могут быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="5988b-114">Blocked items can be returned.</span></span> <span data-ttu-id="5988b-115">Это означает, что ни одна из вышеприведенных настроек не применяется, если товар используется в возвратах и кредит-нотах.</span><span class="sxs-lookup"><span data-stu-id="5988b-115">This means that none of the above settings apply when the item is used on return orders and credit memos.</span></span>

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="5988b-116">Блокировка ввода товара в строки продажи</span><span class="sxs-lookup"><span data-stu-id="5988b-116">To block an item from being entered on sales lines</span></span>  

1.  <span data-ttu-id="5988b-117">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5988b-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5988b-118">Выберите товар, который необходимо заблокировать, а затем установите флажок **Продажи заблокированы**.</span><span class="sxs-lookup"><span data-stu-id="5988b-118">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

<span data-ttu-id="5988b-119">При попытке ввода товара в строку документа продажи или журнала отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="5988b-119">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="5988b-120">Блокировка ввода товара в строки покупки</span><span class="sxs-lookup"><span data-stu-id="5988b-120">To block an item from being entered on purchase lines</span></span>  

1.  <span data-ttu-id="5988b-121">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5988b-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5988b-122">Выберите товар, который необходимо заблокировать, а затем установите флажок **Покупки заблокированы**.</span><span class="sxs-lookup"><span data-stu-id="5988b-122">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

<span data-ttu-id="5988b-123">При попытке ввода товара в строку документа покупки или журнала отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="5988b-123">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="5988b-124">Блокировка товара для учета</span><span class="sxs-lookup"><span data-stu-id="5988b-124">To block an item from being posted</span></span>
1. <span data-ttu-id="5988b-125">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5988b-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="5988b-126">Выберите товар, который необходимо заблокировать, а затем установите флажок **Заблокировано**.</span><span class="sxs-lookup"><span data-stu-id="5988b-126">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

<span data-ttu-id="5988b-127">При попытке учесть любой тип транзакции для товара отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="5988b-127">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span></span>

## <a name="see-also"></a><span data-ttu-id="5988b-128">См. также</span><span class="sxs-lookup"><span data-stu-id="5988b-128">See Also</span></span>  
[<span data-ttu-id="5988b-129">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="5988b-129">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="5988b-130">Наличие</span><span class="sxs-lookup"><span data-stu-id="5988b-130">Inventory</span></span>](inventory-manage-inventory.md)  
