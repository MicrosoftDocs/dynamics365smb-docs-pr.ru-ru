---
title: Работа с данными Business Central в Microsoft Teams | Документация Майкрософт
description: Узнайте, как использовать приложение Business Central для Microsoft Teams.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork
ms.date: 10/08/2020
ms.author: jswymer
ms.openlocfilehash: fbe024f724f018aae6d3aeb5251281bf4c3bfbde
ms.sourcegitcommit: 4bca699d2a5ce182eb5572d72fac4fb478c4f293
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/12/2020
ms.locfileid: "3989429"
---
# <a name="working-with-business-central-data-in-microsoft-teams"></a><span data-ttu-id="cd9eb-103">Работа с данными Business Central в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cd9eb-103">Working with Business Central Data in Microsoft Teams</span></span>

[!INCLUDE [teams_preview.md](includes/teams_preview.md)]

<span data-ttu-id="cd9eb-104">[!INCLUDE [prodshort](includes/prodshort.md)] предлагает приложение, которое соединяет Microsoft Teams с вашими бизнес-данным в [!INCLUDE [prodshort](includes/prodshort.md)], чтобы вы могли быстро обмениваться данными между участниками команды и быстрее отвечать на запросы.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-104">[!INCLUDE [prodshort](includes/prodshort.md)] offers an app that connects Microsoft Teams to your business data in [!INCLUDE [prodshort](includes/prodshort.md)], so you can quickly share details across team members and respond faster to inquiries.</span></span> <span data-ttu-id="cd9eb-105">В этой статье вы узнаете, как использовать приложение для обмена данными [!INCLUDE [prodshort](includes/prodshort.md)] с коллегами в беседе в Teams.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-105">In this article, you'll learn how to use the app to share [!INCLUDE [prodshort](includes/prodshort.md)] data with coworkers in a Teams conversation.</span></span>

## <a name="overview"></a><span data-ttu-id="cd9eb-106">Обзор</span><span class="sxs-lookup"><span data-stu-id="cd9eb-106">Overview</span></span>

<span data-ttu-id="cd9eb-107">Приложение позволяет [!INCLUDE [prodshort](includes/prodshort.md)]:</span><span class="sxs-lookup"><span data-stu-id="cd9eb-107">The [!INCLUDE [prodshort](includes/prodshort.md)] app lets you:</span></span>

- <span data-ttu-id="cd9eb-108">Скопируйте ссылку на любую запись Business Central и вставьте ее в беседу Teams, чтобы поделиться ею с коллегами.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-108">Copy a link to any Business Central record and paste it into a Teams conversation to share with your coworkers.</span></span> <span data-ttu-id="cd9eb-109">Ссылка превратится в компактную интерактивную карточку, отображающую информацию о записи.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-109">The link will expand that into a compact, interactive card that displays information about the record.</span></span>
- <span data-ttu-id="cd9eb-110">После разговора вы и ваши коллеги можете просматривать дополнительные сведения о записи, редактировать данные и принимать меры — не выходя из Teams.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-110">Once in the conversation, you and coworkers can view more details about the record, edit data, and take action - without leaving Teams.</span></span>

