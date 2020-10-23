---
title: Практическое руководство. Настройка клиентов, оплачивающих наличными | Документация Майкрософт
description: В этом разделе описываются шаги для настройки клиента, который осуществляет оплату наличными.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: a4f73de177129f5bc33808e6acf74bd273ae0d33
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3915564"
---
# <a name="set-up-cash-customers"></a><span data-ttu-id="36029-103">Настройка клиентов, оплачивающих наличными</span><span class="sxs-lookup"><span data-stu-id="36029-103">Set Up Cash Customers</span></span>
<span data-ttu-id="36029-104">Счет не может быть создан без номера клиента.</span><span class="sxs-lookup"><span data-stu-id="36029-104">You cannot create an invoice without a customer number.</span></span> <span data-ttu-id="36029-105">Это правило выполняется даже тогда, когда выполняется продажа с наличным расчетом, и по счету клиента записи не производятся.</span><span class="sxs-lookup"><span data-stu-id="36029-105">This is true, even if you make a cash sale and do not have anything to record in a customer account.</span></span>  

## <a name="to-set-up-a-cash-customer"></a><span data-ttu-id="36029-106">Настройка клиента, оплачивающего наличными</span><span class="sxs-lookup"><span data-stu-id="36029-106">To set up a cash customer</span></span>  
1.  <span data-ttu-id="36029-107">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиент**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="36029-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="36029-108">Создайте новую **Карточку клиента**.</span><span class="sxs-lookup"><span data-stu-id="36029-108">Create a new **Customer** card.</span></span> <span data-ttu-id="36029-109">Дополнительные сведения см. в разделе [Регистрация новых клиентов](sales-how-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="36029-109">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span></span>
3.  <span data-ttu-id="36029-110">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="36029-110">In the **No.**</span></span> <span data-ttu-id="36029-111">введите, например, **Касса**.</span><span class="sxs-lookup"><span data-stu-id="36029-111">field, enter **Cash**, for example.</span></span>  
4.  <span data-ttu-id="36029-112">В поле **Название** укажите, например, **Продажа за наличные**.</span><span class="sxs-lookup"><span data-stu-id="36029-112">In the **Name** field, enter **Cash Sale**, for example.</span></span>  
5.  <span data-ttu-id="36029-113">На экспресс-вкладке **Счет** заполните поля **Учетная группа клиента** и **Общая бизнес-группа**.</span><span class="sxs-lookup"><span data-stu-id="36029-113">On the **Invoicing** FastTab, fill in the **Customer Posting Group** and the **Gen. Bus. Posting Group** fields.</span></span>  

 <span data-ttu-id="36029-114">Теперь по клиенту задано достаточное количество информации для выставления счета.</span><span class="sxs-lookup"><span data-stu-id="36029-114">Now you have set up a customer that contains sufficient information for invoicing.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="36029-115">Могла быть выбрана учетная группа, которая уже была использована для продажи в кредит внутри страны.</span><span class="sxs-lookup"><span data-stu-id="36029-115">You may have chosen a posting group that is also used for domestic credit sales.</span></span> <span data-ttu-id="36029-116">Если данные для продаж за наличные требуется отделить, например, использовав специальный счет продажи или счет расчетов с клиентами, то для этой цели может быть настроена еще одна учетная группа.</span><span class="sxs-lookup"><span data-stu-id="36029-116">If you want to maintain separate data on cash sales, for example, with a special sales or receivables account, you can set up an extra posting group for this purpose.</span></span>  
>   
>  <span data-ttu-id="36029-117">Для учетной группы должен быть задан номер счета расчетов с клиентами, даже если после выполнения учета баланс по этому счету всегда будет равен 0.</span><span class="sxs-lookup"><span data-stu-id="36029-117">You must enter a number for a receivables account for the posting group, even though the balance in this account will always be 0 after you post an invoice.</span></span>  

## <a name="see-also"></a><span data-ttu-id="36029-118">См. также</span><span class="sxs-lookup"><span data-stu-id="36029-118">See Also</span></span>
[<span data-ttu-id="36029-119">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="36029-119">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="36029-120">[Регистрация новых клиентов](sales-how-register-new-customers.md)  </span><span class="sxs-lookup"><span data-stu-id="36029-120">[Register New Customers](sales-how-register-new-customers.md)  </span></span>  
[<span data-ttu-id="36029-121">Финансы</span><span class="sxs-lookup"><span data-stu-id="36029-121">Finance</span></span>](finance.md)  

