---
title: "Управление пользователями и ролями | Документы Майкрософт"
description: "Узнайте, как управлять пользователями и ролевыми центрами в Dynamics 365 for Financials."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: e8989767618962a2db861b2df60aa03a2ca2b484
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="users-profiles-and-role-centers-in-dynamics-365-for-financials"></a><span data-ttu-id="c0dcd-103">Пользователи, профили и ролевые центры в Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="c0dcd-103">Users, Profiles, and Role Centers in Dynamics 365 for Financials</span></span>
<span data-ttu-id="c0dcd-104">Всем пользователям в организации, которые имеют доступ к [!INCLUDE[d365fin](includes/d365fin_md.md)], назначается *профиль*, открывающий им доступ к центру *Ролевой центр*.</span><span class="sxs-lookup"><span data-stu-id="c0dcd-104">The people in your company who have access to [!INCLUDE[d365fin](includes/d365fin_md.md)] are all assigned a *profile* that gives them access to a *Role Center*.</span></span> <span data-ttu-id="c0dcd-105">Как администратор, вы можете назначать и изменять профили в [!INCLUDE[d365fin](includes/d365fin_md.md)], а также добавлять и удалять пользователей в рамках своей подписки на [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="c0dcd-105">As an administrator, you can assign and change profiles in [!INCLUDE[d365fin](includes/d365fin_md.md)], and you can add and remove users as part of your [!INCLUDE[d365fin](includes/d365fin_md.md)] subscription.</span></span>  

## <a name="adding-users"></a><span data-ttu-id="c0dcd-106">Добавление пользователей</span><span class="sxs-lookup"><span data-stu-id="c0dcd-106">Adding Users</span></span>
<span data-ttu-id="c0dcd-107">Для добавления пользователей в [!INCLUDE[d365fin](includes/d365fin_md.md)] администратор Office 365 организации сначала должен создать пользователей в центре администрирования Office 365.</span><span class="sxs-lookup"><span data-stu-id="c0dcd-107">To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)], your company's Office 365 administrator must first create the users in the Office 365 Admin Center.</span></span> <span data-ttu-id="c0dcd-108">Дополнительные сведения см. в разделе [Практическое руководство. Управление пользователями и разрешениями](ui-how-users-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="c0dcd-108">For more information, see [How to: Manage Users and Permissions](ui-how-users-permissions.md).</span></span>  

## <a name="profiles"></a><span data-ttu-id="c0dcd-109">Профили</span><span class="sxs-lookup"><span data-stu-id="c0dcd-109">Profiles</span></span>
<span data-ttu-id="c0dcd-110">Профили — это коллекции пользователей [!INCLUDE[d365fin](includes/d365fin_md.md)], которые относятся к одному ролевому центру.</span><span class="sxs-lookup"><span data-stu-id="c0dcd-110">Profiles are collections of [!INCLUDE[d365fin](includes/d365fin_md.md)] users who share the same Role Center.</span></span> <span data-ttu-id="c0dcd-111">Ролевой центр — тип страницы, на которой можно разместить различные части.</span><span class="sxs-lookup"><span data-stu-id="c0dcd-111">A Role Center is a type of page on which you can place different parts.</span></span> <span data-ttu-id="c0dcd-112">Каждая часть представляет собой контейнер, в котором можно размещать другие страницы или предварительно заданные части системы, например части Outlook для добавления задач, уведомлений или заметок.</span><span class="sxs-lookup"><span data-stu-id="c0dcd-112">Each part is a container in which you can host other pages or pre-defined system parts, such as an Outlook part or parts for adding tasks, notifications, or notes.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="c0dcd-113">В текущей версии [!INCLUDE[d365fin](includes/d365fin_md.md)] невозможно добавлять, изменять или удалять профили.</span><span class="sxs-lookup"><span data-stu-id="c0dcd-113">In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)], you cannot add, edit, or delete profiles.</span></span>  

## <a name="configuration-and-personalization"></a><span data-ttu-id="c0dcd-114">Конфигурация и персонализация</span><span class="sxs-lookup"><span data-stu-id="c0dcd-114">Configuration and Personalization</span></span>
<span data-ttu-id="c0dcd-115">Понятие пользовательской настройки ИП в [!INCLUDE[d365fin](includes/d365fin_md.md)] разделено надвое:</span><span class="sxs-lookup"><span data-stu-id="c0dcd-115">The concept of UI customization in [!INCLUDE[d365fin](includes/d365fin_md.md)] is divided in two:</span></span>  

-   <span data-ttu-id="c0dcd-116">Настройка, выполняемая администратором</span><span class="sxs-lookup"><span data-stu-id="c0dcd-116">Configuration, performed by the administrator</span></span>  

-   <span data-ttu-id="c0dcd-117">Персонализация, выполненная пользователями</span><span class="sxs-lookup"><span data-stu-id="c0dcd-117">Personalization, performed by users</span></span>  

<span data-ttu-id="c0dcd-118">Администратор настраивает пользовательский интерфейс для нескольких пользователей, выполняя пользовательскую настройку интерфейса для профиля, к которому относятся пользователи.</span><span class="sxs-lookup"><span data-stu-id="c0dcd-118">The administrator configures the user interface for multiple users by customizing the user interface for a profile that the users are assigned to.</span></span>  

<span data-ttu-id="c0dcd-119">Пользователи персонализируют пользовательский интерфейс персональной версии, настраивая ИП после входа со своими учетными данными.</span><span class="sxs-lookup"><span data-stu-id="c0dcd-119">Users personalize the user interface of their personal version by customizing the user interface under their own user logon.</span></span> <span data-ttu-id="c0dcd-120">Эта персонализация может быть удалена администратором.</span><span class="sxs-lookup"><span data-stu-id="c0dcd-120">This personalization can be deleted by the administrator.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c0dcd-121">См. также</span><span class="sxs-lookup"><span data-stu-id="c0dcd-121">See Also</span></span>  
[<span data-ttu-id="c0dcd-122">Практическое руководство. Управление пользователями и разрешениями</span><span class="sxs-lookup"><span data-stu-id="c0dcd-122">How to: Manage Users and Permissions</span></span>](ui-how-users-permissions.md)  
<!-- [Customize the User Interface](../customize-the-user-interface.md)   
 [Security Overview](../Security%20Overview.md)-->

