---
title: Настройка книг НДС в России
description: Российские улучшения включают работу с книгами НДС.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 2f6188ad8cd09a5569271e232773d96397d0f6af
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3189227"
---
# <a name="set-up-vat-ledgers"></a><span data-ttu-id="35053-103">Настройка книг НДС</span><span class="sxs-lookup"><span data-stu-id="35053-103">Set Up VAT Ledgers</span></span>

<span data-ttu-id="35053-104">Книги НДС используются для хранения сведений о НДС в транзакциях, связанных с товарами и услугами в России или с товарами, импортированными в Россию.</span><span class="sxs-lookup"><span data-stu-id="35053-104">VAT ledgers are used to store details about VAT in transactions that involve goods and services in Russia or goods imported into Russia.</span></span> <span data-ttu-id="35053-105">Можно создать и сохранять различные виды книг НДС.</span><span class="sxs-lookup"><span data-stu-id="35053-105">You can create and store different kinds of VAT ledgers.</span></span> <span data-ttu-id="35053-106">Например, можно создавать книги НДС для следующих целей:</span><span class="sxs-lookup"><span data-stu-id="35053-106">For example, you can create VAT ledgers for:</span></span>  

- <span data-ttu-id="35053-107">Продажи различным группам клиентов</span><span class="sxs-lookup"><span data-stu-id="35053-107">Sales to different groups of customers</span></span>
- <span data-ttu-id="35053-108">Разницы сумма продаж и предоплаты</span><span class="sxs-lookup"><span data-stu-id="35053-108">Sales amount differences and prepayments</span></span>
- <span data-ttu-id="35053-109">Покупки у разных групп поставщиков</span><span class="sxs-lookup"><span data-stu-id="35053-109">Purchases from different vendor groups</span></span>

<span data-ttu-id="35053-110">Чтобы использовать книги НДС, необходимо указать соответствующие серии номеров.</span><span class="sxs-lookup"><span data-stu-id="35053-110">To use VAT ledgers, you must specify the relevant number series.</span></span>

## <a name="to-set-up-vat-ledgers"></a><span data-ttu-id="35053-111">Настройка книг НДС</span><span class="sxs-lookup"><span data-stu-id="35053-111">To set up VAT ledgers</span></span>

1. <span data-ttu-id="35053-112">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка ГК**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="35053-112">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>

2. <span data-ttu-id="35053-113">В окне **Настройка ГК** на экспресс-вкладке **Нумерация** заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="35053-113">In the **General Ledger Setup** window, on the **Numbering** FastTab, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="35053-114">Поле</span><span class="sxs-lookup"><span data-stu-id="35053-114">Field</span></span>                            | <span data-ttu-id="35053-115">Описание</span><span class="sxs-lookup"><span data-stu-id="35053-115">Description</span></span>                                                  |
   | :------------------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="35053-116">**НДС - серия ном. книги покупок**</span><span class="sxs-lookup"><span data-stu-id="35053-116">**VAT Purch. Ledger No. Series**</span></span> | <span data-ttu-id="35053-117">Определяет серию номеров, которую требуется использовать для книг НДС в документах покупки.</span><span class="sxs-lookup"><span data-stu-id="35053-117">Specifies the number series that you want to use for VAT ledgers for purchase documents.</span></span> |
   | <span data-ttu-id="35053-118">**НДС - серия ном. книги продаж**</span><span class="sxs-lookup"><span data-stu-id="35053-118">**VAT Sales Ledger No. Series**</span></span>  | <span data-ttu-id="35053-119">Определяет серию номеров, которую требуется использовать для книг НДС в документах продажи.</span><span class="sxs-lookup"><span data-stu-id="35053-119">Specifies the number series that you want to use for VAT ledgers for sales documents.</span></span> |

   <span data-ttu-id="35053-120">Необходимо обеспечить, чтобы документы покупки у поставщика было невозможно учесть без указания даты и номера счета.</span><span class="sxs-lookup"><span data-stu-id="35053-120">You must ensure that vendor purchase documents cannot be posted without stating the invoice date and number.</span></span>

3. <span data-ttu-id="35053-121">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учетные группы поставщиков**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="35053-121">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendor Posting Groups**, and then choose the related link.</span></span>

