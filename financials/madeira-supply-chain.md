---
title: "Функции цепочки поставок, поддерживаемые в Financials | Документы Майкрософт"
description: "Получите обзор продукта и узнайте об основных понятиях и процессах цепочки поставок, которые являются частью ERP-решения."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: product overview, ERP
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 3bae84075dc505aa9318590b1fac06e4844ffafe
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="overview-of-supply-chain-functionality"></a><span data-ttu-id="b2893-103">Обзор функций цепочки поставок</span><span class="sxs-lookup"><span data-stu-id="b2893-103">Overview of Supply Chain Functionality</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="b2893-104"> поддерживает общие процессы цепочки поставок, хотя и с ограничением по потребностями оптовых организаций и дистрибьюторов без управляемой обработки склада.</span><span class="sxs-lookup"><span data-stu-id="b2893-104"> supports common supply chain processes, although limited to the needs of wholesale and distribution companies without managed warehouse handling.</span></span>

<span data-ttu-id="b2893-105">В дополнение к документам счетов продажи можно управлять выполнением заказов с помощью заказов на продажу, что позволяет отгружать части количества по заказу, например вследствие того, что полное количество недоступно за раз.</span><span class="sxs-lookup"><span data-stu-id="b2893-105">In addition to sales invoice documents, you can manage your order fulfillment with sales orders allowing you to ship parts of an order quantity, for example, because the full quantity is not available at once.</span></span> <span data-ttu-id="b2893-106">Поставки товаров можно отгрузить напрямую от поставщика клиенту, связав заказ на продажу с соответствующим заказом на покупку.</span><span class="sxs-lookup"><span data-stu-id="b2893-106">You can have items drop shipped directly from a vendor to a customer by linking the sales order to the related purchase order.</span></span>

<span data-ttu-id="b2893-107">Количество запасов динамически обновляются по мере продажи и покупки товаров, и информация о наличии или предупреждения отображаются продавцам несколькими способами.</span><span class="sxs-lookup"><span data-stu-id="b2893-107">Your inventory quantities are dynamically updated as you sell and buy items, and availability information or warnings are shown to sales people in several ways.</span></span> <span data-ttu-id="b2893-108">Можно скорректировать количества запасов вручную, выполнив учет напрямую в операции книги товаров, например после инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="b2893-108">You can adjust inventory quantities manually by posting directly to the item ledger entries, for example, after a physical count.</span></span> <span data-ttu-id="b2893-109">Можно предлагать и продавать товары клиентам без ведения запасов по товару.</span><span class="sxs-lookup"><span data-stu-id="b2893-109">You can offer and sell items to your customers without maintaining inventory for them.</span></span> <span data-ttu-id="b2893-110">Если требуется включить такие нескладируемые товары в процесс цепочки поставок, достаточно преобразовать их в обычные товары.</span><span class="sxs-lookup"><span data-stu-id="b2893-110">If you want to include such nonstock items to your supply chain process, you simply convert them to normal items.</span></span>

<span data-ttu-id="b2893-111">В дополнение к документам счета покупки можно выполнять управление на стороне поставки с помощью заказов на покупку, что позволяет регистрировать частичные поступления количества по заказу.</span><span class="sxs-lookup"><span data-stu-id="b2893-111">In addition to purchase invoice documents, you can manage your supply side with purchase orders allowing you to record partial receipts of an order quantity.</span></span> <span data-ttu-id="b2893-112">Простая функция планирования поставок позволяет инициировать покупку непосредственно из счета на продажу, который требует товаров.</span><span class="sxs-lookup"><span data-stu-id="b2893-112">A simple supply planning function allows you to initiate a purchase directly from the sales invoice that requires the items.</span></span>

<span data-ttu-id="b2893-113">И документы продажи, и документы покупки можно учесть как отгруженные, полученные либо полученные с выставленным счетом, что позволяет разделить ответственность ролей обработчиков заказов и учета.</span><span class="sxs-lookup"><span data-stu-id="b2893-113">Both sales and purchase documents can be posted as shipped or received only or as shipped or received and invoiced, allowing you to split the responsibilities of order processors and accounting roles.</span></span>

<span data-ttu-id="b2893-114">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="b2893-114">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="b2893-115">Действие</span><span class="sxs-lookup"><span data-stu-id="b2893-115">To</span></span> | <span data-ttu-id="b2893-116">См.</span><span class="sxs-lookup"><span data-stu-id="b2893-116">See</span></span> |
| --- | --- |
| <span data-ttu-id="b2893-117">Зарегистрировать новых клиентов, сделать предложения по продажам, продать продукты в заказах или счетах, например как прямые поставки, а также управлять возвратами продаж.</span><span class="sxs-lookup"><span data-stu-id="b2893-117">Register new customers, make sales offers, sell products on orders or invoices, for example as drop shipments, and manage sales returns.</span></span> |[<span data-ttu-id="b2893-118">Продажи</span><span class="sxs-lookup"><span data-stu-id="b2893-118">Sales</span></span>](sales-manage-sales.md) |
| <span data-ttu-id="b2893-119">Зарегистрировать новых поставщиков, приобрести товары в заказах или счетах, например инициированные из счетов по продажам, и управлять возвратами покупок.</span><span class="sxs-lookup"><span data-stu-id="b2893-119">Register new vendors, purchase items on orders or invoices, for example initiated from a sales invoice, and manage purchase returns.</span></span> |[<span data-ttu-id="b2893-120">Покупки</span><span class="sxs-lookup"><span data-stu-id="b2893-120">Purchasing</span></span>](purchasing-manage-purchasing.md) |
| <span data-ttu-id="b2893-121">Зарегистрировать новые физические продукты или услуги, скорректировать количества запасов, а также управлять стоимостью запасов с помощью учета скорректированных себестоимостей в главной книге.</span><span class="sxs-lookup"><span data-stu-id="b2893-121">Register new physical or service products, adjust inventory quantities, and manage the inventory value by posting adjusted costs to the general ledger.</span></span> |[<span data-ttu-id="b2893-122">Запасы</span><span class="sxs-lookup"><span data-stu-id="b2893-122">Inventory</span></span>](inventory-manage-inventory.md) |

## <a name="see-also"></a><span data-ttu-id="b2893-123">См. также</span><span class="sxs-lookup"><span data-stu-id="b2893-123">See Also</span></span>
[<span data-ttu-id="b2893-124">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="b2893-124">Setting Up Sales</span></span>](sales-setup-sales.md)  
<span data-ttu-id="b2893-125">[Управление дебиторской задолженностью](receivables-manage-receivables.md)   </span><span class="sxs-lookup"><span data-stu-id="b2893-125">[Managing Receivables](receivables-manage-receivables.md)   </span></span>  
[<span data-ttu-id="b2893-126">Настройка покупки</span><span class="sxs-lookup"><span data-stu-id="b2893-126">Setting Up Purchasing</span></span>](purchasing-setup-purchasing.md)  
<span data-ttu-id="b2893-127">[Управление кредиторской задолженностью](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="b2893-127">[Managing Payables](payables-manage-payables.md)  </span></span>  
<span data-ttu-id="b2893-128">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b2893-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="b2893-129">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="b2893-129">General Business Functionality</span></span>](ui-across-business-areas.md)

