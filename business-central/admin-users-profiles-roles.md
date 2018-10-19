---
title: "Управление пользователями и ролями | Документы Майкрософт"
description: "Узнайте, как управлять пользователями и ролевыми центрами в Business Central."
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: profiles, users
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 1a94d023424c6eceb93af6e9ca89a90a3a94e996
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="understanding-users-profiles-and-role-centers"></a><span data-ttu-id="3cdf4-103">Знакомство с пользователями, профилями и ролевыми центрами</span><span class="sxs-lookup"><span data-stu-id="3cdf4-103">Understanding Users, Profiles, and Role Centers</span></span>

<span data-ttu-id="3cdf4-104">В [!INCLUDE[d365fin](includes/d365fin_md.md)] пользователи добавляются администратором, который также предоставляет доступ к зонам [!INCLUDE[d365fin](includes/d365fin_md.md)], которые требуются им в процессе работы.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], users are added by an administrator who also gives users access to the areas of [!INCLUDE[d365fin](includes/d365fin_md.md)] that they need in their work.</span></span>  

<span data-ttu-id="3cdf4-105">Доступ к функции управляется с помощью *групп пользователей* и *профилей*.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-105">Access to functionality is managed through *user groups* and *profiles*.</span></span> <span data-ttu-id="3cdf4-106">Как администратор вы можете добавлять и удалять пользователей в рамках своей подписки на [!INCLUDE[d365fin](includes/d365fin_md.md)], а также назначать разрешения для пользователей через группы.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-106">As an administrator, you can add and remove users as part of your [!INCLUDE[d365fin](includes/d365fin_md.md)] subscription, and you can assign users permissions through user groups.</span></span>  

## <a name="adding-users"></a><span data-ttu-id="3cdf4-107">Добавление пользователей</span><span class="sxs-lookup"><span data-stu-id="3cdf4-107">Adding Users</span></span>

<span data-ttu-id="3cdf4-108">Для добавления пользователей в [!INCLUDE[d365fin](includes/d365fin_md.md)] Online администратор Office 365 организации сначала должен создать пользователей в центре администрирования Office 365.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-108">To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)] online, your company's Office 365 administrator must first create the users in the Office 365 Admin Center.</span></span> <span data-ttu-id="3cdf4-109">Дополнительные сведения см. в разделе [Добавление пользователей в Office 365 для бизнеса](https://aka.ms/CreateOffice365Users).</span><span class="sxs-lookup"><span data-stu-id="3cdf4-109">For more information, see [Add Users to Office 365 for business](https://aka.ms/CreateOffice365Users).</span></span>

<span data-ttu-id="3cdf4-110">После этого администратор сможет назначить права доступа каждому пользователю и группе пользователей.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-110">Then, the administrator can assign permissions to each user and groups of users.</span></span> <span data-ttu-id="3cdf4-111">Дополнительные сведения см. в разделе [Управление пользователями и разрешениями](ui-how-users-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="3cdf4-111">For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).</span></span>  

### <a name="users-of-on-premises-deployments"></a><span data-ttu-id="3cdf4-112">Пользователи локальных развертываний</span><span class="sxs-lookup"><span data-stu-id="3cdf4-112">Users of on-premises deployments</span></span>

<span data-ttu-id="3cdf4-113">Для локальных развертываний [!INCLUDE[d365fin](includes/d365fin_md.md)] администратор может выбрать между различными механизмами авторизации учетной информации для пользователей.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-113">For on-premises deployments of [!INCLUDE[d365fin](includes/d365fin_md.md)], the administrator can choose between different credential authorization mechanisms for users.</span></span> <span data-ttu-id="3cdf4-114">Затем при создании пользователя необходимо предоставить различную информацию в зависимости от используемого типа учетных данных в конкретном экземпляре [!INCLUDE[server](includes/server.md)].</span><span class="sxs-lookup"><span data-stu-id="3cdf4-114">Then, when you create a user, you provide different information depending on the credential type that you are using in the specific [!INCLUDE[server](includes/server.md)] instance.</span></span> <span data-ttu-id="3cdf4-115">Дополнительные сведения, см. в разделе [Проверка подлинности и типы учетных сведений](/dynamics365/business-central/dev-itpro/administration/users-credential-types) в разделе администрирование для разработчиков и содержимом ITPro для [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3cdf4-115">For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the Administration section of the developer and ITPro content for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="profiles"></a><span data-ttu-id="3cdf4-116">Профили</span><span class="sxs-lookup"><span data-stu-id="3cdf4-116">Profiles</span></span>

