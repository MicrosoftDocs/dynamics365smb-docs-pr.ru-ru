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
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 6379aea58ab7943b117e5b19b22f71193290c2cb
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-enable-application-of-ledger-entries-in-different-currencies"></a><span data-ttu-id="7003c-103">Практическое руководство. Включение операций книги в разных валютах</span><span class="sxs-lookup"><span data-stu-id="7003c-103">How to: Enable Application of Ledger Entries in Different Currencies</span></span>
<span data-ttu-id="7003c-104">В случае, если покупка у поставщика была произведена в одной валюте, а оплата проходит в другой валюте, то можно применить данную оплату к данной покупке.</span><span class="sxs-lookup"><span data-stu-id="7003c-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span></span>

<span data-ttu-id="7003c-105">Аналогично, если продажа клиенту осуществляется в одной валюте, а оплата от него поступает в другой валюте, оплату можно применить к счету продажи.</span><span class="sxs-lookup"><span data-stu-id="7003c-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span></span>

<span data-ttu-id="7003c-106">Далее описывается процедура настройки для операций книги поставщиков в окне **Настройка модуля "Покупки"**.</span><span class="sxs-lookup"><span data-stu-id="7003c-106">The following procedure describes how to set this up for vendor ledger entries in the **Purchases & Payables Setup** window.</span></span> <span data-ttu-id="7003c-107">Настройка аналогична для операций книги клиентов в **Настройка модуля "Продажи"**.</span><span class="sxs-lookup"><span data-stu-id="7003c-107">The setup is similar for customer ledger entries in the **Sales & Receivables Setup** window.</span></span>

> [!NOTE]  
>   <span data-ttu-id="7003c-108">Эта функция требует, чтобы было задано значение **Suite**.</span><span class="sxs-lookup"><span data-stu-id="7003c-108">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="7003c-109">Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="7003c-109">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a><span data-ttu-id="7003c-110">Включение применения операций книги поставщиков в различных валютах</span><span class="sxs-lookup"><span data-stu-id="7003c-110">To enable application of vendor ledger entries in different currencies</span></span>
1. <span data-ttu-id="7003c-111">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Настройка модуля "Покупки"**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="7003c-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="7003c-112">В поле **Применение между валютами** выберите один из следующих параметров.</span><span class="sxs-lookup"><span data-stu-id="7003c-112">In the **Appln. between Currencies** field, select one of the following options.</span></span>

| <span data-ttu-id="7003c-113">Параметр</span><span class="sxs-lookup"><span data-stu-id="7003c-113">Option</span></span> | <span data-ttu-id="7003c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="7003c-114">Description</span></span> |
| --- | --- |
| <span data-ttu-id="7003c-115">Нет</span><span class="sxs-lookup"><span data-stu-id="7003c-115">None</span></span> |<span data-ttu-id="7003c-116">Применение между валютами не разрешено.</span><span class="sxs-lookup"><span data-stu-id="7003c-116">Application between currencies is not allowed.</span></span> |
| <span data-ttu-id="7003c-117">Евро</span><span class="sxs-lookup"><span data-stu-id="7003c-117">EMU</span></span> |<span data-ttu-id="7003c-118">Разрешено применение для валют стран ЕС.</span><span class="sxs-lookup"><span data-stu-id="7003c-118">Application between EMU currencies is allowed.</span></span> |
| <span data-ttu-id="7003c-119">Все</span><span class="sxs-lookup"><span data-stu-id="7003c-119">All</span></span> |<span data-ttu-id="7003c-120">Разрешено применение для всех валют.</span><span class="sxs-lookup"><span data-stu-id="7003c-120">Application between all currencies is allowed.</span></span> |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a><span data-ttu-id="7003c-121">Настройка счетов ГК для разницы округления применения валюты</span><span class="sxs-lookup"><span data-stu-id="7003c-121">To set up G/L accounts for currency application rounding differences</span></span>  
<span data-ttu-id="7003c-122">При применении операций в различных валютах следует настроить счет ГК, по которому будет вестись учет разницы округления.</span><span class="sxs-lookup"><span data-stu-id="7003c-122">If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="7003c-123">Необходимо настроить счета ГК перед выполнением задачи.</span><span class="sxs-lookup"><span data-stu-id="7003c-123">You must set up the general ledger accounts before you complete the task.</span></span> <span data-ttu-id="7003c-124">Дополнительные сведения см. в разделе [Принципы работы с главной книгой и планом счетов](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="7003c-124">For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).</span></span> 
  
1. <span data-ttu-id="7003c-125">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Учетные группы клиента**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="7003c-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer Posting Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="7003c-126">В полях **Деб. счет округл. при прим. валюты** и **Кр. счет округл. при прим. валюты** введите соответствующие счета ГК, чтобы учесть различия в округлении.</span><span class="sxs-lookup"><span data-stu-id="7003c-126">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  
3. <span data-ttu-id="7003c-127">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Учетные группы поставщика**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="7003c-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Posting Groups**, and then choose the related link.</span></span>  
4. <span data-ttu-id="7003c-128">В полях **Деб. счет округл. при прим. валюты** и **Кр. счет округл. при прим. валюты** введите соответствующие счета ГК, чтобы учесть различия в округлении.</span><span class="sxs-lookup"><span data-stu-id="7003c-128">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7003c-129">См. также</span><span class="sxs-lookup"><span data-stu-id="7003c-129">See Also</span></span>
[<span data-ttu-id="7003c-130">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="7003c-130">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="7003c-131">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="7003c-131">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="7003c-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7003c-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

