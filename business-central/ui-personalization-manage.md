---
title: Управление персонализацией в качестве администратора Business Central | Microsoft Docs
description: Узнайте, как настраивать пользовательский интерфейс в соответствии с вашим способом работы.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 08/16/2019
ms.author: jswymer
ms.openlocfilehash: 268d61e05f84643abe8eeeb283bd035e0247fe1c
ms.sourcegitcommit: 81b6062194bf04d8052a3cd394cc0b41e3f53e6d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2019
ms.locfileid: "1887741"
---
# <a name="managing-personalization-as-an-administrator"></a><span data-ttu-id="dd1a0-103">Управление персонализацией в качестве администратора</span><span class="sxs-lookup"><span data-stu-id="dd1a0-103">Managing Personalization as an Administrator</span></span>

<span data-ttu-id="dd1a0-104">Пользователи могут персонализировать свои рабочие области в соответствии со своими предпочтениями.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-104">Users can personalize their workspace to suit their own preferences.</span></span> <span data-ttu-id="dd1a0-105">Как администратор, вы контролируете персонализацию и управляете ее следующими способами:</span><span class="sxs-lookup"><span data-stu-id="dd1a0-105">As an administrator, you control and manage personalization by:</span></span>

-   <span data-ttu-id="dd1a0-106">Включая или отключая функцию персонализации для всего приложения (только локальные установки).</span><span class="sxs-lookup"><span data-stu-id="dd1a0-106">Enabling or disabling the personalization feature for the entire the application (on-premises installation only).</span></span>
-   <span data-ttu-id="dd1a0-107">Включая или отключая функцию персонализации для пользователей определенного профиля.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-107">Enabling or disabling the personalization feature for users of a specific profile.</span></span>
-   <span data-ttu-id="dd1a0-108">Сбрасываю все персонализации страницы, сделанные пользователями.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-108">Clearing any page personalizations that users have made.</span></span>

## <a name="EnablePersonalization"></a><span data-ttu-id="dd1a0-109">Включение или отключение персонализации (только On-Premises)</span><span class="sxs-lookup"><span data-stu-id="dd1a0-109">To enable or disable personalization (On-Premises Only)</span></span>

<span data-ttu-id="dd1a0-110">По умолчанию персонализация в клиенте отключена.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-110">By default, personalization is not enabled in the client.</span></span> <span data-ttu-id="dd1a0-111">Персонализация включается или отключается путем изменения файла конфигурации (navsettings.json) экземпляра Business Central Web Server, который обслуживание клиентов.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-111">You enable or disable personalization by modifying the configuration file (navsettings.json) of the Business Central Web Server instance that serves the clients.</span></span>

