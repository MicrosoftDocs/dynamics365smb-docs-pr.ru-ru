---
title: Регистрация НДС по заказам на покупку в России
description: Российские усовершенствования включают поддержку НДС в заказах на покупку.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 1e2a723eb2b2522a56589c70db9e4aa5b7274fd0
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738261"
---
# <a name="how-to-register-vat-on-purchase-orders"></a><span data-ttu-id="7ecea-103">Практическое руководство. Регистрация НДС по заказам на покупку</span><span class="sxs-lookup"><span data-stu-id="7ecea-103">How to: Register VAT on Purchase Orders</span></span>

<span data-ttu-id="7ecea-104">В России организации должны вести журнал НДС по входящим и исходящим счетам.</span><span class="sxs-lookup"><span data-stu-id="7ecea-104">In Russia, organizations are required to keep a journal of received and issued VAT invoices.</span></span> [!INCLUDE[prodshort](../../includes/prodshort.md)] <span data-ttu-id="7ecea-105">позволяет регистрировать НДС по заказам на покупку, чтобы эта информация отслеживалась в журнале счетов НДС.</span><span class="sxs-lookup"><span data-stu-id="7ecea-105">enables you to register VAT on purchase orders so that the information is tracked in the VAT invoices journal.</span></span>

## <a name="to-register-vat-on-a-purchase-order"></a><span data-ttu-id="7ecea-106">Регистрация НДС по заказам на покупку</span><span class="sxs-lookup"><span data-stu-id="7ecea-106">To register VAT on a purchase order</span></span>

1. <span data-ttu-id="7ecea-107">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказ на покупку**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="7ecea-107">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Order**, and then choose the related link.</span></span> <span data-ttu-id="7ecea-108">Выберите соответствующий заказ на покупку.</span><span class="sxs-lookup"><span data-stu-id="7ecea-108">Select the relevant purchase order.</span></span>

2. <span data-ttu-id="7ecea-109">На экспресс-вкладке **Отгрузка** заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="7ecea-109">On the **Shipping** FastTab, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="7ecea-110">Поле</span><span class="sxs-lookup"><span data-stu-id="7ecea-110">Field</span></span>                    | <span data-ttu-id="7ecea-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7ecea-111">Description</span></span>                                              |
   | :----------------------- | :------------------------------------------------------- |
   | <span data-ttu-id="7ecea-112">**Номер накладной поставщика**</span><span class="sxs-lookup"><span data-stu-id="7ecea-112">**Vendor Receipts No.**</span></span>  | <span data-ttu-id="7ecea-113">Введите идентификационный номер из накладной поставщика.</span><span class="sxs-lookup"><span data-stu-id="7ecea-113">Enter the identification number from the vendor receipt.</span></span> |
   | <span data-ttu-id="7ecea-114">**Дата накладной поставщика**</span><span class="sxs-lookup"><span data-stu-id="7ecea-114">**Vendor Receipts Date**</span></span> | <span data-ttu-id="7ecea-115">Введите дату из накладной поставщика.</span><span class="sxs-lookup"><span data-stu-id="7ecea-115">Enter the date from the vendor receipt.</span></span>                  |

3. <span data-ttu-id="7ecea-116">На экспресс-вкладке **НДС** заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="7ecea-116">On the **VAT** FastTab, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="7ecea-117">Поле</span><span class="sxs-lookup"><span data-stu-id="7ecea-117">Field</span></span>                            | <span data-ttu-id="7ecea-118">Описание</span><span class="sxs-lookup"><span data-stu-id="7ecea-118">Description</span></span>                                                 |
   | :------------------------------- | :---------------------------------------------------------- |
   | <span data-ttu-id="7ecea-119">**Счет-Фактура Но.**</span><span class="sxs-lookup"><span data-stu-id="7ecea-119">**Vendor VAT Invoice No.**</span></span>       | <span data-ttu-id="7ecea-120">Введите номер счета из исходной транзакции НДС.</span><span class="sxs-lookup"><span data-stu-id="7ecea-120">Enter the invoice number from the original VAT transaction.</span></span> |
   | <span data-ttu-id="7ecea-121">**Дата счета-фактуры поставщика**</span><span class="sxs-lookup"><span data-stu-id="7ecea-121">**Vendor VAT Invoice Date**</span></span>      | <span data-ttu-id="7ecea-122">Введите дату счета из исходной транзакции НДС.</span><span class="sxs-lookup"><span data-stu-id="7ecea-122">Enter the invoice date from the original VAT transaction.</span></span>   |
   | <span data-ttu-id="7ecea-123">**Дата получения счета-фактуры поставщика**</span><span class="sxs-lookup"><span data-stu-id="7ecea-123">**Vendor VAT Invoice Rcvd Date**</span></span> | <span data-ttu-id="7ecea-124">Введите дату получения покупки.</span><span class="sxs-lookup"><span data-stu-id="7ecea-124">Enter the date that the purchase was received.</span></span>              |

   <span data-ttu-id="7ecea-125">Транзакция НДС теперь зарегистрирована и будет отслеживаться в журнале счетов НДС после учета заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="7ecea-125">The VAT transaction is now registered and will be tracked in the VAT invoices journal after the purchase order is posted.</span></span>

## <a name="see-also"></a><span data-ttu-id="7ecea-126">См. также</span><span class="sxs-lookup"><span data-stu-id="7ecea-126">See Also</span></span>

[<span data-ttu-id="7ecea-127">Практическое руководство. Настройка книг НДС</span><span class="sxs-lookup"><span data-stu-id="7ecea-127">How to: Set Up VAT Ledgers</span></span>](How-to-Set-Up-VAT-Ledgers.md)  
[<span data-ttu-id="7ecea-128">Практическое руководство. Подготовка операций НДС к учету</span><span class="sxs-lookup"><span data-stu-id="7ecea-128">How to: Prepare VAT Entries for Posting</span></span>](How-to-Prepare-VAT-Entries-for-Posting.md)  
[<span data-ttu-id="7ecea-129">Практическое руководство. Подача отчета об НДС в налоговые органы</span><span class="sxs-lookup"><span data-stu-id="7ecea-129">How to: Report VAT to Tax Authorities</span></span>](../../finance-how-report-vat.md)  
