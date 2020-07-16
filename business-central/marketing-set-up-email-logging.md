---
title: Настройка регистрации электронной почты | Документация Майкрософт
description: Узнайте, как превратить взаимодействие по электронной почте между продавцами и клиентами в реальные возможности продаж.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect, opportunity, email
ms.date: 07/01/2020
ms.author: bholtorf
ms.openlocfilehash: 9ca381bfebcd6db8e67d8153d4d2bc17eeffad81
ms.sourcegitcommit: f9aec4a72172d9270e14e2938c5550d69508f1aa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2020
ms.locfileid: "3532673"
---
# <a name="track-email-message-exchanges-between-salespeople-and-contacts"></a><span data-ttu-id="67e91-103">Отслеживание обмена сообщениями электронной почты между продавцами и контактами</span><span class="sxs-lookup"><span data-stu-id="67e91-103">Track Email Message Exchanges Between Salespeople and Contacts</span></span>

<span data-ttu-id="67e91-104">Получите больше от общения между продавцами и вашими существующими или потенциальными клиентами, отслеживая обмен сообщениями электронной почты, затем превращая их в реальные возможности.</span><span class="sxs-lookup"><span data-stu-id="67e91-104">Get more out of the communications between salespeople and your existing or potential customers by tracking email exchanges, and then turning them into actionable opportunities.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="67e91-105">может работать с Exchange Online, чтобы вести журнал входящих и исходящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="67e91-105">can work with Exchange Online to keep a log of the inbound and outbound messages.</span></span> <span data-ttu-id="67e91-106">Вы можете просматривать и анализировать содержимое каждого сообщения на странице **Журналы взаимодействий**.</span><span class="sxs-lookup"><span data-stu-id="67e91-106">You can view and analyze the contents of each message on the **Interaction Log Entries** page.</span></span>

## <a name="set-up-public-folders-and-rules-for-email-logging-in-exchange-online"></a><span data-ttu-id="67e91-107">Настройка общих папок и правил для регистрации электронной почты в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="67e91-107">Set up Public Folders and Rules for Email Logging in Exchange Online</span></span>

[!INCLUDE[admin-setup-email-public-folder](includes/admin-setup-email-public-folder.md)]

<span data-ttu-id="67e91-108">Далее вы подключаете [!INCLUDE[prodshort](includes/prodshort.md)] с Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="67e91-108">Next, you connect [!INCLUDE[prodshort](includes/prodshort.md)] with Exchange Online.</span></span>

## <a name="setting-up-d365fin-to-log-email-messages"></a><span data-ttu-id="67e91-109">Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] для регистрации сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="67e91-109">Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)] to Log Email Messages</span></span>

<span data-ttu-id="67e91-110">Начните работать с регистрацией электронной почты за два простых шага:</span><span class="sxs-lookup"><span data-stu-id="67e91-110">Get started with email logging in two easy steps:</span></span>

1. <span data-ttu-id="67e91-111">Соедините [!INCLUDE[d365fin](includes/d365fin_md.md)] с Exchange Online для подписки Office 365.</span><span class="sxs-lookup"><span data-stu-id="67e91-111">Connect [!INCLUDE[d365fin](includes/d365fin_md.md)] with Exchange Online for your Office 365 subscription.</span></span> <span data-ttu-id="67e91-112">Exchange Online обрабатывает ваши сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="67e91-112">Exchange Online handles your email messages.</span></span> <span data-ttu-id="67e91-113">Мы упростили этот шаг, предоставив мастер настройки.</span><span class="sxs-lookup"><span data-stu-id="67e91-113">We've made this step easy by providing an assisted setup guide.</span></span> <span data-ttu-id="67e91-114">Вам просто нужны ваши учетные данные администратора для вашей учетной записи администратора в Office 365.</span><span class="sxs-lookup"><span data-stu-id="67e91-114">You just need your administrator credentials for your administrator account in Office 365.</span></span> <span data-ttu-id="67e91-115">Чтобы запустить руководство, выберите **Мастер настройки**, затем выберите **Настройка регистрации электронной почты**.</span><span class="sxs-lookup"><span data-stu-id="67e91-115">To start the guide, go to **Assisted Setup**, and then choose **Set up email logging**.</span></span>  

