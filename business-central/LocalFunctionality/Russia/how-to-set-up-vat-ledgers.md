---
title: Настройка книг НДС в России
description: Российские улучшения включают работу с книгами НДС.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: e17fff56677a8596c6bdfeddd1940879e7b271fc
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5786665"
---
# <a name="set-up-vat-ledgers"></a><span data-ttu-id="2cfc9-103">Настройка книг НДС</span><span class="sxs-lookup"><span data-stu-id="2cfc9-103">Set Up VAT Ledgers</span></span>

<span data-ttu-id="2cfc9-104">Книги НДС используются для хранения сведений о НДС в транзакциях, связанных с товарами и услугами в России или с товарами, импортированными в Россию.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-104">VAT ledgers are used to store details about VAT in transactions that involve goods and services in Russia or goods imported into Russia.</span></span> <span data-ttu-id="2cfc9-105">Можно создать и сохранять различные виды книг НДС.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-105">You can create and store different kinds of VAT ledgers.</span></span> <span data-ttu-id="2cfc9-106">Например, можно создавать книги НДС для следующих целей:</span><span class="sxs-lookup"><span data-stu-id="2cfc9-106">For example, you can create VAT ledgers for:</span></span>  

- <span data-ttu-id="2cfc9-107">Продажи различным группам клиентов</span><span class="sxs-lookup"><span data-stu-id="2cfc9-107">Sales to different groups of customers</span></span>
- <span data-ttu-id="2cfc9-108">Разницы сумма продаж и предоплаты</span><span class="sxs-lookup"><span data-stu-id="2cfc9-108">Sales amount differences and prepayments</span></span>
- <span data-ttu-id="2cfc9-109">Покупки у разных групп поставщиков</span><span class="sxs-lookup"><span data-stu-id="2cfc9-109">Purchases from different vendor groups</span></span>

<span data-ttu-id="2cfc9-110">Чтобы использовать книги НДС, необходимо указать соответствующие серии номеров.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-110">To use VAT ledgers, you must specify the relevant number series.</span></span>

## <a name="to-set-up-vat-ledgers"></a><span data-ttu-id="2cfc9-111">Настройка книг НДС</span><span class="sxs-lookup"><span data-stu-id="2cfc9-111">To set up VAT ledgers</span></span>

1. <span data-ttu-id="2cfc9-112">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка ГК**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-112">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>

2. <span data-ttu-id="2cfc9-113">В окне **Настройка ГК** на экспресс-вкладке **Нумерация** заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-113">In the **General Ledger Setup** window, on the **Numbering** FastTab, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="2cfc9-114">Поле</span><span class="sxs-lookup"><span data-stu-id="2cfc9-114">Field</span></span>                            | <span data-ttu-id="2cfc9-115">Описание</span><span class="sxs-lookup"><span data-stu-id="2cfc9-115">Description</span></span>                                                  |
   | :------------------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="2cfc9-116">**НДС - серия ном. книги покупок**</span><span class="sxs-lookup"><span data-stu-id="2cfc9-116">**VAT Purch. Ledger No. Series**</span></span> | <span data-ttu-id="2cfc9-117">Определяет серию номеров, которую требуется использовать для книг НДС в документах покупки.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-117">Specifies the number series that you want to use for VAT ledgers for purchase documents.</span></span> |
   | <span data-ttu-id="2cfc9-118">**НДС - серия ном. книги продаж**</span><span class="sxs-lookup"><span data-stu-id="2cfc9-118">**VAT Sales Ledger No. Series**</span></span>  | <span data-ttu-id="2cfc9-119">Определяет серию номеров, которую требуется использовать для книг НДС в документах продажи.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-119">Specifies the number series that you want to use for VAT ledgers for sales documents.</span></span> |

   <span data-ttu-id="2cfc9-120">Необходимо обеспечить, чтобы документы покупки у поставщика было невозможно учесть без указания даты и номера счета.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-120">You must ensure that vendor purchase documents cannot be posted without stating the invoice date and number.</span></span>

3. <span data-ttu-id="2cfc9-121">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учетные группы поставщиков**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-121">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendor Posting Groups**, and then choose the related link.</span></span>

