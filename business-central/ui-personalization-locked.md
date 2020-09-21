---
title: Я не могу персонализировать страницу | Документация Майкрософт
description: Объяснение причин, почему невозможно персонализировать страницу и как разблокировать страницу, чтобы ее можно было персонализировать.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: d24e78d7f0286e1ef633008e22ceb3f922b48768
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3781364"
---
# <a name="why-a-page-is-locked-from-personalization"></a><span data-ttu-id="0f925-103">Почему заблокирована персонализация страницы?</span><span class="sxs-lookup"><span data-stu-id="0f925-103">Why a Page is Locked from Personalization</span></span>

<span data-ttu-id="0f925-104">Существует два условия, которые не позволяют персонализировать страницу.</span><span class="sxs-lookup"><span data-stu-id="0f925-104">There are two conditions that prevent you from personalizing a page.</span></span> <span data-ttu-id="0f925-105">Страница может быть заперта (о чем свидетельствует значок ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации")) или заблокирована (о чем свидетельствует значок ![Персонализация заблокирована](media/personalization-blocked-icon.png "Персонализация заблокирована")).</span><span class="sxs-lookup"><span data-stu-id="0f925-105">Either the page is locked (as indicated by the ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock")) icon or it is blocked (as indicated by the ![Personalization blocked](media/personalization-blocked-icon.png "Personalization blocked") icon).</span></span>

## <a name="locked-from-personalizing"></a><span data-ttu-id="0f925-106">Замок персонализации</span><span class="sxs-lookup"><span data-stu-id="0f925-106">Locked from Personalizing</span></span>

<span data-ttu-id="0f925-107">Если в баннере **Персонализация** открытой страницы имеется значок ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации"), это означает, что вы в настоящее время не можете вносить в эту страницу никакие дополнительные изменения, связанные с персонализацией.</span><span class="sxs-lookup"><span data-stu-id="0f925-107">If there is a ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock") icon in the **Personalizing** banner when you open a page, this means that you are currently prevented from making any more personalization changes to the page.</span></span>

<!-- This is because we changed the way personalization works behind the scenes since the last time that you personalized the page. Unfortunately, the old way and new of doing things do not work together.

The page currently includes the last personalization changes that you made. If you want to continue personalizing the page, then you can choose the lock icon and then **Unlock**. Just be aware that if you choose to unlock the page, the current personalization of the page will be cleared, and you will have to start from scratch.
-->

<span data-ttu-id="0f925-108">Для этого может быть две причины.</span><span class="sxs-lookup"><span data-stu-id="0f925-108">There can be two reasons for this:</span></span>

1. <span data-ttu-id="0f925-109">Вы персонализировали страницу ранее, но это делалось с помощью ранней версии подукта.</span><span class="sxs-lookup"><span data-stu-id="0f925-109">You have personalized the page before, but it was done using an earlier version of the product.</span></span> <span data-ttu-id="0f925-110">Мы изменили то, как работает персонализация в фоновом режиме, с момента последней персонализации страницы.</span><span class="sxs-lookup"><span data-stu-id="0f925-110">We changed the way personalization works behind the scenes since the last time that you personalized the page.</span></span> <span data-ttu-id="0f925-111">К сожалению, старый и новый способы персонализации несовместимы.</span><span class="sxs-lookup"><span data-stu-id="0f925-111">Unfortunately, the old way and new way of doing things do not work together.</span></span>

2. <span data-ttu-id="0f925-112">До настоящего времени вы использовали только [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] для персонализации страницы.</span><span class="sxs-lookup"><span data-stu-id="0f925-112">Until now, you have only used the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] to personalize the page.</span></span>

### <a name="unlocking-the-page"></a><span data-ttu-id="0f925-113">Снятие замка со страницы</span><span class="sxs-lookup"><span data-stu-id="0f925-113">Unlocking the Page</span></span>

<span data-ttu-id="0f925-114">Если вы хотите снять замок со страницы и продолжить персонализировать ее, выберите значок ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации"), затем выберите действие **Разблокировать**.</span><span class="sxs-lookup"><span data-stu-id="0f925-114">If you want to unlock a page and continue personalizing it, choose the ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock") icon, and then choose the **Unlock** action.</span></span>  

