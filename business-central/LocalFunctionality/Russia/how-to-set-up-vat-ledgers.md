---
title: Настройка книг НДС в России
description: Российские улучшения включают работу с книгами НДС.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 72bd1ccd837bbcef6a17f78af3d2aa71b4846574
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738246"
---
# <a name="how-to-set-up-vat-ledgers"></a><span data-ttu-id="5d3b7-103">Практическое руководство. Настройка книг НДС</span><span class="sxs-lookup"><span data-stu-id="5d3b7-103">How to: Set Up VAT Ledgers</span></span>

<span data-ttu-id="5d3b7-104">Книги НДС используются для хранения сведений о НДС в транзакциях, связанных с товарами и услугами в России или с товарами, импортированными в Россию.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-104">VAT ledgers are used to store details about VAT in transactions that involve goods and services in Russia or goods imported into Russia.</span></span> <span data-ttu-id="5d3b7-105">Можно создать и сохранять различные виды книг НДС.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-105">You can create and store different kinds of VAT ledgers.</span></span> <span data-ttu-id="5d3b7-106">Например, можно создавать книги НДС для следующих целей:</span><span class="sxs-lookup"><span data-stu-id="5d3b7-106">For example, you can create VAT ledgers for:</span></span>  

- <span data-ttu-id="5d3b7-107">Продажи различным группам клиентов</span><span class="sxs-lookup"><span data-stu-id="5d3b7-107">Sales to different groups of customers</span></span>
- <span data-ttu-id="5d3b7-108">Разницы сумма продаж и предоплаты</span><span class="sxs-lookup"><span data-stu-id="5d3b7-108">Sales amount differences and prepayments</span></span>
- <span data-ttu-id="5d3b7-109">Покупки у разных групп поставщиков</span><span class="sxs-lookup"><span data-stu-id="5d3b7-109">Purchases from different vendor groups</span></span>

<span data-ttu-id="5d3b7-110">Чтобы использовать книги НДС, необходимо указать соответствующие серии номеров.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-110">To use VAT ledgers, you must specify the relevant number series.</span></span>

## <a name="to-set-up-vat-ledgers"></a><span data-ttu-id="5d3b7-111">Настройка книг НДС</span><span class="sxs-lookup"><span data-stu-id="5d3b7-111">To set up VAT ledgers</span></span>

1. <span data-ttu-id="5d3b7-112">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка ГК**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-112">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>

2. <span data-ttu-id="5d3b7-113">В окне **Настройка ГК** на экспресс-вкладке **Нумерация** заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-113">In the **General Ledger Setup** window, on the **Numbering** FastTab, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="5d3b7-114">Поле</span><span class="sxs-lookup"><span data-stu-id="5d3b7-114">Field</span></span>                            | <span data-ttu-id="5d3b7-115">Описание</span><span class="sxs-lookup"><span data-stu-id="5d3b7-115">Description</span></span>                                                  |
   | :------------------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="5d3b7-116">**НДС - серия ном. книги покупок**</span><span class="sxs-lookup"><span data-stu-id="5d3b7-116">**VAT Purch. Ledger No. Series**</span></span> | <span data-ttu-id="5d3b7-117">Определяет серию номеров, которую требуется использовать для книг НДС в документах покупки.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-117">Specifies the number series that you want to use for VAT ledgers for purchase documents.</span></span> |
   | <span data-ttu-id="5d3b7-118">**НДС - серия ном. книги продаж**</span><span class="sxs-lookup"><span data-stu-id="5d3b7-118">**VAT Sales Ledger No. Series**</span></span>  | <span data-ttu-id="5d3b7-119">Определяет серию номеров, которую требуется использовать для книг НДС в документах продажи.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-119">Specifies the number series that you want to use for VAT ledgers for sales documents.</span></span> |

   <span data-ttu-id="5d3b7-120">Необходимо обеспечить, чтобы документы покупки у поставщика было невозможно учесть без указания даты и номера счета.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-120">You must ensure that vendor purchase documents cannot be posted without stating the invoice date and number.</span></span>

3. <span data-ttu-id="5d3b7-121">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учетные группы поставщика**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-121">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendor Posting Groups**, and then choose the related link.</span></span>

