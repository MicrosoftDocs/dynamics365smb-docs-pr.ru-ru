---
title: Управление пользователями и ролями | Документы Майкрософт
description: Узнайте, как управлять пользователями и ролевыми центрами в Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: profiles, users
ms.date: 08/02/2019
ms.author: edupont
ms.openlocfilehash: 27a57490101195f8dc05cc39538260e7db5e46af
ms.sourcegitcommit: 5bcc5f95e450ee9a3d9f7a380e592a5e75c4185b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2019
ms.locfileid: "1858224"
---
# <a name="understanding-users-roles-and-profiles"></a><span data-ttu-id="21964-103">Знакомство с пользователями, ролями и профилями</span><span class="sxs-lookup"><span data-stu-id="21964-103">Understanding Users, Roles, and Profiles</span></span>

<span data-ttu-id="21964-104">В [!INCLUDE[d365fin](includes/d365fin_md.md)] пользователи добавляются администратором, который также предоставляет доступ к зонам [!INCLUDE[d365fin](includes/d365fin_md.md)], которые требуются им в процессе работы.</span><span class="sxs-lookup"><span data-stu-id="21964-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], users are added by an administrator who also gives users access to the areas of [!INCLUDE[d365fin](includes/d365fin_md.md)] that they need in their work.</span></span>  

<span data-ttu-id="21964-105">Доступ к функции управляется с помощью *групп пользователей* и *профилей (ролей)*.</span><span class="sxs-lookup"><span data-stu-id="21964-105">Access to functionality is managed through *user groups* and *profiles (roles)*.</span></span> <span data-ttu-id="21964-106">Как администратор вы можете добавлять и удалять пользователей в рамках своей подписки на [!INCLUDE[d365fin](includes/d365fin_md.md)], а также назначать разрешения для пользователей через группы.</span><span class="sxs-lookup"><span data-stu-id="21964-106">As an administrator, you can add and remove users as part of your [!INCLUDE[d365fin](includes/d365fin_md.md)] subscription, and you can assign users permissions through user groups.</span></span>  

## <a name="adding-users"></a><span data-ttu-id="21964-107">Добавление пользователей</span><span class="sxs-lookup"><span data-stu-id="21964-107">Adding Users</span></span>

<span data-ttu-id="21964-108">Для добавления пользователей в [!INCLUDE[d365fin](includes/d365fin_md.md)] Online администратор Office 365 организации сначала должен создать пользователей в центре администрирования Office 365.</span><span class="sxs-lookup"><span data-stu-id="21964-108">To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)] online, your company's Office 365 administrator must first create the users in the Office 365 Admin Center.</span></span> <span data-ttu-id="21964-109">Дополнительные сведения см. в разделе [Добавление пользователей в Office 365 для бизнеса](https://aka.ms/CreateOffice365Users).</span><span class="sxs-lookup"><span data-stu-id="21964-109">For more information, see [Add Users to Office 365 for business](https://aka.ms/CreateOffice365Users).</span></span>

<span data-ttu-id="21964-110">После этого администратор сможет назначить права доступа каждому пользователю и группе пользователей.</span><span class="sxs-lookup"><span data-stu-id="21964-110">Then, the administrator can assign permissions to each user and groups of users.</span></span> <span data-ttu-id="21964-111">Дополнительные сведения см. в разделе [Управление пользователями и разрешениями](ui-how-users-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="21964-111">For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).</span></span>  

<span data-ttu-id="21964-112">Наиболее сильные права доступа, которые пользователь иметь — это набор разрешений SUPER.</span><span class="sxs-lookup"><span data-stu-id="21964-112">The most powerful permissions that a user can have is the SUPER permission set.</span></span> <span data-ttu-id="21964-113">Каждая организация должна иметь хотя бы одного пользователя с этим набором разрешений, но рекомендуется предоставлять каждому пользователю права доступа, которые соответствуют его потребностям в [!INCLUDE[prodshort](includes/prodshort.md)], и не более того.</span><span class="sxs-lookup"><span data-stu-id="21964-113">Each company must have at least one user with this permission set, but it is a best practice to give each user permissions that match their work needs in [!INCLUDE[prodshort](includes/prodshort.md)] and not more than that.</span></span> <span data-ttu-id="21964-114">Это помогает обеспечить, что пользователям предоставляется доступ только к данным, относящимся к их работе, например.</span><span class="sxs-lookup"><span data-stu-id="21964-114">This helps ensure that users only have access to data that is relevant to their work, for example.</span></span>  

