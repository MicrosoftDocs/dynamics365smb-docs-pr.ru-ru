---
title: "Практическое руководство. Настройка клиентов, оплачивающих наличными | Документы Майкрософт"
description: "В этом разделе описываются шаги для настройки клиента, который осуществляет оплату наличными."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/11/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 93c28879417b12bc142c84c38c054828b380cc53
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-cash-customers"></a><span data-ttu-id="b1bd4-103">Настройка клиентов, оплачивающих наличными</span><span class="sxs-lookup"><span data-stu-id="b1bd4-103">Set Up Cash Customers</span></span>
<span data-ttu-id="b1bd4-104">Счет не может быть создан без номера клиента.</span><span class="sxs-lookup"><span data-stu-id="b1bd4-104">You cannot create an invoice without a customer number.</span></span> <span data-ttu-id="b1bd4-105">Это правило выполняется даже тогда, когда выполняется продажа с наличным расчетом, и по счету клиента записи не производятся.</span><span class="sxs-lookup"><span data-stu-id="b1bd4-105">This is true, even if you make a cash sale and do not have anything to record in a customer account.</span></span>  

## <a name="to-set-up-a-cash-customer"></a><span data-ttu-id="b1bd4-106">Настройка клиента, оплачивающего наличными</span><span class="sxs-lookup"><span data-stu-id="b1bd4-106">To set up a cash customer</span></span>  
1.  <span data-ttu-id="b1bd4-107">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Клиент**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="b1bd4-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b1bd4-108">Создайте новую **Карточку клиента**.</span><span class="sxs-lookup"><span data-stu-id="b1bd4-108">Create a new **Customer** card.</span></span> <span data-ttu-id="b1bd4-109">Дополнительные сведения см. в разделе [Регистрация новых клиентов](sales-how-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="b1bd4-109">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span></span>
3.  <span data-ttu-id="b1bd4-110">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="b1bd4-110">In the **No.**</span></span> <span data-ttu-id="b1bd4-111">введите, например, **Касса**.</span><span class="sxs-lookup"><span data-stu-id="b1bd4-111">field, enter **Cash**, for example.</span></span>  
4.  <span data-ttu-id="b1bd4-112">В поле **Название** укажите, например, **Продажа за наличные**.</span><span class="sxs-lookup"><span data-stu-id="b1bd4-112">In the **Name** field, enter **Cash Sale**, for example.</span></span>  
5.  <span data-ttu-id="b1bd4-113">На экспресс-вкладке **Счет** заполните поля **Учетная группа клиента** и **Общая бизнес-группа**.</span><span class="sxs-lookup"><span data-stu-id="b1bd4-113">On the **Invoicing** FastTab, fill in the **Customer Posting Group** and the **Gen. Bus. Posting Group** fields.</span></span>  

 <span data-ttu-id="b1bd4-114">Теперь по клиенту задано достаточное количество информации для выставления счета.</span><span class="sxs-lookup"><span data-stu-id="b1bd4-114">Now you have set up a customer that contains sufficient information for invoicing.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="b1bd4-115">Могла быть выбрана учетная группа, которая уже была использована для продажи в кредит внутри страны.</span><span class="sxs-lookup"><span data-stu-id="b1bd4-115">You may have chosen a posting group that is also used for domestic credit sales.</span></span> <span data-ttu-id="b1bd4-116">Если данные для продаж за наличные требуется отделить, например, использовав специальный счет продажи или счет расчетов с клиентами, то для этой цели может быть настроена еще одна учетная группа.</span><span class="sxs-lookup"><span data-stu-id="b1bd4-116">If you want to maintain separate data on cash sales, for example, with a special sales or receivables account, you can set up an extra posting group for this purpose.</span></span>  
>   
>  <span data-ttu-id="b1bd4-117">Для учетной группы должен быть задан номер счета расчетов с клиентами, даже если после выполнения учета баланс по этому счету всегда будет равен 0.</span><span class="sxs-lookup"><span data-stu-id="b1bd4-117">You must enter a number for a receivables account for the posting group, even though the balance in this account will always be 0 after you post an invoice.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b1bd4-118">См. также</span><span class="sxs-lookup"><span data-stu-id="b1bd4-118">See Also</span></span>
[<span data-ttu-id="b1bd4-119">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="b1bd4-119">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="b1bd4-120">[Регистрация новых клиентов](sales-how-register-new-customers.md)  </span><span class="sxs-lookup"><span data-stu-id="b1bd4-120">[Register New Customers](sales-how-register-new-customers.md)  </span></span>  
[<span data-ttu-id="b1bd4-121">Финансы</span><span class="sxs-lookup"><span data-stu-id="b1bd4-121">Finance</span></span>](finance.md)  


