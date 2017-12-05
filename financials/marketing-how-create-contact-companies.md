---
title: "Создание контактных организаций | Microsoft Docs"
description: "Описывается, как создать контакт для каждой новой организации или потенциального клиента, с которым вы взаимодействуете."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: c0e678b07c1d5ca73808a2abb5631771dce76fd0
ms.contentlocale: ru-ru
ms.lasthandoff: 11/10/2017

---
# <a name="how-to-create-contact-companies"></a><span data-ttu-id="6d558-103">Как создать контактные организации</span><span class="sxs-lookup"><span data-stu-id="6d558-103">How to: Create Contact Companies</span></span>
<span data-ttu-id="6d558-104">Вы можете создать контакт для каждой новой организации, с которой происходит взаимодействие, например заказчика, поставщика, банка, юридической организации, консультанта и т. д.</span><span class="sxs-lookup"><span data-stu-id="6d558-104">You can create a contact for each new company you interact with, for example, a customer, vendor, prospective customer, bank, law firm, consultant, and so on.</span></span>

<span data-ttu-id="6d558-105">Есть два способа создания контактов: с нуля или на основе имеющегося клиента, поставщика или банковского счета.</span><span class="sxs-lookup"><span data-stu-id="6d558-105">There are two ways to create a contact: from scratch or from an existing customer, vendor, or bank account.</span></span>

<span data-ttu-id="6d558-106">Перед созданием контакта может понадобиться проверить настройки в окне **Маркетинг - настройка**.</span><span class="sxs-lookup"><span data-stu-id="6d558-106">Before creating a contact, you may want to check the settings in the **Marketing Setup** window.</span></span> <span data-ttu-id="6d558-107">Дополнительные сведения см. в разделе [Настройка управления отношениями](marketing-setup-marketing.md).</span><span class="sxs-lookup"><span data-stu-id="6d558-107">For more information, see [Setting Up Relationship Management](marketing-setup-marketing.md).</span></span>

## <a name="create-a-company-contact-from-scratch"></a><span data-ttu-id="6d558-108">Создание контакта организации с нуля</span><span class="sxs-lookup"><span data-stu-id="6d558-108">Create a company contact from scratch</span></span>
1. <span data-ttu-id="6d558-109">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Контакты**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6d558-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Contacts**, and then choose the related link.</span></span>
2. <span data-ttu-id="6d558-110">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="6d558-110">Choose the **New** action.</span></span>
3. <span data-ttu-id="6d558-111">В поле **Номер** введите номер контакта.</span><span class="sxs-lookup"><span data-stu-id="6d558-111">In the **No. field**, enter a number for the contact.</span></span>

    <span data-ttu-id="6d558-112">Вместо этого, если настроены серии номеров для контактов в окне **Маркетинг - настройка**, можно нажать клавишу ВВОД, чтобы выбрать следующий доступный номер контакта.</span><span class="sxs-lookup"><span data-stu-id="6d558-112">Alternatively, if you have set up a number series for contacts in the **Marketing Setup** window, you can press the Enter key to select the next available contact number.</span></span>  
4. <span data-ttu-id="6d558-113">В поле **Тип** выберите **Организация**.</span><span class="sxs-lookup"><span data-stu-id="6d558-113">Set **Type** to **Company**.</span></span>
5. <span data-ttu-id="6d558-114">Заполните остальные поля соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="6d558-114">Fill in the other fields as required.</span></span>

## <a name="to-create-a-company-contact-from-a-customer-vendor-or-bank-account"></a><span data-ttu-id="6d558-115">Создание контакта организации из клиента, поставщика или банковского счета</span><span class="sxs-lookup"><span data-stu-id="6d558-115">To create a company contact from a customer, vendor, or bank account</span></span>
<span data-ttu-id="6d558-116">Если вы уже создали какое-либо количество клиентов, поставщиков и банковских счетов, можно создавать контакты на основе имеющихся данных.</span><span class="sxs-lookup"><span data-stu-id="6d558-116">If you have already set up a number of customers, vendors, and bank accounts, you can create contacts on the basis of the existing data.</span></span> <span data-ttu-id="6d558-117">При создании контакта таким способом сведения о контакте синхронизируются с клиентом, поставщиком или банковским счетом.</span><span class="sxs-lookup"><span data-stu-id="6d558-117">When you create a contact this way, the contact information is synchronized with the customer, vendor, or bank account information.</span></span>