> [!TIP]
> <span data-ttu-id="21964-115">Рекомендуется убедиться, что администратор Office 365 также имеет набор разрешений SUPER в [!INCLUDE[prodshort](includes/prodshort.md)], поскольку это упрощает выполнение многих административных задач, включая настройку интеграции с другими приложениями.</span><span class="sxs-lookup"><span data-stu-id="21964-115">It's a best practice to make sure that the Office 365 administrator also has the SUPER permission set in [!INCLUDE[prodshort](includes/prodshort.md)] because that makes many administrative tasks easier, including setting up integration with other apps.</span></span>

### <a name="users-of-on-premises-deployments"></a><span data-ttu-id="21964-116">Пользователи локальных развертываний</span><span class="sxs-lookup"><span data-stu-id="21964-116">Users of on-premises deployments</span></span>

<span data-ttu-id="21964-117">Для локальных развертываний [!INCLUDE[d365fin](includes/d365fin_md.md)] администратор может выбрать между различными механизмами авторизации учетной информации для пользователей.</span><span class="sxs-lookup"><span data-stu-id="21964-117">For on-premises deployments of [!INCLUDE[d365fin](includes/d365fin_md.md)], the administrator can choose between different credential authorization mechanisms for users.</span></span> <span data-ttu-id="21964-118">Затем при создании пользователя необходимо предоставить различную информацию в зависимости от используемого типа учетных данных в конкретном экземпляре [!INCLUDE[server](includes/server.md)].</span><span class="sxs-lookup"><span data-stu-id="21964-118">Then, when you create a user, you provide different information depending on the credential type that you are using in the specific [!INCLUDE[server](includes/server.md)] instance.</span></span> <span data-ttu-id="21964-119">Дополнительные сведения, см. в разделе [Проверка подлинности и типы учетных сведений](/dynamics365/business-central/dev-itpro/administration/users-credential-types) в разделе администрирование для разработчиков и содержимом ITPro для [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="21964-119">For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the Administration section of the developer and ITPro content for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="profiles-roles"></a><span data-ttu-id="21964-120">Профили (роли)</span><span class="sxs-lookup"><span data-stu-id="21964-120">Profiles (Roles)</span></span>

<span data-ttu-id="21964-121">Всем пользователям в организации, которые имеют доступ к [!INCLUDE[d365fin](includes/d365fin_md.md)], назначается роль, открывающая им доступ к центру *Ролевой центр*.</span><span class="sxs-lookup"><span data-stu-id="21964-121">The people in your company who have access to [!INCLUDE[d365fin](includes/d365fin_md.md)] are all assigned a role that gives them access to a *Role Center*.</span></span>

<span data-ttu-id="21964-122">Профили — это коллекции пользователей [!INCLUDE[d365fin](includes/d365fin_md.md)], которые относятся к одной роли.</span><span class="sxs-lookup"><span data-stu-id="21964-122">Profiles are collections of [!INCLUDE[d365fin](includes/d365fin_md.md)] users who share the same role.</span></span> <span data-ttu-id="21964-123">Ролевой центр является начальной страницей [!INCLUDE[d365fin](includes/d365fin_md.md)], с которой можно быстро запустить наиболее важные задачи и увидеть аналитику и КПЭ.</span><span class="sxs-lookup"><span data-stu-id="21964-123">A Role Center is the entry point and home page for [!INCLUDE[d365fin](includes/d365fin_md.md)] that gives you quick access to your most important tasks and displays various insights and key performance indicators (KPIs) about your work.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="21964-124">В текущей версии [!INCLUDE[d365fin](includes/d365fin_md.md)] Online невозможно добавлять, изменять или удалять профили.</span><span class="sxs-lookup"><span data-stu-id="21964-124">In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you cannot add, edit, or delete profiles.</span></span>  

### <a name="CreateProfile"></a><span data-ttu-id="21964-125">Создание профиля</span><span class="sxs-lookup"><span data-stu-id="21964-125">To create a profile</span></span>

1.  <span data-ttu-id="21964-126">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Профили**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="21964-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="21964-127">На странице **Профили** выберите действие **Создать** для открытия страницы **Создать карточку профиля**.</span><span class="sxs-lookup"><span data-stu-id="21964-127">On the **Profiles** page, choose the **New** action to open the **New Profile Card** page.</span></span>  

3.  <span data-ttu-id="21964-128">В поле **Код профиля** введите название, описывающее требуемую роль пользователей.</span><span class="sxs-lookup"><span data-stu-id="21964-128">In the **Profile ID** field, enter a name that describes the intended role of the users.</span></span>  

4.  <span data-ttu-id="21964-129">В поле **Описание** введите описание кода профиля, например **"Обработчик заказов"**.</span><span class="sxs-lookup"><span data-stu-id="21964-129">In the **Description** field, enter a description of the Profile ID, for example, **Order Processor**.</span></span>  

5.  <span data-ttu-id="21964-130">В поле **Код ролевого центра** установите ролевой центр, который требуется назначить этому профилю.</span><span class="sxs-lookup"><span data-stu-id="21964-130">Set the **Role Center ID** field to the Role Center that you want to assign to the profile.</span></span>  

<span data-ttu-id="21964-131">Процедура изменения существующего профиля такая же за исключением того, что необходимо выбрать существующий профиль на странице **Профили** вместо выбора действия **Создать**.</span><span class="sxs-lookup"><span data-stu-id="21964-131">The procedure for modifying an existing profile is the same, except you select an existing profile on the **Profiles** page instead of choosing the **New** action.</span></span>  


### <a name="copy-a-profile"></a><span data-ttu-id="21964-132">Копирование профиля</span><span class="sxs-lookup"><span data-stu-id="21964-132">Copy a profile</span></span>
<span data-ttu-id="21964-133">Копирование профиля может сэкономить время, если требуется использовать аналогичные настройки в профиле и необходимо изменить лишь несколько настроек.</span><span class="sxs-lookup"><span data-stu-id="21964-133">Copying a profile can save you time if you want to use similar settings on a profile and you only want to change a few settings.</span></span>

1.  <span data-ttu-id="21964-134">Откройте профиль, который необходимо скопировать, затем выберите действие **Копировать профиль**.</span><span class="sxs-lookup"><span data-stu-id="21964-134">Open the profile that you want to copy, and then choose the **Copy Profile** action.</span></span>

2.  <span data-ttu-id="21964-135">В поле **Код нового профиля** введите имя для профиля, который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="21964-135">In **New Profile ID** field, enter a name for the profile that you want to copy.</span></span>

3.  <span data-ttu-id="21964-136">Задайте в поле **Новая область профиля** одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="21964-136">Set the **New Profile Scope** field to one of the following:</span></span>

    - <span data-ttu-id="21964-137">**Система**, чтобы сделать новый профиль доступным всем базам данных арендаторов, которые используют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="21964-137">**System** to make the new profile available to all tenant databases that use the application.</span></span>
    - <span data-ttu-id="21964-138">**Арендатор**, чтобы сделать новый профиль доступным только для базы данных текущего арендатора.</span><span class="sxs-lookup"><span data-stu-id="21964-138">**Tenant** to make the new profile available to just the current tenant database.</span></span>
4. <span data-ttu-id="21964-139">По завершении нажмите кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="21964-139">Choose the **OK** button when done.</span></span>

### <a name="ExportImportProfile"></a><span data-ttu-id="21964-140">Экспорт и импорт профилей</span><span class="sxs-lookup"><span data-stu-id="21964-140">Export and import profiles</span></span>

<span data-ttu-id="21964-141">Можно экспортировать профили в виде XML-файлов в базу данных [!INCLUDE[d365fin](includes/d365fin_md.md)] и импортировать их из этой базы данных.</span><span class="sxs-lookup"><span data-stu-id="21964-141">You can export and import profiles as XML files to and from the a [!INCLUDE[d365fin](includes/d365fin_md.md)] database.</span></span> <span data-ttu-id="21964-142">Экспорт и импорт профиля может сэкономить время при настройке пользовательского интерфейса, так как используется существующая настройка профиля вместо настройки профиля с нуля.</span><span class="sxs-lookup"><span data-stu-id="21964-142">Exporting and importing a profile can save you time when configuring the user interface because you reuse an existing profile configuration instead of having to configure a profile from scratch.</span></span> <span data-ttu-id="21964-143">При имеется профиль, который настроен в базе данных [!INCLUDE[d365fin](includes/d365fin_md.md)], и вы хотите повторно использовать все или некоторые из конфигураций такого же профиля в другой базе данных, можно экспортировать профиль в XML-файл.</span><span class="sxs-lookup"><span data-stu-id="21964-143">If you have a profile that is configured in a [!INCLUDE[d365fin](includes/d365fin_md.md)] database and you would like to reuse all or some of the same profile configurations in another database, you can export the profile to an XML file.</span></span> <span data-ttu-id="21964-144">После этого, можно импортировать XML-файл профиля в другую базу данных.</span><span class="sxs-lookup"><span data-stu-id="21964-144">Then, you can import the profile XML file into the other database.</span></span>

-   <span data-ttu-id="21964-145">Для экспорта профиля можно либо выбрать действие **Экспорт профилей** на странице **Список профилей** или **Карточка профиля**, либо выполнить поиск страницы **Экспорт профилей** и открыть ее.</span><span class="sxs-lookup"><span data-stu-id="21964-145">To export a profile, you can either choose the **Export Profiles** action from the **Profile List** or **Profile Card** page or you can search for and open the **Export Profiles** page.</span></span> <span data-ttu-id="21964-146">Сохраните файл XML в папке на вашем компьютере или в сети.</span><span class="sxs-lookup"><span data-stu-id="21964-146">Save the XML file to a location on your computer or network.</span></span>

-   <span data-ttu-id="21964-147">Для импорта профиля можно либо выбрать действие **Импорт профиля** на странице **Список профилей**, либо выполнить поиск страницы **Импорт профилей** и открыть ее.</span><span class="sxs-lookup"><span data-stu-id="21964-147">To import a profile, you can either choose the **Import Profile** action from the **Profile List** page, or you can search for and open the **Import Profiles** page.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="21964-148">Невозможно импортировать профиль, который уже существует в базе данных, даже если файл XML имеет другое имя или содержимое.</span><span class="sxs-lookup"><span data-stu-id="21964-148">You cannot import a profile that already exists in the database, even though the XML file is named differently or has different content.</span></span> <span data-ttu-id="21964-149">Перед импортом нового профиля необходимо удалить существующий.</span><span class="sxs-lookup"><span data-stu-id="21964-149">You must delete the existing profile before you can import the new profile.</span></span>


## <a name="configuration-and-personalization"></a><span data-ttu-id="21964-150">Конфигурация и персонализация</span><span class="sxs-lookup"><span data-stu-id="21964-150">Configuration and Personalization</span></span>
<!--The concept of UI customization in [!INCLUDE[d365fin](includes/d365fin_md.md)] is divided in two:  

-   Configuration, performed by the administrator  

-   Personalization, performed by users  

The administrator configures the user interface for multiple users by customizing the user interface for a profile that the users are assigned to.  -->

<span data-ttu-id="21964-151">Пользователи персонализируют пользовательский интерфейс персональной версии, настраивая ИП после входа со своими учетными данными.</span><span class="sxs-lookup"><span data-stu-id="21964-151">Users personalize the user interface of their personal version by customizing the user interface under their own user logon.</span></span> <span data-ttu-id="21964-152">Эта персонализация может быть удалена администратором.</span><span class="sxs-lookup"><span data-stu-id="21964-152">This personalization can be deleted by the administrator.</span></span> <span data-ttu-id="21964-153">Дополнительные сведения см. в разделе [Персонализация рабочей области](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="21964-153">For more information, see [Personalizing Your Workspace](ui-personalization-user.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="21964-154">См. также</span><span class="sxs-lookup"><span data-stu-id="21964-154">See Also</span></span>  
[<span data-ttu-id="21964-155">Управление пользователями и разрешениями</span><span class="sxs-lookup"><span data-stu-id="21964-155">Managing Users and Permissions</span></span>](ui-how-users-permissions.md)  
[<span data-ttu-id="21964-156">Управление персонализацией в качестве администратора</span><span class="sxs-lookup"><span data-stu-id="21964-156">Managing Personalization as an Administrator</span></span>](ui-personalization-manage.md)  
[<span data-ttu-id="21964-157">Персонализация рабочей области</span><span class="sxs-lookup"><span data-stu-id="21964-157">Personalizing Your Workspace</span></span>](ui-personalization-user.md)  
