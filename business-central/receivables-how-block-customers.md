---
title: Блокировка продаж клиентам товаров из продаж или покупок
description: В Business Central товар можно пометить как заблокированный для продажи, покупки или всех целей.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: c1b055e5101b99f0b0e1b69169d5c9f2f7e21d09
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2882998"
---
# <a name="block-customers"></a><span data-ttu-id="7d1dc-103">Блокировка клиентов</span><span class="sxs-lookup"><span data-stu-id="7d1dc-103">Block Customers</span></span>
<span data-ttu-id="7d1dc-104">Можно заблокировать клиента, например из-за несостоятельности, чтобы этого клиента нельзя было добавить в документы продажи или чтобы никакие транзакции не могли быть учтены для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-104">You can block a customer, for example because of insolvency, so that the customer cannot be added to sales documents or so that no transactions can be posted for the customer.</span></span>

<span data-ttu-id="7d1dc-105">Помимо блокировки клиента, можно задать, чтобы транзакции расчетов с покупателем для этого клиента были приостановлены в связи с напоминаниями.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-105">In addition to blocking a customer, you can set receivable transactions for the customer to be on hold in connection with reminders.</span></span> <span data-ttu-id="7d1dc-106">Дополнительные сведения см. в разделе [Сбор непогашенных остатков задолженности](receivables-collect-outstanding-balances.md).</span><span class="sxs-lookup"><span data-stu-id="7d1dc-106">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span></span>   

<span data-ttu-id="7d1dc-107">В следующей таблице описаны разные параметры блокировки.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-107">The following table describes the different blocking options.</span></span>  

|<span data-ttu-id="7d1dc-108">Параметр</span><span class="sxs-lookup"><span data-stu-id="7d1dc-108">Option</span></span>|<span data-ttu-id="7d1dc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7d1dc-109">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="7d1dc-110">**Пусто**</span><span class="sxs-lookup"><span data-stu-id="7d1dc-110">**Blank**</span></span>|<span data-ttu-id="7d1dc-111">Транзакции разрешены для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-111">Transactions are allowed for this customer.</span></span>|
|<span data-ttu-id="7d1dc-112">**Отгрузить**</span><span class="sxs-lookup"><span data-stu-id="7d1dc-112">**Ship**</span></span>|<span data-ttu-id="7d1dc-113">Для этого клиента не могут обрабатываться новые заказы и новые расходные накладные.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-113">New orders and new shipments cannot be created for this customer.</span></span> <span data-ttu-id="7d1dc-114">Для существующих расходных накладных, по которым еще не выставлен счет, может быть выставлен счет.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-114">Existing shipments not yet invoiced can be invoiced.</span></span>|  
|<span data-ttu-id="7d1dc-115">**Счет**</span><span class="sxs-lookup"><span data-stu-id="7d1dc-115">**Invoice**</span></span>|<span data-ttu-id="7d1dc-116">Для этого клиента не могут обрабатываться новые заказы, новые расходные накладные и новые счета.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-116">New orders, new shipments, and new invoices cannot be created for this customer.</span></span> <span data-ttu-id="7d1dc-117">Для существующих расходных накладных, по которым еще не выставлен счет, не может быть выставлен счет.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-117">Existing shipments not yet invoiced cannot be invoiced.</span></span>|  
|<span data-ttu-id="7d1dc-118">**Все**</span><span class="sxs-lookup"><span data-stu-id="7d1dc-118">**All**</span></span>|<span data-ttu-id="7d1dc-119">Для данного клиента не разрешены никакие транзакции, включая платежи.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-119">No transaction is allowed for this customer, including payments.</span></span>|  

## <a name="to-block-a-customer"></a><span data-ttu-id="7d1dc-120">Для блокировки клиента</span><span class="sxs-lookup"><span data-stu-id="7d1dc-120">To block a customer</span></span>  
1. <span data-ttu-id="7d1dc-121">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиенты**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="7d1dc-122">Выберите клиента, затем выберите действие **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-122">Select a customer, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="7d1dc-123">Заполните поле **Заблокирован** с помощью одного из параметров, описываемых выше.</span><span class="sxs-lookup"><span data-stu-id="7d1dc-123">Fill in the **Blocked** field with one of the options described above.</span></span>

## <a name="see-also"></a><span data-ttu-id="7d1dc-124">См. также</span><span class="sxs-lookup"><span data-stu-id="7d1dc-124">See Also</span></span>  
[<span data-ttu-id="7d1dc-125">Регистрация новых клиентов</span><span class="sxs-lookup"><span data-stu-id="7d1dc-125">Register New Customers</span></span>](sales-how-register-new-customers.md)  
[<span data-ttu-id="7d1dc-126">Сбор непогашенных остатков задолженности</span><span class="sxs-lookup"><span data-stu-id="7d1dc-126">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="7d1dc-127">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="7d1dc-127">Managing Receivables</span></span>](receivables-manage-receivables.md)  
