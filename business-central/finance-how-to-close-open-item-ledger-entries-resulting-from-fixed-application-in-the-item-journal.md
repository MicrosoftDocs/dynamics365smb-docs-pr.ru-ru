---
title: 'Практическое руководство: закрытие открытых операций в книге товаров, появившихся в результате фиксированного применения в товарном журнале | Документация Майкрософт'
description: Используйте поле **Примен. из операции** на странице **Журнал товаров**, чтобы создать фиксированное применение между входящей транзакцией и исходной исходящей транзакцией. Например, для исправления исходящей транзакции или обработки ее возврата.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 7a7f31ea698a314d8a69c3bf9c2e7ab04ccd5f46
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3783453"
---
# <a name="close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a><span data-ttu-id="17e5b-104">Закрытие открытых операций в книге товаров, появившихся в результате фиксированного применения в товарном журнале</span><span class="sxs-lookup"><span data-stu-id="17e5b-104">Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal</span></span>
<span data-ttu-id="17e5b-105">Используйте поле **Примен. из операции** на странице **Журнал товаров**, чтобы создать фиксированное применение между входящей транзакцией и исходной исходящей транзакцией.</span><span class="sxs-lookup"><span data-stu-id="17e5b-105">You can use the **Applies-from Entry** field on the **Item Journal** page to create a fixed application between an inbound transaction and the original outbound transaction.</span></span> <span data-ttu-id="17e5b-106">Например, для исправления исходящей транзакции или обработки ее возврата.</span><span class="sxs-lookup"><span data-stu-id="17e5b-106">For example, to correct the outbound transaction or to process its return.</span></span> <span data-ttu-id="17e5b-107">Дополнительные сведения см. в поле "Примен. из операции".</span><span class="sxs-lookup"><span data-stu-id="17e5b-107">For more information, see Applies-from Entry.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="17e5b-108">Фиксированные применения, сделанные таким образом, применяют только себестоимость, а не количество.</span><span class="sxs-lookup"><span data-stu-id="17e5b-108">Fixed applications made in this manner only apply the cost, not the quantity.</span></span> <span data-ttu-id="17e5b-109">Соответственно, учтенная положительная операция из книги товаров не закроет примененной исходящей операции и сама останется открытой.</span><span class="sxs-lookup"><span data-stu-id="17e5b-109">Accordingly, the posted positive item ledger entry will not close the applied outbound entry and will itself remain open.</span></span> <span data-ttu-id="17e5b-110">Это также справедливо при учете фиксированного применения для положительной операции в негативной операции, которая не была закрыта обычной положительной операцией; в таком случае как положительная, так и отрицательная операции останутся открытыми.</span><span class="sxs-lookup"><span data-stu-id="17e5b-110">This also applies when you post a fixed application for a positive entry to a negative entry that has not been closed by a regular positive entry, then both the negative and the positive entries will remain open.</span></span>  
>   
>  <span data-ttu-id="17e5b-111">Это также означает, что невозможно закрыть период закрытия склада, если существует такая операция.</span><span class="sxs-lookup"><span data-stu-id="17e5b-111">This also means that you cannot close an inventory period if such an entry exists.</span></span>  

<span data-ttu-id="17e5b-112">Следующая процедура описывает закрытие таких операций посредством двух корректирующих учетов в журнале товаров.</span><span class="sxs-lookup"><span data-stu-id="17e5b-112">The following procedure shows how to close such entries by performing two corrective postings in the item journal.</span></span>  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a><span data-ttu-id="17e5b-113">Закрытие открытых операций в книге товаров, появившихся в результате фиксированного применения в товарном журнале</span><span class="sxs-lookup"><span data-stu-id="17e5b-113">To close open item ledger entries that result from a fixed application in the item journal</span></span>  

1.  <span data-ttu-id="17e5b-114">Используйте поле **Примен. из операции** для учета прихода с соответствующим количеством.</span><span class="sxs-lookup"><span data-stu-id="17e5b-114">Use the **Applies-from Entry** field to post a positive adjustment with the corresponding quantity.</span></span> <span data-ttu-id="17e5b-115">Это закрывает исходную отрицательную операцию с фиксированным применением.</span><span class="sxs-lookup"><span data-stu-id="17e5b-115">This closes the original negative entry with a fixed application.</span></span>  
2.  <span data-ttu-id="17e5b-116">Используйте поле **Примен. к операции** для учета расходов.</span><span class="sxs-lookup"><span data-stu-id="17e5b-116">Use the **Applies-to Entry** field to post a negative adjustment.</span></span> <span data-ttu-id="17e5b-117">Это закрывает исходную корректирующую положительную операцию с фиксированным применением.</span><span class="sxs-lookup"><span data-stu-id="17e5b-117">This closes the original corrective positive entry with a fixed application.</span></span>  

## <a name="see-also"></a><span data-ttu-id="17e5b-118">См. также</span><span class="sxs-lookup"><span data-stu-id="17e5b-118">See Also</span></span>  
[<span data-ttu-id="17e5b-119">Удаление и повторное применение операций журнала товаров</span><span class="sxs-lookup"><span data-stu-id="17e5b-119"> Remove and Reapply Item Ledger Entries</span></span>](finance-how-to-remove-and-reapply-item-entries.md)  
 <span data-ttu-id="17e5b-120">[Обработка возвратов и отмены продажи](sales-how-process-sales-returns-cancellations.md) </span><span class="sxs-lookup"><span data-stu-id="17e5b-120">[Process Sales Returns and Cancellations](sales-how-process-sales-returns-cancellations.md) </span></span>  
 <span data-ttu-id="17e5b-121">[Настройка оценки стоимости запасов и учета себестоимости](finance-set-up-inventory-valuation-and-costing.md) </span><span class="sxs-lookup"><span data-stu-id="17e5b-121">[Setting Up Inventory Valuation and Costing](finance-set-up-inventory-valuation-and-costing.md) </span></span>  
 <span data-ttu-id="17e5b-122">[Управление себестоимостью товаров](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="17e5b-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 [<span data-ttu-id="17e5b-123">Сведения о проектировании: методы учета себестоимости</span><span class="sxs-lookup"><span data-stu-id="17e5b-123">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)
