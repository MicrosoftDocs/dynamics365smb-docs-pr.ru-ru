---
title: "Блокировка товаров для продажи или покупки"
description: "В Business Central товар можно пометить как заблокированный для продажи, покупки или всех целей."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/23/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: c6f10f8252c00bf0a599f9fa794ee36c41ce92be
ms.openlocfilehash: 2f8be478dda62fef2cb34397de488f45d4fcfc0c
ms.contentlocale: ru-ru
ms.lasthandoff: 07/31/2018

---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="6fff9-103">Блокировка товаров для продажи или покупки</span><span class="sxs-lookup"><span data-stu-id="6fff9-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="6fff9-104">Можно заблокировать товар для ввода в строки продажи или покупки либо учета в любой транзакции.</span><span class="sxs-lookup"><span data-stu-id="6fff9-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span></span>  

<span data-ttu-id="6fff9-105">В следующей таблице показано, что происходит при блокировке товаров.</span><span class="sxs-lookup"><span data-stu-id="6fff9-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="6fff9-106">Параметр</span><span class="sxs-lookup"><span data-stu-id="6fff9-106">Option</span></span>|<span data-ttu-id="6fff9-107">Описанием</span><span class="sxs-lookup"><span data-stu-id="6fff9-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="6fff9-108">**Продажи заблокированы**</span><span class="sxs-lookup"><span data-stu-id="6fff9-108">**Sales Blocked**</span></span>|<span data-ttu-id="6fff9-109">Невозможно ввести товар в документ продажи или в журнал товаров продажи.</span><span class="sxs-lookup"><span data-stu-id="6fff9-109">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="6fff9-110">**Покупки заблокированы**</span><span class="sxs-lookup"><span data-stu-id="6fff9-110">**Purchasing Blocked**</span></span>|<span data-ttu-id="6fff9-111">Невозможно ввести товар в документ покупки, в журнал товаров покупки или в процессы планирования покупки.</span><span class="sxs-lookup"><span data-stu-id="6fff9-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="6fff9-112">**Заблокировано**</span><span class="sxs-lookup"><span data-stu-id="6fff9-112">**Blocked**</span></span>|<span data-ttu-id="6fff9-113">Невозможно использовать товар для товарной транзакции.</span><span class="sxs-lookup"><span data-stu-id="6fff9-113">You cannot use the item for any item transaction.</span></span> <span data-ttu-id="6fff9-114">Дополнительные сведения о блокировке товара для всех целей см. в карточке товара.</span><span class="sxs-lookup"><span data-stu-id="6fff9-114">For more information about blocking an item for all purposes, see Item Card.</span></span>|  

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="6fff9-115">Блокировка ввода товара в строки продажи</span><span class="sxs-lookup"><span data-stu-id="6fff9-115">To block an item from being entered on sales lines</span></span>  

1.  <span data-ttu-id="6fff9-116">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Товары**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="6fff9-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6fff9-117">Выберите товар, который необходимо заблокировать, а затем установите флажок **Продажи заблокированы**.</span><span class="sxs-lookup"><span data-stu-id="6fff9-117">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

<span data-ttu-id="6fff9-118">При попытке ввода товара в строку документа продажи или журнала отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="6fff9-118">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="6fff9-119">Блокировка ввода товара в строки покупки</span><span class="sxs-lookup"><span data-stu-id="6fff9-119">To block an item from being entered on purchase lines</span></span>  

1.  <span data-ttu-id="6fff9-120">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Товары**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="6fff9-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6fff9-121">Выберите товар, который необходимо заблокировать, а затем установите флажок **Покупки заблокированы**.</span><span class="sxs-lookup"><span data-stu-id="6fff9-121">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

<span data-ttu-id="6fff9-122">При попытке ввода товара в строку документа покупки или журнала отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="6fff9-122">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="6fff9-123">Блокировка товара для учета</span><span class="sxs-lookup"><span data-stu-id="6fff9-123">To block an item from being posted</span></span>
1. <span data-ttu-id="6fff9-124">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Товары**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="6fff9-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="6fff9-125">Выберите товар, который необходимо заблокировать, а затем установите флажок **Заблокировано**.</span><span class="sxs-lookup"><span data-stu-id="6fff9-125">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

<span data-ttu-id="6fff9-126">При попытке учесть любой тип транзакции для товара отобразится сообщение об ошибке, указывающее, что товар заблокирован.</span><span class="sxs-lookup"><span data-stu-id="6fff9-126">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span></span>

## <a name="see-also"></a><span data-ttu-id="6fff9-127">См. также</span><span class="sxs-lookup"><span data-stu-id="6fff9-127">See Also</span></span>  
[<span data-ttu-id="6fff9-128">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="6fff9-128">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="6fff9-129">Наличие</span><span class="sxs-lookup"><span data-stu-id="6fff9-129">Inventory</span></span>](inventory-manage-inventory.md)  

