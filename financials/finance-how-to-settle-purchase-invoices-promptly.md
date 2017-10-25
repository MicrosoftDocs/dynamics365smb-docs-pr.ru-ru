---
title: "Как немедленно создать документ \"Счет покупки\" | Документы Майкрософт"
description: "В случае потребности в оплате поставщику наличными или чеком, необходимый учет можно производить при учете самого счета."
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: ab72dbc70405323e5dcf7aafb1120f63bd15246c
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-settle-purchase-invoices-promptly"></a><span data-ttu-id="dea58-103">Как немедленно создать документ "Счет покупки"</span><span class="sxs-lookup"><span data-stu-id="dea58-103">How to: Settle Purchase Invoices Promptly</span></span>
<span data-ttu-id="dea58-104">В случае потребности в оплате поставщику наличными или чеком, платеж можно учесть при учете счета.</span><span class="sxs-lookup"><span data-stu-id="dea58-104">If you need to pay the vendor by cash or check, you can post the payment when you post the invoice.</span></span>  
  
### <a name="to-settle-purchase-invoices-promptly"></a><span data-ttu-id="dea58-105">Немедленное создание счетов покупки</span><span class="sxs-lookup"><span data-stu-id="dea58-105">To settle purchase invoices promptly</span></span>  
1. <span data-ttu-id="dea58-106">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Счета покупки**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="dea58-106">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="dea58-107">На вкладке **Главная** выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="dea58-107">On the **Home** tab, choose **New**.</span></span>  
3.  <span data-ttu-id="dea58-108">Для того чтобы произвести оплату наличными или с помощью банковского трансферта, следует ввести номер счета ГК или банковского счета в поле **Номер баланс. счета**.</span><span class="sxs-lookup"><span data-stu-id="dea58-108">To pay either in cash or by bank transfer, enter the number of the general ledger cash account or the bank account in the **Bal. Account No.** field.</span></span>  
  
> [!IMPORTANT]  
>  <span data-ttu-id="dea58-109">Поля **Тип баланс. счета** и **Номер баланс. счета** не включены в стандартную схему заголовка счета.</span><span class="sxs-lookup"><span data-stu-id="dea58-109">The **Bal. Account Type** and **Bal. Account No.** fields are not included in the standard layout of the invoice header.</span></span> <span data-ttu-id="dea58-110">Для того, чтобы произвести учет счета, сначала следует вставить эти поля с помощью проектных средств.</span><span class="sxs-lookup"><span data-stu-id="dea58-110">In order to post the payment of an invoice, you must first insert them with the design facilities.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="dea58-111">Если оплата счетов наличными производится часто, то можно рекомендовать установить специальный метод оплаты с использованием балансирующего счета и ввода этого метода в поле **Способ платежа** на карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="dea58-111">If you frequently pay purchase invoices in cash, it is a good idea to set up a specific payment method with a balancing account and enter this method in the **Payment Method** field on the vendor card.</span></span> <span data-ttu-id="dea58-112">Номер балансирующего счета вставляется автоматически в заголовок счета при создании нового счета.</span><span class="sxs-lookup"><span data-stu-id="dea58-112">The balancing account number is inserted automatically on the invoice header every time you create a new invoice.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="dea58-113">См. также</span><span class="sxs-lookup"><span data-stu-id="dea58-113">See Also</span></span>  
[<span data-ttu-id="dea58-114">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="dea58-114">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="dea58-115">Покупки</span><span class="sxs-lookup"><span data-stu-id="dea58-115">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="dea58-116">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="dea58-116">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