4. <span data-ttu-id="5d3b7-122">В окне **Учетные группы поставщика** для соответствующих учетных групп выберите поле **Счет-фактура обязательна**.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-122">In the **Vendor Posting Groups** window, for the relevant posting groups, select the **VAT Invoice Mandatory** field.</span></span>

   <span data-ttu-id="5d3b7-123">Затем необходимо настроить учет НДС.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-123">Next, you must set up VAT posting.</span></span> <span data-ttu-id="5d3b7-124">Для каждой настройки учета НДС необходимо указать, должны ли операции, которые используют эту настройку, включаться в книги НДС.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-124">For each VAT posting setup you must specify if entries that use the setup must be included in VAT ledgers.</span></span>

5. <span data-ttu-id="5d3b7-125">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка учета НДС**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-125">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Posting Setup**, and then choose the related link.</span></span>

6. <span data-ttu-id="5d3b7-126">В окне **Настройка учета НДС** для каждой настройки учета НДС заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-126">In the **VAT Posting Setup** window, for each VAT posting setup, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="5d3b7-127">Поле</span><span class="sxs-lookup"><span data-stu-id="5d3b7-127">Field</span></span>                           | <span data-ttu-id="5d3b7-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5d3b7-128">Description</span></span>                                                  |
   | :------------------------------ | :----------------------------------------------------------- |
   | <span data-ttu-id="5d3b7-129">**Не включать в книгу НДС**</span><span class="sxs-lookup"><span data-stu-id="5d3b7-129">**Not Include into VAT Ledger**</span></span> | <span data-ttu-id="5d3b7-130">Указывает, должны ли операции, в которых используется настройка, включаться в книги НДС.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-130">Specifies if entries that use the setup must be included in VAT ledgers.</span></span> <span data-ttu-id="5d3b7-131">Дополнительные сведения см. в пункте "Не включать в книгу НДС".</span><span class="sxs-lookup"><span data-stu-id="5d3b7-131">For more information, see Not Include into VAT Ledger.</span></span> |
   | <span data-ttu-id="5d3b7-132">**Освоб. от НДС**</span><span class="sxs-lookup"><span data-stu-id="5d3b7-132">**VAT Exempt**</span></span>                  | <span data-ttu-id="5d3b7-133">Определяет, освобождены ли от НДС операции, использующие эту настройку учета.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-133">Specifies if entries that use this posting setup are VAT exempt.</span></span> <span data-ttu-id="5d3b7-134">Дополнительные сведения см. в пункте "Освоб. от НДС".</span><span class="sxs-lookup"><span data-stu-id="5d3b7-134">For more information, see VAT Exempt.</span></span> |

<span data-ttu-id="5d3b7-135">Теперь можно создавать книги НДС для покупок и продаж.</span><span class="sxs-lookup"><span data-stu-id="5d3b7-135">Now, you can create VAT ledgers for purchases and sales.</span></span>

## <a name="see-also"></a><span data-ttu-id="5d3b7-136">См. также</span><span class="sxs-lookup"><span data-stu-id="5d3b7-136">See Also</span></span>

[<span data-ttu-id="5d3b7-137">Практическое руководство. Подача отчета об НДС в налоговые органы</span><span class="sxs-lookup"><span data-stu-id="5d3b7-137">How to: Report VAT to Tax Authorities</span></span>](../../finance-how-report-vat.md)  
[<span data-ttu-id="5d3b7-138">Практическое руководство. Регистрация НДС по заказам на покупку</span><span class="sxs-lookup"><span data-stu-id="5d3b7-138">How to: Register VAT on Purchase Orders</span></span>](How-to-Register-VAT-on-Purchase-Orders.md)  
[<span data-ttu-id="5d3b7-139">Практическое руководство. Подготовка операций НДС к учету</span><span class="sxs-lookup"><span data-stu-id="5d3b7-139">How to: Prepare VAT Entries for Posting</span></span>](How-to-Prepare-VAT-Entries-for-Posting.md)  
[<span data-ttu-id="5d3b7-140">Практическое руководство. Создание книг НДС</span><span class="sxs-lookup"><span data-stu-id="5d3b7-140">How to: Create VAT Ledgers</span></span>](How-to-Create-VAT-Ledgers.md)  
[<span data-ttu-id="5d3b7-141">Практическое руководство. Создание дополнительных листов</span><span class="sxs-lookup"><span data-stu-id="5d3b7-141">How to: Create Additional Sheets</span></span>](How-to-Create-Additional-Sheets.md)  