<span data-ttu-id="0f925-115">Перед тем как разблокировать страницу, учтите следующее:</span><span class="sxs-lookup"><span data-stu-id="0f925-115">Before you unlock the page, be aware of the following:</span></span>

- <span data-ttu-id="0f925-116">Текущая персонализация страницы будет сброшена.</span><span class="sxs-lookup"><span data-stu-id="0f925-116">The current personalization of the page will be cleared.</span></span> <span data-ttu-id="0f925-117">Страница вернется назад к исходному макеты, и вам придется начинать с начала.</span><span class="sxs-lookup"><span data-stu-id="0f925-117">The page will go back to its original layout, and you will have to start from scratch.</span></span>

- <span data-ttu-id="0f925-118">В [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] страница останется без изменений, и на нее не будут влиять новые изменения персонализации, сделанные в клиенте Business Central.</span><span class="sxs-lookup"><span data-stu-id="0f925-118">In the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)], the page will remain as-is and will not be affected by the new personalization changes made in the Business Central client.</span></span> <span data-ttu-id="0f925-119">В будущем персонализация в [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] и клиенте Business Central будут полностью независимыми друг от друга.</span><span class="sxs-lookup"><span data-stu-id="0f925-119">Going forward, the personalization in the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and Business Central client will be completely separate from each other.</span></span>

## <a name="blocked-from-personalizing"></a><span data-ttu-id="0f925-120">Персонализация заблокирована</span><span class="sxs-lookup"><span data-stu-id="0f925-120">Blocked from Personalizing</span></span>

<span data-ttu-id="0f925-121">Если в баннере **Персонализация** имеется значок ![Персонализация заблокирована](media/personalization-blocked-icon.png "Персонализация заблокирована"), это означает, что вам запрещена любая персонализация на этой странице.</span><span class="sxs-lookup"><span data-stu-id="0f925-121">If there is a ![Personalization blocked](media/personalization-blocked-icon.png "Personalization blocked") icon in the **Personalizing** banner, this means that you are blocked from doing any personalization to the page.</span></span>

<!-- Only text is translated, so removing this image for non-English UX reasons.  ![Personalize blocked](media/personalization-blocked.png "Personalize lock") -->

<span data-ttu-id="0f925-122">Причина этого заключается в том, что ролевой центр или роль, которая в настоящее время связана с вашей учетной записью пользователя, изменяет эту страницу специально для вашей роли.</span><span class="sxs-lookup"><span data-stu-id="0f925-122">The reason for this is that the Role Center or role that is currently associated with your user account modifies this page specifically for your role.</span></span> <span data-ttu-id="0f925-123">Обратитесь за помощью к администратору.</span><span class="sxs-lookup"><span data-stu-id="0f925-123">Contact your administrator for assistance.</span></span> <span data-ttu-id="0f925-124">В качестве альтернативы попробуйте перейти к ролевому центру, который предусматривает ролевую настройку этой страницы.</span><span class="sxs-lookup"><span data-stu-id="0f925-124">Alternatively, try switching to a Role Center that does include role-tailoring for this page.</span></span> <span data-ttu-id="0f925-125">Дополнительные сведения см. в разделе [Изменение базовых настроек](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="0f925-125">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="0f925-126">См. также</span><span class="sxs-lookup"><span data-stu-id="0f925-126">See Also</span></span>
[<span data-ttu-id="0f925-127">Персонализация рабочей области</span><span class="sxs-lookup"><span data-stu-id="0f925-127">Personalize Your Workspace</span></span>](ui-personalization-user.md)  
[<span data-ttu-id="0f925-128">Настройка страниц для профилей</span><span class="sxs-lookup"><span data-stu-id="0f925-128">Customize Pages for Profiles</span></span>](ui-personalization-manage.md)  
[<span data-ttu-id="0f925-129">Изменение базовых настроек</span><span class="sxs-lookup"><span data-stu-id="0f925-129">Change Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="0f925-130">Изменение набора отображаемых функций</span><span class="sxs-lookup"><span data-stu-id="0f925-130">Change Which Features are Displayed</span></span>](ui-experiences.md)  
