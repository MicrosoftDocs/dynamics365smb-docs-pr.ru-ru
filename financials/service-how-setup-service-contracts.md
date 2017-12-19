---
title: "Настройка сервисных контрактов | Microsoft Docs"
description: "Узнайте, как настраивать сервисные контракты."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, cost, service order
ms.date: 08/22/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: aa56764b5f3210229ad21eae6891fb201462209c
ms.openlocfilehash: 203f6ef7f156bdccaa491fdac761711fd32c317e
ms.contentlocale: ru-ru
ms.lasthandoff: 12/14/2017

---

# <a name="how-to-set-up-service-contracts"></a><span data-ttu-id="0df29-103">Практическое руководство. Настройка сервисных контрактов</span><span class="sxs-lookup"><span data-stu-id="0df29-103">How to: Set Up Service Contracts</span></span>
<span data-ttu-id="0df29-104">До начала работы с контрактами необходимо настроить следующее:</span><span class="sxs-lookup"><span data-stu-id="0df29-104">Before you can work with contracts, you must set up the following:</span></span> 

* <span data-ttu-id="0df29-105">**Группы сервисных контрактов**, объединяющие сервисные контракты, которые каким-либо образом связаны.</span><span class="sxs-lookup"><span data-stu-id="0df29-105">**Service contract groups**, which gather service contracts that are related in some way.</span></span>
* <span data-ttu-id="0df29-106">**Группы счетов сервисных контрактов**, которые используются для объединения счетов сервисных контрактов для сервисных счетов, созданных для сервисных контрактов.</span><span class="sxs-lookup"><span data-stu-id="0df29-106">**Service contract account groups**, which are used to group the service contract accounts together for service invoices created for service contracts.</span></span> <span data-ttu-id="0df29-107">Эти группы назначаются сервисным контрактам.</span><span class="sxs-lookup"><span data-stu-id="0df29-107">You assign these groups to service contracts.</span></span>  
* <span data-ttu-id="0df29-108">**Шаблоны контрактов**, которые определяют макеты сервисных контрактов, в которые включаются наиболее часто используемые в сервисных контрактах сведения.</span><span class="sxs-lookup"><span data-stu-id="0df29-108">**Contract templates** that define contract layouts of contracts that include the most commonly used service contract details.</span></span> <span data-ttu-id="0df29-109">При создании предложений сервисных контрактов можно пользоваться шаблонами.</span><span class="sxs-lookup"><span data-stu-id="0df29-109">When you create service contract quotes, you can create them by using templates.</span></span> <span data-ttu-id="0df29-110">При создании предложения по контракту поля автоматически содержат содержимое полей шаблона.</span><span class="sxs-lookup"><span data-stu-id="0df29-110">When you create a contract quote, the fields automatically contain the contents of the template fields.</span></span>
* <span data-ttu-id="0df29-111">**Шаблоны клиентов**, которые позволяет создавать предложения для контактов или потенциальных клиентов, которые не зарегистрированы как клиенты в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="0df29-111">**Customer templates** that let you create quotes for contacts or potential customers who are not registered as customers in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-set-up-a-service-contract-group"></a><span data-ttu-id="0df29-112">Настройка группы сервисных контрактов</span><span class="sxs-lookup"><span data-stu-id="0df29-112">To set up a service contract group</span></span>  
1. <span data-ttu-id="0df29-113">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Группы сервисных контрактов**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="0df29-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Contract Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0df29-114">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="0df29-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="0df29-115">Установите флажок **Скидка только для заказов по контр.**, если нужно, чтобы скидки по контракту или на сервисное обслуживание действовали только для контрактных сервисных заказов, таких как обслуживание.</span><span class="sxs-lookup"><span data-stu-id="0df29-115">Choose the **Disc. on Contr. Orders Only** check box if you want contract or service discounts to be valid only for contract service orders, such as maintenance.</span></span>  

## <a name="to-set-up-a-service-contract-account-group"></a><span data-ttu-id="0df29-116">Настройка учетной группы сервисных контрактов</span><span class="sxs-lookup"><span data-stu-id="0df29-116">To set up a service contract account group</span></span>  
1. <span data-ttu-id="0df29-117">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Учетные группы сервисного контракта**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="0df29-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Serv. Contract Account Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0df29-118">Создать новые учетные группы сервисных контрактов.</span><span class="sxs-lookup"><span data-stu-id="0df29-118">Create a new service contract account group.</span></span>   
3. <span data-ttu-id="0df29-119">Заполните поля **Код** и **Описание**.</span><span class="sxs-lookup"><span data-stu-id="0df29-119">Fill in the **Code** and **Description** fields.</span></span> <span data-ttu-id="0df29-120">В этих полях описываются сервисные учетные группы.</span><span class="sxs-lookup"><span data-stu-id="0df29-120">These fields describe the service account group.</span></span>  
4. <span data-ttu-id="0df29-121">Заполните поле **Непредоплач. контракт - счет**, выберите номер счета ГК по счету без предоплаты.</span><span class="sxs-lookup"><span data-stu-id="0df29-121">Fill in the **Non-Prepaid Contract Acc.** field, choose general ledger account number for the non-prepaid account.</span></span>  
5. <span data-ttu-id="0df29-122">В поле **Непредоплач. контракт - счет** выберите номер счета ГК по счету с предоплатой.</span><span class="sxs-lookup"><span data-stu-id="0df29-122">In the **Prepaid Contract Acc.** field, choose the general ledger account number for the prepaid account.</span></span>  

