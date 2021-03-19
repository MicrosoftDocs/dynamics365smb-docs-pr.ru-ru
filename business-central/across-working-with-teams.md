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
ms.date: 01/20/2021
ms.author: jswymer
ms.openlocfilehash: cbb505865e061bfa8017699a2127206bb25f91b4
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5381985"
---
# <a name="working-with-business-central-data-in-microsoft-teams"></a><span data-ttu-id="d907a-103">Работа с данными Business Central в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d907a-103">Working with Business Central Data in Microsoft Teams</span></span>

[!INCLUDE [online_only](includes/online_only.md)]

<span data-ttu-id="d907a-104">[!INCLUDE [prod_short](includes/prod_short.md)] предлагает приложение, которое соединяет Microsoft Teams с вашими бизнес-данным в [!INCLUDE [prod_short](includes/prod_short.md)], чтобы вы могли быстро обмениваться данными между участниками команды и быстрее отвечать на запросы.</span><span class="sxs-lookup"><span data-stu-id="d907a-104">[!INCLUDE [prod_short](includes/prod_short.md)] offers an app that connects Microsoft Teams to your business data in [!INCLUDE [prod_short](includes/prod_short.md)], so you can quickly share details across team members and respond faster to inquiries.</span></span> <span data-ttu-id="d907a-105">В этой статье вы узнаете, как использовать приложение для обмена данными [!INCLUDE [prod_short](includes/prod_short.md)] с коллегами в беседе в Teams.</span><span class="sxs-lookup"><span data-stu-id="d907a-105">In this article, you'll learn how to use the app to share [!INCLUDE [prod_short](includes/prod_short.md)] data with coworkers in a Teams conversation.</span></span>

## <a name="overview"></a><span data-ttu-id="d907a-106">Обзор</span><span class="sxs-lookup"><span data-stu-id="d907a-106">Overview</span></span>

<span data-ttu-id="d907a-107">Приложение позволяет [!INCLUDE [prod_short](includes/prod_short.md)]:</span><span class="sxs-lookup"><span data-stu-id="d907a-107">The [!INCLUDE [prod_short](includes/prod_short.md)] app lets you:</span></span>

- <span data-ttu-id="d907a-108">Скопируйте ссылку на любую запись Business Central и вставьте ее в беседу Teams, чтобы поделиться ею с коллегами.</span><span class="sxs-lookup"><span data-stu-id="d907a-108">Copy a link to any Business Central record and paste it into a Teams conversation to share with your coworkers.</span></span> <span data-ttu-id="d907a-109">Приложение затем развернет ссылку в компактную интерактивную карточку, отображающую информацию о записи.</span><span class="sxs-lookup"><span data-stu-id="d907a-109">The app will then expand the link into a compact, interactive card that displays information about the record.</span></span>
- <span data-ttu-id="d907a-110">После разговора вы и ваши коллеги можете просматривать дополнительные сведения о записи, редактировать данные и принимать меры &mdash; не выходя из Teams.</span><span class="sxs-lookup"><span data-stu-id="d907a-110">Once in the conversation, you and coworkers can view more details about the record, edit data, and take action&mdash;without leaving Teams.</span></span>

