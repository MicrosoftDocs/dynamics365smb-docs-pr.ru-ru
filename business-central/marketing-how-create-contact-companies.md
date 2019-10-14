---
title: Создание контактных организаций | Документация Майкрософт
description: Описывается, как создать контакт для каждой новой организации или потенциального клиента, с которым вы взаимодействуете.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 10/01/2019
ms.author: jswymer
redirect_url: marketing-create-contact-companies
ms.openlocfilehash: fcd964cc1cea9fb256b58f3a73b061b241d92fe4
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2309248"
---
# <a name="create-contacts"></a><span data-ttu-id="ca2f8-103">Создание контактов</span><span class="sxs-lookup"><span data-stu-id="ca2f8-103">Create Contacts</span></span>
<span data-ttu-id="ca2f8-104">Вы можете создать контакт для каждой новой организации, с которой происходит взаимодействие, например заказчика, поставщика, банка, юридической организации, консультанта и т. д.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-104">You can create a contact for each new company you interact with, for example, a customer, vendor, prospective customer, bank, law firm, consultant, and so on.</span></span>

<span data-ttu-id="ca2f8-105">Есть два способа создания контактов: с нуля или на основе имеющегося клиента, поставщика или банковского счета.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-105">There are two ways to create a contact: from scratch or from an existing customer, vendor, or bank account.</span></span>

## <a name="create-a-company-contact-from-scratch"></a><span data-ttu-id="ca2f8-106">Создание контакта организации с нуля</span><span class="sxs-lookup"><span data-stu-id="ca2f8-106">Create a company contact from scratch</span></span>
1. <span data-ttu-id="ca2f8-107">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Контакты**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Contacts**, and then choose the related link.</span></span>
2. <span data-ttu-id="ca2f8-108">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-108">Choose the **New** action.</span></span>
3. <span data-ttu-id="ca2f8-109">В поле **Номер** введите номер контакта.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-109">In the **No. field**, enter a number for the contact.</span></span>

    <span data-ttu-id="ca2f8-110">Вместо этого, если настроены серии номеров для контактов на странице **Маркетинг - настройка**, можно нажать клавишу ВВОД, чтобы выбрать следующий доступный номер контакта.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-110">Alternatively, if you have set up a number series for contacts on the **Marketing Setup** page, you can press the Enter key to select the next available contact number.</span></span>  
4. <span data-ttu-id="ca2f8-111">В поле **Тип** выберите **Организация**.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-111">Set **Type** to **Company**.</span></span>
5. <span data-ttu-id="ca2f8-112">Заполните остальные поля соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-112">Fill in the other fields as required.</span></span>

## <a name="to-create-a-company-contact-from-a-customer-vendor-or-bank-account"></a><span data-ttu-id="ca2f8-113">Создание контакта организации из клиента, поставщика или банковского счета</span><span class="sxs-lookup"><span data-stu-id="ca2f8-113">To create a company contact from a customer, vendor, or bank account</span></span>
<span data-ttu-id="ca2f8-114">Если вы уже создали какое-либо количество клиентов, поставщиков и банковских счетов, можно создавать контакты на основе имеющихся данных.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-114">If you have already set up a number of customers, vendors, and bank accounts, you can create contacts on the basis of the existing data.</span></span> <span data-ttu-id="ca2f8-115">При создании контакта таким способом сведения о контакте синхронизируются с клиентом, поставщиком или банковским счетом.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-115">When you create a contact this way, the contact information is synchronized with the customer, vendor, or bank account information.</span></span>

> [!NOTE]  
>   <span data-ttu-id="ca2f8-116">Прежде чем можно будет создавать контактные организации таким образом, необходимо указать код деловых отношений для клиентов, поставщиков или банковских счетов на странице **Настройка модуля "Маркетинг"**.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-116">Before you can create contact companies this way, you must specify a business relation code for customers, vendors, and bank accounts on the **Marketing Setup** page.</span></span> <span data-ttu-id="ca2f8-117">Если вы будет создавать контакты из банковских счетов, вы должны также указать серии номеров для банковских счетов на странице **Настройка ГК**.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-117">If you will be creating contacts from a bank accounts, you must also specify numbers series for bank accounts on the **General Ledger Setup** page.</span></span>