4. <span data-ttu-id="2cfc9-122">В окне **Учетные группы поставщика** для соответствующих учетных групп выберите поле **Счет-фактура обязательна**.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-122">In the **Vendor Posting Groups** window, for the relevant posting groups, select the **VAT Invoice Mandatory** field.</span></span>

   <span data-ttu-id="2cfc9-123">Затем необходимо настроить учет НДС.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-123">Next, you must set up VAT posting.</span></span> <span data-ttu-id="2cfc9-124">Для каждой настройки учета НДС необходимо указать, должны ли операции, которые используют эту настройку, включаться в книги НДС.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-124">For each VAT posting setup you must specify if entries that use the setup must be included in VAT ledgers.</span></span>

5. <span data-ttu-id="2cfc9-125">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **НДС настройка учета**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-125">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Posting Setup**, and then choose the related link.</span></span>

6. <span data-ttu-id="2cfc9-126">В окне **Настройка учета НДС** для каждой настройки учета НДС заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-126">In the **VAT Posting Setup** window, for each VAT posting setup, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="2cfc9-127">Поле</span><span class="sxs-lookup"><span data-stu-id="2cfc9-127">Field</span></span>                           | <span data-ttu-id="2cfc9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2cfc9-128">Description</span></span>                                                  |
   | :------------------------------ | :----------------------------------------------------------- |
   | <span data-ttu-id="2cfc9-129">**Не включать в книгу НДС**</span><span class="sxs-lookup"><span data-stu-id="2cfc9-129">**Not Include into VAT Ledger**</span></span> | <span data-ttu-id="2cfc9-130">Указывает, должны ли операции, в которых используется настройка, включаться в книги НДС.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-130">Specifies if entries that use the setup must be included in VAT ledgers.</span></span> <span data-ttu-id="2cfc9-131">Дополнительные сведения см. в пункте "Не включать в книгу НДС".</span><span class="sxs-lookup"><span data-stu-id="2cfc9-131">For more information, see Not Include into VAT Ledger.</span></span> |
   | <span data-ttu-id="2cfc9-132">**Освоб. от НДС**</span><span class="sxs-lookup"><span data-stu-id="2cfc9-132">**VAT Exempt**</span></span>                  | <span data-ttu-id="2cfc9-133">Определяет, освобождены ли от НДС операции, использующие эту настройку учета.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-133">Specifies if entries that use this posting setup are VAT exempt.</span></span> <span data-ttu-id="2cfc9-134">Дополнительные сведения см. в пункте "Освоб. от НДС".</span><span class="sxs-lookup"><span data-stu-id="2cfc9-134">For more information, see VAT Exempt.</span></span> |

<span data-ttu-id="2cfc9-135">Теперь можно создавать книги НДС для покупок и продаж.</span><span class="sxs-lookup"><span data-stu-id="2cfc9-135">Now, you can create VAT ledgers for purchases and sales.</span></span>

## <a name="see-also"></a><span data-ttu-id="2cfc9-136">См. также</span><span class="sxs-lookup"><span data-stu-id="2cfc9-136">See Also</span></span>

[<span data-ttu-id="2cfc9-137">Подача отчета об НДС в налоговые органы</span><span class="sxs-lookup"><span data-stu-id="2cfc9-137">Report VAT to Tax Authorities</span></span>](../../finance-how-report-vat.md)  
[<span data-ttu-id="2cfc9-138">Регистрация НДС по заказам на покупку</span><span class="sxs-lookup"><span data-stu-id="2cfc9-138">Register VAT on Purchase Orders</span></span>](How-to-Register-VAT-on-Purchase-Orders.md)  
[<span data-ttu-id="2cfc9-139">Подготовка операций НДС к учету</span><span class="sxs-lookup"><span data-stu-id="2cfc9-139">Prepare VAT Entries for Posting</span></span>](How-to-Prepare-VAT-Entries-for-Posting.md)  
[<span data-ttu-id="2cfc9-140">Создание книг НДС</span><span class="sxs-lookup"><span data-stu-id="2cfc9-140">Create VAT Ledgers</span></span>](How-to-Create-VAT-Ledgers.md)  
[<span data-ttu-id="2cfc9-141">Создание дополнительных листов</span><span class="sxs-lookup"><span data-stu-id="2cfc9-141">Create Additional Sheets</span></span>](How-to-Create-Additional-Sheets.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]