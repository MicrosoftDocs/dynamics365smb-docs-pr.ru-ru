---
title: Учет документов продаж | Документы Майкрософт
description: Узнайте о различных функциях учета для учета торговых документов, а также о том, как можно обновлять учтенные документы.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 01e831ddddeffe6a64c6de24b4cd8c1b94bad9c3
ms.sourcegitcommit: a88d1e9c0ab647cb8d9d81d32c0bdc82843f4145
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "1796899"
---
# <a name="posting-sales"></a><span data-ttu-id="b1037-103">Учет продаж</span><span class="sxs-lookup"><span data-stu-id="b1037-103">Posting Sales</span></span>
<span data-ttu-id="b1037-104">В разделе **Учетная группа** в документе продажи можно выбирать следующие функции учета:</span><span class="sxs-lookup"><span data-stu-id="b1037-104">In the **Posting group** on a sales document, you can choose between the following posting functions:</span></span>

* <span data-ttu-id="b1037-105">**Учесть**</span><span class="sxs-lookup"><span data-stu-id="b1037-105">**Post**</span></span>
* <span data-ttu-id="b1037-106">**Тестовый отчет**</span><span class="sxs-lookup"><span data-stu-id="b1037-106">**Test Report**</span></span>
* <span data-ttu-id="b1037-107">**Учесть и отправить**</span><span class="sxs-lookup"><span data-stu-id="b1037-107">**Post and Send**</span></span>
* <span data-ttu-id="b1037-108">**Учет и печать**</span><span class="sxs-lookup"><span data-stu-id="b1037-108">**Post and Print**</span></span>
* <span data-ttu-id="b1037-109">**Учесть и отправить по эл. почте**</span><span class="sxs-lookup"><span data-stu-id="b1037-109">**Post and Email**</span></span>
* <span data-ttu-id="b1037-110">**Пакетный учет**</span><span class="sxs-lookup"><span data-stu-id="b1037-110">**Post Batch**</span></span>
* <span data-ttu-id="b1037-111">**Предварительный просмотр учета**</span><span class="sxs-lookup"><span data-stu-id="b1037-111">**Preview Posting**</span></span>

<span data-ttu-id="b1037-112">После заполнения всех строк и ввода всей информации в заказ на продажу его можно учесть.</span><span class="sxs-lookup"><span data-stu-id="b1037-112">When you have completed all the lines and entered all the information on the sales order, you can post it.</span></span> <span data-ttu-id="b1037-113">Это создает отгрузку и счет.</span><span class="sxs-lookup"><span data-stu-id="b1037-113">This creates a shipment and an invoice.</span></span>

<span data-ttu-id="b1037-114">Когда учитывается заказ на продажу, обновляются счет клиента, главная книга и записи книги операций по товарам.</span><span class="sxs-lookup"><span data-stu-id="b1037-114">When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.</span></span>

<span data-ttu-id="b1037-115">По каждому заказу на продажу в таблице **Операция ГК** создается операция продажи.</span><span class="sxs-lookup"><span data-stu-id="b1037-115">For each sales order, a sales entry is created in the **G/L Entry** table.</span></span> <span data-ttu-id="b1037-116">Операция создается также в счете клиента в таблице **Книга операций клиентов**, а операция ГК создается в соответствующем счете дебеторской задолженности.</span><span class="sxs-lookup"><span data-stu-id="b1037-116">An entry is also created in the customer's account in the **Cust. Ledger Entry** table and a general ledger entry is created in the relevant receivables account.</span></span> <span data-ttu-id="b1037-117">Кроме этого, в результате учета заказа может быть создана операция НДС и операция Главной книги по сумме скидки.</span><span class="sxs-lookup"><span data-stu-id="b1037-117">In addition, posting the order may result in a VAT entry and a general ledger entry for the discount amount.</span></span> <span data-ttu-id="b1037-118">Учет операции по скидке зависит от содержимого поля **Учет скидки** на странице **Настройка модуля продажи**.</span><span class="sxs-lookup"><span data-stu-id="b1037-118">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field on the **Sales & Receivables Setup** page.</span></span>

