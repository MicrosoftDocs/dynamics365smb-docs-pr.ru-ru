---
title: Применение операций в различных валютах | Документация Майкрософт
description: Операции книги можно применят в разных валютах, например, если вы продаете в одной валюте, а принимаете оплату в другой.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, payment, reconcile
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: c11939306e56299347a5f80d9ccfbc35c22fe5aa
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3917030"
---
# <a name="enable-application-of-ledger-entries-in-different-currencies"></a><span data-ttu-id="3863b-103">Включение операций книги в разных валютах</span><span class="sxs-lookup"><span data-stu-id="3863b-103">Enable Application of Ledger Entries in Different Currencies</span></span>
<span data-ttu-id="3863b-104">В случае, если покупка у поставщика была произведена в одной валюте, а оплата проходит в другой валюте, то можно применить данную оплату к данной покупке.</span><span class="sxs-lookup"><span data-stu-id="3863b-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span></span>

<span data-ttu-id="3863b-105">Аналогично, если продажа клиенту осуществляется в одной валюте, а оплата от него поступает в другой валюте, оплату можно применить к счету продажи.</span><span class="sxs-lookup"><span data-stu-id="3863b-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span></span>

<span data-ttu-id="3863b-106">Далее описывается процедура настройки для операций книги поставщиков на странице **Настройка модуля "Покупки"**.</span><span class="sxs-lookup"><span data-stu-id="3863b-106">The following procedure describes how to set this up for vendor ledger entries on the **Purchases & Payables Setup** page.</span></span> <span data-ttu-id="3863b-107">Настройка аналогична для операций книги клиентов на странице **Настройка модуля "Продажи"**.</span><span class="sxs-lookup"><span data-stu-id="3863b-107">The setup is similar for customer ledger entries on the **Sales & Receivables Setup** page.</span></span>

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a><span data-ttu-id="3863b-108">Включение применения операций книги поставщиков в различных валютах</span><span class="sxs-lookup"><span data-stu-id="3863b-108">To enable application of vendor ledger entries in different currencies</span></span>
1. <span data-ttu-id="3863b-109">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Покупки и кредиторская задолженность"**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="3863b-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="3863b-110">В поле **Применение между валютами** выберите один из следующих параметров.</span><span class="sxs-lookup"><span data-stu-id="3863b-110">In the **Appln. between Currencies** field, select one of the following options.</span></span>

| <span data-ttu-id="3863b-111">Параметр</span><span class="sxs-lookup"><span data-stu-id="3863b-111">Option</span></span> | <span data-ttu-id="3863b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3863b-112">Description</span></span> |
| --- | --- |
| <span data-ttu-id="3863b-113">Нет</span><span class="sxs-lookup"><span data-stu-id="3863b-113">None</span></span> |<span data-ttu-id="3863b-114">Применение между валютами не разрешено.</span><span class="sxs-lookup"><span data-stu-id="3863b-114">Application between currencies is not allowed.</span></span> |
| <span data-ttu-id="3863b-115">Евро</span><span class="sxs-lookup"><span data-stu-id="3863b-115">EMU</span></span> |<span data-ttu-id="3863b-116">Разрешено применение для валют стран ЕС.</span><span class="sxs-lookup"><span data-stu-id="3863b-116">Application between EMU currencies is allowed.</span></span> |
| <span data-ttu-id="3863b-117">Все</span><span class="sxs-lookup"><span data-stu-id="3863b-117">All</span></span> |<span data-ttu-id="3863b-118">Разрешено применение для всех валют.</span><span class="sxs-lookup"><span data-stu-id="3863b-118">Application between all currencies is allowed.</span></span> |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a><span data-ttu-id="3863b-119">Настройка счетов ГК для разницы округления применения валюты</span><span class="sxs-lookup"><span data-stu-id="3863b-119">To set up G/L accounts for currency application rounding differences</span></span>  
<span data-ttu-id="3863b-120">При применении операций в различных валютах следует настроить счет ГК, по которому будет вестись учет разницы округления.</span><span class="sxs-lookup"><span data-stu-id="3863b-120">If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="3863b-121">Необходимо настроить счета ГК перед выполнением задачи.</span><span class="sxs-lookup"><span data-stu-id="3863b-121">You must set up the general ledger accounts before you complete the task.</span></span> <span data-ttu-id="3863b-122">Дополнительные сведения см. в разделе [Принципы работы с главной книгой и планом счетов](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="3863b-122">For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).</span></span>

1. <span data-ttu-id="3863b-123">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учетные группы клиента**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="3863b-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer Posting Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3863b-124">В полях **Деб. счет округл. при прим. валюты** и **Кр. счет округл. при прим. валюты** введите соответствующие счета ГК, чтобы учесть различия в округлении.</span><span class="sxs-lookup"><span data-stu-id="3863b-124">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  
3. <span data-ttu-id="3863b-125">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учетные группы поставщиков**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="3863b-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendor Posting Groups**, and then choose the related link.</span></span>  
4. <span data-ttu-id="3863b-126">В полях **Деб. счет округл. при прим. валюты** и **Кр. счет округл. при прим. валюты** введите соответствующие счета ГК, чтобы учесть различия в округлении.</span><span class="sxs-lookup"><span data-stu-id="3863b-126">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3863b-127">См. также</span><span class="sxs-lookup"><span data-stu-id="3863b-127">See Also</span></span>
[<span data-ttu-id="3863b-128">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="3863b-128">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="3863b-129">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="3863b-129">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="3863b-130">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3863b-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
