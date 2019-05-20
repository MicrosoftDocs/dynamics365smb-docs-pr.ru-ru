---
title: Создание среды "песочницы" | Документы Майкрософт
description: Создайте среду для исследования, обучения, демонстрации, разработки и тестирования.
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sandbox, demo, develop
ms.date: 04/01/2019
ms.author: solsen
ms.openlocfilehash: 113c081e60b825c48cfb85ae3475a713a1a1e215
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1241664"
---
[!INCLUDE[d365fin_early_release](includes/d365fin_early_release.md.md)]

# <a name="creating-a-sandbox-environment"></a><span data-ttu-id="07acf-103">Создание среды "песочницы"</span><span class="sxs-lookup"><span data-stu-id="07acf-103">Creating a Sandbox Environment</span></span>
<span data-ttu-id="07acf-104">Среда песочницы (функция для предварительного ознакомления) представляет собой непроизводственный экземпляр [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07acf-104">A sandbox environment (Preview) is a non-production instance of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="07acf-105">В среде песочницы, изолированной от производственной среды, можно безопасно исследовать, обучать, демонстрировать, разрабатывать и тестировать сервисы без риска повлиять на данные или настройки производственной среды.</span><span class="sxs-lookup"><span data-stu-id="07acf-105">Isolated from production, a sandbox environment is the place to safely explore, learn, demo, develop, and test the service without the risk of affecting the data and settings of your production environment.</span></span>

## <a name="to-create-a-sandbox-environment"></a><span data-ttu-id="07acf-106">Создание среды "песочницы"</span><span class="sxs-lookup"><span data-stu-id="07acf-106">To create a sandbox environment</span></span>
<span data-ttu-id="07acf-107">Чтобы можно было создать среду песочницы, необходима подписка на [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07acf-107">You must have a subscription to [!INCLUDE[d365fin](includes/d365fin_md.md)] to be able to create a sandbox environment.</span></span> <span data-ttu-id="07acf-108">В каждой подписке может быть только одна среда песочницы.</span><span class="sxs-lookup"><span data-stu-id="07acf-108">There can only be one sandbox environment per subscription.</span></span>

1. <span data-ttu-id="07acf-109">Выполните вход в производственный экземпляр службы [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07acf-109">Sign in to your production instance of the [!INCLUDE[d365fin](includes/d365fin_md.md)] service.</span></span>
2. <span data-ttu-id="07acf-110">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Среда "песочницы"**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="07acf-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sandbox Environment**, and then choose the related link.</span></span>
<!-- ![Sandbox Environment Setup](./media/across-sandbox/sandbox-environment-setup.png) -->
3. <span data-ttu-id="07acf-111">Выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="07acf-111">Select **Create**.</span></span>  
  <span data-ttu-id="07acf-112">В браузере откроется другая вкладка для завершения настройки среды песочницы.</span><span class="sxs-lookup"><span data-stu-id="07acf-112">Another tab in your browser will open for finishing the setup of your sandbox environment.</span></span>
> [!NOTE]  
>  <span data-ttu-id="07acf-113">Если в браузере включена блокировка всплывающих окон, измените ее, чтобы разрешить URL-адреса с адреса \*.businesscentral.dynamics.com.</span><span class="sxs-lookup"><span data-stu-id="07acf-113">If you have pop-up blocker enabled in your browser, change it to allow URLs from the \*.businesscentral.dynamics.com address.</span></span>   

4. <span data-ttu-id="07acf-114">Когда среда песочницы будет готова, вы будете перенаправлены в приветственный мастер среды песочницы.</span><span class="sxs-lookup"><span data-stu-id="07acf-114">When the sandbox environment is ready, you will be redirected to sandbox environment's Welcome wizard.</span></span>
<!-- ![Sandbox Welcome Wizard](./media/across-sandbox/sandbox-wizard.png) -->

5. <span data-ttu-id="07acf-115">Выберите **Узнать больше**, чтобы ознакомиться с сценариями, которые можно попробовать в среде песочницы.</span><span class="sxs-lookup"><span data-stu-id="07acf-115">Choose **Learn more** to read about scenarios that you can try in a sandbox environment.</span></span> <span data-ttu-id="07acf-116">Или выберите **Закрыть**, чтобы перейти в ролевой центр экземпляра "песочницы" [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07acf-116">Or, choose **Close** to continue to the Role Center of your [!INCLUDE[d365fin](includes/d365fin_md.md)] sandbox instance.</span></span>
6. <span data-ttu-id="07acf-117">В верхней части ролевого центра появится уведомление о том, что это среда песочницы.</span><span class="sxs-lookup"><span data-stu-id="07acf-117">At the top of the Role Center, a notification appears to inform you that this is a sandbox environment.</span></span> <span data-ttu-id="07acf-118">Тип среды также отображается в строке заголовка клиента.</span><span class="sxs-lookup"><span data-stu-id="07acf-118">You can also see the type of the environment in the title bar of the client.</span></span>
<!-- ![Sandbox RoleCenter Notification](./media/across-sandbox/sandbox-rolecenter-notification.png) --> <span data-ttu-id="07acf-119">В среде песочницы создан новый арендатор.</span><span class="sxs-lookup"><span data-stu-id="07acf-119">In the sandbox environment, a new tenant has been created.</span></span> <span data-ttu-id="07acf-120">Для этого арендатора загружены демонстрационные данные по умолчанию компании CRONUS.</span><span class="sxs-lookup"><span data-stu-id="07acf-120">This tenant is loaded with default demonstration data for the CRONUS company.</span></span> <span data-ttu-id="07acf-121">При создании песочницы никакие данные не копируются и не переносятся каким-либо другим образом из производственной среды.</span><span class="sxs-lookup"><span data-stu-id="07acf-121">No data is copied or otherwise transferred from the production environment during the sandbox creation.</span></span>

7. <span data-ttu-id="07acf-122">В любой момент можно вернуться на страницу **Среда "песочницы"** и сбросить среду "песочницы".</span><span class="sxs-lookup"><span data-stu-id="07acf-122">At any time, you can return to the **Sandbox Environment** page, and reset the sandbox environment.</span></span>
> [!NOTE]  
>  <span data-ttu-id="07acf-123">При сбросе среды песочницы она полностью удаляется, а затем создается заново с демонстрационными данными по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="07acf-123">Resetting the sandbox environment will remove it completely, and then create it again with the default demonstration data.</span></span>  

8. <span data-ttu-id="07acf-124">Для переключения между производственной средой и средой песочницы можно использовать средства запуска приложений Business Central.</span><span class="sxs-lookup"><span data-stu-id="07acf-124">To switch between your production and sandbox environments, you can use the Business Central app launcher.</span></span>
<!-- ![Sandbox Dynamics365 Menu](./media/across-sandbox/sandbox-dynamics365-menu.png) -->

9. <span data-ttu-id="07acf-125">Администратор или другой пользователь может ограничить или даже блокировать доступ некоторых пользователей к среде песочницы.</span><span class="sxs-lookup"><span data-stu-id="07acf-125">It is possible for an administrator or another user to limit or even block access for some users to the sandbox environment.</span></span> <span data-ttu-id="07acf-126">Это можно сделать с помощью стандартных функций безопасности для продукта, таких как карта пользователя, группы пользователей и наборы разрешений.</span><span class="sxs-lookup"><span data-stu-id="07acf-126">This can be done by using the standard security features of the product, such as the User card, User Groups, and Permission Sets.</span></span>

<!-- ![Sandbox Permission Sets](./media/across-sandbox/sandbox-permission-sets.png) -->

## <a name="advanced-functionality-in-the-sandbox-environment"></a><span data-ttu-id="07acf-127">Расширенная функциональная возможность в среде песочницы</span><span class="sxs-lookup"><span data-stu-id="07acf-127">Advanced functionality in the sandbox environment</span></span>
### <a name="designer"></a><span data-ttu-id="07acf-128">Дизайнер</span><span class="sxs-lookup"><span data-stu-id="07acf-128">Designer</span></span>
<span data-ttu-id="07acf-129">В среде песочницы имеется включенная функция **Конструктор**, которую можно активировать, выбрав значок конструктора ![Конструктор](./media/across-sandbox/sandbox-inclient-design-icon.png) на странице.</span><span class="sxs-lookup"><span data-stu-id="07acf-129">In a sandbox environment, you will find the **Designer** enabled, which you can activate by selecting the design icon ![Designer](./media/across-sandbox/sandbox-inclient-design-icon.png) on a page.</span></span>

<!-- ![In-client Designer](./media/across-sandbox/sandbox-inclient-designer.png) -->

### <a name="enable-the-advanced-user-experience"></a><span data-ttu-id="07acf-130">Включение расширенных возможностей пользователя</span><span class="sxs-lookup"><span data-stu-id="07acf-130">Enable the advanced user experience</span></span>
<span data-ttu-id="07acf-131">Можно включить и попробовать расширенные (полные) функциональные возможности [!INCLUDE[d365fin](includes/d365fin_md.md)] в среде арендатора песочницы, задав поле **Опыт** на странице **Информация о компании**.</span><span class="sxs-lookup"><span data-stu-id="07acf-131">It is possible to enable and try the advanced (full) functionality of [!INCLUDE[d365fin](includes/d365fin_md.md)] in a sandbox tenant by setting the **Experience** field on the **Company Information** page.</span></span>

<!-- ![Sandbox Environment Advanced](./media/across-sandbox/sandbox-advanced.png) -->

<!-- ![Sandbox Production](./media/across-sandbox/sandbox-production.png) -->

<span data-ttu-id="07acf-132">После включения расширенных функциональных возможностей в арендаторе песочницы вы получаете доступ ко всем стандартным профилям и ролевым центрам.</span><span class="sxs-lookup"><span data-stu-id="07acf-132">After you’ve enabled the advanced functionality in a sandbox tenant, you get access to all the standard Profiles and Role Centers.</span></span> <span data-ttu-id="07acf-133">Можно также создать полностью настроенную пробную организацию, включая демонстрационные данные и доступ к расширенным возможностям продукта.</span><span class="sxs-lookup"><span data-stu-id="07acf-133">You can also create an evaluation company that is fully set up, including demonstration data and access to the advanced areas of the product.</span></span>

<!-- ![Sandbox New Company](./media/across-sandbox/sandbox-newcompany.png) -->


## <a name="see-also"></a><span data-ttu-id="07acf-134">См. также</span><span class="sxs-lookup"><span data-stu-id="07acf-134">See Also</span></span>
<span data-ttu-id="07acf-135">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="07acf-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
