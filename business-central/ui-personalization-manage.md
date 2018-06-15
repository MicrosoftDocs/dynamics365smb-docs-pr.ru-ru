---
title: "Управление персонализацией в качестве администратора Financials | Microsoft Docs"
description: "Узнайте, как настраивать пользовательский интерфейс в соответствии с вашим способом работы."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 07/26/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 7c346455a9e27d7274b116754f1d594484b95d67
ms.openlocfilehash: 2d9b45bf21d325e60beadedfc94827d7f3fda075
ms.contentlocale: ru-ru
ms.lasthandoff: 04/18/2018

---
# <a name="managing-personalization-as-an-administrator"></a><span data-ttu-id="fe458-103">Управление персонализацией в качестве администратора</span><span class="sxs-lookup"><span data-stu-id="fe458-103">Managing Personalization as an Administrator</span></span>
<!--NAV in the Web client-->
<span data-ttu-id="fe458-104">Пользователи могут персонализировать свои рабочие области в соответствии со своими предпочтениями.</span><span class="sxs-lookup"><span data-stu-id="fe458-104">Users can personalize their workspace to suit their own preferences.</span></span> <span data-ttu-id="fe458-105">Как администратор, вы можете контролировать персонализацию и управлять ею, отключая для пользователей возможно персонализации страниц и сбрасываю всю персонализацию любой страницы, которую могли сделать пользователи.</span><span class="sxs-lookup"><span data-stu-id="fe458-105">As an administrator, you can control and manage personalization by disabling the ability for users to personalize pages and clearing any page personalizations that users have made.</span></span>

## <a name="disable-personalization-for-a-profile"></a><span data-ttu-id="fe458-106">Отключение персонализации для профиля</span><span class="sxs-lookup"><span data-stu-id="fe458-106">Disable personalization for a profile</span></span>
<span data-ttu-id="fe458-107">Всем пользователям, которые принадлежат к определенному профилю, можно отключить возможность персонализировать их страницы.</span><span class="sxs-lookup"><span data-stu-id="fe458-107">You can prevent all users that belong to a specific profile from being able to personalize their pages.</span></span>
1.  <span data-ttu-id="fe458-108">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Профили**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="fe458-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span></span>
2.  <span data-ttu-id="fe458-109">Выберите профиль в списке, который необходимо изменить.</span><span class="sxs-lookup"><span data-stu-id="fe458-109">Select the profile in the list that you want to modify.</span></span>
3. <span data-ttu-id="fe458-110">Установите флажок **Отключить персонализацию**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="fe458-110">Select the **Disable personalization** check box, and then choose the **OK** button.</span></span>

## <a name="clear-user-personalizations"></a><span data-ttu-id="fe458-111">Очистка пользовательских персонализаций</span><span class="sxs-lookup"><span data-stu-id="fe458-111">Clear user personalizations</span></span>

<span data-ttu-id="fe458-112">При очистки персонализации страницы восстанавливается первоначальный макет страницы до того, как была произведена какая-либо персонализация.</span><span class="sxs-lookup"><span data-stu-id="fe458-112">Clearing page personalization changes the page back to its original layout before any personalization was made.</span></span> <span data-ttu-id="fe458-113">Существует два способа очистить персонализации, которые пользователи сделали на страницах: с помощью страницы **Удалить персонализацию пользователя** и с помощью страницы **Карточка персонализации пользователя**.</span><span class="sxs-lookup"><span data-stu-id="fe458-113">There are two ways to clear the personalizations that users have made to pages: using the **Delete User Personalization** page and using the **User Personalization Card** page.</span></span>

### <a name="clear-user-personalizations-by-using-the-delete-user-personalization-page"></a><span data-ttu-id="fe458-114">Очистка персонализаций пользователя с помощью страницы "Удалить персонализацию пользователя"</span><span class="sxs-lookup"><span data-stu-id="fe458-114">Clear user personalizations by using the Delete User Personalization page</span></span>

<span data-ttu-id="fe458-115">Страница **Удалить персонализацию пользователя** позволяет удалять персонализацию для отдельных страниц для каждого пользователя по-отдельности.</span><span class="sxs-lookup"><span data-stu-id="fe458-115">The **Delete User Personalization** page enables you to clear personalizations on a per-page basis for each user individually.</span></span>