2. <span data-ttu-id="67e91-116">Убедитесь, что действительные адреса электронной почты были введены в [!INCLUDE[d365fin](includes/d365fin_md.md)] для ваших продавцов и контактов, в зависимости от того, являются ли они потенциальными или существующими клиентами.</span><span class="sxs-lookup"><span data-stu-id="67e91-116">Make sure that valid email addresses have been entered in [!INCLUDE[d365fin](includes/d365fin_md.md)] for your sales people and contacts, depending on whether they are potential or existing customers.</span></span> <span data-ttu-id="67e91-117">Для этого для каждого клиента или продавца откройте карточку **Контакт** или **Менеджер по продажам/закупкам** и посмотрите в поле **Адрес эл. почты**.</span><span class="sxs-lookup"><span data-stu-id="67e91-117">To do that, for each customer or salesperson, open the **Contact** or **Salesperson/Purchaser** card and have a look in the **Email** field.</span></span>

> [!Tip]
> <span data-ttu-id="67e91-118">После выполнения шагов в руководстве вы можете проверить, было ли соединение успешным.</span><span class="sxs-lookup"><span data-stu-id="67e91-118">After you complete the steps in the guide you can check whether the connection was successful.</span></span> <span data-ttu-id="67e91-119">Выполните поиск **Настройка модуля "Маркетинг"**, выберите **Процесс**, затем **Функции**, потом **Проверить настройку регистрации эл. почты**.</span><span class="sxs-lookup"><span data-stu-id="67e91-119">Search for **Marketing Setup**, choose **Process**, then **Functions**, and then **Validate Email Logging Setup**.</span></span>

## <a name="viewing-email-message-exchanges-in-the-interaction-log"></a><span data-ttu-id="67e91-120">Просмотр обмена сообщениями электронной почты в журнале взаимодействия</span><span class="sxs-lookup"><span data-stu-id="67e91-120">Viewing Email Message Exchanges in the Interaction Log</span></span>

[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="67e91-121">создает запись на странице **Журнал взаимодействия** каждый раз, когда продавец и контакт обмениваются сообщениями электронной почты.</span><span class="sxs-lookup"><span data-stu-id="67e91-121">creates an entry on the **Interaction Log** page each time a salesperson and a contact exchange an email message.</span></span> <span data-ttu-id="67e91-122">Чтобы просмотреть журнал взаимодействия, откройте карточку **Контакт** или **Менеджер по продажам/закупкам** для человека, затем выберите **Навигатор**, **История**, затем выберите **Журналы взаимодействий**.</span><span class="sxs-lookup"><span data-stu-id="67e91-122">To view the interaction log, open the **Contact** or **Salesperson\*Purchaser** card for the person, and then choose **Navigate**, **History**, and then choose **Interaction Log Entries**.</span></span> <span data-ttu-id="67e91-123">Есть несколько вещей, которые мы можем сделать с каждой записью в журнале, например:</span><span class="sxs-lookup"><span data-stu-id="67e91-123">There are a few things we can do with each entry in the log, for example:</span></span>

- <span data-ttu-id="67e91-124">Просмотрите содержимое сообщения электронной почты, которым обменялись собеседники, нажав действие **Показать вложения**.</span><span class="sxs-lookup"><span data-stu-id="67e91-124">View the content of the email message that was exchanged by clicking the **Show Attachments** action.</span></span>
- <span data-ttu-id="67e91-125">Превратите обмен электронной почтой в возможность продажи — если запись выглядит многообещающей, вы можете превратить ее в возможность, а затем управлять ее продвижением к продаже.</span><span class="sxs-lookup"><span data-stu-id="67e91-125">Turn an email exchange into a sales opportunity - If an entry looks promising, you can turn it into an opportunity and then manage its progress toward a sale.</span></span> <span data-ttu-id="67e91-126">Для этого выберите запись, затем выберите действие **Создать возможность**.</span><span class="sxs-lookup"><span data-stu-id="67e91-126">To do that, choose the entry, and then choose the **Create Opportunity** action.</span></span> <span data-ttu-id="67e91-127">Дополнительные сведения см. в разделе [Управление возможностями продаж](marketing-manage-sales-opportunities.md).</span><span class="sxs-lookup"><span data-stu-id="67e91-127">For more information, see [Managing Sales Opportunities](marketing-manage-sales-opportunities.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="67e91-128">См. также</span><span class="sxs-lookup"><span data-stu-id="67e91-128">See Also</span></span>
[<span data-ttu-id="67e91-129">Управление отношениями</span><span class="sxs-lookup"><span data-stu-id="67e91-129">Managing Relationships</span></span>](marketing-relationship-management.md)