> [!NOTE]  
>   <span data-ttu-id="6d558-118">Прежде чем можно будет создавать контактные организации таким образом, необходимо указать код деловых отношений для клиентов, поставщиков или банковских счетов в окне **Настройка модуля "Маркетинг"**.</span><span class="sxs-lookup"><span data-stu-id="6d558-118">Before you can create contact companies this way, you must specify a business relation code for customers, vendors, and bank accounts in the **Marketing Setup** window.</span></span> <span data-ttu-id="6d558-119">Если вы будет создавать контакты из банковских счетов, вы должны также указать серии номеров для банковских счетов в окне **Настройка ГК**.</span><span class="sxs-lookup"><span data-stu-id="6d558-119">If you will be creating contacts from a bank accounts, you must also specify numbers series for bank accounts in the **General Ledger Setup** window.</span></span>

1. <span data-ttu-id="6d558-120">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите одно из следующих значений в зависимости от того, откуда требуется создать контакты, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="6d558-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter one of the following, depending on from where you want to create contacts, and then choose the related link.</span></span>
   * <span data-ttu-id="6d558-121">**Создать контакты из клиентов**</span><span class="sxs-lookup"><span data-stu-id="6d558-121">**Create Contacts from Customers**</span></span>
   * <span data-ttu-id="6d558-122">**Создать контакты из поставщиков**</span><span class="sxs-lookup"><span data-stu-id="6d558-122">**Create Contacts from Vendors**</span></span>
   * <span data-ttu-id="6d558-123">**Создать контакты из банк. счетов**</span><span class="sxs-lookup"><span data-stu-id="6d558-123">**Create Contacts from Bank Accounts**</span></span>
2. <span data-ttu-id="6d558-124">В открывшемся окне пакетного задания в разделе **Клиент**, **Поставщик** или **Банковский счет** установите фильтры, если требуется создать контакты из конкретных клиентов, поставщиков или банковских счетов.</span><span class="sxs-lookup"><span data-stu-id="6d558-124">In the batch job window that opens, in the **Customer**, **Vendor**, or **Bank Account** section, set filters if you want to create contacts from specific customers, vendors, or bank accounts.</span></span>
3. <span data-ttu-id="6d558-125">Нажмите кнопку **ОК** для начала создания контактов.</span><span class="sxs-lookup"><span data-stu-id="6d558-125">Choose the **OK** button to start creating contacts.</span></span>

    <span data-ttu-id="6d558-126">Новым контактам присваиваются следующие номера контактов из серии номеров.</span><span class="sxs-lookup"><span data-stu-id="6d558-126">The next contact numbers in the number series are assigned to the new contacts.</span></span> <span data-ttu-id="6d558-127">Деловое отношение поставщиков, указанное в окне **Настройка модуля "Маркетинг"**, назначается созданным новым контактам.</span><span class="sxs-lookup"><span data-stu-id="6d558-127">The business relation for vendors that is specified in the **Marketing Setup** window is assigned to the newly created contacts.</span></span>

> [!TIP]  
>   <span data-ttu-id="6d558-128">Вы также можете создать клиента, поставщика или банковский счет из контакта.</span><span class="sxs-lookup"><span data-stu-id="6d558-128">You can also create a customer, vendor, or bank account from a contact.</span></span> <span data-ttu-id="6d558-129">Дополнительные сведения см. в разделе [Создание клиента, поставщика или банковского счета из клиента](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="6d558-129">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="6d558-130">См. также</span><span class="sxs-lookup"><span data-stu-id="6d558-130">See Also</span></span>
[<span data-ttu-id="6d558-131">Синхронизация контактов с клиентами, поставщиками и банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="6d558-131">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span></span>](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[<span data-ttu-id="6d558-132">Назначение деловых отношений контакту</span><span class="sxs-lookup"><span data-stu-id="6d558-132">Assign Business Relations to a Contact</span></span>](marketing-business-relations.md#AssignBusRelContact)  
[<span data-ttu-id="6d558-133">Присвоение отраслевых групп контакту</span><span class="sxs-lookup"><span data-stu-id="6d558-133">Assign Industry Groups to a Contact</span></span>](marketing-industry-groups.md#AssignIndustryGroupContact)  
[<span data-ttu-id="6d558-134">Назначение групп рассылки контакту</span><span class="sxs-lookup"><span data-stu-id="6d558-134">Assign Mailing Groups to a Contact</span></span>](marketing-mailing-groups.md#AssignMailGroupContact)  
[<span data-ttu-id="6d558-135">Как создать контактные лица</span><span class="sxs-lookup"><span data-stu-id="6d558-135">How to: Create Contact Persons</span></span>](marketing-create-contact-persons.md)  
[<span data-ttu-id="6d558-136">Работа с Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="6d558-136">Working with Dynamics 365</span></span>](ui-work-product.md)

