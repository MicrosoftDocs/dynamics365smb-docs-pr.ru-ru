---
title: Поиск контактов из Microsoft Teams
description: Узнайте, как искать клиентов, поставщиков и другие контакты Business Central из Microsoft Teams.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, contacts, search, messaging extensions
ms.date: 04/12/2021
ms.author: jswymer
ms.openlocfilehash: 77108cab69a05165616ad5e1a44f1a3ddc9d4cd9
ms.sourcegitcommit: e13b80d4e5141f414109e660e0918eae561acb36
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "5882499"
---
# <a name="searching-for-customers-vendors-and-other-contacts-from-microsoft-teams"></a><span data-ttu-id="46e61-103">Поиск клиентов, поставщиков и других контактов из Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="46e61-103">Searching for Customers, Vendors, and Other Contacts from Microsoft Teams</span></span>

<span data-ttu-id="46e61-104">[!INCLUDE [online_only](includes/online_only.md)].</span><span class="sxs-lookup"><span data-stu-id="46e61-104">[!INCLUDE [online_only](includes/online_only.md)].</span></span> <span data-ttu-id="46e61-105">Представлено в выпуске волны 1 2021 года.</span><span class="sxs-lookup"><span data-stu-id="46e61-105">Introduced in 2021 release wave 1.</span></span>

