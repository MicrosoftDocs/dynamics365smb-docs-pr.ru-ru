---
title: Синхронизация контактов с клиентами и поставщиками | Документы Майкрософт
description: Вы можете связать или синхронизировать информацию о контактах, т. е. о клиентах, поставщиках или банковских счетах, чтобы централизованно обновлять эту информацию.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, CRM, integration, couple
ms.date: 04/01/2019
ms.author: edupont
redirect_url: marketing-create-contact-companies
ms.openlocfilehash: 96ec0862cf93cf9b0bf240ef65bc7ff79b3ccfb5
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "934076"
---
# <a name="synchronizing-contacts-with-customers-vendors-and-bank-accounts"></a><span data-ttu-id="93158-103">Синхронизация контактов с клиентами, поставщиками и банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="93158-103">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span></span>
<span data-ttu-id="93158-104">Если какие-то контакты являются еще и клиентами, поставщиками или банковскими счетами, можно синхронизировать контактную информацию с соответствующим клиентом, поставщиком или банковским счетом.</span><span class="sxs-lookup"><span data-stu-id="93158-104">If some of your contacts are also customers, vendors, or bank accounts, you can synchronize the contact information with the related customer, vendor, or bank account.</span></span> <span data-ttu-id="93158-105">Синхронизация делает общую информацию между контактами и клиентами, поставщиками или банковским счетом одинаковой.</span><span class="sxs-lookup"><span data-stu-id="93158-105">Synchronization makes information that is common between contacts and customers, vendors, or bank account the same.</span></span>  

## <a name="different-ways-to-synchronize-contacts-with-customers-vendors-and-bank-accounts"></a><span data-ttu-id="93158-106">Различные способы синхронизации контактов с клиентами, поставщиками и банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="93158-106">Different Ways to Synchronize Contacts with Customers, Vendors and Bank Accounts</span></span>
<span data-ttu-id="93158-107">Контакты можно синхронизировать с заказчиками, поставщиками или банковскими счетами тремя способами:</span><span class="sxs-lookup"><span data-stu-id="93158-107">You can synchronize your contacts with customers, vendors, or bank accounts by three methods:</span></span>

