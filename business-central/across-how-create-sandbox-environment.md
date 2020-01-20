---
title: Создание среды "песочницы" | Документация Майкрософт
description: Создайте среду для исследования, обучения, демонстрации, разработки и тестирования.
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sandbox, demo, develop
ms.date: 12/10/2019
ms.author: solsen
ms.openlocfilehash: 7d189ab6fa5aff518b643c797b7600570fcad43e
ms.sourcegitcommit: 3d128a00358668b3fdd105ebf4604ca4e2b6743c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2019
ms.locfileid: "2910640"
---
# <a name="creating-a-sandbox-environment-in-include-prodshortincludesprodshortmd"></a><span data-ttu-id="1e983-103">Создание среды "песочницы" в [!INCLUDE [prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="1e983-103">Creating a Sandbox Environment in [!INCLUDE [prodshort](includes/prodshort.md)]</span></span>

<span data-ttu-id="1e983-104">В [!INCLUDE [prodshort](includes/prodshort.md)] вы можете легко создать безопасную среду, в которой тестировать, обучать или устранять неполадки, не нарушая рабочие процессы вашей компании или бизнес-данные.</span><span class="sxs-lookup"><span data-stu-id="1e983-104">With [!INCLUDE [prodshort](includes/prodshort.md)], you can easily create a safe environment where you can test, train, or troubleshoot without disturbing your company's work processes or business data.</span></span> <span data-ttu-id="1e983-105">Такая непроизводственная среда называется *песочницей*.</span><span class="sxs-lookup"><span data-stu-id="1e983-105">Such a non-production environment is called a *sandbox*.</span></span> <span data-ttu-id="1e983-106">В среде песочницы, изолированной от производственной среды, можно безопасно исследовать, обучать, демонстрировать, разрабатывать и тестировать сервисы без риска повлиять на данные или настройки производственной среды.</span><span class="sxs-lookup"><span data-stu-id="1e983-106">Isolated from production, a sandbox environment is the place to safely explore, learn, demo, develop, and test the service without the risk of affecting the data and settings of your production environment.</span></span>  

