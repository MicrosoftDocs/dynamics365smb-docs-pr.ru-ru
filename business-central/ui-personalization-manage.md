---
title: Настройка страниц для ролей | Документация Майкрософт
description: Узнайте, как настроить пользовательский интерфейс для профиля (роли), чтобы все пользователи, которым назначена эта роль, видели настроенную рабочую область.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: cee71cea69468a45b2e731632fce3827c54794c1
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3781339"
---
# <a name="customize-pages-for-profiles"></a><span data-ttu-id="fe66a-103">Настройка страниц для профилей</span><span class="sxs-lookup"><span data-stu-id="fe66a-103">Customize Pages for Profiles</span></span>
<span data-ttu-id="fe66a-104">Пользователи могут персонализировать страницы, из которых состоят их рабочие области, в соответствии со своими предпочтениями.</span><span class="sxs-lookup"><span data-stu-id="fe66a-104">Users can personalize pages that make up their workspace to suit their own preferences.</span></span> <span data-ttu-id="fe66a-105">Дополнительные сведения см. в разделе [Персонализация рабочей области](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="fe66a-105">For more information, see [Personalize Your Workspace](ui-personalization-user.md).</span></span>

<span data-ttu-id="fe66a-106">Администраторы могут настраивать страницы для профиля в соответствии со связанной бизнес-ролью или отделом, например, чтобы все пользователи, которым назначен профиль, видели настроенные макеты страниц.</span><span class="sxs-lookup"><span data-stu-id="fe66a-106">Administrators can customize pages for a profile, according to the related business role or department, for example, so that all users that are assigned the profile will see the customized page layout.</span></span> <span data-ttu-id="fe66a-107">При настройке страниц администратор использует ту же функциональность, что и пользователи при персонализации страниц.</span><span class="sxs-lookup"><span data-stu-id="fe66a-107">The administrator customizes pages by using the same functionality as users do when they personalize pages.</span></span>

> [!NOTE]
> <span data-ttu-id="fe66a-108">Как правило, профили соответствуют ролям пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="fe66a-108">The typical business use of a profile is a role.</span></span> <span data-ttu-id="fe66a-109">Поэтому в пользовательском интерфейсе профиль называется *Профиль (роль)*.</span><span class="sxs-lookup"><span data-stu-id="fe66a-109">A profile is therefore named *Profile (Role)* in the UI.</span></span>

<span data-ttu-id="fe66a-110">Настройка страниц начинается со страницы **Профили (роли)** — отправной точка администратора для управления профилями пользователей на отдельных карточках профилей.</span><span class="sxs-lookup"><span data-stu-id="fe66a-110">Page customization starts from the **Profiles (Roles)** page, the administrator's starting point for managing users' profiles on individual profile cards.</span></span> <span data-ttu-id="fe66a-111">Помимо настройки макета страницы, вы можете управлять рядом других параметров для профилей на странице **Профиль (роль)** для каждого профиля.</span><span class="sxs-lookup"><span data-stu-id="fe66a-111">In addition to customizing the page layout, you control various other settings for profiles on the **Profile (Role)** page for each profile.</span></span> <span data-ttu-id="fe66a-112">Дополнительные сведения см. в разделе [Управление профилями](admin-users-profiles-roles.md).</span><span class="sxs-lookup"><span data-stu-id="fe66a-112">For more information, see [Manage Profiles](admin-users-profiles-roles.md).</span></span>

## <a name="to-customize-pages-for-a-profile"></a><span data-ttu-id="fe66a-113">Настройка страниц для профиля</span><span class="sxs-lookup"><span data-stu-id="fe66a-113">To customize pages for a profile</span></span>
1. <span data-ttu-id="fe66a-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Профили (роли)**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="fe66a-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Profiles (Roles)**, and then choose the related link.</span></span>
2. <span data-ttu-id="fe66a-115">Выберите строку профиля, для которого вы хотите настроить страницы, а затем выберите действие **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="fe66a-115">Select the line for the profile that you want to customize pages for, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="fe66a-116">Выберите действие **Настроить страницы**.</span><span class="sxs-lookup"><span data-stu-id="fe66a-116">Choose the **Customize pages** action.</span></span>

    [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="fe66a-117">открывается на новой вкладке браузера для выбранного профиля с активированным баннером **Настройка**.</span><span class="sxs-lookup"><span data-stu-id="fe66a-117">opens on a new browser tab for the selected profile with the **Customizing** banner activated.</span></span> <span data-ttu-id="fe66a-118">Баннер **Настройка** баннер предлагает ту же функциональность, что и баннер **Персонализация**, который доступен пользователям.</span><span class="sxs-lookup"><span data-stu-id="fe66a-118">The **Customizing** banner offers the same functionality as the **Personalizing** banner that is available to users.</span></span>

4. <span data-ttu-id="fe66a-119">Настройте страницы в соответствии с потребностями соответствующей роли или отдела так же, как это сделал бы пользователь при персонализации.</span><span class="sxs-lookup"><span data-stu-id="fe66a-119">Customize pages according to the needs of the role or department in question in the same way as a user would do when personalizing.</span></span> <span data-ttu-id="fe66a-120">Дополнительные сведения см. в разделе [Персонализация рабочей области](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="fe66a-120">For more information, see [Personalize Your Workspace](ui-personalization-user.md).</span></span>

    > [!NOTE]
    > <span data-ttu-id="fe66a-121">Для навигации во время персонализации используйте Ctrl + щелчок по действию, если оно выделено стрелкой.</span><span class="sxs-lookup"><span data-stu-id="fe66a-121">To navigate during personalization, use Ctrl + Click on an action if it is highlighted by the arrowhead.</span></span>

5. <span data-ttu-id="fe66a-122">Закончив вносить изменения в макет на одной или нескольких страницах, выберите кнопку **Готово** на баннере **Настройка**.</span><span class="sxs-lookup"><span data-stu-id="fe66a-122">When you have finished changing the layout on one or more pages, choose the **Done** button on the **Customizing** banner.</span></span>
6. <span data-ttu-id="fe66a-123">Закройте вкладку браузера.</span><span class="sxs-lookup"><span data-stu-id="fe66a-123">Close the browser tab.</span></span>

<span data-ttu-id="fe66a-124">Настройка страниц для профиля записана.</span><span class="sxs-lookup"><span data-stu-id="fe66a-124">The customization of pages is now recorded for the profile.</span></span>

## <a name="to-view-all-customized-pages-for-a-profile"></a><span data-ttu-id="fe66a-125">Просмотр всех настроенных страниц для профиля</span><span class="sxs-lookup"><span data-stu-id="fe66a-125">To view all customized pages for a profile</span></span>
<span data-ttu-id="fe66a-126">Вы можете посмотреть, какие страницы настроены для профиля, — например, чтобы спланировать, какие из них следует настроить дополнительно или удалить.</span><span class="sxs-lookup"><span data-stu-id="fe66a-126">You can get an overview of which pages are customized for a profile, for example to plan which to customize further or delete.</span></span>

- <span data-ttu-id="fe66a-127">На странице **Профиль (роль)** выберите действие **Настроенные страницы**.</span><span class="sxs-lookup"><span data-stu-id="fe66a-127">On the **Profile (Role)** page, choose the **Customized Pages** action.</span></span>

## <a name="to-delete-all-customizations-for-a-profile"></a><span data-ttu-id="fe66a-128">Удаление всех настроек для профиля.</span><span class="sxs-lookup"><span data-stu-id="fe66a-128">To delete all customizations for a profile</span></span>
<span data-ttu-id="fe66a-129">Можно отменить все настройки, сделанные для профиля.</span><span class="sxs-lookup"><span data-stu-id="fe66a-129">You can cancel all customizations that you have made for a profile.</span></span> <span data-ttu-id="fe66a-130">Настройки, связанные с расширениями, и сделанные пользователями персонализации при этом удалены не будут.</span><span class="sxs-lookup"><span data-stu-id="fe66a-130">Customizations introduced with an extension and personalizations made by a user will not be deleted.</span></span> <span data-ttu-id="fe66a-131">Удалить все персонализации можно с помощью другого действия.</span><span class="sxs-lookup"><span data-stu-id="fe66a-131">You can delete all personalizations with another action.</span></span> <span data-ttu-id="fe66a-132">Дополнительные сведения см. в разделе [Удаление всех персонализаций, сделанных пользователем](admin-users-profiles-roles.md#to-delete-all-personalizations-made-by-a-user).</span><span class="sxs-lookup"><span data-stu-id="fe66a-132">For more information, see [To delete all personalizations made by a user](admin-users-profiles-roles.md#to-delete-all-personalizations-made-by-a-user).</span></span>

- <span data-ttu-id="fe66a-133">На странице **Профиль (роль)** для настроенного профиля выберите действие **Очистить настроенные страницы**.</span><span class="sxs-lookup"><span data-stu-id="fe66a-133">On the **Profile (Role)** page for a customized profile, choose the **Clear customized pages** action.</span></span>

<span data-ttu-id="fe66a-134">Макет на страницах профиля сбрасывается в макет, используемый по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fe66a-134">The layout on pages for the profile is reset to the default layout.</span></span>  

## <a name="to-delete-customization-for-specific-pages-for-a-profile"></a><span data-ttu-id="fe66a-135">Удаление настройки для конкретных страниц профиля</span><span class="sxs-lookup"><span data-stu-id="fe66a-135">To delete customization for specific pages for a profile</span></span>
<span data-ttu-id="fe66a-136">Можно удалить настройки отдельных страниц, сделанные для профиля.</span><span class="sxs-lookup"><span data-stu-id="fe66a-136">You can delete individual page customizations that you have made for a profile.</span></span> <span data-ttu-id="fe66a-137">Настройки, связанные с расширениями, и сделанные пользователями персонализации при этом удалены не будут.</span><span class="sxs-lookup"><span data-stu-id="fe66a-137">Customizations introduced with an extension and personalizations made by a user will not be deleted.</span></span> <span data-ttu-id="fe66a-138">Удалить персонализации конкретных страниц можно с помощью другого действия.</span><span class="sxs-lookup"><span data-stu-id="fe66a-138">You can delete specific page personalizations with another action.</span></span> <span data-ttu-id="fe66a-139">Дополнительные сведения см. в разделе [Удаление персонализаций для конкретных страниц](admin-users-profiles-roles.md#to-delete-personalizations-for-specific-pages).</span><span class="sxs-lookup"><span data-stu-id="fe66a-139">For more information, see [To delete personalizations for specific pages](admin-users-profiles-roles.md#to-delete-personalizations-for-specific-pages).</span></span>

1. <span data-ttu-id="fe66a-140">На странице **Профиль (роль)** выберите действие **Настроенные страницы**.</span><span class="sxs-lookup"><span data-stu-id="fe66a-140">On the **Profile (Role)** page, choose the **Customized Pages** action.</span></span>
2. <span data-ttu-id="fe66a-141">На странице **Настройки профиля** выберите одну или несколько строк настроек страниц, которые вы хотите удалить, а затем выберите действие **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="fe66a-141">On the **Profile Customizations** page, select on or more lines for page customizations that you want to delete, and then choose the **Delete** action.</span></span>

<span data-ttu-id="fe66a-142">Макет на выбранных страницах корректируется с учетом внесенных вами изменений.</span><span class="sxs-lookup"><span data-stu-id="fe66a-142">The layout on the selected pages is adjusted to the changes you made.</span></span>

## <a name="see-also"></a><span data-ttu-id="fe66a-143">См. также</span><span class="sxs-lookup"><span data-stu-id="fe66a-143">See Also</span></span>
[<span data-ttu-id="fe66a-144">Персонализация рабочей области</span><span class="sxs-lookup"><span data-stu-id="fe66a-144">Personalize Your Workspace</span></span>](ui-personalization-user.md)  
[<span data-ttu-id="fe66a-145">Управление профилями</span><span class="sxs-lookup"><span data-stu-id="fe66a-145">Manage Profiles</span></span>](admin-users-profiles-roles.md)  
[<span data-ttu-id="fe66a-146">Изменение базовых настроек</span><span class="sxs-lookup"><span data-stu-id="fe66a-146">Change Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="fe66a-147">Изменение набора отображаемых функций</span><span class="sxs-lookup"><span data-stu-id="fe66a-147">Change Which Features are Displayed</span></span>](ui-experiences.md)  
<span data-ttu-id="fe66a-148">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fe66a-148">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
