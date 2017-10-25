---
title: "Создание среды \"песочницы\" | Документы Майкрософт"
description: "Создайте среду для исследования, обучения, демонстрации, разработки и тестирования."
author: SusanneWindfeldPedersen
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sandbox, demo, develop
ms.date: 08/18/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: d7bcb866d5f69e77e5a175d0b73e8ac03cf09d98
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
[!INCLUDE[d365fin_early_release](includes/d365fin_early_release.md.md)]

# <a name="how-to-create-a-sandbox-environment"></a><span data-ttu-id="26b8a-103">Практическое руководство. Создание среды "песочницы"</span><span class="sxs-lookup"><span data-stu-id="26b8a-103">How to: Create a Sandbox Environment</span></span>
<span data-ttu-id="26b8a-104">Среда песочницы (функция для предварительного ознакомления) представляет собой непроизводственный экземпляр [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="26b8a-104">A sandbox environment (Preview) is a non-production instance of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="26b8a-105">В среде песочницы, изолированной от производственной среды, можно безопасно исследовать, обучать, демонстрировать, разрабатывать и тестировать сервисы без риска повлиять на данные или настройки производственной среды.</span><span class="sxs-lookup"><span data-stu-id="26b8a-105">Isolated from production, a sandbox environment is the place to safely explore, learn, demo, develop, and test the service without the risk of affecting the data and settings of your production environment.</span></span>

## <a name="to-create-a-sandbox-environment"></a><span data-ttu-id="26b8a-106">Создание среды "песочницы"</span><span class="sxs-lookup"><span data-stu-id="26b8a-106">To create a sandbox environment</span></span>
<span data-ttu-id="26b8a-107">Чтобы можно было создать среду песочницы, необходима подписка на [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="26b8a-107">You must have a subscription to [!INCLUDE[d365fin](includes/d365fin_md.md)] to be able to create a sandbox environment.</span></span> <span data-ttu-id="26b8a-108">В каждой подписке может быть только одна среда песочницы.</span><span class="sxs-lookup"><span data-stu-id="26b8a-108">There can only be one sandbox environment per subscription.</span></span>

1. <span data-ttu-id="26b8a-109">Выполните вход в производственный экземпляр службы [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="26b8a-109">Sign in to your production instance of the [!INCLUDE[d365fin](includes/d365fin_md.md)] service.</span></span>
2. <span data-ttu-id="26b8a-110">Выберите ![Поиск страницы или отчета](media/ui-search/search_small.png "значок поиска страницы или отчета"), введите **Среда "песочницы"**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="26b8a-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sandbox Environment**, and then choose the related link.</span></span>
<span data-ttu-id="26b8a-111">![Настройка среды "песочницы"](./media/across-sandbox/sandbox-environment-setup.png)</span><span class="sxs-lookup"><span data-stu-id="26b8a-111">![Sandbox Environment Setup](./media/across-sandbox/sandbox-environment-setup.png)</span></span>
3. <span data-ttu-id="26b8a-112">Выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="26b8a-112">Select **Create**.</span></span>  
  <span data-ttu-id="26b8a-113">В браузере откроется другая вкладка для завершения настройки среды песочницы.</span><span class="sxs-lookup"><span data-stu-id="26b8a-113">Another tab in your browser will open for finishing the setup of your sandbox environment.</span></span>
> [!NOTE]  
>  <span data-ttu-id="26b8a-114">Если в браузере включена блокировка всплывающих окон, измените ее, чтобы разрешить URL-адреса с адреса *.financials.dynamics.com.</span><span class="sxs-lookup"><span data-stu-id="26b8a-114">If you have pop-up blocker enabled in your browser, change it to allow URLs from the *.financials.dynamics.com address.</span></span>   

4. <span data-ttu-id="26b8a-115">Когда среда песочницы будет готова, вы будете перенаправлены в приветственный мастер среды песочницы.</span><span class="sxs-lookup"><span data-stu-id="26b8a-115">When the sandbox environment is ready, you will be redirected to sandbox environment's Welcome wizard.</span></span>
<span data-ttu-id="26b8a-116">![Приветственный мастер "песочницы"](./media/across-sandbox/sandbox-wizard.png)</span><span class="sxs-lookup"><span data-stu-id="26b8a-116">![Sandbox Welcome Wizard](./media/across-sandbox/sandbox-wizard.png)</span></span>

5. <span data-ttu-id="26b8a-117">Выберите **Узнать больше**, чтобы ознакомиться с сценариями, которые можно попробовать в среде песочницы.</span><span class="sxs-lookup"><span data-stu-id="26b8a-117">Choose **Learn more** to read about scenarios that you can try in a sandbox environment.</span></span> <span data-ttu-id="26b8a-118">Или выберите **Закрыть**, чтобы перейти в ролевой центр экземпляра "песочницы" [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="26b8a-118">Or, choose **Close** to continue to the Role Center of your [!INCLUDE[d365fin](includes/d365fin_md.md)] sandbox instance.</span></span>
6. <span data-ttu-id="26b8a-119">В верхней части ролевого центра появится уведомление о том, что это среда песочницы.</span><span class="sxs-lookup"><span data-stu-id="26b8a-119">At the top of the Role Center, a notification appears to inform you that this is a sandbox environment.</span></span> <span data-ttu-id="26b8a-120">Тип среды также отображается в строке заголовка клиента.</span><span class="sxs-lookup"><span data-stu-id="26b8a-120">You can also see the type of the environment in the title bar of the client.</span></span>
<span data-ttu-id="26b8a-121">![Уведомление ролевого центра "песочницы"](./media/across-sandbox/sandbox-rolecenter-notification.png)</span><span class="sxs-lookup"><span data-stu-id="26b8a-121">![Sandbox RoleCenter Notification](./media/across-sandbox/sandbox-rolecenter-notification.png)</span></span>  
<span data-ttu-id="26b8a-122">В среде песочницы создан новый арендатор.</span><span class="sxs-lookup"><span data-stu-id="26b8a-122">In the sandbox environment, a brand-new tenant has been created.</span></span> <span data-ttu-id="26b8a-123">Для этого арендатора загружены демонстрационные данные по умолчанию компании CRONUS.</span><span class="sxs-lookup"><span data-stu-id="26b8a-123">This tenant is loaded with default demonstration data for the CRONUS company.</span></span> <span data-ttu-id="26b8a-124">При создании песочницы никакие данные не копируются и не переносятся каким-либо другим образом из производственной среды.</span><span class="sxs-lookup"><span data-stu-id="26b8a-124">No data is copied or otherwise transferred from the production environment during the sandbox creation.</span></span>
7.  <span data-ttu-id="26b8a-125">В любой момент можно вернуться на страницу **Среда "песочницы"** и сбросить среду "песочницы".</span><span class="sxs-lookup"><span data-stu-id="26b8a-125">At any time, you can return to the **Sandbox Environment** page, and reset the sandbox environment.</span></span>
> [!NOTE]  
>  <span data-ttu-id="26b8a-126">При сбросе среды песочницы она полностью удаляется, а затем создается заново с демонстрационными данными по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="26b8a-126">Resetting the sandbox environment will remove it completely, and then create it again with the default demonstration data.</span></span>  

8.  <span data-ttu-id="26b8a-127">Для переключения между производственной средой и средой песочницы можно использовать средства запуска приложений Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="26b8a-127">To switch between your production and sandbox environments, you can use the Dynamics 365 app launcher.</span></span>
<span data-ttu-id="26b8a-128">![Меню песочницы Dynamics365](./media/across-sandbox/sandbox-dynamics365-menu.png)</span><span class="sxs-lookup"><span data-stu-id="26b8a-128">![Sandbox Dynamics365 Menu](./media/across-sandbox/sandbox-dynamics365-menu.png)</span></span>

9.  <span data-ttu-id="26b8a-129">Администратор или другой пользователь может ограничить или даже блокировать доступ некоторых пользователей к среде песочницы.</span><span class="sxs-lookup"><span data-stu-id="26b8a-129">It is possible for an administrator or another user to limit or even block access for some users to the sandbox environment.</span></span> <span data-ttu-id="26b8a-130">Это можно сделать с помощью стандартных функций безопасности для продукта, таких как карта пользователя, группы пользователей и наборы разрешений.</span><span class="sxs-lookup"><span data-stu-id="26b8a-130">This can be done by using the standard security features of the product, such as the User card, User Groups, and Permission Sets.</span></span>

![Наборы разрешений песочницы](./media/across-sandbox/sandbox-permission-sets.png)

## <a name="advanced-functionality-in-the-sandbox-environment"></a><span data-ttu-id="26b8a-132">Расширенная функциональная возможность в среде песочницы</span><span class="sxs-lookup"><span data-stu-id="26b8a-132">Advanced functionality in the sandbox environment</span></span>
### <a name="the-in-client-designer"></a><span data-ttu-id="26b8a-133">Конструктор в клиенте.</span><span class="sxs-lookup"><span data-stu-id="26b8a-133">The in-client designer</span></span>
<span data-ttu-id="26b8a-134">В среде песочницы имеется включенная функция конструктора в клиенте, которую можно активировать, выбрав значок конструктора</span><span class="sxs-lookup"><span data-stu-id="26b8a-134">In a sandbox environment, you will find the in-client designer feature enabled, which you can activate by selecting the design icon</span></span> ![Дизайнер](./media/across-sandbox/sandbox-inclient-design-icon.png) <span data-ttu-id="26b8a-136">на странице.</span><span class="sxs-lookup"><span data-stu-id="26b8a-136">on a page.</span></span>

![Конструктор в клиенте](./media/across-sandbox/sandbox-inclient-designer.png)

### <a name="enable-the-advanced-user-experience"></a><span data-ttu-id="26b8a-138">Включение расширенных возможностей пользователя</span><span class="sxs-lookup"><span data-stu-id="26b8a-138">Enable the advanced user experience</span></span>
<span data-ttu-id="26b8a-139">Можно включить и попробовать расширенные (полные) функциональные возможности [!INCLUDE[d365fin](includes/d365fin_md.md)] в среде арендатора песочницы, задав поле **Опыт** на странице **Информация о компании**.</span><span class="sxs-lookup"><span data-stu-id="26b8a-139">It is possible to enable and try the advanced (full) functionality of [!INCLUDE[d365fin](includes/d365fin_md.md)] in a sandbox tenant by setting the **Experience** field on the **Company Information** page.</span></span>

![Расширенная среда "песочницы"](./media/across-sandbox/sandbox-advanced.png)

![Производство песочницы](./media/across-sandbox/sandbox-production.png)

<span data-ttu-id="26b8a-142">После включения расширенных функциональных возможностей в арендаторе песочницы вы получаете доступ ко всем стандартным профилям и ролевым центрам.</span><span class="sxs-lookup"><span data-stu-id="26b8a-142">After you’ve enabled the advanced functionality in a sandbox tenant, you get access to all the standard Profiles and Role Centers.</span></span> <span data-ttu-id="26b8a-143">Можно также создать полностью настроенную пробную организацию, включая демонстрационные данные и доступ к расширенным возможностям продукта.</span><span class="sxs-lookup"><span data-stu-id="26b8a-143">You can also create an evaluation company that is fully set up, including demonstration data and access to the advanced areas of the product.</span></span>

![Новая компания в песочнице](./media/across-sandbox/sandbox-newcompany.png)


## <a name="see-also"></a><span data-ttu-id="26b8a-145">См. также</span><span class="sxs-lookup"><span data-stu-id="26b8a-145">See Also</span></span>
<span data-ttu-id="26b8a-146">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="26b8a-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

