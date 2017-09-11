---
title: "Применение операций в различных валютах | Документы Майкрософт"
description: "Операции книги можно применят в разных валютах, например, если вы продаете в одной валюте, а принимаете оплату в другой."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, payment, reconcile
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 035f4c0e98e3b7ba308319c2017568de832e26c5
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-enable-application-of-ledger-entries-in-different-currencies"></a><span data-ttu-id="d27c0-103">Практическое руководство. Включение операций книги в разных валютах</span><span class="sxs-lookup"><span data-stu-id="d27c0-103">How to: Enable Application of Ledger Entries in Different Currencies</span></span>
<span data-ttu-id="d27c0-104">В случае, если покупка у поставщика была произведена в одной валюте, а оплата проходит в другой валюте, то можно применить данную оплату к данной покупке.</span><span class="sxs-lookup"><span data-stu-id="d27c0-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span></span>

<span data-ttu-id="d27c0-105">Аналогично, если продажа клиенту осуществляется в одной валюте, а оплата от него поступает в другой валюте, оплату можно применить к счету продажи.</span><span class="sxs-lookup"><span data-stu-id="d27c0-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span></span>

<span data-ttu-id="d27c0-106">Далее описывается процедура настройки для операций книги поставщиков в окне **Настройка модуля "Покупки"**.</span><span class="sxs-lookup"><span data-stu-id="d27c0-106">The following procedure describes how to set this up for vendor ledger entries in the **Purchases & Payables Setup** window.</span></span> <span data-ttu-id="d27c0-107">Настройка аналогична для операций книги клиентов в **Настройка модуля "Продажи"**.</span><span class="sxs-lookup"><span data-stu-id="d27c0-107">The setup is similar for customer ledger entries in the **Sales & Receivables Setup** window.</span></span>

> [!NOTE]  
>   <span data-ttu-id="d27c0-108">Эта функция требует, чтобы было задано значение **Пакет**.</span><span class="sxs-lookup"><span data-stu-id="d27c0-108">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="d27c0-109">Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="d27c0-109">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a><span data-ttu-id="d27c0-110">Включение применения операций книги поставщиков в различных валютах</span><span class="sxs-lookup"><span data-stu-id="d27c0-110">To enable application of vendor ledger entries in different currencies</span></span>
1. <span data-ttu-id="d27c0-111">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Настройка модуля "Покупки"**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d27c0-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="d27c0-112">В поле **Применение между валютами** выберите один из следующих параметров.</span><span class="sxs-lookup"><span data-stu-id="d27c0-112">In the **Appln. between Currencies** field, select one of the following options.</span></span>

| <span data-ttu-id="d27c0-113">Параметр</span><span class="sxs-lookup"><span data-stu-id="d27c0-113">Option</span></span> | <span data-ttu-id="d27c0-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d27c0-114">Description</span></span> |
| --- | --- |
| <span data-ttu-id="d27c0-115">Нет</span><span class="sxs-lookup"><span data-stu-id="d27c0-115">None</span></span> |<span data-ttu-id="d27c0-116">Применение между валютами не разрешено.</span><span class="sxs-lookup"><span data-stu-id="d27c0-116">Application between currencies is not allowed.</span></span> |
| <span data-ttu-id="d27c0-117">Евро</span><span class="sxs-lookup"><span data-stu-id="d27c0-117">EMU</span></span> |<span data-ttu-id="d27c0-118">Разрешено применение для валют стран ЕС.</span><span class="sxs-lookup"><span data-stu-id="d27c0-118">Application between EMU currencies is allowed.</span></span> |
| <span data-ttu-id="d27c0-119">Все</span><span class="sxs-lookup"><span data-stu-id="d27c0-119">All</span></span> |<span data-ttu-id="d27c0-120">Разрешено применение для всех валют.</span><span class="sxs-lookup"><span data-stu-id="d27c0-120">Application between all currencies is allowed.</span></span> |

## <a name="see-also"></a><span data-ttu-id="d27c0-121">См. также</span><span class="sxs-lookup"><span data-stu-id="d27c0-121">See Also</span></span>
[<span data-ttu-id="d27c0-122">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="d27c0-122">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="d27c0-123">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="d27c0-123">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="d27c0-124">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d27c0-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