1. <span data-ttu-id="ca2f8-118">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите одно из следующего, в зависимости от того, где требуется создать контакты, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter one of the following, depending on from where you want to create contacts, and then choose the related link.</span></span>
   * <span data-ttu-id="ca2f8-119">**Создать контакты из клиентов**</span><span class="sxs-lookup"><span data-stu-id="ca2f8-119">**Create Contacts from Customers**</span></span>
   * <span data-ttu-id="ca2f8-120">**Создать контакты из поставщиков**</span><span class="sxs-lookup"><span data-stu-id="ca2f8-120">**Create Contacts from Vendors**</span></span>
   * <span data-ttu-id="ca2f8-121">**Создать контакты из банк. счетов**</span><span class="sxs-lookup"><span data-stu-id="ca2f8-121">**Create Contacts from Bank Accounts**</span></span>
2. <span data-ttu-id="ca2f8-122">На открывшейся странице пакетного задания в разделе **Клиент**, **Поставщик** или **Банковский счет** установите фильтры, если требуется создать контакты из конкретных клиентов, поставщиков или банковских счетов.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-122">In the batch job page that opens, in the **Customer**, **Vendor**, or **Bank Account** section, set filters if you want to create contacts from specific customers, vendors, or bank accounts.</span></span>
3. <span data-ttu-id="ca2f8-123">Нажмите кнопку **ОК** для начала создания контактов.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-123">Choose the **OK** button to start creating contacts.</span></span>

    <span data-ttu-id="ca2f8-124">Новым контактам присваиваются следующие номера контактов из серии номеров.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-124">The next contact numbers in the number series are assigned to the new contacts.</span></span> <span data-ttu-id="ca2f8-125">Деловое отношение поставщиков, указанное на странице **Настройка модуля "Маркетинг"**, назначается созданным новым контактам.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-125">The business relation for vendors that is specified on the **Marketing Setup** page is assigned to the newly created contacts.</span></span>

> [!TIP]  
>   <span data-ttu-id="ca2f8-126">Вы также можете создать клиента, поставщика или банковский счет из контакта.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-126">You can also create a customer, vendor, or bank account from a contact.</span></span> <span data-ttu-id="ca2f8-127">Дополнительные сведения см. в разделе [Создание клиента, поставщика или банковского счета из клиента](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="ca2f8-127">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="ca2f8-128">См. также</span><span class="sxs-lookup"><span data-stu-id="ca2f8-128">See Also</span></span>
[<span data-ttu-id="ca2f8-129">Синхронизация контактов с клиентами, поставщиками и банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="ca2f8-129">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span></span>](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[<span data-ttu-id="ca2f8-130">Назначение деловых отношений контакту</span><span class="sxs-lookup"><span data-stu-id="ca2f8-130">Assign Business Relations to a Contact</span></span>](marketing-business-relations.md#AssignBusRelContact)  
[<span data-ttu-id="ca2f8-131">Присвоение отраслевых групп контакту</span><span class="sxs-lookup"><span data-stu-id="ca2f8-131">Assign Industry Groups to a Contact</span></span>](marketing-industry-groups.md#AssignIndustryGroupContact)  
[<span data-ttu-id="ca2f8-132">Назначение групп рассылки контакту</span><span class="sxs-lookup"><span data-stu-id="ca2f8-132">Assign Mailing Groups to a Contact</span></span>](marketing-mailing-groups.md#AssignMailGroupContact)  
[<span data-ttu-id="ca2f8-133">Создание контактных лиц</span><span class="sxs-lookup"><span data-stu-id="ca2f8-133">Create Contact Persons</span></span>](marketing-create-contact-persons.md)  
[<span data-ttu-id="ca2f8-134">Работа с Business Central</span><span class="sxs-lookup"><span data-stu-id="ca2f8-134">Working with Business Central</span></span>](ui-work-product.md)
