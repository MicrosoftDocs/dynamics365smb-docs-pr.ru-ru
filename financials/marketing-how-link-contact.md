---
title: "Связывание контактов с клиентами и поставщиками | Документы Майкрософт"
description: "Далее описывается процедура связывания контакта с клиентом, поставщиком или банковским счетом из той же компании, чтобы вы могли синхронизировать общие данные."
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
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: f5bbadb37a40dbc7b06668d940d2be9569aaa8e8
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-link-contacts-with-customers-vendors-and-bank-accounts"></a><span data-ttu-id="a449e-103">Практическое руководство. Связывание контактов с клиентами, поставщиками и банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="a449e-103">How to: Link Contacts With Customers, Vendors, and Bank Accounts</span></span>
<span data-ttu-id="a449e-104">Если у вас есть контакт и клиент, поставщик или банковский счет из одной и той же организации, вы можете связать два объекта.</span><span class="sxs-lookup"><span data-stu-id="a449e-104">If you have contact and either a customer, vendor, or bank account for the same company, you can link the two entities.</span></span> <span data-ttu-id="a449e-105">Связывание двух объектов позволяет синхронизировать общие данные, чтобы они были одинаковыми в обоих местах.</span><span class="sxs-lookup"><span data-stu-id="a449e-105">Linking the two entities enables you to synchronize data that is common so that it is the same in both places.</span></span>

## <a name="link-a-contact-to-an-existing-customer-vendor-or-bank-account"></a><span data-ttu-id="a449e-106">Связывание контакта с существующим клиентом, поставщиком или банковским счетом</span><span class="sxs-lookup"><span data-stu-id="a449e-106">Link a Contact to an Existing Customer, Vendor, or Bank Account</span></span>
1. <span data-ttu-id="a449e-107">Откройте контакт, который требуется связать.</span><span class="sxs-lookup"><span data-stu-id="a449e-107">Open the contact that you want to link.</span></span>
2. <span data-ttu-id="a449e-108">Выберите действие **Связать с существующим**, а затем выберите **Клиент**, **Поставщик** или **Банк**.</span><span class="sxs-lookup"><span data-stu-id="a449e-108">Choose the **Link with existing** action, and then choose **Customer**, **Vendor**, or **Bank**.</span></span>
3. <span data-ttu-id="a449e-109">Выберите клиента, поставщика или банковский счет для связывания.</span><span class="sxs-lookup"><span data-stu-id="a449e-109">Select the customer, vendor, or bank account to link to.</span></span>

   <span data-ttu-id="a449e-110">В поле **Текущие главные поля** следует указывать, каким из полей следует отдавать приоритет в случае конфликта информации, общей для контакта и клиента, поставщика или счета.</span><span class="sxs-lookup"><span data-stu-id="a449e-110">In the **Current Master Fields**, you specify which fields should prioritize in case of conflicting information in fields common to the contact and customer, vendor, or account.</span></span> <span data-ttu-id="a449e-111">Например, если код менеджера по продажам в контакте отличается от кода у клиента, можно выбрать **Контакт**, чтобы использовать информацию в контакте.</span><span class="sxs-lookup"><span data-stu-id="a449e-111">For example, if the salesperson code is different in the contact than the customer, you can decide, by selecting **Contact**, to use the information in the contact.</span></span>

## <a name="see-also"></a><span data-ttu-id="a449e-112">См. также</span><span class="sxs-lookup"><span data-stu-id="a449e-112">See Also</span></span>
[<span data-ttu-id="a449e-113">Синхронизация контактов с клиентами, поставщиками и банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="a449e-113">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span></span>](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[<span data-ttu-id="a449e-114">Создание контактов и управление ими</span><span class="sxs-lookup"><span data-stu-id="a449e-114">Creating and Managing Contacts</span></span>](marketing-contacts.md)  
<span data-ttu-id="a449e-115">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a449e-115">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

