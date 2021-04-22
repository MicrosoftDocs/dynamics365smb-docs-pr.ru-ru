---
title: Закрытие записей в книге товаров, полученных при использовании фиксированного применения
description: Узнайте, как можно создать фиксированное применение между входящей транзакцией и исходной исходящей транзакцией в журнале товаров.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 4fac4871fdf42210dfd48ca6dd7d9c2fede0c7ef
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788287"
---
# <a name="close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a><span data-ttu-id="84029-103">Закрытие открытых операций в книге товаров, появившихся в результате фиксированного применения в товарном журнале</span><span class="sxs-lookup"><span data-stu-id="84029-103">Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal</span></span>

<span data-ttu-id="84029-104">Используйте поле **Примен. из операции** на странице **Журнал товаров**, чтобы создать фиксированное применение между входящей транзакцией и исходной исходящей транзакцией.</span><span class="sxs-lookup"><span data-stu-id="84029-104">You can use the **Applies-from Entry** field on the **Item Journal** page to create a fixed application between an inbound transaction and the original outbound transaction.</span></span> <span data-ttu-id="84029-105">Например, для исправления исходящей транзакции или обработки ее возврата.</span><span class="sxs-lookup"><span data-stu-id="84029-105">For example, to correct the outbound transaction or to process its return.</span></span>  

> [!IMPORTANT]  
> <span data-ttu-id="84029-106">Фиксированные применения, сделанные таким образом, применяют только себестоимость, а не количество.</span><span class="sxs-lookup"><span data-stu-id="84029-106">Fixed applications made in this manner only apply the cost, not the quantity.</span></span> <span data-ttu-id="84029-107">Соответственно, учтенная положительная операция из книги товаров не закроет примененной исходящей операции и сама останется открытой.</span><span class="sxs-lookup"><span data-stu-id="84029-107">Accordingly, the posted positive item ledger entry will not close the applied outbound entry and will itself remain open.</span></span> <span data-ttu-id="84029-108">Это также справедливо при учете фиксированного применения для положительной операции в негативной операции, которая не была закрыта обычной положительной операцией; в таком случае как положительная, так и отрицательная операции останутся открытыми.</span><span class="sxs-lookup"><span data-stu-id="84029-108">This also applies when you post a fixed application for a positive entry to a negative entry that has not been closed by a regular positive entry, then both the negative and the positive entries will remain open.</span></span>  
>
> <span data-ttu-id="84029-109">Это также означает, что невозможно закрыть период закрытия склада, если существует такая операция.</span><span class="sxs-lookup"><span data-stu-id="84029-109">This also means that you cannot close an inventory period if such an entry exists.</span></span>  

<span data-ttu-id="84029-110">Можно изменить и повторно применить операции применения при определенных условиях с помощью страницы **Лист применения**.</span><span class="sxs-lookup"><span data-stu-id="84029-110">You can change and reapply application entries under certain conditions by using the **Application Worksheet** page.</span></span>  

<span data-ttu-id="84029-111">Следующая процедура описывает закрытие таких операций посредством двух корректирующих учетов в журнале товаров.</span><span class="sxs-lookup"><span data-stu-id="84029-111">The following procedure shows how to close such entries by performing two corrective postings in the item journal.</span></span>  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a><span data-ttu-id="84029-112">Закрытие открытых операций в книге товаров, появившихся в результате фиксированного применения в товарном журнале</span><span class="sxs-lookup"><span data-stu-id="84029-112">To close open item ledger entries that result from a fixed application in the item journal</span></span>  

1. <span data-ttu-id="84029-113">Используйте поле **Примен. из операции** для учета прихода с соответствующим количеством.</span><span class="sxs-lookup"><span data-stu-id="84029-113">Use the **Applies-from Entry** field to post a positive adjustment with the corresponding quantity.</span></span> <span data-ttu-id="84029-114">Это закрывает исходную отрицательную операцию с фиксированным применением.</span><span class="sxs-lookup"><span data-stu-id="84029-114">This closes the original negative entry with a fixed application.</span></span>  

    <span data-ttu-id="84029-115">Поле **Примен. из операции** указывает номер исходящей учтенной товарной операции, себестоимость которой передается во входящую учтенную товарную операцию при учете входящей транзакции типа **Приход** или **Покупка** с помощью журнала товаров.</span><span class="sxs-lookup"><span data-stu-id="84029-115">The **Applies-from Entry** field specifies the number of the outbound item ledger entry whose cost is forwarded to the inbound item ledger entry when you post an inbound transaction of type **Positive Adjmt.** or **Purchase** with the item journal.</span></span>  
2. <span data-ttu-id="84029-116">Используйте поле **Примен. к операции** для учета расходов.</span><span class="sxs-lookup"><span data-stu-id="84029-116">Use the **Applies-to Entry** field to post a negative adjustment.</span></span> <span data-ttu-id="84029-117">Это закрывает исходную корректирующую положительную операцию с фиксированным применением.</span><span class="sxs-lookup"><span data-stu-id="84029-117">This closes the original corrective positive entry with a fixed application.</span></span>  

    <span data-ttu-id="84029-118">Поле **Примен. к операции** определяет, должно ли количество в строке журнала товаров применяться к уже учтенному документу.</span><span class="sxs-lookup"><span data-stu-id="84029-118">The **Applies-to Entry** field specifies if the quantity in the item journal line should be applied to an already-posted document.</span></span> <span data-ttu-id="84029-119">Если это имеет место, то введите номер учтенной товарной операции, к которой должна применяться строка журнала товаров.</span><span class="sxs-lookup"><span data-stu-id="84029-119">If this is the case, enter the entry number of the item ledger entry to which the item journal line should be applied.</span></span>

## <a name="see-also"></a><span data-ttu-id="84029-120">См. также</span><span class="sxs-lookup"><span data-stu-id="84029-120">See Also</span></span>

[<span data-ttu-id="84029-121">Удаление и повторное применение операций журнала товаров</span><span class="sxs-lookup"><span data-stu-id="84029-121">Remove and Reapply Item Ledger Entries</span></span>](finance-how-to-remove-and-reapply-item-entries.md)  
[<span data-ttu-id="84029-122">Обработка возвратов и отмены продажи</span><span class="sxs-lookup"><span data-stu-id="84029-122">Process Sales Returns and Cancellations</span></span>](sales-how-process-sales-returns-cancellations.md)  
[<span data-ttu-id="84029-123">Настройка оценки стоимости запасов и учета себестоимости</span><span class="sxs-lookup"><span data-stu-id="84029-123">Setting Up Inventory Valuation and Costing</span></span>](finance-set-up-inventory-valuation-and-costing.md)  
[<span data-ttu-id="84029-124">Управление себестоимостью товаров</span><span class="sxs-lookup"><span data-stu-id="84029-124">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="84029-125">Сведения о проектировании: методы учета себестоимости</span><span class="sxs-lookup"><span data-stu-id="84029-125">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]