---
title: "Создание клиента или поставщика из контакта | Microsoft Docs"
description: "Вы можете сохранить существующий контакт как клиента, поставщика или банковский счет с помощью имеющихся данных и указав деловое отношение."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, client, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 0c4cf74ef7b0b2e48a8608a0859a71b919e46397
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="create-a-customer-vendor-or-bank-account-from-a-contact"></a><span data-ttu-id="3d8a9-103">Создание клиента, поставщика или банковского счета из клиента</span><span class="sxs-lookup"><span data-stu-id="3d8a9-103">Create a Customer, Vendor, or Bank Account From a Contact</span></span>
<span data-ttu-id="3d8a9-104">Вам может понадобиться записать некоторые существующие контакты как клиентов, поставщиков или банковские счета.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-104">You may want to record some of your existing contacts as customers, vendors, or bank accounts.</span></span> <span data-ttu-id="3d8a9-105">Создание клиента, поставщика или банковского счета из контакта позволяет использовать существующие данные.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-105">Creating a customer, vendor, or bank account from a contact enables you use existing data.</span></span> <span data-ttu-id="3d8a9-106">При создании клиента, поставщика или банковского счета таким образом они синхронизируются с контактом.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-106">When you create a customer, vendor, or bank account this way, it is synchronized with the contact.</span></span> <span data-ttu-id="3d8a9-107">Синхронизация делает общую информацию между контактами и клиентами, поставщиками или банковским счетом одинаковой.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-107">Synchronization makes information that is common between contacts and customers, vendors, or bank account the same.</span></span>

<span data-ttu-id="3d8a9-108">Прежде чем можно будет записывать контакты таким образом, необходимо указать код бизнес-отношений для клиентов, поставщиков или банковских счетов в окне **Настройка модуля Маркетинг**.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-108">Before you can record contacts this way, you must specify a business relation code for customers, vendors, and bank accounts in the **Marketing Setup** window.</span></span> <span data-ttu-id="3d8a9-109">Если вы будет записывать контакты как банковские счета, вы должны также указать серии номеров для банковских счетов в окне **Настройка ГК**.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-109">If you will be recording contacts as bank accounts, you must also specify numbers series for bank accounts in the **General Ledger Setup** window.</span></span>

## <a name="to-create-a-contact-as-a-customer-vendor-or-bank-account"></a><span data-ttu-id="3d8a9-110">Создание контакта в качестве клиента, поставщика или банковского счета</span><span class="sxs-lookup"><span data-stu-id="3d8a9-110">To create a contact as a customer, vendor, or bank account</span></span>
1. <span data-ttu-id="3d8a9-111">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Контакты**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Contacts**, and then choose the related link.</span></span>
2. <span data-ttu-id="3d8a9-112">Выберите контакт, который требуется создать как клиента, поставщика или банковский счет.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-112">Select the contact you want to create as a customer, vendor, or bank account.</span></span>
3. <span data-ttu-id="3d8a9-113">Выберите действие **Создать как**, а затем выберите **Клиент**, **Поставщик** или **Банк**.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-113">Choose the **Create As** action, and then choose either **Customer**, **Vendor**, or **Bank**.</span></span>
4. <span data-ttu-id="3d8a9-114">Подтвердите удаление в появившемся окне.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-114">Confirm the subsequent message.</span></span>

<span data-ttu-id="3d8a9-115">Сведения о контакте перемещаются из карточки **Контакт** в карточку **Банковский счет**, карточку **Клиент** или карточку **Поставщик**.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-115">The contact information is transferred from the **Contact** card to the **Bank Account** card, the **Customer** card, or the **Vendor** card.</span></span> <span data-ttu-id="3d8a9-116">Может возникнуть необходимость добавить определенные сведения в каждую карточку, например о счетах и оплате.</span><span class="sxs-lookup"><span data-stu-id="3d8a9-116">You may want to add specific information to each of the cards, such as invoicing and payment details.</span></span>

## <a name="see-also"></a><span data-ttu-id="3d8a9-117">См. также</span><span class="sxs-lookup"><span data-stu-id="3d8a9-117">See Also</span></span>
[<span data-ttu-id="3d8a9-118">Создание контактных организаций</span><span class="sxs-lookup"><span data-stu-id="3d8a9-118">Create Contact Companies</span></span>](marketing-create-contact-companies.md)  
[<span data-ttu-id="3d8a9-119">Создание контактных лиц</span><span class="sxs-lookup"><span data-stu-id="3d8a9-119">Create Contact Persons</span></span>](marketing-create-contact-persons.md)  
[<span data-ttu-id="3d8a9-120">Настройка управления отношениями</span><span class="sxs-lookup"><span data-stu-id="3d8a9-120">Setting Up Relationship Management</span></span>](marketing-setup-marketing.md)  
[<span data-ttu-id="3d8a9-121">Синхронизация контактов с клиентами, поставщиками и банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="3d8a9-121">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span></span>](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[<span data-ttu-id="3d8a9-122">Связывание контактов с существующими клиентами, поставщиками или банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="3d8a9-122">Link Contacts to Existing Customers, Vendors, or Bank Accounts</span></span>](marketing-how-link-contact.md)  
[<span data-ttu-id="3d8a9-123">Назначение деловых отношений контакту</span><span class="sxs-lookup"><span data-stu-id="3d8a9-123">Assign Business Relations to a Contact</span></span>](marketing-business-relations.md#AssignBusRelContact)  
[<span data-ttu-id="3d8a9-124">Работа с Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="3d8a9-124">Working with Finance and Operations, Business edition</span></span>](ui-work-product.md)