* <span data-ttu-id="93158-108">Свяжите контакты с имеющимися клиентами, поставщиками или банковскими счетами.</span><span class="sxs-lookup"><span data-stu-id="93158-108">Link contacts with existing customers, vendors, or bank accounts from the contact card.</span></span> <span data-ttu-id="93158-109">Дополнительные сведения см. в разделе [Связывание контактов с клиентами, поставщиками и банковскими счетами](marketing-how-link-contact.md).</span><span class="sxs-lookup"><span data-stu-id="93158-109">For more information, see [Link Contacts With Customers, Vendors, and Bank Accounts](marketing-how-link-contact.md).</span></span>
* <span data-ttu-id="93158-110">Создавайте клиентов, поставщиков или банковские счета из контакта.</span><span class="sxs-lookup"><span data-stu-id="93158-110">Create customers, vendors, or bank accounts from the contact.</span></span> <span data-ttu-id="93158-111">Дополнительные сведения см. в разделе [Создание клиента, поставщика или банковского счета из клиента](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="93158-111">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span></span>
* <span data-ttu-id="93158-112">Создать контакты из клиентов, поставщиков или банковских счетов.</span><span class="sxs-lookup"><span data-stu-id="93158-112">Create contacts from customers, vendors or bank accounts.</span></span> <span data-ttu-id="93158-113">Дополнительные сведения см. в разделе [Создание контакта организации из клиента, поставщика или банковского счета](marketing-how-create-contact-companies.md).</span><span class="sxs-lookup"><span data-stu-id="93158-113">For more information, see [Create a company contact from a customer, vendor, or bank account](marketing-how-create-contact-companies.md).</span></span>

## <a name="consequences-of-synchronization"></a><span data-ttu-id="93158-114">Последствия синхронизации</span><span class="sxs-lookup"><span data-stu-id="93158-114">Consequences of Synchronization</span></span>
<span data-ttu-id="93158-115">Когда контакт синхронизирован с клиентом, поставщиком или банковским счетом:</span><span class="sxs-lookup"><span data-stu-id="93158-115">When the contact is synchronized with the customer, vendor, bank account:</span></span>

* <span data-ttu-id="93158-116">Необходимо обновить информацию только в одном месте.</span><span class="sxs-lookup"><span data-stu-id="93158-116">You only have to update information in one place.</span></span> <span data-ttu-id="93158-117">Например, если изменить номер телефона в контакте, те же изменения будут автоматически внесены в запись клиента, поставщика или банковского счета.</span><span class="sxs-lookup"><span data-stu-id="93158-117">For example, if you modify the phone number on the contact, the phone number is automatically updated with the same modification on the customer, the vendor, or the bank account.</span></span>
* <span data-ttu-id="93158-118">Если была указана серия номеров для контактов, при создании карточки клиента, поставщика или банковского счета будет автоматически создана карточка контакта для клиента, поставщика или банковского счета.</span><span class="sxs-lookup"><span data-stu-id="93158-118">If you have specified a number series for contacts, when you create a customer card, a vendor card, or a bank account card, a contact card is automatically created for the customer, vendor or bank account.</span></span>
* <span data-ttu-id="93158-119">Непосредственно из контакта можно создавать предложения и заказы на продажу, а также предложения и заказы на покупку;</span><span class="sxs-lookup"><span data-stu-id="93158-119">You can create sales quotes and orders, and purchase quotes and orders from the contact.</span></span>
* <span data-ttu-id="93158-120">Можно регистрировать взаимодействия при выполнении действий, таких как печать заказов и общих заказов, создание сервисных заказов на продажу, отправка сообщений электронной почты и т. д.</span><span class="sxs-lookup"><span data-stu-id="93158-120">You can have your interactions recorded when you perform actions such as printing orders, blanket orders, creating sales service orders, sending e-mails, and so on.</span></span>
* <span data-ttu-id="93158-121">При удалении контакта, связанного с клиентом, поставщиком или банковским счетом, удаляется только контакт.</span><span class="sxs-lookup"><span data-stu-id="93158-121">If you delete a contact linked to a customer, vendor or bank account, only the contact is removed.</span></span> <span data-ttu-id="93158-122">Клиент, поставщик или банковский счет остаются.</span><span class="sxs-lookup"><span data-stu-id="93158-122">The customer, vendor, or bank account remains.</span></span>
* <span data-ttu-id="93158-123">При удалении клиента, поставщика или банковского счета, связанного с контактом, контакт сохраняется.</span><span class="sxs-lookup"><span data-stu-id="93158-123">If you delete a customer, vendor, bank account linked to a contact, the contact remains.</span></span>

> [!NOTE]  
>   <span data-ttu-id="93158-124">Некоторые подробности, например сведения о счетах и учете, не отображаются в карточке контакта.</span><span class="sxs-lookup"><span data-stu-id="93158-124">Some details, such as invoicing and posting details, do not appear on the contact card.</span></span> <span data-ttu-id="93158-125">Следовательно, может потребоваться добавить их вручную в карточку клиента, поставщика или банковского счета при создании контактов как клиентов, поставщиков или банковских счетов.</span><span class="sxs-lookup"><span data-stu-id="93158-125">Therefore, you may want to add them manually on the customer card, vendor card, or bank account card when you create contacts as customers, vendors or bank accounts.</span></span>

## <a name="see-also"></a><span data-ttu-id="93158-126">См. также</span><span class="sxs-lookup"><span data-stu-id="93158-126">See Also</span></span>
[<span data-ttu-id="93158-127">Управление контактами</span><span class="sxs-lookup"><span data-stu-id="93158-127">Managing Contacts</span></span>](marketing-contacts.md)  
<span data-ttu-id="93158-128">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="93158-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