<span data-ttu-id="46e61-106">[!INCLUDE [prod_short](includes/prod_short.md)] имеет комплексную систему управления деловыми контактами, которая необходима пользователям с ролями отдела продажами, операционного отдела или других подразделений.</span><span class="sxs-lookup"><span data-stu-id="46e61-106">[!INCLUDE [prod_short](includes/prod_short.md)] has a comprehensive business contact management system that is essential for users in sales, operations, or other departmental roles.</span></span> <span data-ttu-id="46e61-107">Если вы являетесь пользователем с одной из этих ролей, вам часто нужно искать, встречаться или начинать разговор со своими поставщиками, клиентами и другими контактами.</span><span class="sxs-lookup"><span data-stu-id="46e61-107">If you're a user in one of these roles, you'll often need to look up, meet, or start a conversation with your vendors, customers, and other contacts.</span></span> <span data-ttu-id="46e61-108">С приложением [!INCLUDE [prod_short](includes/prod_short.md)] для Teams вы можете выполнять эти задачи прямо из Teams, не переключаясь на [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="46e61-108">With the [!INCLUDE [prod_short](includes/prod_short.md)] app for Teams, you can do these tasks directly from Teams, without having to switch to [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="46e61-109">Из Teams вы можете:</span><span class="sxs-lookup"><span data-stu-id="46e61-109">From within Teams, you can:</span></span>

- <span data-ttu-id="46e61-110">Искать контакты [!INCLUDE [prod_short](includes/prod_short.md)] из командного поля Teams или из области создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="46e61-110">Look up [!INCLUDE [prod_short](includes/prod_short.md)] contacts from the Teams command box or from the message compose area.</span></span> <span data-ttu-id="46e61-111">Контакты могут включать потенциальных клиентов, поставщиков, клиентов или другие деловые отношения.</span><span class="sxs-lookup"><span data-stu-id="46e61-111">Contacts can include prospects, vendors, customers, or other business relationships.</span></span>
- <span data-ttu-id="46e61-112">Делиться контактом как карточкой в разговоре Teams.</span><span class="sxs-lookup"><span data-stu-id="46e61-112">Share a contact as a card in a Teams conversation.</span></span>
- <span data-ttu-id="46e61-113">Просматривать сведения о контактах, историю взаимодействия и другие аналитические сведения, например о невыплаченных платежах или открытых документах.</span><span class="sxs-lookup"><span data-stu-id="46e61-113">View details about contact information, interaction history, and other insights like outstanding payments or open documents.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46e61-114">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="46e61-114">Prerequisites</span></span>

- <span data-ttu-id="46e61-115">У вас есть доступ к Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="46e61-115">You have access to Microsoft Teams.</span></span>
- <span data-ttu-id="46e61-116">Вы установили приложение [!INCLUDE [prod_short](includes/prod_short.md)] в Teams.</span><span class="sxs-lookup"><span data-stu-id="46e61-116">You've installed the [!INCLUDE [prod_short](includes/prod_short.md)] app in Teams.</span></span> <span data-ttu-id="46e61-117">Для получения дополнительной информации см.[ Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="46e61-117">For more information, see [Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>
- <span data-ttu-id="46e61-118">У вас есть учетная запись [!INCLUDE [prod_short](includes/prod_short.md)] с доступом к контактам хотя бы в одной компании.</span><span class="sxs-lookup"><span data-stu-id="46e61-118">You've got a [!INCLUDE [prod_short](includes/prod_short.md)] account with access to contacts in at least one company.</span></span>

> [!NOTE]
> <span data-ttu-id="46e61-119">Независимо от того, выполняете ли вы поиск из командного поля или из окна создания сообщения, вас могут попросить войти в систему или настроить приложение в первый раз.</span><span class="sxs-lookup"><span data-stu-id="46e61-119">Whether you searching from the command box or message compose box, you may be asked to sign in or set up the app the first time.</span></span> <span data-ttu-id="46e61-120">Этот шаг необходим для поиска контактов в нужной компании Business Central.</span><span class="sxs-lookup"><span data-stu-id="46e61-120">This step is necessary to search for contacts in the right Business Central company.</span></span> <span data-ttu-id="46e61-121">Для получения информации о настройке приложения для выбора вашей компании см. раздел [Изменение компании и других параметров в Teams](across-teams-settings.md).</span><span class="sxs-lookup"><span data-stu-id="46e61-121">For information about setting up the app to choose your company, see [Changing Company and Other Settings in Teams](across-teams-settings.md).</span></span>

## <a name="look-up-contacts-from-the-command-box"></a><span data-ttu-id="46e61-122">Поиск контактов из командного поля</span><span class="sxs-lookup"><span data-stu-id="46e61-122">Look up contacts from the command box</span></span>

<span data-ttu-id="46e61-123">Командное поле находится в верхней части каждого экрана в Teams.</span><span class="sxs-lookup"><span data-stu-id="46e61-123">The command box is at the top of every screen in Teams.</span></span> <span data-ttu-id="46e61-124">Оно позволяет вам искать, предпринимать быстрые действия или запускать приложения, такие как приложение [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="46e61-124">It lets you search, take quick actions, or launch apps, like the [!INCLUDE [prod_short](includes/prod_short.md)] app.</span></span> <span data-ttu-id="46e61-125">Поиск из командного поля отлично подходит для быстрого поиска контактов и связанных с ними данных для личного использования.</span><span class="sxs-lookup"><span data-stu-id="46e61-125">Searching from the command box is great for quickly looking up contacts and their related data for your own use.</span></span> <span data-ttu-id="46e61-126">Например, предположим, что вы хотите найти адрес электронной почты поставщика, чтобы назначить встречу в календаре.</span><span class="sxs-lookup"><span data-stu-id="46e61-126">For example, suppose you want to look up an email address of a vendor to set up a calendar meeting.</span></span> <span data-ttu-id="46e61-127">Или, может быть, вы хотите посмотреть историю взаимодействия во время встречи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="46e61-127">Or maybe you want to look up interaction history during a meeting with a customer.</span></span>

1. <span data-ttu-id="46e61-128">В командном поле введите **@Business Central**, затем выберите приложение Business Central из результатов.</span><span class="sxs-lookup"><span data-stu-id="46e61-128">In the command box, type **@Business Central**, then select the Business Central app from the results.</span></span>

    ![Открытие приложения Business Central для поиска контактов из командного поля](media/teams-contacts-command-1.png)

2. <span data-ttu-id="46e61-130">В поле **Business Central** начните вводить текст для поиска, например имя, адрес или номер телефона.</span><span class="sxs-lookup"><span data-stu-id="46e61-130">In the **Business Central** box, start typing search text, like a name, address, or phone number.</span></span>

    <span data-ttu-id="46e61-131">По мере ввода будут появляться совпадающие результаты.</span><span class="sxs-lookup"><span data-stu-id="46e61-131">As you type, matching results will appear.</span></span>

    ![Поиск контактов Business Central из командного поля в Teams](media/teams-contacts-command-2.png)
3. <span data-ttu-id="46e61-133">Выберите контакт из результатов.</span><span class="sxs-lookup"><span data-stu-id="46e61-133">Select a contact from the results.</span></span>

    <span data-ttu-id="46e61-134">Карточка контакта отображается под командным полем.</span><span class="sxs-lookup"><span data-stu-id="46e61-134">The contact card appears beneath the command box.</span></span>

4. <span data-ttu-id="46e61-135">Если вы хотите добавить карточку контакта в разговор, перейдите в правый верхний угол карточки, выберите **... (Дополнительные параметры)** > **Копировать**.</span><span class="sxs-lookup"><span data-stu-id="46e61-135">If you want to add the contact card into a conversation, go to the upper right corner of the card, select **... (More options)** > **Copy**.</span></span> <span data-ttu-id="46e61-136">Затем вставьте копию в поле создания сообщения беседы.</span><span class="sxs-lookup"><span data-stu-id="46e61-136">Then, paste the copy in the message compose box of a conversation.</span></span>  

<span data-ttu-id="46e61-137">Дополнительные общие сведения о командном поле в Teams см. в разделе [Teams — использование командного поля](https://support.microsoft.com/en-us/office/use-the-command-box-13c4e429-7324-4886-b377-5dbed539193b).</span><span class="sxs-lookup"><span data-stu-id="46e61-137">For more general information about the command box in Teams, see [Teams - Use the command box](https://support.microsoft.com/en-us/office/use-the-command-box-13c4e429-7324-4886-b377-5dbed539193b).</span></span>

## <a name="look-up-contacts-from-the-message-compose-box"></a><span data-ttu-id="46e61-138">Поиск контактов из поля создания сообщения</span><span class="sxs-lookup"><span data-stu-id="46e61-138">Look up contacts from the message compose box</span></span>

<span data-ttu-id="46e61-139">Преимущество использования окна создания сообщения заключается в том, что вы можете добавить карточку контакта непосредственно в беседу, чтобы ее могли видеть другие.</span><span class="sxs-lookup"><span data-stu-id="46e61-139">The advantage of using the message compose box is that you can add a contact card directly to a conversation, for others to see.</span></span>

1. <span data-ttu-id="46e61-140">Под полем создания сообщения выберите значок **Business Central**, чтобы запустить приложение.</span><span class="sxs-lookup"><span data-stu-id="46e61-140">Beneath to message compose box, select the **Business Central** icon to launch the app.</span></span>

    <span data-ttu-id="46e61-141">Если вы не видите значок **Business Central**, выберите **... (Расширения для сообщений)**.</span><span class="sxs-lookup"><span data-stu-id="46e61-141">If you don't see the **Business Central** icon, select **... (Messaging extensions)**.</span></span>

    ![Открытие приложения Business Central для поиска контактов из поля сообщения](media/teams-contacts-message-box.png)

2. <span data-ttu-id="46e61-143">В поле **Business Central** начните вводить текст для поиска, например имя, адрес или номер телефона.</span><span class="sxs-lookup"><span data-stu-id="46e61-143">In the **Business Central** box, start typing search text, like a name, address, or phone number.</span></span>

    <span data-ttu-id="46e61-144">По мере ввода будут появляться совпадающие результаты.</span><span class="sxs-lookup"><span data-stu-id="46e61-144">As you type, matching results will appear.</span></span>

    ![Поиск контактов Business Central из поля сообщения](media/teams-contacts-5.png)
3. <span data-ttu-id="46e61-146">Выберите контакт из результатов.</span><span class="sxs-lookup"><span data-stu-id="46e61-146">Select a contact from the results.</span></span>

    <span data-ttu-id="46e61-147">Карточка контакта появится в поле создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="46e61-147">The contact card appears in the message compose box.</span></span>

    > [!NOTE]
    > <span data-ttu-id="46e61-148">Карточка контакта не сразу отправляется в беседу, чтобы ее могли увидеть другие.</span><span class="sxs-lookup"><span data-stu-id="46e61-148">The contact card isn't sent to the conversation right away for others to see.</span></span> <span data-ttu-id="46e61-149">У вас есть возможность просмотреть содержимое карточки и добавить текст до или после нее по своему усмотрению.</span><span class="sxs-lookup"><span data-stu-id="46e61-149">You have the opportunity to review the contents of the card, and add text before or after it as you like.</span></span> <span data-ttu-id="46e61-150">Затем отправьте свое сообщение в чат, когда будете готовы.</span><span class="sxs-lookup"><span data-stu-id="46e61-150">Then, send your message to the chat when ready.</span></span>

### <a name="heres-another-way"></a><span data-ttu-id="46e61-151">Вот другой способ</span><span class="sxs-lookup"><span data-stu-id="46e61-151">Here's another way</span></span>

1. <span data-ttu-id="46e61-152">Вместо использования значка **Business Central**, введите **@ Business Central** прямо в поле создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="46e61-152">Instead of using the **Business Central** icon, type **@Business Central** directly in the message compose box.</span></span>
2. <span data-ttu-id="46e61-153">Введите в поле условия поиска.</span><span class="sxs-lookup"><span data-stu-id="46e61-153">Enter your search terms in the box.</span></span>
3. <span data-ttu-id="46e61-154">Используйте клавиши со стрелками вверх и вниз на клавиатуре, чтобы выбрать контакт, затем нажмите клавишу "Ввод", чтобы выбрать его.</span><span class="sxs-lookup"><span data-stu-id="46e61-154">Use the up and down arrow keys on the keyboard to choose a contact, then press Enter to select it.</span></span>

## <a name="viewing-contact-card-details"></a><span data-ttu-id="46e61-155">Просмотр сведений в карточке контакта</span><span class="sxs-lookup"><span data-stu-id="46e61-155">Viewing contact card details</span></span>

<span data-ttu-id="46e61-156">Карточка контакта в Teams дает вам быстрый обзор клиента, поставщика или контакта.</span><span class="sxs-lookup"><span data-stu-id="46e61-156">The contact card in Teams gives you a quick overview of the customer, vendor, or contact.</span></span> <span data-ttu-id="46e61-157">Карточка интерактивная &mdash; это означает, что вы можете просмотреть дополнительную информацию или даже изменить контакт с помощью кнопки **Сведения** или **В новом окне**.</span><span class="sxs-lookup"><span data-stu-id="46e61-157">The card is interactive&mdash;meaning you can view more information or even modify a contact by using the **Details** or **Pop-out** buttons.</span></span>

<span data-ttu-id="46e61-158">Кнопка **Сведения** открывает окно в Teams, в котором отображается дополнительная информация о контакте, но не столько, сколько вы бы увидели в [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="46e61-158">The **Details** button opens a window within Teams that displays more information about the contact, but not as much as you'd see in [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="46e61-159">Чтобы увидеть всю информацию о контакте в [!INCLUDE [prod_short](includes/prod_short.md)], выберите **В новом окне**.</span><span class="sxs-lookup"><span data-stu-id="46e61-159">To see all the information about a contact in [!INCLUDE [prod_short](includes/prod_short.md)], select **Pop-out**.</span></span>

<span data-ttu-id="46e61-160">Карточка контакта работает так же, как карточки для записей, таких как товары, клиенты или заказы на продажу.</span><span class="sxs-lookup"><span data-stu-id="46e61-160">The contact card works just like cards for records, like items, customers, or sales orders.</span></span> <span data-ttu-id="46e61-161">Дополнительные сведения о карточках см. в разделе [Просмотр сведений карточки](across-working-with-teams.md#view-card-details).</span><span class="sxs-lookup"><span data-stu-id="46e61-161">For more information about cards, see [View card details](across-working-with-teams.md#view-card-details).</span></span>

> [!NOTE]
> <span data-ttu-id="46e61-162">Все участники беседы Teams смогут просматривать карточки для контакта Business Central, которые вы отправляете в беседу.</span><span class="sxs-lookup"><span data-stu-id="46e61-162">All participants in a Teams conversation will be able to view cards for Business Central contact that you submit to a conversation.</span></span> <span data-ttu-id="46e61-163">Но чтобы просмотреть более подробную информацию о записях, используя кнопки **Подробнее** или **Открыть на новой вкладке**, им потребуется доступ [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="46e61-163">But to view more details about records, by using the **Details** or **Pop out** buttons on a card, they'll need access to [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="46e61-164">Дополнительные сведения см. в разделе [Управление интеграцией Microsoft Teams](admin-teams-integration.md#minimum-requirements-1).</span><span class="sxs-lookup"><span data-stu-id="46e61-164">For more information, see [Managing Microsoft Teams Integration](admin-teams-integration.md#minimum-requirements-1).</span></span>

## <a name="see-also"></a><span data-ttu-id="46e61-165">См. также</span><span class="sxs-lookup"><span data-stu-id="46e61-165">See Also</span></span>

[<span data-ttu-id="46e61-166">Обзор интеграции Business Central и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="46e61-166">Business Central and Microsoft Teams Integration Overview</span></span>](across-teams-overview.md)  
<span data-ttu-id="46e61-167">[Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="46e61-167">[Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>  
[<span data-ttu-id="46e61-168">Вопросы и ответы по Teams</span><span class="sxs-lookup"><span data-stu-id="46e61-168">Teams FAQ</span></span>](teams-faq.md)  
[<span data-ttu-id="46e61-169">Устранение неполадок Teams</span><span class="sxs-lookup"><span data-stu-id="46e61-169">Troubleshooting Teams</span></span>](admin-teams-troubleshooting.md)  
[<span data-ttu-id="46e61-170">Разработка для интеграции Teams</span><span class="sxs-lookup"><span data-stu-id="46e61-170">Developing for Teams Integration</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]