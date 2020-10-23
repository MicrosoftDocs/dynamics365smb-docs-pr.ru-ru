---
title: Управление интеграцией Microsoft Teams с Business Central | Документация Майкрософт
description: Управление интеграцией Business Central с Microsoft Teams.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork
ms.date: 10/08/2020
ms.author: jswymer
ms.openlocfilehash: 3c04dfb2f77eba906b2567ca9438849e1cc20861
ms.sourcegitcommit: 4bca699d2a5ce182eb5572d72fac4fb478c4f293
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/12/2020
ms.locfileid: "3989362"
---
# <a name="managing-microsoft-teams-integration-with-business-central"></a><span data-ttu-id="7c9c6-103">Управление интеграцией Microsoft Teams с Business Central</span><span class="sxs-lookup"><span data-stu-id="7c9c6-103">Managing Microsoft Teams Integration with Business Central</span></span>

[!INCLUDE [teams_preview.md](includes/teams_preview.md)]

<span data-ttu-id="7c9c6-104">В этой статье представлен обзор того, что вы можете делать как администратор для управления интеграцией Microsoft Teams с [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="7c9c6-104">This article provides an overview of what you can do as an administrator to control Microsoft Teams integration with [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>

## <a name="in-microsoft-teams"></a><span data-ttu-id="7c9c6-105">В Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7c9c6-105">In Microsoft Teams</span></span>

### <a name="minimum-requirements"></a><span data-ttu-id="7c9c6-106">Минимальные требования</span><span class="sxs-lookup"><span data-stu-id="7c9c6-106">Minimum requirements</span></span>

<span data-ttu-id="7c9c6-107">В этом разделе описаны минимальные требования для работы функций приложения [!INCLUDE [prodshort](includes/prodshort.md)] в Teams.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-107">This section describes the minimum requirements for the [!INCLUDE [prodshort](includes/prodshort.md)] app features to work in Teams.</span></span>

- <span data-ttu-id="7c9c6-108">Необходимые лицензии</span><span class="sxs-lookup"><span data-stu-id="7c9c6-108">Required licenses</span></span>

    <span data-ttu-id="7c9c6-109">В этой таблице представлен обзор лицензий, необходимых для работы функций приложения [!INCLUDE [prodshort](includes/prodshort.md)] в Teams.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-109">This table gives you an overview of the licenses needed for the [!INCLUDE [prodshort](includes/prodshort.md)] app features to work in Teams.</span></span>

    |<span data-ttu-id="7c9c6-110">Какая</span><span class="sxs-lookup"><span data-stu-id="7c9c6-110">What</span></span>|<span data-ttu-id="7c9c6-111">Лицензия Teams</span><span class="sxs-lookup"><span data-stu-id="7c9c6-111">Teams license</span></span>|<span data-ttu-id="7c9c6-112">Лицензия Business Central</span><span class="sxs-lookup"><span data-stu-id="7c9c6-112">Business Central license</span></span>|
    |----|---|---|
    |<span data-ttu-id="7c9c6-113">Вставьте ссылку в запись [!INCLUDE [prodshort](includes/prodshort.md)] в беседу и отправьте как карточку.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-113">Paste a link to a [!INCLUDE [prodshort](includes/prodshort.md)] record into a conversation, and send it as a card.</span></span>|<span data-ttu-id="7c9c6-114">![флажок](media/check.png "галочка")</span><span class="sxs-lookup"><span data-stu-id="7c9c6-114">![check mark](media/check.png "check")</span></span>|<span data-ttu-id="7c9c6-115">![флажок](media/check.png "галочка")</span><span class="sxs-lookup"><span data-stu-id="7c9c6-115">![check mark](media/check.png "check")</span></span>|
    |<span data-ttu-id="7c9c6-116">Посмотреть карточку записи [!INCLUDE [prodshort](includes/prodshort.md)] в разговоре.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-116">View a card of a [!INCLUDE [prodshort](includes/prodshort.md)] record in a conversation.</span></span>|<span data-ttu-id="7c9c6-117">![флажок](media/check.png "галочка")</span><span class="sxs-lookup"><span data-stu-id="7c9c6-117">![check mark](media/check.png "check")</span></span>||
    |<span data-ttu-id="7c9c6-118">Посмотреть подробности карточки записи [!INCLUDE [prodshort](includes/prodshort.md)] в разговоре.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-118">View more details of card for a [!INCLUDE [prodshort](includes/prodshort.md)] record in a conversation.</span></span>|<span data-ttu-id="7c9c6-119">![флажок](media/check.png "галочка")</span><span class="sxs-lookup"><span data-stu-id="7c9c6-119">![check mark](media/check.png "check")</span></span>|<span data-ttu-id="7c9c6-120">![флажок](media/check.png "галочка")</span><span class="sxs-lookup"><span data-stu-id="7c9c6-120">![check mark](media/check.png "check")</span></span>|

- <span data-ttu-id="7c9c6-121">Разрешить предварительный просмотр URL-адресов</span><span class="sxs-lookup"><span data-stu-id="7c9c6-121">Allow URL previews</span></span>

    <span data-ttu-id="7c9c6-122">Параметр политики **Разрешить предварительный просмотр URL-адресов** должен быть включен.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-122">**Allow URL previews** policy setting must be turned on.</span></span> <span data-ttu-id="7c9c6-123">В противном случае невозможно создать карточку для ссылок Business Central, вставленных в беседу Teams.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-123">Otherwise, a card can't be generated for Business Central links pasted into a Teams conversation.</span></span> <span data-ttu-id="7c9c6-124">Для получения дополнительной информации об этом параметре см. [Управляйте политиками обмена сообщениями в Teams](/microsoftteams/messaging-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="7c9c6-124">For more information about this setting, see [Manage messaging policies in Teams](/microsoftteams/messaging-policies-in-teams).</span></span>

### <a name="managing-the-business-central-app-optional"></a><span data-ttu-id="7c9c6-125">Управление приложением Business Central (необязательно)</span><span class="sxs-lookup"><span data-stu-id="7c9c6-125">Managing the Business Central app (optional)</span></span>

<span data-ttu-id="7c9c6-126">Как администратор Teams вы можете управлять всеми приложениями для своей организации, включая приложение [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="7c9c6-126">As a Teams administrator, you can manage all apps for your organization, including the [!INCLUDE [prodshort](includes/prodshort.md)] app.</span></span> <span data-ttu-id="7c9c6-127">Вы можете утвердить или установить приложение [!INCLUDE [prodshort](includes/prodshort.md)] для вашей организации, запретить пользователю устанавливать приложение и т. д.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-127">You can approve or install the [!INCLUDE [prodshort](includes/prodshort.md)] app for your organization, block user's from installing the app, and more.</span></span>

<span data-ttu-id="7c9c6-128">Для получения дополнительной информации см. следующие статьи в документации Microsoft Teams:</span><span class="sxs-lookup"><span data-stu-id="7c9c6-128">For more information, see the following articles in the Microsoft Teams documentation:</span></span>

- [<span data-ttu-id="7c9c6-129">Управляйте своими приложениями в центре администрирования Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7c9c6-129">Manage your apps in the Microsoft Teams admin center</span></span>](https://docs.microsoft.com/MicrosoftTeams/manage-apps)
- [<span data-ttu-id="7c9c6-130">Управляйте политиками настройки приложений в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7c9c6-130">Manage app setup policies in Microsoft Teams</span></span>](https://docs.microsoft.com/microsoftteams/teams-app-setup-policies)

## <a name="in-prodshort"></a><span data-ttu-id="7c9c6-131">В [!INCLUDE [prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="7c9c6-131">In [!INCLUDE [prodshort](includes/prodshort.md)]</span></span>

### <a name="minimum-requirements"></a><span data-ttu-id="7c9c6-132">Минимальные требования</span><span class="sxs-lookup"><span data-stu-id="7c9c6-132">Minimum requirements</span></span>

- <span data-ttu-id="7c9c6-133">Версия [!INCLUDE [prodshort](includes/prodshort.md)]:</span><span class="sxs-lookup"><span data-stu-id="7c9c6-133">[!INCLUDE [prodshort](includes/prodshort.md)] version:</span></span>

    <span data-ttu-id="7c9c6-134">[!INCLUDE [prodshort](includes/prodshort.md)] выпуск 2020, волна 2 (версия 17) или новее.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-134">[!INCLUDE [prodshort](includes/prodshort.md)] 2020 release wave 2 (version 17) or later.</span></span> <span data-ttu-id="7c9c6-135">Интеграция Teams поддерживается только для [!INCLUDE [prodshort](includes/prodshort.md)] (онлайн); не локально.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-135">Teams integration is only supported for [!INCLUDE [prodshort](includes/prodshort.md)] online; not on-premises.</span></span>

- <span data-ttu-id="7c9c6-136">Codeunit **2718, поставщик сводки по страницам** публикуется как веб-сервис:</span><span class="sxs-lookup"><span data-stu-id="7c9c6-136">Codeunit **2718 Page Summary Provider** is published as a web service:</span></span>

    <span data-ttu-id="7c9c6-137">Этот codeunit публикуется как веб-служба по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-137">This codeunit is published as a web service by default.</span></span> <span data-ttu-id="7c9c6-138">codeunit является частью системного приложения [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="7c9c6-138">The codeunit is part of the [!INCLUDE [prodshort](includes/prodshort.md)] system application.</span></span> <span data-ttu-id="7c9c6-139">Он используется для получения данных поля для страницы [!INCLUDE [prodshort](includes/prodshort.md)], добавленной в беседу Teams.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-139">It's used to get the field data for a [!INCLUDE [prodshort](includes/prodshort.md)] page added to a Teams conversation.</span></span> 

- <span data-ttu-id="7c9c6-140">Разрешения пользователя:</span><span class="sxs-lookup"><span data-stu-id="7c9c6-140">User permissions:</span></span>

    <span data-ttu-id="7c9c6-141">Как правило, страницы и данные, которые пользователи могут просматривать и редактировать в беседе Teams, контролируются их разрешениями в [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="7c9c6-141">For the most part, the pages and data that users can view and edit in a Teams conversation is controlled by their permissions in [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>
    
    - <span data-ttu-id="7c9c6-142">Чтобы вставить ссылку [!INCLUDE [prodshort](includes/prodshort.md)] в беседу Teams и развернуть ее в карточку, пользователи должны иметь как минимум разрешение на чтение страницы и ее данных.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-142">To paste a [!INCLUDE [prodshort](includes/prodshort.md)] link into a Teams conversation and have it expand into a card, users must have at least read permission on the page and its data.</span></span>
    - <span data-ttu-id="7c9c6-143">После того, как карточка отправлена в беседу, любой пользователь в этой беседе может просматривать эту карточку без разрешения Business Central.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-143">Once a card is submitted into a conversation, any user in that conversation can view that card without permission to Business Central.</span></span>
    - <span data-ttu-id="7c9c6-144">Чтобы просмотреть подробную информацию о карте или открыть запись в [!INCLUDE [prodshort](includes/prodshort.md)], пользователи должны иметь разрешение на чтение страницы и ее данных.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-144">To view more details for a card or open the record in [!INCLUDE [prodshort](includes/prodshort.md)], users must have read permission on the page and its data.</span></span>
    - <span data-ttu-id="7c9c6-145">Чтобы изменить данные, пользователю необходимо изменить разрешения.</span><span class="sxs-lookup"><span data-stu-id="7c9c6-145">To change data, user's need modify permissions.</span></span>
    
    <span data-ttu-id="7c9c6-146">Сведения о разрешениях см. в разделе [Назначение разрешений пользователям и группам](ui-define-granular-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="7c9c6-146">For information about permissions, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="7c9c6-147">См. также</span><span class="sxs-lookup"><span data-stu-id="7c9c6-147">See Also</span></span>
[<span data-ttu-id="7c9c6-148">Обзор интеграции Business Central и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7c9c6-148">Business Central and Microsoft Teams Integration Overview</span></span>](across-teams-overview.md)  
<span data-ttu-id="7c9c6-149">[Установите приложение [!INCLUDE [prodshort](includes/prodshort.md)] для Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="7c9c6-149">[Install the [!INCLUDE [prodshort](includes/prodshort.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>  
[<span data-ttu-id="7c9c6-150">Разработка для интеграции Teams</span><span class="sxs-lookup"><span data-stu-id="7c9c6-150">Developing for Teams Integration</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  
[<span data-ttu-id="7c9c6-151">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="7c9c6-151">Getting Started</span></span>](product-get-started.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
