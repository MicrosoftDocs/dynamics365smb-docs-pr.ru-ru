---
title: Книги НДС в России
description: Российские улучшения включают работу с книгами НДС.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 694bad6242e9cc723064e8754586a5899507e5dd
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738232"
---
# <a name="vat-ledgers"></a><span data-ttu-id="444da-103">Книги НДС</span><span class="sxs-lookup"><span data-stu-id="444da-103">VAT Ledgers</span></span>

<span data-ttu-id="444da-104">Функция книги НДС позволяет создавать и печатать следующие окна:</span><span class="sxs-lookup"><span data-stu-id="444da-104">The VAT ledger feature enables you to create and print the following windows:</span></span>

- <span data-ttu-id="444da-105">НДС Книга покупок</span><span class="sxs-lookup"><span data-stu-id="444da-105">VAT Purchase Ledger</span></span>
- <span data-ttu-id="444da-106">НДС Книга продаж</span><span class="sxs-lookup"><span data-stu-id="444da-106">VAT Sales Ledger</span></span>
- <span data-ttu-id="444da-107">Дополнительный лист НДС книги покупок</span><span class="sxs-lookup"><span data-stu-id="444da-107">VAT Purchase Ledger Additional Sheet</span></span>
- <span data-ttu-id="444da-108">Дополнительный лист НДС книги продаж</span><span class="sxs-lookup"><span data-stu-id="444da-108">VAT Sales Ledger Additional Sheet</span></span>

## <a name="vat-purchase-ledgers-and-vat-sales-ledgers"></a><span data-ttu-id="444da-109">"НДС - книги покупок" и "НДС - книги продаж"</span><span class="sxs-lookup"><span data-stu-id="444da-109">VAT Purchase Ledgers and VAT Sales Ledgers</span></span>

<span data-ttu-id="444da-110">Перед созданием книг НДС необходимо настроить серию номеров и группы учета поставщиков.</span><span class="sxs-lookup"><span data-stu-id="444da-110">Before you can create VAT ledgers, you must set up number series and vendor posting groups.</span></span> <span data-ttu-id="444da-111">Также необходимо настроить учетные группы НДС для определения того, как операции НДС должны быть включены в книги НДС.</span><span class="sxs-lookup"><span data-stu-id="444da-111">You must also set up VAT posting groups to identify how VAT entries must be included in VAT ledgers.</span></span> <span data-ttu-id="444da-112">Кроме того, для каждой настройки учета НДС следует определить, должны ли операции, которые используют эту настройку, включаться в книги НДС, а также освобождены ли эти операции от НДС.</span><span class="sxs-lookup"><span data-stu-id="444da-112">Also, for each VAT posting setup, you must specify if entries that use the setup must be included in VAT ledgers, and if the entries are VAT exempt.</span></span> <span data-ttu-id="444da-113">Дополнительные сведения см. в разделе [Практическое руководство. Настройка книг НДС](How-to-Set-Up-VAT-Ledgers.md).</span><span class="sxs-lookup"><span data-stu-id="444da-113">For more information, see [How to: Set Up VAT Ledgers](How-to-Set-Up-VAT-Ledgers.md).</span></span>

<span data-ttu-id="444da-114">Можно создать любое количество книг НДС.</span><span class="sxs-lookup"><span data-stu-id="444da-114">You can create and store any number of VAT ledgers.</span></span> <span data-ttu-id="444da-115">Например, можно создать следующие книги:</span><span class="sxs-lookup"><span data-stu-id="444da-115">For example, you can create the following:</span></span> 

- <span data-ttu-id="444da-116">Книги продаж для различных групп клиентов.</span><span class="sxs-lookup"><span data-stu-id="444da-116">Sales ledgers for different groups of customers.</span></span>
- <span data-ttu-id="444da-117">Дополнительные книги продаж для разниц суммы и предоплат.</span><span class="sxs-lookup"><span data-stu-id="444da-117">Additional sales ledgers for amount differences and prepayments.</span></span>
- <span data-ttu-id="444da-118">Объединенные книги продаж для компании в целом.</span><span class="sxs-lookup"><span data-stu-id="444da-118">Joint sales ledgers for the whole company.</span></span>