1. <span data-ttu-id="dd1a0-112">Чтобы включить персонализацию, добавьте следующую строку в файл navsettings.json:</span><span class="sxs-lookup"><span data-stu-id="dd1a0-112">To enable personalization, add the following line in the navsettings.json file:</span></span>

    ```
    "PersonalizationEnabled": "true"
    ```

    <span data-ttu-id="dd1a0-113">Чтобы отключить персонализацию, удалите эту строку или измените ее на:</span><span class="sxs-lookup"><span data-stu-id="dd1a0-113">To disable personalization, remove this line or change it to:</span></span>

    ```
    "PersonalizationEnabled": "false"
    ```

    <span data-ttu-id="dd1a0-114">Дополнительные сведения о том, как изменять файл navsettings.json, см. в разделе [Непосредственное изменение файла navsettings.json](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configure-web-server?branch=master#Settings)</span><span class="sxs-lookup"><span data-stu-id="dd1a0-114">For more information about how to modify the navsettings.json file, see [Modify the navsettings.json file directly](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configure-web-server?branch=master#Settings).</span></span>

2. <span data-ttu-id="dd1a0-115">Создайте и загрузите символы приложения.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-115">Generate and download the application symbols.</span></span>

    <span data-ttu-id="dd1a0-116">Это необязательный шаг, который не требуется для включения персонализации.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-116">This step is optional, and not required to enable personalization.</span></span> <span data-ttu-id="dd1a0-117">Однако он гарантирует, что новые страницы, которые созданы разработчиками, можно персонализировать.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-117">However, it ensures that new pages that are created by developers can be personalized.</span></span>

    1. <span data-ttu-id="dd1a0-118">Сначала создайте символы, запустив файл finsql.exe с помощью команды `generatesymbolreference`.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-118">First, you generate the symbols by running finsql.exe with `generatesymbolreference` command.</span></span> <span data-ttu-id="dd1a0-119">Файл finsql.exe находится в папке установки для среды разработки [!INCLUDE[server](includes/server.md)] и Dynamics NAV (CSIDE).</span><span class="sxs-lookup"><span data-stu-id="dd1a0-119">The finsql.exe file is located in the installation folder for the [!INCLUDE[server](includes/server.md)] and Dynamics NAV Development Environment (CSIDE).</span></span> <span data-ttu-id="dd1a0-120">Для генерации символов откройте командную строку, перейдите в каталог, в котором хранится файл, и запустите следующую команду:</span><span class="sxs-lookup"><span data-stu-id="dd1a0-120">To generate the symbols, open a command prompt, change to the directory where the file is store, and the run the following command:</span></span>

        ```
        finsql.exe Command=generatesymbolreference, Database="<Database Name>", ServerName=<SQL Server Name\<Server Instance>
        ```
    <span data-ttu-id="dd1a0-121">Например:</span><span class="sxs-lookup"><span data-stu-id="dd1a0-121">For example:</span></span>

        ```
        finsql.exe Command=generatesymbolreference, Database="Demo Database BC", ServerName=MySQLServer\BCDEMO
        ```

    <span data-ttu-id="dd1a0-122">Дополнительные сведения см. в разделе [Одновременный запуск C/SIDE и AL](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-running-cside-and-al-side-by-side).</span><span class="sxs-lookup"><span data-stu-id="dd1a0-122">For more information, see [Running C/SIDE and AL Side-by-Side](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-running-cside-and-al-side-by-side).</span></span>

    2. <span data-ttu-id="dd1a0-123">Настройте экземпляр [!INCLUDE[nav_server_md](includes/nav_server_md.md)] на **Включить загрузку ссылок символов приложений при запуске сервера** (EnableSymbolLoadingAtServerStartup).</span><span class="sxs-lookup"><span data-stu-id="dd1a0-123">Configure [!INCLUDE[nav_server_md](includes/nav_server_md.md)] instance to **Enable loading application symbol references at server startup** (EnableSymbolLoadingAtServerStartup).</span></span> <span data-ttu-id="dd1a0-124">Дополнительные сведения см. в разделе [Настройка Business Central Server](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configure-server-instance#development-settings).</span><span class="sxs-lookup"><span data-stu-id="dd1a0-124">For more information, see [Configuring Business Central Server](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configure-server-instance#development-settings).</span></span>

## <a name="to-disable-personalization-for-a-profile"></a><span data-ttu-id="dd1a0-125">Отключение персонализации для профиля</span><span class="sxs-lookup"><span data-stu-id="dd1a0-125">To disable personalization for a profile</span></span>

<span data-ttu-id="dd1a0-126">Всем пользователям, которые принадлежат к определенному профилю, можно отключить возможность персонализировать их страницы.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-126">You can prevent all users that belong to a specific profile from being able to personalize their pages.</span></span>

1. <span data-ttu-id="dd1a0-127">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Профили**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Profiles**, and then choose the related link.</span></span>
2. <span data-ttu-id="dd1a0-128">Выберите профиль в списке, который необходимо изменить.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-128">Select the profile in the list that you want to modify.</span></span>
3. <span data-ttu-id="dd1a0-129">Установите флажок **Отключить персонализацию**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-129">Select the **Disable personalization** check box, and then choose the **OK** button.</span></span>

> [!NOTE]  
> <span data-ttu-id="dd1a0-130">В Business Central Online можно отключить персонализацию только для профиля клиента, но не для системных профилей.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-130">In Business Central online, you can only disable personalization for a tenant profile, not for system profiles.</span></span> 

## <a name="to-clear-user-personalizations"></a><span data-ttu-id="dd1a0-131">Очистка пользовательских персонализаций</span><span class="sxs-lookup"><span data-stu-id="dd1a0-131">To clear user personalizations</span></span>

<span data-ttu-id="dd1a0-132">При очистки персонализации страницы восстанавливается первоначальный макет страницы до того, как была произведена какая-либо персонализация.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-132">Clearing page personalization changes the page back to its original layout before any personalization was made.</span></span> <span data-ttu-id="dd1a0-133">Существует два способа очистить персонализации, которые пользователи сделали на страницах: с помощью страницы **Удалить персонализацию пользователя** и с помощью страницы **Карточка персонализации пользователя**.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-133">There are two ways to clear the personalizations that users have made to pages: using the **Delete User Personalization** page and using the **User Personalization Card** page.</span></span>

### <a name="to-clear-user-personalizations-by-using-the-delete-user-personalization-page"></a><span data-ttu-id="dd1a0-134">Очистка персонализаций пользователя с помощью страницы "Удалить персонализацию пользователя"</span><span class="sxs-lookup"><span data-stu-id="dd1a0-134">To clear user personalizations by using the Delete User Personalization page</span></span>

<span data-ttu-id="dd1a0-135">Страница **Удалить персонализацию пользователя** позволяет удалять персонализацию для отдельных страниц для каждого пользователя по-отдельности.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-135">The **Delete User Personalization** page enables you to clear personalizations on a per-page basis for each user individually.</span></span>

1. <span data-ttu-id="dd1a0-136">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Удалить персонализацию пользователя**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="dd1a0-137">На этой странице отображаются все страницы, которые были персонализированы, и пользователь, которому принадлежит эта страница.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-137">The page lists all the pages that have been personalized and the user it belongs to.</span></span>

    >[!NOTE]
    > <span data-ttu-id="dd1a0-138">Флажок в столбцах **Персонализация унаследованных данных** указывает, что персонализация была выполнен а более старой версии [!INCLUDE[d365fin](includes/d365fin_md.md)], в которой персонализация выполнялась не так, как сейчас.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-138">A check mark in the **Legacy Personalization** columns indicates that the personalization was done in an older version of [!INCLUDE[d365fin](includes/d365fin_md.md)], which handled personalization different than it does now.</span></span> <span data-ttu-id="dd1a0-139">Для пользователей, которые пытаются персонализировать эти страницы, эта операция блокируется, если они не решат разблокировать страницу.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-139">Users who try to personalize these pages are locked from doing so unless they choose to unlock the page.</span></span> <span data-ttu-id="dd1a0-140">Дополнительные сведения см. в разделе [Почему заблокирована персонализация страницы?](ui-personalization-locked.md).</span><span class="sxs-lookup"><span data-stu-id="dd1a0-140">For more information, see [Why a page is locked from personalizing](ui-personalization-locked.md).</span></span>

2. <span data-ttu-id="dd1a0-141">Выберите операцию, которую требуется удалить, затем выберите действие **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-141">Select the entry that you want to delete, and then choose the **Delete** action.</span></span>

    <span data-ttu-id="dd1a0-142">Пользователь увидит изменения при следующем входе в систему.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-142">The user will see the changes the next time they sign-in.</span></span>

### <a name="to-clear-user-personalizations-by-using-the-user-personalization-card-page"></a><span data-ttu-id="dd1a0-143">Очистка персонализаций пользователя с помощью страницы "Карточка персонализации пользователя"</span><span class="sxs-lookup"><span data-stu-id="dd1a0-143">To clear user personalizations by using the User Personalization Card page</span></span>

<span data-ttu-id="dd1a0-144">Страница **Карточка персонализации пользователя** позволяет удалять персонализацию для всех страниц определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-144">The **User Personalization Card** page enables you to clear the personalization on all pages for specific user.</span></span> <span data-ttu-id="dd1a0-145">Для этого необходимо разрешение на запись для таблицы 2000000072 **Профиль**.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-145">This requires write permission to Table 2000000072 **Profile**.</span></span>

1. <span data-ttu-id="dd1a0-146">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Персонализация пользователя**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-146">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="dd1a0-147">На странице **Персонализация пользователя** перечисляются все пользователи, у которых потенциально есть персонализированные страницы.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-147">The **User Personalization** page lists all users who potentially have personalized pages.</span></span> <span data-ttu-id="dd1a0-148">Если не удается найти пользователя в списке, это означает, что у него нет никаких персонализированных страниц.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-148">If you cannot find a user in the list, this means that they do not have any personalized pages.</span></span>

2. <span data-ttu-id="dd1a0-149">Выберите пользователя из списка, затем выберите действие **Правка**.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-149">Select the user from the list, and then choose the **Edit** action.</span></span>

3. <span data-ttu-id="dd1a0-150">На вкладке **Действия** выберите **Очистить персонализированные страницы**.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-150">On the **Actions** tab, choose **Clear Personalized Pages**.</span></span>

    <span data-ttu-id="dd1a0-151">Пользователь увидит изменения при следующем входе в систему.</span><span class="sxs-lookup"><span data-stu-id="dd1a0-151">The user will see the changes the next time they sign-in.</span></span>

## <a name="see-also"></a><span data-ttu-id="dd1a0-152">См. также</span><span class="sxs-lookup"><span data-stu-id="dd1a0-152">See Also</span></span>
[<span data-ttu-id="dd1a0-153">Персонализация рабочей области</span><span class="sxs-lookup"><span data-stu-id="dd1a0-153">Personalizing Your Workspace</span></span>](ui-personalization-user.md)  
<span data-ttu-id="dd1a0-154">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="dd1a0-154">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="dd1a0-155">Изменение базовых настроек</span><span class="sxs-lookup"><span data-stu-id="dd1a0-155">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="dd1a0-156">Изменение набора отображаемых функций</span><span class="sxs-lookup"><span data-stu-id="dd1a0-156">Changing Which Features are Displayed</span></span>](ui-experiences.md)  