<span data-ttu-id="cd9eb-111">[![Интеграция Teams с Business Central](media/teams-intro-v3.png)](media/teams-intro-v3.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="cd9eb-111">[![Teams integration with Business Central](media/teams-intro-v3.png)](media/teams-intro-v3.png#lightbox)</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd9eb-112">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="cd9eb-112">Prerequisites</span></span>

- <span data-ttu-id="cd9eb-113">У вас есть доступ к Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-113">You have access to Microsoft Teams.</span></span>
- <span data-ttu-id="cd9eb-114">Вы установили приложение [!INCLUDE [prodshort](includes/prodshort.md)] в Teams.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-114">You've installed the [!INCLUDE [prodshort](includes/prodshort.md)] app in Teams.</span></span> <span data-ttu-id="cd9eb-115">Для получения дополнительной информации см.[ Установка приложения [!INCLUDE [prodshort](includes/prodshort.md)] для Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="cd9eb-115">For more information, see [Install the [!INCLUDE [prodshort](includes/prodshort.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>

> [!NOTE]
> <span data-ttu-id="cd9eb-116">Все участники беседы Teams смогут просматривать карточки для записей Business Central, которые вы отправляете в беседу.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-116">All participants in a Teams conversation will be able to view cards for Business Central records that you submit to the conversation.</span></span> <span data-ttu-id="cd9eb-117">Но чтобы просмотреть более подробную информацию о записях, используя кнопки **Подробнее** или **Открыть на новой вкладке**, им потребуется доступ [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="cd9eb-117">But to view more details about records, by using the **Details** or **Pop-out** buttons on a card, they'll need access to [!INCLUDE [prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="cd9eb-118">Дополнительные сведения см. в разделе [Управление интеграцией Microsoft Teams](admin-teams-integration.md#minimum-requirements-1).</span><span class="sxs-lookup"><span data-stu-id="cd9eb-118">For more information, see [Managing Microsoft Teams Integration](admin-teams-integration.md#minimum-requirements-1).</span></span>
<!--
- People You and your coworkers have the following permissions in [!INCLUDE [prodshort](includes/prodshort.md)]
  - To paste a [!INCLUDE [prodshort](includes/prodshort.md)] link into a Teams conversation and have it expand into a card, you have to have at least permission to view the page and its data.
  - Once a card is submitted into a conversation, any user in that conversation can view that card without having permission to Business Central.
  - For other users to view more details from card, they must also have view permission, as a minimum, to the page and its data. If they want to change data, they'll need modify permissions.

  Setting up permissions is typically done by an administrator. For more information, see [Managing Microsoft Teams Integration](admin-teams-integration.md).-->

## <a name="include-a-business-central-card-in-a-teams-conversation"></a><span data-ttu-id="cd9eb-119">Включите карточку Business Central в беседу в Teams</span><span class="sxs-lookup"><span data-stu-id="cd9eb-119">Include a Business Central card in a Teams conversation</span></span>

1. <span data-ttu-id="cd9eb-120">Водите в [!INCLUDE [prodshort](includes/prodshort.md)], используя ваш браузер.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-120">Sign in to [!INCLUDE [prodshort](includes/prodshort.md)] using your browser.</span></span>
2. <span data-ttu-id="cd9eb-121">Откройте запись, которое требуется поделиться.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-121">Open the record that you want to share.</span></span>

    <span data-ttu-id="cd9eb-122">Приложение предназначено для отображения страниц типа карточек из [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="cd9eb-122">The app is designed to display card type pages from [!INCLUDE [prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="cd9eb-123">Итак, откройте страницу, которая отображает одну запись, например товар, клиента или заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-123">So open a page that displays a single record, like an item, customer, or sales order.</span></span> <span data-ttu-id="cd9eb-124">Вы не можете использовать его для центров ролей или страниц, отображающих несколько записей в списке.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-124">You can't use it for role centers or pages that display several records in a list.</span></span>

3. <span data-ttu-id="cd9eb-125">Скопируйте весь URL-адрес из адресной строки браузера.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-125">Copy the entire URL from the browser's address bar.</span></span>

   ![Скопируйте URL-адрес Business Central из браузера](media/teams-url.png)
4. <span data-ttu-id="cd9eb-127">Перейдите в Teams и начните разговор, который может быть чатом с человеком, группой людей или групповым каналом.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-127">Go to Teams and start a conversation, which can be chat with a person, group of persons, or a team channel.</span></span>

    <!--Teams imposes a few limitations here eg. you cannot unfurl a link during a Voice/Video call :/ We should probably only mention this in a Troubleshooting section (and i hope it will also be fixed soon)-->
5. <span data-ttu-id="cd9eb-128">Вставьте URL-адрес в поле, в которое вы добавляете сообщение.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-128">Paste the URL into the box where you add a message.</span></span>

   ![Вставьте URL-адрес Business Central в Teams](media/teams-paste-url.png)
6. <span data-ttu-id="cd9eb-130">Когда вы впервые вставите ссылку в беседу, вам будет предложено войти в [!INCLUDE [prodshort](includes/prodshort.md)] и дать согласие на получение данных приложением.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-130">The first time you paste a link into a conversation, you'll be asked to sign in to [!INCLUDE [prodshort](includes/prodshort.md)] and give consent for the app to retrieve data.</span></span> <span data-ttu-id="cd9eb-131">Просто следуйте инструкциям на экране.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-131">Just follow the on-screen instructions.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cd9eb-132">Вам нужно выполнить этот шаг только один раз.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-132">You'll only have to do this step once.</span></span>

7. <span data-ttu-id="cd9eb-133">Подождите, пока в окне сообщения появится карточка.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-133">Wait a moment while a card is generated in the message box.</span></span>

8. <span data-ttu-id="cd9eb-134">Когда карточка появится, внимательно проверьте содержимое карточки на наличие конфиденциальной информации перед отправкой сообщения.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-134">When the card appears, review the contents of the card carefully for any sensitive information before sending the message.</span></span> <span data-ttu-id="cd9eb-135">Этот шаг важен, потому что как только вы отправите сообщение, все участники беседы смогут увидеть карточку.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-135">This step is important because once you send the message, everyone in the conversation can see the card.</span></span>

9. <span data-ttu-id="cd9eb-136">Если карточка выглядит хорошо, выберите **Отправить**, чтобы отправить ее в беседу.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-136">If the card looks good, select **Send** to submit it to the conversation.</span></span>

    > [!TIP]
    > <span data-ttu-id="cd9eb-137">После появления карточки и до того, как вы выберете **Отправить**, вы можете удалить вставленный URL-адрес, если хотите.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-137">After the card appears, and before you select **Send**, you can delete the pasted URL if you like.</span></span>

10. <span data-ttu-id="cd9eb-138">Чтобы просмотреть дополнительные сведения или внести изменения в запись, выберите **Подробнее**.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-138">To view more details or make changes to the record, select **Details**.</span></span>

    <span data-ttu-id="cd9eb-139">Страница сведений похожа на то, что вы бы видели в [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="cd9eb-139">The details page is similar to what you'd see in [!INCLUDE [prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="cd9eb-140">Но для Teams версия немного урезана.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-140">But it's slightly trimmed for Teams.</span></span> <span data-ttu-id="cd9eb-141">Когда вы закончите просмотр и внесите изменения, закройте окно, чтобы вернуться к беседе Teams.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-141">When you're finished viewing and making changes, close the window to return to the Teams conversation.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cd9eb-142">Любые внесенные вами изменения не будут отражены в карточке до тех пор, пока вы в следующий раз не вставите ссылку на нее в беседу.</span><span class="sxs-lookup"><span data-stu-id="cd9eb-142">Any changes you make won't be reflected in the card until the next time you paste its link in a conversation.</span></span>

## <a name="see-also"></a><span data-ttu-id="cd9eb-143">См. также</span><span class="sxs-lookup"><span data-stu-id="cd9eb-143">See Also</span></span>

[<span data-ttu-id="cd9eb-144">Обзор интеграции Business Central и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cd9eb-144">Business Central and Microsoft Teams Integration Overview</span></span>](across-teams-overview.md)  
<span data-ttu-id="cd9eb-145">[Установите приложение [!INCLUDE [prodshort](includes/prodshort.md)] для Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="cd9eb-145">[Install the [!INCLUDE [prodshort](includes/prodshort.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>  
[<span data-ttu-id="cd9eb-146">Разработка для интеграции Teams</span><span class="sxs-lookup"><span data-stu-id="cd9eb-146">Developing for Teams Integration</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  
[<span data-ttu-id="cd9eb-147">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="cd9eb-147">Getting Started</span></span>](product-get-started.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