<span data-ttu-id="444da-119">Для создания книги НДС необходимо сначала определить тип книги НДС, а затем следует добавить строки в книгу НДС покупок или книгу НДС продаж с помощью пакетных заданий **Создание книги покупок** и **Создание книги продаж**.</span><span class="sxs-lookup"><span data-stu-id="444da-119">To create a VAT ledger, first you must define a VAT ledger type, and then you must add lines to the VAT purchase ledger or VAT sales ledger by using the **Create VAT Purchase Ledger** and **Create VAT Sales Ledger** batch jobs.</span></span> <span data-ttu-id="444da-120">После добавления строк в книгу НДС можно распечатать ее.</span><span class="sxs-lookup"><span data-stu-id="444da-120">When you have added lines to the VAT ledger, you can print it.</span></span>

<span data-ttu-id="444da-121">Дополнительные сведения см. в разделе [Практическое руководство. Создание книг НДС](How-to-Create-VAT-Ledgers.md).</span><span class="sxs-lookup"><span data-stu-id="444da-121">For more information, see [How to: Create VAT Ledgers](How-to-Create-VAT-Ledgers.md).</span></span>

## <a name="marking-a-vat-purchase-ledger"></a><span data-ttu-id="444da-122">Маркировка НДС книги покупок</span><span class="sxs-lookup"><span data-stu-id="444da-122">Marking a VAT Purchase Ledger</span></span>

<span data-ttu-id="444da-123">НДС для документов покупки должен быть отражен в книге покупок.</span><span class="sxs-lookup"><span data-stu-id="444da-123">The VAT for purchase documents must be reflected in the purchase ledger.</span></span> <span data-ttu-id="444da-124">Возвраты от клиентов должны отражаться в книгах покупок.</span><span class="sxs-lookup"><span data-stu-id="444da-124">Return orders of the customers must be reflected in purchase books.</span></span>

<span data-ttu-id="444da-125">В следующей процедуре показан порядок маркировки НДС книги покупок.</span><span class="sxs-lookup"><span data-stu-id="444da-125">The following procedure shows how to mark a VAT purchase ledger.</span></span> 

1. <span data-ttu-id="444da-126">В окне **Возврат продажи** или **Кредит-нота продажи** установите флажок **Включить в НДС книгу покупок**.</span><span class="sxs-lookup"><span data-stu-id="444da-126">In the **Sales Return Order** window or the **Sales Credit Memo** window, select the **Include in Purch. VAT Ledger** check box.</span></span>

<span data-ttu-id="444da-127">Эти маркированные документы будут отражены в книге покупок или книге продаж.</span><span class="sxs-lookup"><span data-stu-id="444da-127">These marked documents will be reflected in the purchase book or in the sales book.</span></span> <span data-ttu-id="444da-128">Возвраты маркируются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="444da-128">Sales return orders are marked by default.</span></span>

## <a name="see-also"></a><span data-ttu-id="444da-129">См. также</span><span class="sxs-lookup"><span data-stu-id="444da-129">See Also</span></span>

[<span data-ttu-id="444da-130">Практическое руководство. Настройка книг НДС</span><span class="sxs-lookup"><span data-stu-id="444da-130">How to: Set Up VAT Ledgers</span></span>](How-to-Set-Up-VAT-Ledgers.md)  
[<span data-ttu-id="444da-131">Практическое руководство. Создание книг НДС</span><span class="sxs-lookup"><span data-stu-id="444da-131">How to: Create VAT Ledgers</span></span>](How-to-Create-VAT-Ledgers.md)  
[<span data-ttu-id="444da-132">Практическое руководство. Создание дополнительных листов</span><span class="sxs-lookup"><span data-stu-id="444da-132">How to: Create Additional Sheets</span></span>](How-to-Create-Additional-Sheets.md)  
[<span data-ttu-id="444da-133">Учет НДС в продажах</span><span class="sxs-lookup"><span data-stu-id="444da-133">Posting VAT on Sales</span></span>](Posting-VAT-on-Sales.md)  
