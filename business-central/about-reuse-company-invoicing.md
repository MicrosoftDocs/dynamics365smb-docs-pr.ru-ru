---
title: "Использование Invoicing и Business Central | Документы Майкрософт"
description: "Обходное решение для доступа к Microsoft Invoicing при регистрации на Dynamics 365 Business Central."
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/26/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: add32e82465610830b68a979e238103bfa10d438
ms.openlocfilehash: 95213b7d5881945bb2880e6288eef1b415427ca5
ms.contentlocale: ru-ru
ms.lasthandoff: 11/29/2018

---
# <a name="using-the-same-office-365-account-in-included365finincludesd365finlongmdmd-and-microsoft-invoicing"></a><span data-ttu-id="26c2c-103">Использование одной и той же учетной записи Office 365 в [!INCLUDE[d365fin](includes/d365fin_long_md.md)] и Microsoft Invoicing</span><span class="sxs-lookup"><span data-stu-id="26c2c-103">Using the same Office 365 Account in [!INCLUDE[d365fin](includes/d365fin_long_md.md)] and Microsoft Invoicing</span></span>
<span data-ttu-id="26c2c-104">При регистрации на пробную версию [!INCLUDE[d365fin](includes/d365fin_md.md)] можно перейти на 30-дневную фазу оценки, начать подписку или прекратить использование [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="26c2c-104">When you sign up for a trial with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can move to a 30-day evaluation phase, you can start a subscription, or you can stop using [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="26c2c-105">Во всех случаях при входе на портал Office может отобразиться плитка **Microsoft Invoicing**, которую можно нажать.</span><span class="sxs-lookup"><span data-stu-id="26c2c-105">In all cases, if you log into the Office Portal, you might see a tile called **Microsoft Invoicing** and click it.</span></span> <span data-ttu-id="26c2c-106">Это часть подписки Office 365 Business Premium, поэтому не все пользователи увидят эту плитку на портале Office.</span><span class="sxs-lookup"><span data-stu-id="26c2c-106">This is part of the Office 365 Business Premium subscription, so not everyone will see that tile in the Office Portal.</span></span>  

<span data-ttu-id="26c2c-107">Если открыть Microsoft Invoicing, отобразится сообщение о невозможности получить доступ к Microsoft Invoicing, поскольку ваша учетная запись используется в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="26c2c-107">If you access Microsoft Invoicing, you will see a message that you cannot access Microsoft Invoicing because your account is used in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="26c2c-108">Подобное сообщение отображается при установке мобильного приложения для Invoicing.</span><span class="sxs-lookup"><span data-stu-id="26c2c-108">You see a similar message if you install the mobile app for Invoicing.</span></span>  

## <a name="workaround"></a><span data-ttu-id="26c2c-109">Обходное решение</span><span class="sxs-lookup"><span data-stu-id="26c2c-109">Workaround</span></span>
<span data-ttu-id="26c2c-110">Invoicing и [!INCLUDE[d365fin](includes/d365fin_md.md)] используют одну и ту же платформу.</span><span class="sxs-lookup"><span data-stu-id="26c2c-110">Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)] have a shared platform.</span></span> <span data-ttu-id="26c2c-111">Это означает, что вы распознаетесь как существующий пользователь [!INCLUDE[d365fin](includes/d365fin_md.md)] при нажатии Invoicing в бизнес-центре.</span><span class="sxs-lookup"><span data-stu-id="26c2c-111">That means that you are recognized as an existing user of [!INCLUDE[d365fin](includes/d365fin_md.md)] when you click Invoicing in the Business center.</span></span> <span data-ttu-id="26c2c-112">Причиной этого является то, что Invoicing не может использовать ту же организацию, что и [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="26c2c-112">The reason is that Invoicing cannot use the same company as [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="26c2c-113">Поэтому вам следует выполнить вход в [!INCLUDE[d365fin](includes/d365fin_md.md)] и переименовать существующую организацию, а затем создать новую организацию, которую можно использовать в Invoicing.</span><span class="sxs-lookup"><span data-stu-id="26c2c-113">So you will have to log into [!INCLUDE[d365fin](includes/d365fin_md.md)] and rename your existing company, and then create a new company that you can then use in Invoicing.</span></span> <span data-ttu-id="26c2c-114">В этом обходном решении данные не перемещаются и не перезаписываются.</span><span class="sxs-lookup"><span data-stu-id="26c2c-114">No data is moved or overwritten during this workaround.</span></span>

### <a name="to-rename-your-company"></a><span data-ttu-id="26c2c-115">Переименование организации</span><span class="sxs-lookup"><span data-stu-id="26c2c-115">To rename your company</span></span>
1.  <span data-ttu-id="26c2c-116">Войдите в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="26c2c-116">Sign in to your [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
2.  <span data-ttu-id="26c2c-117">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Компании**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="26c2c-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Companies**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="26c2c-118">На странице **Организации** нажмите кнопку **Изменить список**.</span><span class="sxs-lookup"><span data-stu-id="26c2c-118">On the **Companies** page, choose the **Edit List** button.</span></span>  
4.  <span data-ttu-id="26c2c-119">Измените имя записи *Моя организация* на другое.</span><span class="sxs-lookup"><span data-stu-id="26c2c-119">Change the name of the *My Company* entry to something else.</span></span>  

    <span data-ttu-id="26c2c-120">Подождите несколько минут.</span><span class="sxs-lookup"><span data-stu-id="26c2c-120">Wait a number of minutes.</span></span> <span data-ttu-id="26c2c-121">Будут внесены некоторые изменения в основную базу данных, что займет некоторое время.</span><span class="sxs-lookup"><span data-stu-id="26c2c-121">We’ll be making a number of changes in the underlying database, and that takes a while.</span></span>
5.  <span data-ttu-id="26c2c-122">После того, как система будет готова к работе, нажмите кнопку **Создать новую организацию**.</span><span class="sxs-lookup"><span data-stu-id="26c2c-122">When the system is ready again, choose the **Create New Company** button.</span></span>  
6.  <span data-ttu-id="26c2c-123">В открывшемся диалоговом окне укажите имя как *Моя организация* и выберите параметр **Производственный выпуск — только данные настройки**.</span><span class="sxs-lookup"><span data-stu-id="26c2c-123">In the dialog that appears, specify the name as *My Company*, and choose the **Production – Setup Data Only** option.</span></span>  

<span data-ttu-id="26c2c-124">Выполнение этой операции также займет несколько минут.</span><span class="sxs-lookup"><span data-stu-id="26c2c-124">This again takes a number of minutes.</span></span> <span data-ttu-id="26c2c-125">По завершении процесса можно будет получить доступ к Invoicing в рамках Office 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="26c2c-125">When the process completes, you will be able to access Invoicing as part of your Office 365 Business Premium experience.</span></span>  

### <a name="what-about-my-data"></a><span data-ttu-id="26c2c-126">Что происходит с данными?</span><span class="sxs-lookup"><span data-stu-id="26c2c-126">What about my data?</span></span>
<span data-ttu-id="26c2c-127">При переименовании имени первоначальной организации таблицы баз данных, в которых хранятся существующие данные [!INCLUDE[d365fin](includes/d365fin_md.md)], будут переименованы, но сами данные не будут изменены.</span><span class="sxs-lookup"><span data-stu-id="26c2c-127">When you rename the original My Company, the database tables that store your existing [!INCLUDE[d365fin](includes/d365fin_md.md)] data are renamed, but the data itself is not touched.</span></span>  

<span data-ttu-id="26c2c-128">Если используется и Invoicing, и [!INCLUDE[d365fin](includes/d365fin_md.md)], данные хранятся в двух различных контейнерах (двух организациях).</span><span class="sxs-lookup"><span data-stu-id="26c2c-128">If you use both Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)], the data is stored in two different containers (the two companies).</span></span> <span data-ttu-id="26c2c-129">Данные не используются совместно, поэтому потребуется управлять клиентами и товарами в обеих организациях.</span><span class="sxs-lookup"><span data-stu-id="26c2c-129">Nothing is shared, so you'll have to manage customers and items in both companies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="26c2c-130">См. также</span><span class="sxs-lookup"><span data-stu-id="26c2c-130">See Also</span></span>
[<span data-ttu-id="26c2c-131">Вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="26c2c-131">Frequently Asked Questions</span></span>](across-faq.md)  
[<span data-ttu-id="26c2c-132">Администрация</span><span class="sxs-lookup"><span data-stu-id="26c2c-132">Administration</span></span>](admin-setup-and-administration.md)  

