---
title: "Настройка сервисных контрактов | Microsoft Docs"
description: "Узнайте, как настраивать сервисные контракты."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, cost, service order
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: a965721aef3769aa1e794c0edb9ffa48faf99541
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---

# <a name="set-up-service-contracts"></a><span data-ttu-id="3c1d2-103">Настройка сервисных контрактов</span><span class="sxs-lookup"><span data-stu-id="3c1d2-103">Set Up Service Contracts</span></span>
<span data-ttu-id="3c1d2-104">До начала работы с контрактами необходимо настроить следующее:</span><span class="sxs-lookup"><span data-stu-id="3c1d2-104">Before you can work with contracts, you must set up the following:</span></span> 

* <span data-ttu-id="3c1d2-105">**Группы сервисных контрактов**, объединяющие сервисные контракты, которые каким-либо образом связаны.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-105">**Service contract groups**, which gather service contracts that are related in some way.</span></span>
* <span data-ttu-id="3c1d2-106">**Группы счетов сервисных контрактов**, которые используются для объединения счетов сервисных контрактов для сервисных счетов, созданных для сервисных контрактов.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-106">**Service contract account groups**, which are used to group the service contract accounts together for service invoices created for service contracts.</span></span> <span data-ttu-id="3c1d2-107">Эти группы назначаются сервисным контрактам.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-107">You assign these groups to service contracts.</span></span>  
* <span data-ttu-id="3c1d2-108">**Шаблоны контрактов**, которые определяют макеты сервисных контрактов, в которые включаются наиболее часто используемые в сервисных контрактах сведения.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-108">**Contract templates** that define contract layouts of contracts that include the most commonly used service contract details.</span></span> <span data-ttu-id="3c1d2-109">При создании предложений сервисных контрактов можно пользоваться шаблонами.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-109">When you create service contract quotes, you can create them by using templates.</span></span> <span data-ttu-id="3c1d2-110">При создании предложения по контракту поля автоматически содержат содержимое полей шаблона.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-110">When you create a contract quote, the fields automatically contain the contents of the template fields.</span></span>
* <span data-ttu-id="3c1d2-111">**Шаблоны клиентов**, которые позволяет создавать предложения для контактов или потенциальных клиентов, которые не зарегистрированы как клиенты в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3c1d2-111">**Customer templates** that let you create quotes for contacts or potential customers who are not registered as customers in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-set-up-a-service-contract-group"></a><span data-ttu-id="3c1d2-112">Настройка группы сервисных контрактов</span><span class="sxs-lookup"><span data-stu-id="3c1d2-112">To set up a service contract group</span></span>  
1. <span data-ttu-id="3c1d2-113">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Группы сервисных контрактов**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Contract Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3c1d2-114">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="3c1d2-115">Установите флажок **Скидка только для заказов по контр.**, если нужно, чтобы скидки по контракту или на сервисное обслуживание действовали только для контрактных сервисных заказов, таких как обслуживание.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-115">Choose the **Disc. on Contr. Orders Only** check box if you want contract or service discounts to be valid only for contract service orders, such as maintenance.</span></span>  

## <a name="to-set-up-a-service-contract-account-group"></a><span data-ttu-id="3c1d2-116">Настройка учетной группы сервисных контрактов</span><span class="sxs-lookup"><span data-stu-id="3c1d2-116">To set up a service contract account group</span></span>  
1. <span data-ttu-id="3c1d2-117">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учетные группы сервисного контракта**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Serv. Contract Account Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3c1d2-118">Создать новые учетные группы сервисных контрактов.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-118">Create a new service contract account group.</span></span>   
3. <span data-ttu-id="3c1d2-119">Заполните поля **Код** и **Описание**.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-119">Fill in the **Code** and **Description** fields.</span></span> <span data-ttu-id="3c1d2-120">В этих полях описываются сервисные учетные группы.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-120">These fields describe the service account group.</span></span>  
4. <span data-ttu-id="3c1d2-121">Заполните поле **Непредоплач. контракт - счет**, выберите номер счета ГК по счету без предоплаты.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-121">Fill in the **Non-Prepaid Contract Acc.** field, choose general ledger account number for the non-prepaid account.</span></span>  
5. <span data-ttu-id="3c1d2-122">В поле **Непредоплач. контракт - счет** выберите номер счета ГК по счету с предоплатой.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-122">In the **Prepaid Contract Acc.** field, choose the general ledger account number for the prepaid account.</span></span>  

