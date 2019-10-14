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
ms.date: 10/01/2019
ms.author: solsen
ms.openlocfilehash: d945a6b851c20479a4c8c83f38b8fc8ccdfd6765
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2300429"
---
# <a name="creating-a-sandbox-environment"></a><span data-ttu-id="6d54c-103">Создание среды "песочницы"</span><span class="sxs-lookup"><span data-stu-id="6d54c-103">Creating a Sandbox Environment</span></span>
<span data-ttu-id="6d54c-104">Среда песочницы (функция для предварительного ознакомления) представляет собой непроизводственный экземпляр [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6d54c-104">A sandbox environment (Preview) is a non-production instance of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="6d54c-105">В среде песочницы, изолированной от производственной среды, можно безопасно исследовать, обучать, демонстрировать, разрабатывать и тестировать сервисы без риска повлиять на данные или настройки производственной среды.</span><span class="sxs-lookup"><span data-stu-id="6d54c-105">Isolated from production, a sandbox environment is the place to safely explore, learn, demo, develop, and test the service without the risk of affecting the data and settings of your production environment.</span></span>

## <a name="to-create-a-sandbox-environment"></a><span data-ttu-id="6d54c-106">Создание среды "песочницы"</span><span class="sxs-lookup"><span data-stu-id="6d54c-106">To create a sandbox environment</span></span>
<span data-ttu-id="6d54c-107">Чтобы можно было создать среду песочницы, необходима подписка на [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6d54c-107">You must have a subscription to [!INCLUDE[d365fin](includes/d365fin_md.md)] to be able to create a sandbox environment.</span></span> <span data-ttu-id="6d54c-108">В каждой подписке может быть только одна среда песочницы.</span><span class="sxs-lookup"><span data-stu-id="6d54c-108">There can only be one sandbox environment per subscription.</span></span>

1. <span data-ttu-id="6d54c-109">Выполните вход в производственный экземпляр службы [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6d54c-109">Sign in to your production instance of the [!INCLUDE[d365fin](includes/d365fin_md.md)] service.</span></span>

2. <span data-ttu-id="6d54c-110">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Среда "песочницы"**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="6d54c-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sandbox Environment**, and then choose the related link.</span></span>
<!-- ![Sandbox Environment Setup](./media/across-sandbox/sandbox-environment-setup.png) -->
3. <span data-ttu-id="6d54c-111">Нажмите кнопку **Создать**.</span><span class="sxs-lookup"><span data-stu-id="6d54c-111">Choose the **Create** button.</span></span>  

    <span data-ttu-id="6d54c-112">Откроется еще одна вкладка с [!INCLUDE[d365fin](includes/d365fin_md.md)], на которой вы можете завершить настройку среды песочницы.</span><span class="sxs-lookup"><span data-stu-id="6d54c-112">Another tab with [!INCLUDE[d365fin](includes/d365fin_md.md)] opens where you can finish the setup of your sandbox environment.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="6d54c-113">Если в браузере включена блокировка всплывающих окон, измените ее, чтобы разрешить URL-адреса с адреса \*.businesscentral.dynamics.com.</span><span class="sxs-lookup"><span data-stu-id="6d54c-113">If you have pop-up blocker enabled in your browser, change it to allow URLs from the \*.businesscentral.dynamics.com address.</span></span>

4. <span data-ttu-id="6d54c-114">Когда среда песочницы будет готова, вы будете перенаправлены в приветственный мастер среды песочницы.</span><span class="sxs-lookup"><span data-stu-id="6d54c-114">When the sandbox environment is ready, you will be redirected to sandbox environment's Welcome wizard.</span></span>
<!-- ![Sandbox Welcome Wizard](./media/across-sandbox/sandbox-wizard.png) -->

5. <span data-ttu-id="6d54c-115">Нажмите кнопку **Подробнее**, чтобы прочитать о сценариях, которые вы можете попробовать в среде песочницы, или кнопку **Закрыть**, чтобы перейти к ролевому центру вашего экземпляр песочницы [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6d54c-115">Choose the **Learn more** button to read about scenarios that you can try in a sandbox environment or choose the **Close** button to continue to the Role Center of your [!INCLUDE[d365fin](includes/d365fin_md.md)] sandbox instance.</span></span>

    <span data-ttu-id="6d54c-116">В верхней части ролевого центра появится уведомление о том, что это среда песочницы.</span><span class="sxs-lookup"><span data-stu-id="6d54c-116">At the top of the Role Center, a notification appears to inform you that this is a sandbox environment.</span></span> <span data-ttu-id="6d54c-117">Тип среды также отображается в строке заголовка клиента.</span><span class="sxs-lookup"><span data-stu-id="6d54c-117">You can also see the type of the environment in the title bar of the client.</span></span>
    <!-- ![Sandbox RoleCenter Notification](./media/across-sandbox/sandbox-rolecenter-notification.png) -->

    > [!NOTE]
    > <span data-ttu-id="6d54c-118">Созданная таким образом среда песочницы содержит только демонстрационные данные по умолчанию для компании CRONUS.</span><span class="sxs-lookup"><span data-stu-id="6d54c-118">A sandbox environment created in this way only contains the default demonstration data for the CRONUS company.</span></span> <span data-ttu-id="6d54c-119">Никакие данные не копируются и не переносятся каким-либо другим образом из производственной среды.</span><span class="sxs-lookup"><span data-stu-id="6d54c-119">No data is copied or otherwise transferred from the production environment.</span></span><br /><br />
    > <span data-ttu-id="6d54c-120">Вы также можете создать среду песочницы, содержащую производственные данные.</span><span class="sxs-lookup"><span data-stu-id="6d54c-120">You can also create a sandbox environment containing the production data.</span></span> <span data-ttu-id="6d54c-121">Вы должны сделать это через центр администрирования.</span><span class="sxs-lookup"><span data-stu-id="6d54c-121">You must do this through the administration center.</span></span> <span data-ttu-id="6d54c-122">Дополнительные сведения см. в разделе [Управление средами](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments) в справке для разработчиков и ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="6d54c-122">For more information, see [Managing Environments](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments) in the Developer and IT-Pro help.</span></span>

6. <span data-ttu-id="6d54c-123">В любой момент можно вернуться на страницу **Среда "песочницы"** и сбросить среду "песочницы".</span><span class="sxs-lookup"><span data-stu-id="6d54c-123">At any time, you can return to the **Sandbox Environment** page, and reset the sandbox environment.</span></span>
    > [!NOTE]  
    >  <span data-ttu-id="6d54c-124">При сбросе среды песочницы она полностью удаляется, а затем создается заново с демонстрационными данными по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6d54c-124">Resetting the sandbox environment will remove it completely, and then create it again with the default demonstration data.</span></span>  

7. <span data-ttu-id="6d54c-125">Для переключения между производственной средой и средой песочницы можно использовать средства запуска приложений Business Central.</span><span class="sxs-lookup"><span data-stu-id="6d54c-125">To switch between your production and sandbox environments, you can use the Business Central app launcher.</span></span>
<!-- ![Sandbox Dynamics365 Menu](./media/across-sandbox/sandbox-dynamics365-menu.png) -->

8. <span data-ttu-id="6d54c-126">Администратор или другой пользователь может ограничить или даже блокировать доступ некоторых пользователей к среде песочницы.</span><span class="sxs-lookup"><span data-stu-id="6d54c-126">It is possible for an administrator or another user to limit or even block access for some users to the sandbox environment.</span></span> <span data-ttu-id="6d54c-127">Это можно сделать с помощью стандартных функций безопасности для продукта, таких как карта пользователя, группы пользователей и наборы разрешений.</span><span class="sxs-lookup"><span data-stu-id="6d54c-127">This can be done by using the standard security features of the product, such as the User card, user groups, and permission sets.</span></span>

<!-- ![Sandbox Permission Sets](./media/across-sandbox/sandbox-permission-sets.png) -->

## <a name="advanced-functionality-in-the-sandbox-environment"></a><span data-ttu-id="6d54c-128">Расширенная функциональная возможность в среде песочницы</span><span class="sxs-lookup"><span data-stu-id="6d54c-128">Advanced Functionality in the Sandbox Environment</span></span>
### <a name="designer"></a><span data-ttu-id="6d54c-129">Дизайнер</span><span class="sxs-lookup"><span data-stu-id="6d54c-129">Designer</span></span>
<span data-ttu-id="6d54c-130">В среде песочницы имеется включенная функция **Конструктор**, которую можно активировать, выбрав значок конструктора ![Конструктор](./media/across-sandbox/sandbox-inclient-design-icon.png) на странице.</span><span class="sxs-lookup"><span data-stu-id="6d54c-130">In a sandbox environment, you will find the **Designer** enabled, which you can activate by selecting the design icon ![Designer](./media/across-sandbox/sandbox-inclient-design-icon.png) on a page.</span></span>

<!-- ![In-client Designer](./media/across-sandbox/sandbox-inclient-designer.png) -->

### <a name="to-enable-the-advanced-user-experience"></a><span data-ttu-id="6d54c-131">Включение расширенных возможностей пользователя</span><span class="sxs-lookup"><span data-stu-id="6d54c-131">To enable the advanced user experience</span></span>
<span data-ttu-id="6d54c-132">Можно включить и попробовать расширенные (полные) функциональные возможности [!INCLUDE[d365fin](includes/d365fin_md.md)] в среде арендатора песочницы, задав поле **Опыт** на странице **Информация о компании**.</span><span class="sxs-lookup"><span data-stu-id="6d54c-132">It is possible to enable and try the advanced (full) functionality of [!INCLUDE[d365fin](includes/d365fin_md.md)] in a sandbox tenant by setting the **Experience** field on the **Company Information** page.</span></span>

<!-- ![Sandbox Environment Advanced](./media/across-sandbox/sandbox-advanced.png) -->

<!-- ![Sandbox Production](./media/across-sandbox/sandbox-production.png) -->

<span data-ttu-id="6d54c-133">После включения расширенных функциональных возможностей в арендаторе песочницы вы получаете доступ ко всем стандартным профилям (ролям) и ролевым центрам.</span><span class="sxs-lookup"><span data-stu-id="6d54c-133">After you have enabled the advanced functionality in a sandbox tenant, you get access to all the standard profiles (roles) and Role Centers.</span></span> <span data-ttu-id="6d54c-134">Можно также создать полностью настроенную пробную организацию, включая демонстрационные данные и доступ к расширенным возможностям продукта.</span><span class="sxs-lookup"><span data-stu-id="6d54c-134">You can also create an evaluation company that is fully set up, including demonstration data and access to the advanced areas of the product.</span></span>

<!-- ![Sandbox New Company](./media/across-sandbox/sandbox-newcompany.png) -->


## <a name="see-also"></a><span data-ttu-id="6d54c-135">См. также</span><span class="sxs-lookup"><span data-stu-id="6d54c-135">See Also</span></span>
<span data-ttu-id="6d54c-136">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6d54c-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