<span data-ttu-id="d907a-111">[![Интеграция Teams с Business Central](media/teams-intro-v3.png)](media/teams-intro-v3.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d907a-111">[![Teams integration with Business Central](media/teams-intro-v3.png)](media/teams-intro-v3.png#lightbox)</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d907a-112">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="d907a-112">Prerequisites</span></span>

- <span data-ttu-id="d907a-113">У вас есть доступ к Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d907a-113">You have access to Microsoft Teams.</span></span>
- <span data-ttu-id="d907a-114">Вы установили приложение [!INCLUDE [prod_short](includes/prod_short.md)] в Teams.</span><span class="sxs-lookup"><span data-stu-id="d907a-114">You've installed the [!INCLUDE [prod_short](includes/prod_short.md)] app in Teams.</span></span> <span data-ttu-id="d907a-115">Для получения дополнительной информации см.[ Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="d907a-115">For more information, see [Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>

> [!NOTE]
> <span data-ttu-id="d907a-116">Все участники беседы Teams смогут просматривать карточки для записей Business Central, которые вы отправляете в беседу.</span><span class="sxs-lookup"><span data-stu-id="d907a-116">All participants in a Teams conversation will be able to view cards for Business Central records that you submit to the conversation.</span></span> <span data-ttu-id="d907a-117">Но чтобы просмотреть более подробную информацию о записях, используя кнопки **Подробнее** или **Открыть на новой вкладке**, им потребуется доступ [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="d907a-117">But to view more details about records, by using the **Details** or **Pop out** buttons on a card, they'll need access to [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="d907a-118">Дополнительные сведения см. в разделе [Управление интеграцией Microsoft Teams](admin-teams-integration.md#minimum-requirements-1).</span><span class="sxs-lookup"><span data-stu-id="d907a-118">For more information, see [Managing Microsoft Teams Integration](admin-teams-integration.md#minimum-requirements-1).</span></span>

## <a name="include-a-business-central-card-in-a-teams-conversation"></a><span data-ttu-id="d907a-119">Включите карточку Business Central в беседу в Teams</span><span class="sxs-lookup"><span data-stu-id="d907a-119">Include a Business Central card in a Teams conversation</span></span>

1. <span data-ttu-id="d907a-120">Водите в [!INCLUDE [prod_short](includes/prod_short.md)], используя ваш браузер.</span><span class="sxs-lookup"><span data-stu-id="d907a-120">Sign in to [!INCLUDE [prod_short](includes/prod_short.md)] using your browser.</span></span>
2. <span data-ttu-id="d907a-121">Откройте запись, которое требуется поделиться.</span><span class="sxs-lookup"><span data-stu-id="d907a-121">Open the record that you want to share.</span></span>

    <span data-ttu-id="d907a-122">Приложение предназначено для отображения страниц типа карточек из [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="d907a-122">The app is designed to display card type pages from [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="d907a-123">Итак, откройте страницу, которая отображает одну запись, например товар, клиента или заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="d907a-123">So open a page that displays a single record, like an item, customer, or sales order.</span></span> <span data-ttu-id="d907a-124">Вы не можете использовать его для центров ролей или страниц, отображающих несколько записей в списке.</span><span class="sxs-lookup"><span data-stu-id="d907a-124">You can't use it for role centers or pages that display several records in a list.</span></span>

3. <span data-ttu-id="d907a-125">Скопируйте весь URL-адрес из адресной строки браузера.</span><span class="sxs-lookup"><span data-stu-id="d907a-125">Copy the entire URL from the browser's address bar.</span></span>

   ![Скопируйте URL-адрес Business Central из браузера](media/teams-url-v2.png)
4. <span data-ttu-id="d907a-127">Перейдите в Teams и начните разговор, который может быть чатом с человеком, группой людей или групповым каналом.</span><span class="sxs-lookup"><span data-stu-id="d907a-127">Go to Teams and start a conversation, which can be chat with a person, group of persons, or a team channel.</span></span>

    <!--Teams imposes a few limitations here eg. you cannot unfurl a link during a Voice/Video call :/ We should probably only mention this in a Troubleshooting section (and i hope it will also be fixed soon)-->
5. <span data-ttu-id="d907a-128">Вставьте URL-адрес в поле сообщение, в которое вы составляете сообщение.</span><span class="sxs-lookup"><span data-stu-id="d907a-128">Paste the URL in the message box where you compose a message.</span></span>

   ![Вставьте URL-адрес Business Central в Teams](media/teams-paste-url-v2.png)
6. <span data-ttu-id="d907a-130">Когда вы впервые вставите ссылку в беседу, вам будет предложено войти в [!INCLUDE [prod_short](includes/prod_short.md)] и дать согласие на получение данных приложением.</span><span class="sxs-lookup"><span data-stu-id="d907a-130">The first time you paste a link into a conversation, you'll be asked to sign in to [!INCLUDE [prod_short](includes/prod_short.md)] and give consent for the app to retrieve data.</span></span> <span data-ttu-id="d907a-131">Просто следуйте инструкциям на экране.</span><span class="sxs-lookup"><span data-stu-id="d907a-131">Just follow the on-screen instructions.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d907a-132">Вам нужно выполнить этот шаг только один раз.</span><span class="sxs-lookup"><span data-stu-id="d907a-132">You'll only have to do this step once.</span></span>

7. <span data-ttu-id="d907a-133">Подождите, пока в окне сообщения появится карточка.</span><span class="sxs-lookup"><span data-stu-id="d907a-133">Wait a moment while a card is generated in the message box.</span></span>

8. <span data-ttu-id="d907a-134">Когда карточка появится, внимательно проверьте содержимое карточки на наличие конфиденциальной информации перед отправкой сообщения.</span><span class="sxs-lookup"><span data-stu-id="d907a-134">When the card appears, review the contents of the card carefully for any sensitive information before sending the message.</span></span> <span data-ttu-id="d907a-135">Этот шаг важен, потому что как только вы отправите сообщение, все участники беседы смогут увидеть карточку.</span><span class="sxs-lookup"><span data-stu-id="d907a-135">This step is important because once you send the message, everyone in the conversation can see the card.</span></span>

9. <span data-ttu-id="d907a-136">Если карточка выглядит хорошо, выберите **Отправить**, чтобы отправить ее в беседу.</span><span class="sxs-lookup"><span data-stu-id="d907a-136">If the card looks good, select **Send** to submit it to the conversation.</span></span>

    > [!TIP]
    > <span data-ttu-id="d907a-137">После появления карточки и до того, как вы выберете **Отправить**, вы можете удалить вставленный URL-адрес, если хотите.</span><span class="sxs-lookup"><span data-stu-id="d907a-137">After the card appears, and before you select **Send**, you can delete the pasted URL if you like.</span></span>

10. <span data-ttu-id="d907a-138">Чтобы просмотреть дополнительные сведения или внести изменения в запись, отображаемую на карточке, выберите **Подробнее**.</span><span class="sxs-lookup"><span data-stu-id="d907a-138">To view more details or make changes to the record shown in the card, select **Details**.</span></span> <span data-ttu-id="d907a-139">Дополнительные сведения см. в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="d907a-139">For more information, see the next section.</span></span>

## <a name="view-card-details"></a><span data-ttu-id="d907a-140">Просмотр сведений карточки</span><span class="sxs-lookup"><span data-stu-id="d907a-140">View card details</span></span>

<span data-ttu-id="d907a-141">После отправки карточки в беседу все участники с [надлежащими разрешениями](admin-teams-integration.md#permissions) могут выбрать **Детали**, чтобы открыть окно, в котором отображается дополнительная информация о записи &mdash; и, возможно, внести изменения в запись.</span><span class="sxs-lookup"><span data-stu-id="d907a-141">Once a card's been sent to a conversation, all participants with the [proper permissions](admin-teams-integration.md#permissions) can select **Details** to open a window that displays more information about the record&mdash;and possibly make changes to the record.</span></span> <span data-ttu-id="d907a-142">Неважно, отправляете ли вы карточку или получаете ее.</span><span class="sxs-lookup"><span data-stu-id="d907a-142">It doesn't matter if you're the one sending the card or the one receiving the card.</span></span> <span data-ttu-id="d907a-143">Функция **Детали** особенно полезна для получателей, поскольку она быстро предоставляет им краткую и целевую информацию о записи, в отличие от необходимости сканировать всю запись.</span><span class="sxs-lookup"><span data-stu-id="d907a-143">The **Details** feature is especially useful to recipients, because it quickly provides them with concise, targeted information about the record, as opposed to having to scan the full record.</span></span>

<span data-ttu-id="d907a-144">Окно сведений похоже на то, что вы бы видели в записи [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="d907a-144">The details window is similar to what you'd see in [!INCLUDE [prod_short](includes/prod_short.md)] the record.</span></span> <span data-ttu-id="d907a-145">Но для Teams версия немного урезана.</span><span class="sxs-lookup"><span data-stu-id="d907a-145">But it's slightly trimmed for Teams.</span></span> <span data-ttu-id="d907a-146">Когда вы закончите просмотр и внесите изменения, закройте окно, чтобы вернуться к беседе Teams.</span><span class="sxs-lookup"><span data-stu-id="d907a-146">When you're finished viewing and making changes, close the window to return to the Teams conversation.</span></span>

<span data-ttu-id="d907a-147">При работе с данными карточки следует помнить о нескольких вещах:</span><span class="sxs-lookup"><span data-stu-id="d907a-147">Here are a couple things to keep in mind when working with the card details:</span></span>

- <span data-ttu-id="d907a-148">Чтобы открыть сведения о карточке, пользователи должны иметь разрешение на странице и ее данных в [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="d907a-148">To open the card details, users must have permission on the page and its data in [!INCLUDE [prod_short](includes/prod_short.md)].</span></span>
- <span data-ttu-id="d907a-149">Карточки в чатах Teams не обновляются автоматически при внесении изменений.</span><span class="sxs-lookup"><span data-stu-id="d907a-149">Cards in Teams chats aren't automatically updated to changes.</span></span> <span data-ttu-id="d907a-150">Любые изменения, которые вы сохраняете в записи в окне сведений, сохраняются в [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="d907a-150">Any changes you save to a record in the details window are saved in [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="d907a-151">Но карточка в Teams не будет отображать изменения в преобразовании, пока вы снова не вставите ссылку.</span><span class="sxs-lookup"><span data-stu-id="d907a-151">But the card in Teams won't show the changes in the conversion, until you paste the link again.</span></span>

<span data-ttu-id="d907a-152">Подробнее о работе с карточками и сведениях о карточках см. в разделе [Вопросы и ответы по Teams](teams-faq.md).</span><span class="sxs-lookup"><span data-stu-id="d907a-152">To learn more about working with cards and card details, see [Teams FAQ](teams-faq.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="d907a-153">См. также</span><span class="sxs-lookup"><span data-stu-id="d907a-153">See Also</span></span>

[<span data-ttu-id="d907a-154">Обзор интеграции Business Central и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d907a-154">Business Central and Microsoft Teams Integration Overview</span></span>](across-teams-overview.md)  
<span data-ttu-id="d907a-155">[Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="d907a-155">[Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>  
[<span data-ttu-id="d907a-156">Вопросы и ответы по Teams</span><span class="sxs-lookup"><span data-stu-id="d907a-156">Teams FAQ</span></span>](teams-faq.md)  
[<span data-ttu-id="d907a-157">Устранение неполадок Teams</span><span class="sxs-lookup"><span data-stu-id="d907a-157">Troubleshooting Teams</span></span>](admin-teams-troubleshooting.md)  
[<span data-ttu-id="d907a-158">Разработка для интеграции Teams</span><span class="sxs-lookup"><span data-stu-id="d907a-158">Developing for Teams Integration</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]