## <a name="to-set-up-a-contract-template"></a><span data-ttu-id="0df29-123">Настройка шаблона контрактов</span><span class="sxs-lookup"><span data-stu-id="0df29-123">To set up a contract template</span></span>  
1. <span data-ttu-id="0df29-124">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Сервисный контракт - шаблоны**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="0df29-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Contract Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0df29-125">Создать новый шаблон сервисного контракта.</span><span class="sxs-lookup"><span data-stu-id="0df29-125">Create a new service contract template.</span></span>  
3. <span data-ttu-id="0df29-126">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="0df29-126">In the **No.**</span></span> <span data-ttu-id="0df29-127">введите номер для шаблона контакта.</span><span class="sxs-lookup"><span data-stu-id="0df29-127">field, enter a number for the contract template.</span></span>  
  
     <span data-ttu-id="0df29-128">Вместо этого, если в окне **Сервисный центр - настройка** настроены серии номеров шаблонов контрактов, можно нажать клавишу ВВОД, для ввода следующего свободного номера шаблона контракта.</span><span class="sxs-lookup"><span data-stu-id="0df29-128">Alternatively, if you have set up number series for contract templates in the **Service Mgt. Setup** window, you can press the Enter key to enter the next available contract template number.</span></span> <span data-ttu-id="0df29-129">Заполните другие поля, если это требуется.</span><span class="sxs-lookup"><span data-stu-id="0df29-129">Fill in the other fields if appropriate.</span></span>  
  
4. <span data-ttu-id="0df29-130">На экспресс-вкладке **Счет** заполните поле **Код учетной группы серв. контрактов**, **Расчетный период** и т. п.</span><span class="sxs-lookup"><span data-stu-id="0df29-130">On the **Invoice** FastTab, fill in the **Serv. Contract Acc. Group Code** field, the **Invoice Period**, and so on.</span></span> <span data-ttu-id="0df29-131">Заполните другие поля, если это требуется.</span><span class="sxs-lookup"><span data-stu-id="0df29-131">Fill in the other fields if appropriate.</span></span>  
5. <span data-ttu-id="0df29-132">Выберите действие **Скидки на сервисное обслуживание** для добавления скидок по контракту.</span><span class="sxs-lookup"><span data-stu-id="0df29-132">Choose the **Service Discounts** action to add contract discounts.</span></span>  

## <a name="to-set-up-a-customer-template"></a><span data-ttu-id="0df29-133">Настройка шаблона клиентов</span><span class="sxs-lookup"><span data-stu-id="0df29-133">To set up a customer template</span></span>  
1. <span data-ttu-id="0df29-134">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Клиент - шаблоны**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="0df29-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0df29-135">Создать новую карточку шаблона клиента.</span><span class="sxs-lookup"><span data-stu-id="0df29-135">Create a new customer template card.</span></span>  
3. <span data-ttu-id="0df29-136">На экспресс-вкладке **Общее** в полях **Код** и **Описание** введите соответственно код и описание шаблона клиента.</span><span class="sxs-lookup"><span data-stu-id="0df29-136">On the **General** FastTab, enter a code and a description for the customer template in the **Code** and **Description** fields respectively.</span></span> 
4. <span data-ttu-id="0df29-137">Чтобы определить критерии поиска, заполните другие поля, например **Код страны/региона**, **Код территории** и **Код языка**.</span><span class="sxs-lookup"><span data-stu-id="0df29-137">To define search criteria, fill in the other fields, such as **Country/Region Code**, **Territory Code**, and **Language Code**.</span></span>  
5. <span data-ttu-id="0df29-138">Заполните поля **Общая бизнес-группа** и **Учетная группа клиента**.</span><span class="sxs-lookup"><span data-stu-id="0df29-138">Fill in the **Gen. Bus. Posting Group** and **Customer Posting Group** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0df29-139">См. также</span><span class="sxs-lookup"><span data-stu-id="0df29-139">See Also</span></span>
[<span data-ttu-id="0df29-140">Настройка управления сервисным обслуживанием</span><span class="sxs-lookup"><span data-stu-id="0df29-140">Setting Up Service Management</span></span>](service-setup-service.md)
