---
title: "Создание контактных организаций | Microsoft Docs"
description: "Описывается, как создать контакт для каждой новой организации или потенциального клиента, с которым вы взаимодействуете."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 10/01/2018
ms.author: jswymer
redirect_url: marketing-create-contact-companies
ms.translationtype: HT
ms.sourcegitcommit: 8a73de1aa2f4a0f633c401ea341bb7bde6579723
ms.openlocfilehash: 932ae29ff302390962bf9ca4dc48d2d76fce1ca2
ms.contentlocale: ru-ru
ms.lasthandoff: 12/11/2018

---
# <a name="create-contact-companies"></a><span data-ttu-id="3ecd0-103">Создание контактных организаций</span><span class="sxs-lookup"><span data-stu-id="3ecd0-103">Create Contact Companies</span></span>
<span data-ttu-id="3ecd0-104">Вы можете создать контакт для каждой новой организации, с которой происходит взаимодействие, например заказчика, поставщика, банка, юридической организации, консультанта и т. д.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-104">You can create a contact for each new company you interact with, for example, a customer, vendor, prospective customer, bank, law firm, consultant, and so on.</span></span>

<span data-ttu-id="3ecd0-105">Есть два способа создания контактов: с нуля или на основе имеющегося клиента, поставщика или банковского счета.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-105">There are two ways to create a contact: from scratch or from an existing customer, vendor, or bank account.</span></span>

<span data-ttu-id="3ecd0-106">Перед созданием контакта может понадобиться проверить настройки на странице **Маркетинг - настройка**.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-106">Before creating a contact, you may want to check the settings on the **Marketing Setup** page.</span></span> <span data-ttu-id="3ecd0-107">Дополнительные сведения см. в разделе [Настройка управления отношениями](marketing-setup-marketing.md).</span><span class="sxs-lookup"><span data-stu-id="3ecd0-107">For more information, see [Setting Up Relationship Management](marketing-setup-marketing.md).</span></span>

## <a name="create-a-company-contact-from-scratch"></a><span data-ttu-id="3ecd0-108">Создание контакта организации с нуля</span><span class="sxs-lookup"><span data-stu-id="3ecd0-108">Create a company contact from scratch</span></span>
1. <span data-ttu-id="3ecd0-109">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Контакты**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Contacts**, and then choose the related link.</span></span>
2. <span data-ttu-id="3ecd0-110">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-110">Choose the **New** action.</span></span>
3. <span data-ttu-id="3ecd0-111">В поле **Номер** введите номер контакта.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-111">In the **No. field**, enter a number for the contact.</span></span>

    <span data-ttu-id="3ecd0-112">Вместо этого, если настроены серии номеров для контактов на странице **Маркетинг - настройка**, можно нажать клавишу ВВОД, чтобы выбрать следующий доступный номер контакта.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-112">Alternatively, if you have set up a number series for contacts on the **Marketing Setup** page, you can press the Enter key to select the next available contact number.</span></span>  
4. <span data-ttu-id="3ecd0-113">В поле **Тип** выберите **Организация**.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-113">Set **Type** to **Company**.</span></span>
5. <span data-ttu-id="3ecd0-114">Заполните остальные поля соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-114">Fill in the other fields as required.</span></span>

## <a name="to-create-a-company-contact-from-a-customer-vendor-or-bank-account"></a><span data-ttu-id="3ecd0-115">Создание контакта организации из клиента, поставщика или банковского счета</span><span class="sxs-lookup"><span data-stu-id="3ecd0-115">To create a company contact from a customer, vendor, or bank account</span></span>
<span data-ttu-id="3ecd0-116">Если вы уже создали какое-либо количество клиентов, поставщиков и банковских счетов, можно создавать контакты на основе имеющихся данных.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-116">If you have already set up a number of customers, vendors, and bank accounts, you can create contacts on the basis of the existing data.</span></span> <span data-ttu-id="3ecd0-117">При создании контакта таким способом сведения о контакте синхронизируются с клиентом, поставщиком или банковским счетом.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-117">When you create a contact this way, the contact information is synchronized with the customer, vendor, or bank account information.</span></span>