1.  <span data-ttu-id="fe458-116">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Удалить персонализацию пользователя**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="fe458-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="fe458-117">На этой странице отображаются все страницы, которые были персонализированы, и пользователь, которому принадлежит эта страница.</span><span class="sxs-lookup"><span data-stu-id="fe458-117">The page lists all the pages that have been personalized and the user it belongs to.</span></span>

    >[!NOTE]
    > <span data-ttu-id="fe458-118">Флажок в столбцах **Персонализация унаследованных данных** указывает, что персонализация была выполнен а более старой версии [!INCLUDE[d365fin](includes/d365fin_md.md)], в которой персонализация выполнялась не так, как сейчас.</span><span class="sxs-lookup"><span data-stu-id="fe458-118">A check mark in the **Legacy Personalization** columns indicates that the personalization was done in an older version of [!INCLUDE[d365fin](includes/d365fin_md.md)], which handled personalization different than it does now.</span></span> <span data-ttu-id="fe458-119">Для пользователей, которые пытаются персонализировать эти страницы, эта операция блокируется, если они не решат разблокировать страницу.</span><span class="sxs-lookup"><span data-stu-id="fe458-119">Users who try to personalize these pages are locked from doing so unless they choose to unlock the page.</span></span> <span data-ttu-id="fe458-120">Дополнительные сведения см. в разделе [Почему заблокирована персонализация страницы?](ui-personalization-locked.md).</span><span class="sxs-lookup"><span data-stu-id="fe458-120">For more information, see [Why a page is locked from personalizing](ui-personalization-locked.md).</span></span>

2. <span data-ttu-id="fe458-121">Выберите операцию, которую требуется удалить, затем выберите действие **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="fe458-121">Select the entry that you want to delete, and then choose the **Delete** action.</span></span>

    <span data-ttu-id="fe458-122">Пользователь увидит изменения при следующем входе в систему.</span><span class="sxs-lookup"><span data-stu-id="fe458-122">The user will see the changes the next time they sign-in.</span></span>

### <a name="clear-user-personalizations-by-using-the-user-personalization-card-page"></a><span data-ttu-id="fe458-123">Очистка персонализаций пользователя с помощью страницы "Карточка персонализации пользователя"</span><span class="sxs-lookup"><span data-stu-id="fe458-123">Clear user personalizations by using the User Personalization Card page</span></span>

<span data-ttu-id="fe458-124">Страница **Карточка персонализации пользователя** позволяет удалять персонализацию для всех страниц определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="fe458-124">The **User Personalization Card** page enables you to clear the personalization on all pages for specific user.</span></span> <span data-ttu-id="fe458-125">Для этого необходимо разрешение на запись для таблицы 2000000072 **Профиль**.</span><span class="sxs-lookup"><span data-stu-id="fe458-125">This requires write permission to Table 2000000072 **Profile**.</span></span>

1.  <span data-ttu-id="fe458-126">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Персонализация пользователя**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="fe458-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="fe458-127">На странице **Персонализация пользователя** перечисляются все пользователи, у которых потенциально есть персонализированные страницы.</span><span class="sxs-lookup"><span data-stu-id="fe458-127">The **User Personalization** page lists all users who potentially have personalized pages.</span></span> <span data-ttu-id="fe458-128">Если не удается найти пользователя в списке, это означает, что у него нет никаких персонализированных страниц.</span><span class="sxs-lookup"><span data-stu-id="fe458-128">If you cannot find a user in the list, this means that they do not have any personalized pages.</span></span>

2. <span data-ttu-id="fe458-129">Выберите пользователя из списка, затем выберите действие **Правка**.</span><span class="sxs-lookup"><span data-stu-id="fe458-129">Select the user from the list, and then choose the **Edit** action.</span></span>

3.  <span data-ttu-id="fe458-130">На вкладке **Действия** выберите **Очистить персонализированные страницы**.</span><span class="sxs-lookup"><span data-stu-id="fe458-130">On the **Actions** tab, choose **Clear Personalized Pages**.</span></span>

    <span data-ttu-id="fe458-131">Пользователь увидит изменения при следующем входе в систему.</span><span class="sxs-lookup"><span data-stu-id="fe458-131">The user will see the changes the next time they sign-in.</span></span>

## <a name="see-also"></a><span data-ttu-id="fe458-132">См. также</span><span class="sxs-lookup"><span data-stu-id="fe458-132">See Also</span></span>
[<span data-ttu-id="fe458-133">Персонализация рабочей области</span><span class="sxs-lookup"><span data-stu-id="fe458-133">Personalizing Your Workspace</span></span>](ui-personalization-user.md)  
<span data-ttu-id="fe458-134">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fe458-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="fe458-135">Изменение базовых настроек</span><span class="sxs-lookup"><span data-stu-id="fe458-135">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="fe458-136">Изменение набора отображаемых функций</span><span class="sxs-lookup"><span data-stu-id="fe458-136">Changing Which Features are Displayed</span></span>](ui-experiences.md)  

