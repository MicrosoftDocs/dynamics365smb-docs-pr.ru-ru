---
title: "Использование Invoicing и Finance and Operations, Business edition | Microsoft Docs"
description: "Обходное решение для доступа к Microsoft Invoicing при регистрации в Dynamics 365 for Finance and Operations, Business edition."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/22/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: abceec5b1bc588e2842d0f512240c30eccbf6f8e
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="using-the-same-office-365-account-in-included365finincludesd365finlongmdmd-and-microsoft-invoicing"></a><span data-ttu-id="3daa0-103">Использование одной и той же учетной записи Office 365 в [!INCLUDE[d365fin](includes/d365fin_long_md.md)] и Microsoft Invoicing</span><span class="sxs-lookup"><span data-stu-id="3daa0-103">Using the same Office 365 Account in [!INCLUDE[d365fin](includes/d365fin_long_md.md)] and Microsoft Invoicing</span></span>
<span data-ttu-id="3daa0-104">При регистрации на пробную версию [!INCLUDE[d365fin](includes/d365fin_md.md)] можно перейти на 30-дневную фазу оценки, начать подписку или прекратить использование [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3daa0-104">When you sign up for a trial with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can move to a 30-day evaluation phase, you can start a subscription, or you can stop using [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="3daa0-105">Во всех случаях при входе на портал Office может отобразиться плитка **Бизнес-центр**, которую можно нажать.</span><span class="sxs-lookup"><span data-stu-id="3daa0-105">In all cases, if you log into the Office Portal, you might see a tile called **Business center** and click it.</span></span> <span data-ttu-id="3daa0-106">Это часть подписки Office 365 Business Premium, поэтому не все пользователи увидят эту плитку на портале Office.</span><span class="sxs-lookup"><span data-stu-id="3daa0-106">This is part of the Office 365 Business Premium subscription, so not everyone will see that tile in the Office Portal.</span></span>  

<span data-ttu-id="3daa0-107">При доступе к бизнес-центру отобразится раздел **Выставление счетов**.</span><span class="sxs-lookup"><span data-stu-id="3daa0-107">If you do access the Business center, you will see a section called **Invoicing**.</span></span> <span data-ttu-id="3daa0-108">Если открыть этот раздел, отобразится сообщение о невозможности получить доступ к Microsoft Invoicing, поскольку ваша учетная запись используется в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3daa0-108">If you access that section, you will see a message that you cannot access Microsoft Invoicing because your account is used in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="3daa0-109">Подобное сообщение отображается при установке мобильного приложения для Invoicing.</span><span class="sxs-lookup"><span data-stu-id="3daa0-109">You see a similar message if you install the mobile app for Invoicing.</span></span>  

## <a name="workaround"></a><span data-ttu-id="3daa0-110">Обходное решение</span><span class="sxs-lookup"><span data-stu-id="3daa0-110">Workaround</span></span>
<span data-ttu-id="3daa0-111">Invoicing и [!INCLUDE[d365fin](includes/d365fin_md.md)] используют одну и ту же платформу.</span><span class="sxs-lookup"><span data-stu-id="3daa0-111">Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)] have a shared platform.</span></span> <span data-ttu-id="3daa0-112">Это означает, что вы распознаетесь как существующий пользователь [!INCLUDE[d365fin](includes/d365fin_md.md)] при нажатии Invoicing в бизнес-центре.</span><span class="sxs-lookup"><span data-stu-id="3daa0-112">That means that you are recognized as an existing user of [!INCLUDE[d365fin](includes/d365fin_md.md)] when you click Invoicing in the Business center.</span></span> <span data-ttu-id="3daa0-113">Причиной этого является то, что Invoicing не может использовать ту же организацию, что и [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3daa0-113">The reason is that Invoicing cannot use the same company as [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="3daa0-114">Поэтому вам следует выполнить вход в [!INCLUDE[d365fin](includes/d365fin_md.md)] и переименовать существующую организацию, а затем создать новую организацию, которую можно использовать в Invoicing.</span><span class="sxs-lookup"><span data-stu-id="3daa0-114">So you will have to log into [!INCLUDE[d365fin](includes/d365fin_md.md)] and rename your existing company, and then create a new company that you can then use in Invoicing.</span></span> <span data-ttu-id="3daa0-115">В этом обходном решении данные не перемещаются и не перезаписываются.</span><span class="sxs-lookup"><span data-stu-id="3daa0-115">No data is moved or overwritten during this workaround.</span></span>

### <a name="to-rename-your-company"></a><span data-ttu-id="3daa0-116">Переименование организации</span><span class="sxs-lookup"><span data-stu-id="3daa0-116">To rename your company</span></span>
1.  <span data-ttu-id="3daa0-117">Войдите в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3daa0-117">Sign in to your [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
2.  <span data-ttu-id="3daa0-118">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Организации**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3daa0-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Companies**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="3daa0-119">В окне **Организации** нажмите кнопку **Изменить список**.</span><span class="sxs-lookup"><span data-stu-id="3daa0-119">In the **Companies** window, choose the **Edit List** button.</span></span>  
4.  <span data-ttu-id="3daa0-120">Измените имя записи *Моя организация* на другое.</span><span class="sxs-lookup"><span data-stu-id="3daa0-120">Change the name of the *My Company* entry to something else.</span></span>  

    <span data-ttu-id="3daa0-121">Подождите несколько минут.</span><span class="sxs-lookup"><span data-stu-id="3daa0-121">Wait a number of minutes.</span></span> <span data-ttu-id="3daa0-122">Будут внесены некоторые изменения в основную базу данных, что займет некоторое время.</span><span class="sxs-lookup"><span data-stu-id="3daa0-122">We’ll be making a number of changes in the underlying database, and that takes a while.</span></span>
5.  <span data-ttu-id="3daa0-123">После того, как система будет готова к работе, нажмите кнопку **Создать новую организацию**.</span><span class="sxs-lookup"><span data-stu-id="3daa0-123">When the system is ready again, choose the **Create New Company** button.</span></span>  
6.  <span data-ttu-id="3daa0-124">В открывшемся диалоговом окне укажите имя как *Моя организация* и выберите параметр **Производственный выпуск Suite — только данные настройки**.</span><span class="sxs-lookup"><span data-stu-id="3daa0-124">In the dialog that appears, specify the name as *My Company*, and choose the **Suite Production – Setup Data Only** option.</span></span>  

<span data-ttu-id="3daa0-125">Выполнение этой операции также займет несколько минут.</span><span class="sxs-lookup"><span data-stu-id="3daa0-125">This again takes a number of minutes.</span></span> <span data-ttu-id="3daa0-126">По завершении процесса можно будет получить доступ к Invoicing в рамках Office 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="3daa0-126">When the process completes, you will be able to access Invoicing as part of your Office 365 Business Premium experience.</span></span>  

### <a name="what-about-my-data"></a><span data-ttu-id="3daa0-127">Что происходит с данными?</span><span class="sxs-lookup"><span data-stu-id="3daa0-127">What about my data?</span></span>
<span data-ttu-id="3daa0-128">При переименовании имени первоначальной организации таблицы баз данных, в которых хранятся существующие данные [!INCLUDE[d365fin](includes/d365fin_md.md)], будут переименованы, но сами данные не будут изменены.</span><span class="sxs-lookup"><span data-stu-id="3daa0-128">When you rename the original My Company, the database tables that store your existing [!INCLUDE[d365fin](includes/d365fin_md.md)] data are renamed, but the data itself is not touched.</span></span>  

<span data-ttu-id="3daa0-129">Если используется и Invoicing, и [!INCLUDE[d365fin](includes/d365fin_md.md)], данные хранятся в двух различных контейнерах (двух организациях).</span><span class="sxs-lookup"><span data-stu-id="3daa0-129">If you use both Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)], the data is stored in two different containers (the two companies).</span></span> <span data-ttu-id="3daa0-130">Данные не используются совместно, поэтому потребуется управлять клиентами и товарами в обеих организациях.</span><span class="sxs-lookup"><span data-stu-id="3daa0-130">Nothing is shared, so you'll have to manage customers and items in both companies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3daa0-131">См. также</span><span class="sxs-lookup"><span data-stu-id="3daa0-131">See Also</span></span>
[<span data-ttu-id="3daa0-132">Вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="3daa0-132">Frequently Asked Questions</span></span>](across-faq.md)  
[<span data-ttu-id="3daa0-133">Настройка и администрирование</span><span class="sxs-lookup"><span data-stu-id="3daa0-133">Setup and Administration</span></span>](admin-setup-and-administration.md)  