<span data-ttu-id="3cdf4-117">Всем пользователям в организации, которые имеют доступ к [!INCLUDE[d365fin](includes/d365fin_md.md)], назначается *профиль*, открывающий им доступ к центру *Ролевой центр*.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-117">The people in your company who have access to [!INCLUDE[d365fin](includes/d365fin_md.md)] are all assigned a *profile* that gives them access to a *Role Center*.</span></span>

<span data-ttu-id="3cdf4-118">Профили — это коллекции пользователей [!INCLUDE[d365fin](includes/d365fin_md.md)], которые относятся к одному ролевому центру.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-118">Profiles are collections of [!INCLUDE[d365fin](includes/d365fin_md.md)] users who share the same Role Center.</span></span> <span data-ttu-id="3cdf4-119">Ролевой центр является начальной страницей [!INCLUDE[d365fin](includes/d365fin_md.md)], с которой можно быстро запустить наиболее важные задачи и увидеть аналитику и КПЭ.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-119">A Role Center is the entry point and home page for [!INCLUDE[d365fin](includes/d365fin_md.md)] that gives you quick access to your most important tasks and displays various insights and key performance indicators (KPIs) about your work.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="3cdf4-120">В текущей версии [!INCLUDE[d365fin](includes/d365fin_md.md)] Online невозможно добавлять, изменять или удалять профили.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-120">In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you cannot add, edit, or delete profiles.</span></span>  

## <a name="configuration-and-personalization"></a><span data-ttu-id="3cdf4-121">Конфигурация и персонализация</span><span class="sxs-lookup"><span data-stu-id="3cdf4-121">Configuration and Personalization</span></span>
<!--The concept of UI customization in [!INCLUDE[d365fin](includes/d365fin_md.md)] is divided in two:  

-   Configuration, performed by the administrator  

-   Personalization, performed by users  

The administrator configures the user interface for multiple users by customizing the user interface for a profile that the users are assigned to.  -->
<span data-ttu-id="3cdf4-122">Пользователи персонализируют пользовательский интерфейс персональной версии, настраивая ИП после входа со своими учетными данными.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-122">Users personalize the user interface of their personal version by customizing the user interface under their own user logon.</span></span> <span data-ttu-id="3cdf4-123">Эта персонализация может быть удалена администратором.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-123">This personalization can be deleted by the administrator.</span></span> <span data-ttu-id="3cdf4-124">Дополнительные сведения см. в разделе [Персонализация рабочей области](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="3cdf4-124">For more information, see [Personalizing Your Workspace](ui-personalization-user.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="3cdf4-125">См. также</span><span class="sxs-lookup"><span data-stu-id="3cdf4-125">See Also</span></span>  
[<span data-ttu-id="3cdf4-126">Управление пользователями и разрешениями</span><span class="sxs-lookup"><span data-stu-id="3cdf4-126">Managing Users and Permissions</span></span>](ui-how-users-permissions.md)  
[<span data-ttu-id="3cdf4-127">Управление персонализацией в качестве администратора</span><span class="sxs-lookup"><span data-stu-id="3cdf4-127">Managing Personalization as an Administrator</span></span>](ui-personalization-manage.md)  
[<span data-ttu-id="3cdf4-128">Персонализация рабочей области</span><span class="sxs-lookup"><span data-stu-id="3cdf4-128">Personalizing Your Workspace</span></span>](ui-personalization-user.md)  