## <a name="to-set-up-a-contract-template"></a><span data-ttu-id="3c1d2-123">Настройка шаблона контрактов</span><span class="sxs-lookup"><span data-stu-id="3c1d2-123">To set up a contract template</span></span>  
1. <span data-ttu-id="3c1d2-124">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Шаблоны сервисного контракта**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Contract Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3c1d2-125">Создать новый шаблон сервисного контракта.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-125">Create a new service contract template.</span></span>  
3. <span data-ttu-id="3c1d2-126">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="3c1d2-126">In the **No.**</span></span> <span data-ttu-id="3c1d2-127">введите номер для шаблона контакта.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-127">field, enter a number for the contract template.</span></span>  
  
     <span data-ttu-id="3c1d2-128">Вместо этого, если на странице **Сервисный центр - настройка** настроены серии номеров шаблонов контрактов, можно нажать клавишу ВВОД, для ввода следующего свободного номера шаблона контракта.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-128">Alternatively, if you have set up number series for contract templates on the **Service Mgt. Setup** page, you can press the Enter key to enter the next available contract template number.</span></span> <span data-ttu-id="3c1d2-129">Заполните другие поля, если это требуется.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-129">Fill in the other fields if appropriate.</span></span>  
  
4. <span data-ttu-id="3c1d2-130">На экспресс-вкладке **Счет** заполните поле **Код учетной группы серв. контрактов**, **Расчетный период** и т. п.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-130">On the **Invoice** FastTab, fill in the **Serv. Contract Acc. Group Code** field, the **Invoice Period**, and so on.</span></span> <span data-ttu-id="3c1d2-131">Заполните другие поля, если это требуется.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-131">Fill in the other fields if appropriate.</span></span>  
5. <span data-ttu-id="3c1d2-132">Выберите действие **Скидки на сервисное обслуживание** для добавления скидок по контракту.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-132">Choose the **Service Discounts** action to add contract discounts.</span></span>  

## <a name="to-set-up-a-customer-template"></a><span data-ttu-id="3c1d2-133">Настройка шаблона клиентов</span><span class="sxs-lookup"><span data-stu-id="3c1d2-133">To set up a customer template</span></span>  
1. <span data-ttu-id="3c1d2-134">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Шаблоны клиента**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3c1d2-135">Создать новую карточку шаблона клиента.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-135">Create a new customer template card.</span></span>  
3. <span data-ttu-id="3c1d2-136">На экспресс-вкладке **Общее** в полях **Код** и **Описание** введите соответственно код и описание шаблона клиента.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-136">On the **General** FastTab, enter a code and a description for the customer template in the **Code** and **Description** fields respectively.</span></span> 
4. <span data-ttu-id="3c1d2-137">Чтобы определить критерии поиска, заполните другие поля, например **Код страны/региона**, **Код территории** и **Код языка**.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-137">To define search criteria, fill in the other fields, such as **Country/Region Code**, **Territory Code**, and **Language Code**.</span></span>  
5. <span data-ttu-id="3c1d2-138">Заполните поля **Общая бизнес-группа** и **Учетная группа клиента**.</span><span class="sxs-lookup"><span data-stu-id="3c1d2-138">Fill in the **Gen. Bus. Posting Group** and **Customer Posting Group** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3c1d2-139">См. также</span><span class="sxs-lookup"><span data-stu-id="3c1d2-139">See Also</span></span>
[<span data-ttu-id="3c1d2-140">Настройка управления сервисным обслуживанием</span><span class="sxs-lookup"><span data-stu-id="3c1d2-140">Setting Up Service Management</span></span>](service-setup-service.md)
