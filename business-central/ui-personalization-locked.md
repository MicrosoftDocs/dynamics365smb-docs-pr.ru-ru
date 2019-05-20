---
title: Я не могу персонализировать страницу | Microsoft Docs
description: Объяснение причин, почему невозможно персонализировать страницу и как разблокировать страницу, чтобы ее можно было персонализировать.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: 64995372f68ed2804bc165823dacc34ad6a3194d
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1251289"
---
# <a name="why-a-page-is-locked-from-personalization"></a><span data-ttu-id="a77d7-103">Почему заблокирована персонализация страницы?</span><span class="sxs-lookup"><span data-stu-id="a77d7-103">Why a Page is Locked from Personalization</span></span>

<span data-ttu-id="a77d7-104">Существует два условия, которые не позволяют персонализировать страницу.</span><span class="sxs-lookup"><span data-stu-id="a77d7-104">There are two conditions that prevent you from personalizing a page.</span></span> <span data-ttu-id="a77d7-105">Либо страница заперта (как показано значком ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации")), либо она заблокирована как показано значком ![Персонализация заблокирована](media/personalization-blocked-icon.png "Персонализация заблокирована")).</span><span class="sxs-lookup"><span data-stu-id="a77d7-105">Either the page is locked (as indicated by ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock")) or it is blocked (as indicated by ![Personalization blocked](media/personalization-blocked-icon.png "Personalization blocked")).</span></span>

## <a name="locked-from-personalizing"></a><span data-ttu-id="a77d7-106">Замок персонализации</span><span class="sxs-lookup"><span data-stu-id="a77d7-106">Locked from Personalizing</span></span>

<span data-ttu-id="a77d7-107">Если в баннере **Персонализация** открытой страницы имеется значок ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации") (как показано), это означает, что вы в настоящее время не можете делать никаких дополнительных изменений персонализации на этой странице.</span><span class="sxs-lookup"><span data-stu-id="a77d7-107">If there is a ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock") icon in the **Personalizing** banner when you open a page (as shown), this means that you are currently prevented from making any more personalization changes to the page.</span></span>

<span data-ttu-id="a77d7-108">![Замок персонализации](media/personalization-locked.png "Замок персонализации")</span><span class="sxs-lookup"><span data-stu-id="a77d7-108">![Personalize Lock](media/personalization-locked.png "Personalize lock")</span></span>


<!-- This is because we changed the way personalization works behind the scenes since the last time that you personalized the page. Unfortunately, the old way and new of doing things do not work together.

The page currently includes the last personalization changes that you made. If you want to continue personalizing the page, then you can choose the lock icon and then **Unlock**. Just be aware that if you choose to unlock the page, the current personalization of the page will be cleared, and you will have to start from scratch.
-->

<span data-ttu-id="a77d7-109">Для этого может быть две причины.</span><span class="sxs-lookup"><span data-stu-id="a77d7-109">There can be two reasons for this:</span></span>

1. <span data-ttu-id="a77d7-110">Вы персонализировали страницу ранее, но это делалось с помощью ранней версии подукта.</span><span class="sxs-lookup"><span data-stu-id="a77d7-110">You have personalized the page before, but it was done using an earlier version of the product.</span></span> <span data-ttu-id="a77d7-111">Мы изменили то, как работает персонализация в фоновом режиме, с момента последней персонализации страницы.</span><span class="sxs-lookup"><span data-stu-id="a77d7-111">We changed the way personalization works behind the scenes since the last time that you personalized the page.</span></span> <span data-ttu-id="a77d7-112">К сожалению, старый и новый способы персонализации несовместимы.</span><span class="sxs-lookup"><span data-stu-id="a77d7-112">Unfortunately, the old way and new way of doing things do not work together.</span></span>

2. <span data-ttu-id="a77d7-113">До настоящего времени вы использовали только [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] для персонализации страницы.</span><span class="sxs-lookup"><span data-stu-id="a77d7-113">Until now, you have only used the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] to personalize the page.</span></span>

### <a name="unlocking-the-page"></a><span data-ttu-id="a77d7-114">Снятие замка со страницы</span><span class="sxs-lookup"><span data-stu-id="a77d7-114">Unlocking the Page</span></span>

<span data-ttu-id="a77d7-115">Если нужно разблокировать страницу и продолжить персонализировать ее, выберите ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации"), затем **Разблокировать**.</span><span class="sxs-lookup"><span data-stu-id="a77d7-115">If you want to unlock a page and continue personalizing it, choose ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock"), and then **Unlock**.</span></span>  

