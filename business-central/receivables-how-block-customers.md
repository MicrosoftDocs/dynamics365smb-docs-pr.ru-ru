---
title: Как заблокировать продажи клиентам
description: При необходимости вы можете заблокировать включение клиента в документы продажи и другие операции продажи.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 720eb2d5899ba067dbcee8dc97492ebcd01b1abd
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3779180"
---
# <a name="block-customers"></a><span data-ttu-id="10828-103">Блокировка клиентов</span><span class="sxs-lookup"><span data-stu-id="10828-103">Block Customers</span></span>
<span data-ttu-id="10828-104">Можно заблокировать клиента, например из-за несостоятельности, чтобы этого клиента нельзя было добавить в документы продажи или чтобы никакие транзакции не могли быть учтены для клиента.</span><span class="sxs-lookup"><span data-stu-id="10828-104">You can block a customer, for example because of insolvency, so that the customer cannot be added to sales documents or so that no transactions can be posted for the customer.</span></span>

<span data-ttu-id="10828-105">Помимо блокировки клиента, можно задать, чтобы транзакции расчетов с покупателем для этого клиента были приостановлены в связи с напоминаниями.</span><span class="sxs-lookup"><span data-stu-id="10828-105">In addition to blocking a customer, you can set receivable transactions for the customer to be on hold in connection with reminders.</span></span> <span data-ttu-id="10828-106">Дополнительные сведения см. в разделе [Сбор непогашенных остатков задолженности](receivables-collect-outstanding-balances.md).</span><span class="sxs-lookup"><span data-stu-id="10828-106">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span></span>   

<span data-ttu-id="10828-107">В следующей таблице описаны разные варианты блокировки клиентов.</span><span class="sxs-lookup"><span data-stu-id="10828-107">The following table describes the options for blocking customers.</span></span>  

|<span data-ttu-id="10828-108">Параметр</span><span class="sxs-lookup"><span data-stu-id="10828-108">Option</span></span>|<span data-ttu-id="10828-109">Описание</span><span class="sxs-lookup"><span data-stu-id="10828-109">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="10828-110">**Пусто**</span><span class="sxs-lookup"><span data-stu-id="10828-110">**Blank**</span></span>|<span data-ttu-id="10828-111">Транзакции разрешены для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="10828-111">Transactions are allowed for this customer.</span></span>|
|<span data-ttu-id="10828-112">**Отгрузить**</span><span class="sxs-lookup"><span data-stu-id="10828-112">**Ship**</span></span>|<span data-ttu-id="10828-113">Для этого клиента не могут обрабатываться новые заказы и новые расходные накладные.</span><span class="sxs-lookup"><span data-stu-id="10828-113">New orders and new shipments cannot be created for this customer.</span></span> <span data-ttu-id="10828-114">Для существующих расходных накладных, по которым еще не выставлен счет, может быть выставлен счет.</span><span class="sxs-lookup"><span data-stu-id="10828-114">Existing shipments not yet invoiced can be invoiced.</span></span>|  
|<span data-ttu-id="10828-115">**Счет**</span><span class="sxs-lookup"><span data-stu-id="10828-115">**Invoice**</span></span>|<span data-ttu-id="10828-116">Для этого клиента не могут обрабатываться новые заказы, новые расходные накладные и новые счета.</span><span class="sxs-lookup"><span data-stu-id="10828-116">New orders, new shipments, and new invoices cannot be created for this customer.</span></span> <span data-ttu-id="10828-117">Для существующих расходных накладных, по которым еще не выставлен счет, не может быть выставлен счет.</span><span class="sxs-lookup"><span data-stu-id="10828-117">Existing shipments not yet invoiced cannot be invoiced.</span></span> <span data-ttu-id="10828-118">Вы по-прежнему можете отправлять клиентам напоминания и процент-ноты.</span><span class="sxs-lookup"><span data-stu-id="10828-118">You can still send reminders and finance charge memos to the customer.</span></span>|  
|<span data-ttu-id="10828-119">**Все**</span><span class="sxs-lookup"><span data-stu-id="10828-119">**All**</span></span>|<span data-ttu-id="10828-120">Для данного клиента не разрешены никакие транзакции, включая платежи.</span><span class="sxs-lookup"><span data-stu-id="10828-120">No transaction is allowed for this customer, including payments.</span></span>|  

## <a name="to-block-a-customer"></a><span data-ttu-id="10828-121">Для блокировки клиента</span><span class="sxs-lookup"><span data-stu-id="10828-121">To block a customer</span></span>  
1. <span data-ttu-id="10828-122">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиенты**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="10828-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="10828-123">Выберите клиента, затем выберите действие **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="10828-123">Select a customer, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="10828-124">в поле **Заблокировано** выберите, что блокировать, как описано в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="10828-124">In the **Blocked** field, choose what to block, as described in the table above.</span></span>

## <a name="see-also"></a><span data-ttu-id="10828-125">См. также</span><span class="sxs-lookup"><span data-stu-id="10828-125">See Also</span></span>  
[<span data-ttu-id="10828-126">Регистрация новых клиентов</span><span class="sxs-lookup"><span data-stu-id="10828-126">Register New Customers</span></span>](sales-how-register-new-customers.md)  
[<span data-ttu-id="10828-127">Сбор непогашенных остатков задолженности</span><span class="sxs-lookup"><span data-stu-id="10828-127">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="10828-128">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="10828-128">Managing Receivables</span></span>](receivables-manage-receivables.md)  