> [!NOTE]  
>   <span data-ttu-id="3ecd0-118">Прежде чем можно будет создавать контактные организации таким образом, необходимо указать код деловых отношений для клиентов, поставщиков или банковских счетов на странице **Настройка модуля "Маркетинг"**.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-118">Before you can create contact companies this way, you must specify a business relation code for customers, vendors, and bank accounts on the **Marketing Setup** page.</span></span> <span data-ttu-id="3ecd0-119">Если вы будет создавать контакты из банковских счетов, вы должны также указать серии номеров для банковских счетов на странице **Настройка ГК**.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-119">If you will be creating contacts from a bank accounts, you must also specify numbers series for bank accounts on the **General Ledger Setup** page.</span></span>

1. <span data-ttu-id="3ecd0-120">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите одно из следующего, в зависимости от того, где требуется создать контакты, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter one of the following, depending on from where you want to create contacts, and then choose the related link.</span></span>
   * <span data-ttu-id="3ecd0-121">**Создать контакты из клиентов**</span><span class="sxs-lookup"><span data-stu-id="3ecd0-121">**Create Contacts from Customers**</span></span>
   * <span data-ttu-id="3ecd0-122">**Создать контакты из поставщиков**</span><span class="sxs-lookup"><span data-stu-id="3ecd0-122">**Create Contacts from Vendors**</span></span>
   * <span data-ttu-id="3ecd0-123">**Создать контакты из банк. счетов**</span><span class="sxs-lookup"><span data-stu-id="3ecd0-123">**Create Contacts from Bank Accounts**</span></span>
2. <span data-ttu-id="3ecd0-124">На открывшейся странице пакетного задания в разделе **Клиент**, **Поставщик** или **Банковский счет** установите фильтры, если требуется создать контакты из конкретных клиентов, поставщиков или банковских счетов.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-124">In the batch job page that opens, in the **Customer**, **Vendor**, or **Bank Account** section, set filters if you want to create contacts from specific customers, vendors, or bank accounts.</span></span>
3. <span data-ttu-id="3ecd0-125">Нажмите кнопку **ОК** для начала создания контактов.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-125">Choose the **OK** button to start creating contacts.</span></span>

    <span data-ttu-id="3ecd0-126">Новым контактам присваиваются следующие номера контактов из серии номеров.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-126">The next contact numbers in the number series are assigned to the new contacts.</span></span> <span data-ttu-id="3ecd0-127">Деловое отношение поставщиков, указанное на странице **Настройка модуля "Маркетинг"**, назначается созданным новым контактам.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-127">The business relation for vendors that is specified on the **Marketing Setup** page is assigned to the newly created contacts.</span></span>

> [!TIP]  
>   <span data-ttu-id="3ecd0-128">Вы также можете создать клиента, поставщика или банковский счет из контакта.</span><span class="sxs-lookup"><span data-stu-id="3ecd0-128">You can also create a customer, vendor, or bank account from a contact.</span></span> <span data-ttu-id="3ecd0-129">Дополнительные сведения см. в разделе [Создание клиента, поставщика или банковского счета из клиента](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="3ecd0-129">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="3ecd0-130">См. также</span><span class="sxs-lookup"><span data-stu-id="3ecd0-130">See Also</span></span>
[<span data-ttu-id="3ecd0-131">Синхронизация контактов с клиентами, поставщиками и банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="3ecd0-131">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span></span>](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[<span data-ttu-id="3ecd0-132">Назначение деловых отношений контакту</span><span class="sxs-lookup"><span data-stu-id="3ecd0-132">Assign Business Relations to a Contact</span></span>](marketing-business-relations.md#AssignBusRelContact)  
[<span data-ttu-id="3ecd0-133">Присвоение отраслевых групп контакту</span><span class="sxs-lookup"><span data-stu-id="3ecd0-133">Assign Industry Groups to a Contact</span></span>](marketing-industry-groups.md#AssignIndustryGroupContact)  
[<span data-ttu-id="3ecd0-134">Назначение групп рассылки контакту</span><span class="sxs-lookup"><span data-stu-id="3ecd0-134">Assign Mailing Groups to a Contact</span></span>](marketing-mailing-groups.md#AssignMailGroupContact)  
[<span data-ttu-id="3ecd0-135">Создание контактных лиц</span><span class="sxs-lookup"><span data-stu-id="3ecd0-135">Create Contact Persons</span></span>](marketing-create-contact-persons.md)  
[<span data-ttu-id="3ecd0-136">Работа с Business Central</span><span class="sxs-lookup"><span data-stu-id="3ecd0-136">Working with Business Central</span></span>](ui-work-product.md)

