---
title: Использование Invoicing и Business Central | Документы Майкрософт
description: Обходное решение для доступа к Microsoft Invoicing при регистрации на Dynamics 365 Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Invoicing, Office 365
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: 0173d64e140cfea91bf7f08d821c2d30cf0eb7b3
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1241488"
---
# <a name="using-the-same-office-365-account-in-included365finincludesd365finlongmdmd-and-microsoft-invoicing"></a><span data-ttu-id="07139-103">Использование одной и той же учетной записи Office 365 в [!INCLUDE[d365fin](includes/d365fin_long_md.md)] и Microsoft Invoicing</span><span class="sxs-lookup"><span data-stu-id="07139-103">Using the same Office 365 Account in [!INCLUDE[d365fin](includes/d365fin_long_md.md)] and Microsoft Invoicing</span></span>
<span data-ttu-id="07139-104">При регистрации на пробную версию [!INCLUDE[d365fin](includes/d365fin_md.md)] можно перейти на 30-дневную фазу оценки, начать подписку или прекратить использование [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07139-104">When you sign up for a trial with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can move to a 30-day evaluation phase, you can start a subscription, or you can stop using [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="07139-105">Во всех случаях при входе на портал Office может отобразиться плитка **Microsoft Invoicing**, которую можно нажать.</span><span class="sxs-lookup"><span data-stu-id="07139-105">In all cases, if you sign in to the Office Portal, you might see a tile called **Microsoft Invoicing** and click it.</span></span> <span data-ttu-id="07139-106">Это часть подписки Office 365 Business Premium, поэтому не все пользователи увидят эту плитку на портале Office.</span><span class="sxs-lookup"><span data-stu-id="07139-106">This is part of the Office 365 Business Premium subscription, so not everyone will see that tile in the Office Portal.</span></span>  

<span data-ttu-id="07139-107">Если открыть Microsoft Invoicing, отобразится сообщение о невозможности получить доступ к Microsoft Invoicing, поскольку ваша учетная запись используется в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07139-107">If you access Microsoft Invoicing, you will see a message that you cannot access Microsoft Invoicing because your account is used in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="07139-108">Подобное сообщение отображается при установке мобильного приложения для Invoicing.</span><span class="sxs-lookup"><span data-stu-id="07139-108">You see a similar message if you install the mobile app for Invoicing.</span></span>  

## <a name="workaround"></a><span data-ttu-id="07139-109">Обходное решение</span><span class="sxs-lookup"><span data-stu-id="07139-109">Workaround</span></span>
<span data-ttu-id="07139-110">Invoicing и [!INCLUDE[d365fin](includes/d365fin_md.md)] используют одну и ту же платформу.</span><span class="sxs-lookup"><span data-stu-id="07139-110">Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)] have a shared platform.</span></span> <span data-ttu-id="07139-111">Это означает, что вы распознаетесь как существующий пользователь [!INCLUDE[d365fin](includes/d365fin_md.md)] при нажатии Invoicing на портале Office.</span><span class="sxs-lookup"><span data-stu-id="07139-111">That means that you are recognized as an existing user of [!INCLUDE[d365fin](includes/d365fin_md.md)] when you click Invoicing in the Office Portal.</span></span> <span data-ttu-id="07139-112">Причиной этого является то, что Invoicing не может использовать ту же организацию, что и [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07139-112">The reason is that Invoicing cannot use the same company as [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="07139-113">Поэтому вам следует выполнить вход в [!INCLUDE[d365fin](includes/d365fin_md.md)] и переименовать существующую организацию, а затем создать новую организацию, которую можно использовать в Invoicing.</span><span class="sxs-lookup"><span data-stu-id="07139-113">So you will have to sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)] and rename your existing company, and then create a new company that you can then use in Invoicing.</span></span> <span data-ttu-id="07139-114">В этом обходном решении данные не перемещаются и не перезаписываются.</span><span class="sxs-lookup"><span data-stu-id="07139-114">No data is moved or overwritten during this workaround.</span></span>

### <a name="to-rename-your-company"></a><span data-ttu-id="07139-115">Переименование организации</span><span class="sxs-lookup"><span data-stu-id="07139-115">To rename your company</span></span>
1. <span data-ttu-id="07139-116">Выполните вход в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07139-116">Sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>
2. <span data-ttu-id="07139-117">В правом верхнем углу щелкните значок **Параметры** ![Параметры](media/ui-experience/settings_icon_small.png "Значок \"Параметры\" для ролевого центра"), а затем выберите **Мои настройки**.</span><span class="sxs-lookup"><span data-stu-id="07139-117">In the top right corner, choose the **Settings** icon ![Settings](media/ui-experience/settings_icon_small.png "Settings icon for role center"), and then choose **My Settings**.</span></span>
3. <span data-ttu-id="07139-118">В поле **Организация** выберите другую организацию.</span><span class="sxs-lookup"><span data-stu-id="07139-118">In the **Company** field, choose a different company.</span></span>
4. <span data-ttu-id="07139-119">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Компании**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="07139-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Companies**, and then choose the related link.</span></span>  
5. <span data-ttu-id="07139-120">На странице **Организации** выберите **Изменить список**.</span><span class="sxs-lookup"><span data-stu-id="07139-120">On the **Companies** page, choose **Edit List**.</span></span>  
6. <span data-ttu-id="07139-121">Измените имя записи *Моя организация* на другое.</span><span class="sxs-lookup"><span data-stu-id="07139-121">Change the name of the *My Company* entry to something else.</span></span>  

    <span data-ttu-id="07139-122">Подождите несколько минут.</span><span class="sxs-lookup"><span data-stu-id="07139-122">Wait a number of minutes.</span></span> <span data-ttu-id="07139-123">Будут внесены некоторые изменения в основную базу данных, что займет некоторое время.</span><span class="sxs-lookup"><span data-stu-id="07139-123">We’ll be making a number of changes in the underlying database, and that takes a while.</span></span>
7.  <span data-ttu-id="07139-124">После того, как система будет готова к работе, нажмите кнопку **Создать новую организацию**.</span><span class="sxs-lookup"><span data-stu-id="07139-124">When the system is ready again, choose the **Create New Company** button.</span></span>  
8.  <span data-ttu-id="07139-125">В открывшемся диалоговом окне укажите имя как *Моя организация* и выберите параметр **Производственный выпуск — только данные настройки**.</span><span class="sxs-lookup"><span data-stu-id="07139-125">In the dialog that appears, specify the name as *My Company*, and choose the **Production – Setup Data Only** option.</span></span>  

<span data-ttu-id="07139-126">Выполнение этой операции также займет несколько минут.</span><span class="sxs-lookup"><span data-stu-id="07139-126">This again takes a number of minutes.</span></span> <span data-ttu-id="07139-127">По завершении процесса можно будет получить доступ к Invoicing в рамках Office 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="07139-127">When the process completes, you will be able to access Invoicing as part of your Office 365 Business Premium experience.</span></span>  

### <a name="what-about-my-data"></a><span data-ttu-id="07139-128">Что происходит с данными?</span><span class="sxs-lookup"><span data-stu-id="07139-128">What about my data?</span></span>
<span data-ttu-id="07139-129">При переименовании имени первоначальной организации таблицы баз данных, в которых хранятся существующие данные [!INCLUDE[d365fin](includes/d365fin_md.md)], будут переименованы, но сами данные не будут изменены.</span><span class="sxs-lookup"><span data-stu-id="07139-129">When you rename the original My Company, the database tables that store your existing [!INCLUDE[d365fin](includes/d365fin_md.md)] data are renamed, but the data itself is not touched.</span></span>  

<span data-ttu-id="07139-130">Если используется и Invoicing, и [!INCLUDE[d365fin](includes/d365fin_md.md)], данные хранятся в двух различных контейнерах (двух организациях).</span><span class="sxs-lookup"><span data-stu-id="07139-130">If you use both Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)], the data is stored in two different containers (the two companies).</span></span> <span data-ttu-id="07139-131">Данные не используются совместно, поэтому потребуется управлять клиентами и товарами в обеих организациях.</span><span class="sxs-lookup"><span data-stu-id="07139-131">Nothing is shared, so you'll have to manage customers and items in both companies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="07139-132">См. также</span><span class="sxs-lookup"><span data-stu-id="07139-132">See Also</span></span>
[<span data-ttu-id="07139-133">Вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="07139-133">Frequently Asked Questions</span></span>](across-faq.md)  
[<span data-ttu-id="07139-134">Администрация</span><span class="sxs-lookup"><span data-stu-id="07139-134">Administration</span></span>](admin-setup-and-administration.md)  