<span data-ttu-id="1e983-107">Ваш администратор может создавать среду "песочницы" в [центре администрирования](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments?toc=/dynamics365/business-central/toc.json), но если вы хотите быстро протестировать что-нибудь, вы можете создать среду "песочницы" из [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="1e983-107">Your administrator can create sandbox environments in the [administration center](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments?toc=/dynamics365/business-central/toc.json), but if you want to quickly test something, you can create a sandbox environment from inside [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>  

> [!NOTE]
> <span data-ttu-id="1e983-108">Формально среды "песочницы" сильно отличаются от производственных сред, даже если ваш администратор создает "песочницу", включающую производственные данные.</span><span class="sxs-lookup"><span data-stu-id="1e983-108">Technically, sandbox environments are very different from production environments, even if your administrator creates a sandbox that includes production data.</span></span> <span data-ttu-id="1e983-109">Вы не можете использовать песочницу для сравнительного и не можете, например, запросить экспорт базы данных.</span><span class="sxs-lookup"><span data-stu-id="1e983-109">You cannot use a sandbox for benchmarking, and you cannot request a database export, for example.</span></span> <span data-ttu-id="1e983-110">Если вы хотите создать "песочницу" для сравнительного тестирования, ваш администратор может создать выделенную производственную среду в центре администрирования.</span><span class="sxs-lookup"><span data-stu-id="1e983-110">If you want to create a sandbox for benchmarking, your administrator can create a dedicated production environment in the administration center.</span></span> <span data-ttu-id="1e983-111">Дополнительные сведения см. в разделе [Типы сред](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments#types-of-environments).</span><span class="sxs-lookup"><span data-stu-id="1e983-111">For more information, see [Types of environments](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments#types-of-environments).</span></span>

## <a name="to-create-a-sandbox-environment-in-your-include-prodshortincludesprodshortmd"></a><span data-ttu-id="1e983-112">Создание среды "песочницы" в [!INCLUDE [prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="1e983-112">To create a sandbox environment in your [!INCLUDE [prodshort](includes/prodshort.md)]</span></span>

1. <span data-ttu-id="1e983-113">Выполните вход в производственный экземпляр [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1e983-113">Sign in to your production instance of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

2. <span data-ttu-id="1e983-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Среда "песочницы"**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1e983-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sandbox Environment**, and then choose the related link.</span></span>
    <!-- ![Sandbox Environment Setup](./media/across-sandbox/sandbox-environment-setup.png) -->
3. <span data-ttu-id="1e983-115">Нажмите кнопку **Создать**.</span><span class="sxs-lookup"><span data-stu-id="1e983-115">Choose the **Create** button.</span></span>  

    <span data-ttu-id="1e983-116">Откроется еще одна вкладка с [!INCLUDE[d365fin](includes/d365fin_md.md)], на которой вы можете завершить настройку среды песочницы.</span><span class="sxs-lookup"><span data-stu-id="1e983-116">Another tab with [!INCLUDE[d365fin](includes/d365fin_md.md)] opens where you can finish the setup of your sandbox environment.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="1e983-117">Если в браузере включена блокировка всплывающих окон, измените ее, чтобы разрешить URL-адреса с адреса \*.businesscentral.dynamics.com.</span><span class="sxs-lookup"><span data-stu-id="1e983-117">If you have pop-up blocker enabled in your browser, change it to allow URLs from the \*.businesscentral.dynamics.com address.</span></span>

<span data-ttu-id="1e983-118">Когда среда песочницы будет готова, вы будете перенаправлены в приветственный мастер среды песочницы.</span><span class="sxs-lookup"><span data-stu-id="1e983-118">When the sandbox environment is ready, you will be redirected to sandbox environment's Welcome wizard.</span></span>
<!-- ![Sandbox Welcome Wizard](./media/across-sandbox/sandbox-wizard.png) -->

<span data-ttu-id="1e983-119">Нажмите кнопку **Подробнее**, чтобы прочитать о сценариях для разработчиков, которые вы можете попробовать в среде песочницы, или кнопку **Закрыть**, чтобы перейти к ролевому центру вашего экземпляр песочницы [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1e983-119">You can choose the **Learn more** button to read about developer scenarios that you can try in a sandbox environment or choose the **Close** button to continue to the Role Center of your [!INCLUDE[d365fin](includes/d365fin_md.md)] sandbox instance.</span></span>

<span data-ttu-id="1e983-120">В верхней части ролевого центра появится уведомление о том, что это среда песочницы.</span><span class="sxs-lookup"><span data-stu-id="1e983-120">At the top of the Role Center, a notification appears to inform you that this is a sandbox environment.</span></span> <span data-ttu-id="1e983-121">Тип среды также отображается в строке заголовка клиента.</span><span class="sxs-lookup"><span data-stu-id="1e983-121">You can also see the type of the environment in the title bar of the client.</span></span>
    <!-- ![Sandbox RoleCenter Notification](./media/across-sandbox/sandbox-rolecenter-notification.png) -->

> [!NOTE]
> <span data-ttu-id="1e983-122">Созданная таким образом среда песочницы содержит только демонстрационные данные по умолчанию для компании CRONUS.</span><span class="sxs-lookup"><span data-stu-id="1e983-122">A sandbox environment created in this way only contains the default demonstration data for the CRONUS company.</span></span> <span data-ttu-id="1e983-123">Никакие данные не копируются и не переносятся каким-либо другим образом из производственной среды.</span><span class="sxs-lookup"><span data-stu-id="1e983-123">No data is copied or otherwise transferred from the production environment.</span></span><br /><br />
> <span data-ttu-id="1e983-124">Вы также можете создать среду песочницы, содержащую производственные данные.</span><span class="sxs-lookup"><span data-stu-id="1e983-124">You can also create a sandbox environment containing the production data.</span></span> <span data-ttu-id="1e983-125">Вы должны сделать это через центр администрирования.</span><span class="sxs-lookup"><span data-stu-id="1e983-125">You must do this through the administration center.</span></span> <span data-ttu-id="1e983-126">Дополнительные сведения см. в разделе [Управление средами](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments) в справке для разработчиков и ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="1e983-126">For more information, see [Managing Environments](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments) in the Developer and IT-Pro help.</span></span>

<span data-ttu-id="1e983-127">В любой момент можно вернуться на страницу **Среда "песочницы"** и сбросить среду "песочницы".</span><span class="sxs-lookup"><span data-stu-id="1e983-127">At any time, you can return to the **Sandbox Environment** page, and reset the sandbox environment.</span></span>

> [!NOTE]  
> <span data-ttu-id="1e983-128">При сбросе среды песочницы она полностью удаляется, а затем создается заново с демонстрационными данными по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1e983-128">Resetting the sandbox environment will remove it completely, and then create it again with the default demonstration data.</span></span>  

<!--To switch between your production and sandbox environments, you can use the Business Central app launcher.
    ![Sandbox Dynamics365 Menu](./media/across-sandbox/sandbox-dynamics365-menu.png) -->

<span data-ttu-id="1e983-129">Администратор может ограничить или даже блокировать доступ некоторых пользователей к среде "песочницы".</span><span class="sxs-lookup"><span data-stu-id="1e983-129">An administrator can limit or even block access for some users to the sandbox environment.</span></span> <span data-ttu-id="1e983-130">Это можно сделать с помощью стандартных функций безопасности для продукта, таких как карта пользователя, группы пользователей и наборы разрешений.</span><span class="sxs-lookup"><span data-stu-id="1e983-130">This can be done by using the standard security features of the product, such as the User card, user groups, and permission sets.</span></span> <span data-ttu-id="1e983-131">Дополнительные сведения см. в разделе [Назначение разрешений пользователям и группам](ui-define-granular-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="1e983-131">For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span></span>  

<!-- ![Sandbox Permission Sets](./media/across-sandbox/sandbox-permission-sets.png) -->

## <a name="advanced-functionality-in-the-sandbox-environment"></a><span data-ttu-id="1e983-132">Расширенная функциональная возможность в среде песочницы</span><span class="sxs-lookup"><span data-stu-id="1e983-132">Advanced Functionality in the Sandbox Environment</span></span>

<span data-ttu-id="1e983-133">Среда "песочницы" не менее полезна, потому что она включает в себя несколько удобных функций.</span><span class="sxs-lookup"><span data-stu-id="1e983-133">The sandbox environment is not least useful because it includes a couple of handy features.</span></span>

### <a name="designer"></a><span data-ttu-id="1e983-134">Конструктор</span><span class="sxs-lookup"><span data-stu-id="1e983-134">Designer</span></span>

<span data-ttu-id="1e983-135">В среде "песочницы" включен **Конструктор**.</span><span class="sxs-lookup"><span data-stu-id="1e983-135">In a sandbox environment, you will find the **Designer** enabled.</span></span> <span data-ttu-id="1e983-136">Вы можете активировать конструктор, выбрав значок конструктора ![Конструктор](./media/across-sandbox/sandbox-inclient-design-icon.png) на странице или выбрав дизайн пункт меню **Конструктор** в меню настроек ![Настройки](media/ui-experience/settings_icon_small.png).</span><span class="sxs-lookup"><span data-stu-id="1e983-136">You can activate Designer by selecting the design icon ![Designer](./media/across-sandbox/sandbox-inclient-design-icon.png) on a page, or by choosing the **Design** menu item in the ![Settings](media/ui-experience/settings_icon_small.png) Settings menu.</span></span>

<!-- ![In-client Designer](./media/across-sandbox/sandbox-inclient-designer.png) -->

### <a name="to-enable-the-advanced-user-experience"></a><span data-ttu-id="1e983-137">Включение расширенных возможностей пользователя</span><span class="sxs-lookup"><span data-stu-id="1e983-137">To enable the advanced user experience</span></span>
<span data-ttu-id="1e983-138">Можно включить и попробовать полные функциональные возможности стандартной версии [!INCLUDE[d365fin](includes/d365fin_md.md)] в среде арендатора песочницы, задав поле **Опыт** на странице **Информация о компании**.</span><span class="sxs-lookup"><span data-stu-id="1e983-138">It is possible to enable and try the full functionality of the standard version of [!INCLUDE[d365fin](includes/d365fin_md.md)] in a sandbox tenant by setting the **Experience** field on the **Company Information** page.</span></span>

<!-- ![Sandbox Environment Advanced](./media/across-sandbox/sandbox-advanced.png) -->

<!-- ![Sandbox Production](./media/across-sandbox/sandbox-production.png) -->

<span data-ttu-id="1e983-139">После того как вы включили вариант настройки *Premium*, вы получаете доступ ко всем стандартным профилям (ролям) и ролевым центрам стандартной версии.</span><span class="sxs-lookup"><span data-stu-id="1e983-139">After you have enabled the *Premium* user experience, you get access to all the standard profiles (roles) and Role Centers in the standard version.</span></span> <span data-ttu-id="1e983-140">Можно также создать полностью настроенную пробную организацию, включая демонстрационные данные и доступ к расширенным возможностям продукта.</span><span class="sxs-lookup"><span data-stu-id="1e983-140">You can also create an evaluation company that is fully set up, including demonstration data and access to the advanced areas of the product.</span></span> <span data-ttu-id="1e983-141">Кроме того, вы можете связаться с партнером по перепродаже для демонстрации возможностей.</span><span class="sxs-lookup"><span data-stu-id="1e983-141">Alternatively, contact a reselling partner for a demonstration of the capabilities.</span></span> <span data-ttu-id="1e983-142">Для получения дополнительной информации см. раздел [Как найти партнера по перепродаже?](across-faq.md#findpartner),</span><span class="sxs-lookup"><span data-stu-id="1e983-142">For more information, see [How do I find a reselling partner?](across-faq.md#findpartner).</span></span>  

<!-- ![Sandbox New Company](./media/across-sandbox/sandbox-newcompany.png) -->

## <a name="see-also"></a><span data-ttu-id="1e983-143">См. также</span><span class="sxs-lookup"><span data-stu-id="1e983-143">See Also</span></span>

<span data-ttu-id="1e983-144">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1e983-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="1e983-145">[Пробные версии и подписки [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](across-preview.md)</span><span class="sxs-lookup"><span data-stu-id="1e983-145">[[!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] Trials and Subscriptions](across-preview.md)</span></span>  
[<span data-ttu-id="1e983-146">Управление средами в центре администрирования Business Central</span><span class="sxs-lookup"><span data-stu-id="1e983-146">Managing Environments in the Business Central administration center</span></span>](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments)  