<span data-ttu-id="b1037-119">Для каждой строки заказа на продажу будет создаваться операция книги товаров в таблице **Книга операций по товарам** (если строки продажи содержат номера товаров) или операция ГК в таблице **Операция ГК** (если строки продажи содержат счет ГК).</span><span class="sxs-lookup"><span data-stu-id="b1037-119">For each sales order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the sales lines contain item numbers) or a general ledger entry will be created in the **G/L Entry** table (if the sales lines contain a general ledger account).</span></span> <span data-ttu-id="b1037-120">В дополнение к этому заказы продажи всегда записываются в таблицах **«Расх. накладная - заголовок»** и **Заголовок счета продаж**.</span><span class="sxs-lookup"><span data-stu-id="b1037-120">In addition to this, sales orders are always recorded in the **Sales Shipment Header** and **Sales Invoice Header** tables.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="b1037-121">При учете заказа можно создавать, как расходную накладную, так и счет.</span><span class="sxs-lookup"><span data-stu-id="b1037-121">When you post an order, you can create both a shipment and an invoice.</span></span> <span data-ttu-id="b1037-122">Их можно выполнять одновременно и независимо друг от друга.</span><span class="sxs-lookup"><span data-stu-id="b1037-122">These can be done at the same time or independently.</span></span> <span data-ttu-id="b1037-123">Можно создавать частичную расходную накладную и частичный счет, заполнив поля **Кол-во для отгрузки** и **Кол-во для выставления счета** в строках отдельных заказов на продажу перед учетом.</span><span class="sxs-lookup"><span data-stu-id="b1037-123">You can also create a partial shipment and a partial invoice by completing the **Qty. to Ship** and **Qty. to Invoice** fields on the individual sales order lines before you post.</span></span> <span data-ttu-id="b1037-124">Следует отметить, что невозможно создавать счет по тому, что еще не отгружено.</span><span class="sxs-lookup"><span data-stu-id="b1037-124">Note that you cannot create an invoice for something that is not shipped.</span></span> <span data-ttu-id="b1037-125">Т.е. прежде, чем выставлять счет, следует зарегистрировать расходную накладную или следует выбрать одновременное выполнение отгрузки и выставления счета.</span><span class="sxs-lookup"><span data-stu-id="b1037-125">That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.</span></span>

<span data-ttu-id="b1037-126">Если учет завершен, учтенные строки продажи удаляются из заказа.</span><span class="sxs-lookup"><span data-stu-id="b1037-126">When the posting is completed, the posted sales lines are removed from the order.</span></span> <span data-ttu-id="b1037-127">При завершении учета появляется соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="b1037-127">A message tells you when the posting is completed.</span></span> <span data-ttu-id="b1037-128">После этого появится возможность просмотра учтенных операций на различных страницах, содержащих учтенные операции, в том числе на страницах **Книга операций по клиентам**, **Операции ГК**, **Книга операций по товарам**, **Учтенные расх. накладные продажи** и **Учтенные счета продажи**.</span><span class="sxs-lookup"><span data-stu-id="b1037-128">After this, you will be able to see the posted entries in the various pages that contain posted entries, such as the **Cust. Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Posted Sales Shipments**, and **Posted Sales Invoices** pages.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b1037-129">См. также</span><span class="sxs-lookup"><span data-stu-id="b1037-129">See Also</span></span>

[<span data-ttu-id="b1037-130">Продажи</span><span class="sxs-lookup"><span data-stu-id="b1037-130">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="b1037-131">Отправка документов по электронной почте</span><span class="sxs-lookup"><span data-stu-id="b1037-131">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
[<span data-ttu-id="b1037-132">Исправление или отмена неоплаченных счетов продажи</span><span class="sxs-lookup"><span data-stu-id="b1037-132">Correct or Cancel Unpaid Sales Invoices</span></span>](sales-how-correct-cancel-sales-invoice.md)  
[<span data-ttu-id="b1037-133">Использование функции "Что вы хотите сделать" для поиска функций и информации</span><span class="sxs-lookup"><span data-stu-id="b1037-133">Using Tell Me to Find Features and Information</span></span>](ui-search.md)  
<span data-ttu-id="b1037-134">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b1037-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