4. <span data-ttu-id="35053-122">В окне **Учетные группы поставщика** для соответствующих учетных групп выберите поле **Счет-фактура обязательна**.</span><span class="sxs-lookup"><span data-stu-id="35053-122">In the **Vendor Posting Groups** window, for the relevant posting groups, select the **VAT Invoice Mandatory** field.</span></span>

   <span data-ttu-id="35053-123">Затем необходимо настроить учет НДС.</span><span class="sxs-lookup"><span data-stu-id="35053-123">Next, you must set up VAT posting.</span></span> <span data-ttu-id="35053-124">Для каждой настройки учета НДС необходимо указать, должны ли операции, которые используют эту настройку, включаться в книги НДС.</span><span class="sxs-lookup"><span data-stu-id="35053-124">For each VAT posting setup you must specify if entries that use the setup must be included in VAT ledgers.</span></span>

5. <span data-ttu-id="35053-125">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **НДС настройка учета**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="35053-125">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Posting Setup**, and then choose the related link.</span></span>

6. <span data-ttu-id="35053-126">В окне **Настройка учета НДС** для каждой настройки учета НДС заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="35053-126">In the **VAT Posting Setup** window, for each VAT posting setup, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="35053-127">Поле</span><span class="sxs-lookup"><span data-stu-id="35053-127">Field</span></span>                           | <span data-ttu-id="35053-128">Описание</span><span class="sxs-lookup"><span data-stu-id="35053-128">Description</span></span>                                                  |
   | :------------------------------ | :----------------------------------------------------------- |
   | <span data-ttu-id="35053-129">**Не включать в книгу НДС**</span><span class="sxs-lookup"><span data-stu-id="35053-129">**Not Include into VAT Ledger**</span></span> | <span data-ttu-id="35053-130">Указывает, должны ли операции, в которых используется настройка, включаться в книги НДС.</span><span class="sxs-lookup"><span data-stu-id="35053-130">Specifies if entries that use the setup must be included in VAT ledgers.</span></span> <span data-ttu-id="35053-131">Дополнительные сведения см. в пункте "Не включать в книгу НДС".</span><span class="sxs-lookup"><span data-stu-id="35053-131">For more information, see Not Include into VAT Ledger.</span></span> |
   | <span data-ttu-id="35053-132">**Освоб. от НДС**</span><span class="sxs-lookup"><span data-stu-id="35053-132">**VAT Exempt**</span></span>                  | <span data-ttu-id="35053-133">Определяет, освобождены ли от НДС операции, использующие эту настройку учета.</span><span class="sxs-lookup"><span data-stu-id="35053-133">Specifies if entries that use this posting setup are VAT exempt.</span></span> <span data-ttu-id="35053-134">Дополнительные сведения см. в пункте "Освоб. от НДС".</span><span class="sxs-lookup"><span data-stu-id="35053-134">For more information, see VAT Exempt.</span></span> |

<span data-ttu-id="35053-135">Теперь можно создавать книги НДС для покупок и продаж.</span><span class="sxs-lookup"><span data-stu-id="35053-135">Now, you can create VAT ledgers for purchases and sales.</span></span>

## <a name="see-also"></a><span data-ttu-id="35053-136">См. также</span><span class="sxs-lookup"><span data-stu-id="35053-136">See Also</span></span>

[<span data-ttu-id="35053-137">Подача отчета об НДС в налоговые органы</span><span class="sxs-lookup"><span data-stu-id="35053-137">Report VAT to Tax Authorities</span></span>](../../finance-how-report-vat.md)  
[<span data-ttu-id="35053-138">Регистрация НДС по заказам на покупку</span><span class="sxs-lookup"><span data-stu-id="35053-138">Register VAT on Purchase Orders</span></span>](How-to-Register-VAT-on-Purchase-Orders.md)  
[<span data-ttu-id="35053-139">Подготовка операций НДС к учету</span><span class="sxs-lookup"><span data-stu-id="35053-139">Prepare VAT Entries for Posting</span></span>](How-to-Prepare-VAT-Entries-for-Posting.md)  
[<span data-ttu-id="35053-140">Создание книг НДС</span><span class="sxs-lookup"><span data-stu-id="35053-140">Create VAT Ledgers</span></span>](How-to-Create-VAT-Ledgers.md)  
[<span data-ttu-id="35053-141">Создание дополнительных листов</span><span class="sxs-lookup"><span data-stu-id="35053-141">Create Additional Sheets</span></span>](How-to-Create-Additional-Sheets.md)  
