---
title: "Создание контактных лиц | Microsoft Docs"
description: "Описывается, как создать карточку контакта для каждого нового лица или потенциального клиента, с которым у вас деловые отношения."
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 0371e226de78c8c3894b47e5bebaf0aaf422666c
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="create-contact-persons"></a><span data-ttu-id="24129-103">Создание контактных лиц</span><span class="sxs-lookup"><span data-stu-id="24129-103">Create Contact Persons</span></span>
<span data-ttu-id="24129-104">Можно создавать карточку контакта для каждого контакта внутри организации, с которой происходит взаимодействие.</span><span class="sxs-lookup"><span data-stu-id="24129-104">You can create a contact card for each contact who works for the companies you interact with.</span></span> <span data-ttu-id="24129-105">Для каждой контактной организации можно ввести любое желаемое число контактных лиц.</span><span class="sxs-lookup"><span data-stu-id="24129-105">For each contact company you can enter as many contact persons as you want.</span></span> <span data-ttu-id="24129-106">Также можно создавать карточки контакта, которые будут зарегистрированы как независимые.</span><span class="sxs-lookup"><span data-stu-id="24129-106">You can also create contact cards for the persons that you want to record as independent.</span></span>

> [!TIP]  
>   <span data-ttu-id="24129-107">Перед созданием контакта может понадобиться проверить настройки **Наследования** в окне **Маркетинг - настройка**.</span><span class="sxs-lookup"><span data-stu-id="24129-107">Before creating a contact, you may want to check the **Inheritance** settings in the **Marketing Setup** window.</span></span> <span data-ttu-id="24129-108">Настройка наследования позволяет автоматически копировать информацию об организациях контактов, которая является общей для контактных лиц (например, адреса), из организации контакта в контактное лицо при каждом создании контактного лица для зарегистрированной контактной организации.</span><span class="sxs-lookup"><span data-stu-id="24129-108">Setting up inheritance enables information about contact companies that is common to contact persons, such as address details, to be automatically copied from the contact company to the contact person each time you create a contact person for a recorded contact company.</span></span>

## <a name="to-create-a-contact-card-for-a-person"></a><span data-ttu-id="24129-109">Создание карточки контакта для отдельного лица</span><span class="sxs-lookup"><span data-stu-id="24129-109">To create a contact card for a person</span></span>
1. <span data-ttu-id="24129-110">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Контакты**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="24129-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Contacts**, and then choose the related link.</span></span>
2. <span data-ttu-id="24129-111">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="24129-111">Choose the **New** action.</span></span>
3. <span data-ttu-id="24129-112">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="24129-112">In the **No.**</span></span> <span data-ttu-id="24129-113">введите номер контакта.</span><span class="sxs-lookup"><span data-stu-id="24129-113">field, enter a number for the contact.</span></span>

    <span data-ttu-id="24129-114">Вместо этого, если настроены серии номеров для контактов в окне **Маркетинг - настройка**, можно нажать клавишу ВВОД, чтобы выбрать следующий доступный номер контакта.</span><span class="sxs-lookup"><span data-stu-id="24129-114">Alternatively, if you have set up a number series for contacts in the **Marketing Setup** window, you can press the Enter key to select the next available contact number.</span></span> <span data-ttu-id="24129-115">Дополнительные сведения см. в разделе [Создание серий номеров](ui-create-number-series.md).</span><span class="sxs-lookup"><span data-stu-id="24129-115">For more information, see [Creating Number Series](ui-create-number-series.md).</span></span>
4. <span data-ttu-id="24129-116">В поле **Тип** выберите **Человек**.</span><span class="sxs-lookup"><span data-stu-id="24129-116">In the **Type** field, select **Person**.</span></span>
5. <span data-ttu-id="24129-117">Заполните остальные поля в карточке контакта.</span><span class="sxs-lookup"><span data-stu-id="24129-117">Fill in the other fields on the contact card.</span></span>

> [!NOTE]  
>   <span data-ttu-id="24129-118">Содержимое полей, выбранных на в разделе **Наследование** окна **Настройка модуля "Маркетинг"**, копируется из организации в карточки пользователей, работающих в этой организации.</span><span class="sxs-lookup"><span data-stu-id="24129-118">The contents of the fields that you have selected in the **Inheritance** section of the **Marketing Setup** window are copied from the company to the persons within that company.</span></span>

## <a name="see-also"></a><span data-ttu-id="24129-119">См. также</span><span class="sxs-lookup"><span data-stu-id="24129-119">See Also</span></span>
[<span data-ttu-id="24129-120">Настройка управления отношениями</span><span class="sxs-lookup"><span data-stu-id="24129-120">Setting Up Relationship Management</span></span>](marketing-setup-marketing.md)  
[<span data-ttu-id="24129-121">Присвоение групп рассылки контакту</span><span class="sxs-lookup"><span data-stu-id="24129-121">Assigning Mailing Groups to a Contact</span></span>](marketing-mailing-groups.md#AssignMailGroupContact)  
[<span data-ttu-id="24129-122">Настройка должностных обязанностей в контактах</span><span class="sxs-lookup"><span data-stu-id="24129-122">Set Up Job Responsibilities on Contacts</span></span>](marketing-job-responsibilities.md)  
[<span data-ttu-id="24129-123">Настройка организационных уровней для контактных лиц</span><span class="sxs-lookup"><span data-stu-id="24129-123">Set Up Organizational Levels for Contact Persons</span></span>](marketing-organizational-levels.md)  
[<span data-ttu-id="24129-124">Синхронизация контактов с клиентами, поставщиками и банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="24129-124">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span></span>](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[<span data-ttu-id="24129-125">Использование анкет профилей для классификации бизнес-контактов</span><span class="sxs-lookup"><span data-stu-id="24129-125">Use Profile Questionnaires to Classify Business Contacts</span></span>](marketing-create-contact-profile-questionnaire.md)  
[<span data-ttu-id="24129-126">Работа с Business Central</span><span class="sxs-lookup"><span data-stu-id="24129-126">Working with Business Central</span></span>](ui-work-product.md)  