<span data-ttu-id="a77d7-116">Перед тем как разблокировать страницу, учтите следующее:</span><span class="sxs-lookup"><span data-stu-id="a77d7-116">Before you unlock the page, be aware of the following:</span></span>

- <span data-ttu-id="a77d7-117">Текущая персонализация страницы будет сброшена.</span><span class="sxs-lookup"><span data-stu-id="a77d7-117">The current personalization of the page will be cleared.</span></span> <span data-ttu-id="a77d7-118">Страница вернется назад к исходному макеты, и вам придется начинать с начала.</span><span class="sxs-lookup"><span data-stu-id="a77d7-118">The page will go back to its original layout, and you will have to start from scratch.</span></span>

- <span data-ttu-id="a77d7-119">В [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] страница останется без изменений, и на нее не будут влиять новые изменения персонализации, сделанные в клиенте Business Central.</span><span class="sxs-lookup"><span data-stu-id="a77d7-119">In the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)], the page will remain as-is and will not be affected by the new personalization changes made in the Business Central client.</span></span> <span data-ttu-id="a77d7-120">В будущем персонализация в [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] и клиенте Business Central будут полностью независимыми друг от друга.</span><span class="sxs-lookup"><span data-stu-id="a77d7-120">Going forward, the personalization in the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and Business Central client will be completely separate from each other.</span></span>

## <a name="blocked-from-personalizing"></a><span data-ttu-id="a77d7-121">Персонализация заблокирована</span><span class="sxs-lookup"><span data-stu-id="a77d7-121">Blocked from Personalizing</span></span>

<span data-ttu-id="a77d7-122">Если в баннере персонализации имеется значок ![Персонализация заблокирована](media/personalization-blocked-icon.png "Персонализация заблокирована"), это означает, что вам запрещена любая персонализация на этой странице.</span><span class="sxs-lookup"><span data-stu-id="a77d7-122">If there is a ![Personalization blocked](media/personalization-blocked-icon.png "Personalization blocked") icon in the Personalizing banner, this means that you are blocked from doing any personalization to the page.</span></span>

<span data-ttu-id="a77d7-123">![Персонализация заблокирована](media/personalization-blocked.png "Замок персонализации")</span><span class="sxs-lookup"><span data-stu-id="a77d7-123">![Personalize blocked](media/personalization-blocked.png "Personalize lock")</span></span>

<span data-ttu-id="a77d7-124">Причина этого заключается в том, что ролевой центр или профиль, который в настоящее время связан с вашей учетной записью пользователя, изменяет эту страницу специально для вашей роли.</span><span class="sxs-lookup"><span data-stu-id="a77d7-124">The reason for this is that the Role Center or profile that is currently associated with your user account modifies this page specifically for your role.</span></span> <span data-ttu-id="a77d7-125">Обратитесь к администратору за помощью или, если это имеет смысл, попробуйте переключиться на ролевой центр (из [**Мои настройки**](https://businesscentral.dynamics.com?page=9176 "Прямой переход на вашу страницу пользовательских настроек в Business Central")), который действительно включает настройку для ролей для этой страницы.</span><span class="sxs-lookup"><span data-stu-id="a77d7-125">Please contact your administrator for assistance or, if it makes sense, try switching to a Role Center (from  [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central")) that does include role-tailoring for this page.</span></span>

## <a name="see-also"></a><span data-ttu-id="a77d7-126">См. также</span><span class="sxs-lookup"><span data-stu-id="a77d7-126">See Also</span></span>
[<span data-ttu-id="a77d7-127">Персонализация рабочей области</span><span class="sxs-lookup"><span data-stu-id="a77d7-127">Personalizing Your Workspace</span></span>](ui-personalization-manage.md)  
[<span data-ttu-id="a77d7-128">Управление персонализацией</span><span class="sxs-lookup"><span data-stu-id="a77d7-128">Managing Personalization</span></span>](ui-personalization-manage.md)  
[<span data-ttu-id="a77d7-129">Изменение базовых настроек</span><span class="sxs-lookup"><span data-stu-id="a77d7-129">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="a77d7-130">Изменение набора отображаемых функций</span><span class="sxs-lookup"><span data-stu-id="a77d7-130">Changing Which Features are Displayed</span></span>](ui-experiences.md)  
