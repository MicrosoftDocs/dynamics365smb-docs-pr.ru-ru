---
title: Использование данных для создания приложения | Документация Майкрософт
description: Данные Business Central можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания бизнес-приложения с помощью Power Apps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: OData, Power App, SOAP
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 25607473e20bca8cec8cd65e2e808e12dda47869
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5774540"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-power-apps"></a><span data-ttu-id="e360c-103">Подключение к данным Business Central для создания бизнес-приложения с помощью Power Apps</span><span class="sxs-lookup"><span data-stu-id="e360c-103">Connecting to Your Business Central Data to Build a Business App Using Power Apps</span></span>

<span data-ttu-id="e360c-104">Данные [!INCLUDE[prod_short](includes/prod_short.md)] можно сделать доступными в качестве источника данных в Power Apps.</span><span class="sxs-lookup"><span data-stu-id="e360c-104">You can make your [!INCLUDE[prod_short](includes/prod_short.md)] data available as a data source in Power Apps.</span></span>  

> [!NOTE]  
> <span data-ttu-id="e360c-105">Вы должны иметь допустимую учетную запись в [!INCLUDE[prod_short](includes/prod_short.md)] и в Power Apps.</span><span class="sxs-lookup"><span data-stu-id="e360c-105">You must have a valid account with [!INCLUDE[prod_short](includes/prod_short.md)] and with Power Apps.</span></span>  

## <a name="to-add-prod_short-as-a-data-source-in-power-apps"></a><span data-ttu-id="e360c-106">Добавление [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных в Power Apps</span><span class="sxs-lookup"><span data-stu-id="e360c-106">To add [!INCLUDE[prod_short](includes/prod_short.md)] as a data source in Power Apps</span></span>

1. <span data-ttu-id="e360c-107">В браузере перейдите к [powerapps.microsoft.com](https://powerapps.microsoft.com/) и выполните вход.</span><span class="sxs-lookup"><span data-stu-id="e360c-107">In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/), and then sign in.</span></span>
2. <span data-ttu-id="e360c-108">На домашней странице, в разделе **Начать с данных**, выберите плитка **Другие источники данных**.</span><span class="sxs-lookup"><span data-stu-id="e360c-108">On the Home page, in the **Start from data** section, choose the **Other data sources** tile.</span></span>  

    <span data-ttu-id="e360c-109">Это открывает Power Apps Studio.</span><span class="sxs-lookup"><span data-stu-id="e360c-109">This opens Power Apps Studio.</span></span> <span data-ttu-id="e360c-110">При первом входе в систему необходимо указать страну/регион.</span><span class="sxs-lookup"><span data-stu-id="e360c-110">On first login, you must specify the country/region.</span></span>  
3. <span data-ttu-id="e360c-111">В списке доступных соединений выберите **Business Central**, затем нажмите кнопку **Создать**.</span><span class="sxs-lookup"><span data-stu-id="e360c-111">In the list of available connections, choose **Business Central**, and then choose the **Create** button.</span></span>

    <span data-ttu-id="e360c-112">Power Apps подключится к вашему экземпляру [!INCLUDE[prod_short](includes/prod_short.md)] с использованием учетных данных, с которыми вы выполнили вход.</span><span class="sxs-lookup"><span data-stu-id="e360c-112">Power Apps will connect to your [!INCLUDE[prod_short](includes/prod_short.md)] using the credentials that you are signed in with.</span></span> <span data-ttu-id="e360c-113">Если вы не являетесь администратором [!INCLUDE[prod_short](includes/prod_short.md)], может потребоваться выполнить вход с другой учетной записью.</span><span class="sxs-lookup"><span data-stu-id="e360c-113">If you are not an administrator of your [!INCLUDE[prod_short](includes/prod_short.md)], you may have to sign in with another account.</span></span>  

4. <span data-ttu-id="e360c-114">Power Apps отобразит список *сред и организаций*, доступных в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="e360c-114">Power Apps will display a list of *Environments and companies* that are available from [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="e360c-115">Выберите среду и организацию, содержащую данные, к которым вы хотите подключиться, такие как *РАБОЧАЯ — Моя компания*.</span><span class="sxs-lookup"><span data-stu-id="e360c-115">Choose the environment and company that contains the data you want to connect to, such as *PRODUCTION - My Company*.</span></span>  

5. <span data-ttu-id="e360c-116">Далее вам будет представлен список таблиц, которые предоставляются как часть API для вашей среды.</span><span class="sxs-lookup"><span data-stu-id="e360c-116">Next, you will be presented with a list of tables that are exposed as part of the API for your environment.</span></span> <span data-ttu-id="e360c-117">Выберите таблицу, к которой вы хотите подключиться, а затем выберите **Подключить**.</span><span class="sxs-lookup"><span data-stu-id="e360c-117">Select the table that you want to connect to, and then choose **Connect**.</span></span>

<span data-ttu-id="e360c-118">Эти так называемые таблицы отображаются как конечные точки соединителем [!INCLUDE[prod_short](includes/prod_short.md)] для Power Apps.</span><span class="sxs-lookup"><span data-stu-id="e360c-118">These so-called tables are exposed as endpoints by the [!INCLUDE[prod_short](includes/prod_short.md)] connector for Power Apps.</span></span>  

> [!NOTE]
> <span data-ttu-id="e360c-119">Если требуется включение данных из других таблиц в [!INCLUDE[prod_short](includes/prod_short.md)] в ваше приложение, необходимо работать с разработчиком для определения пользовательского API-интерфейса в [!INCLUDE[prod_short](includes/prod_short.md)], затем использовать этот пользовательский API-интерфейс через пользовательский соединитель в Power Apps.</span><span class="sxs-lookup"><span data-stu-id="e360c-119">If you want to include data from other tables in [!INCLUDE[prod_short](includes/prod_short.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE[prod_short](includes/prod_short.md)] and then consume that custom API through a custom connector in Power Apps.</span></span> <span data-ttu-id="e360c-120">Дополнительные сведения см. в разделе [Создание пользовательского соединителя с нуля](/connectors/custom-connectors/define-blank).</span><span class="sxs-lookup"><span data-stu-id="e360c-120">For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).</span></span>  

<span data-ttu-id="e360c-121">На этом шаге вы успешно подключились с данным [!INCLUDE[prod_short](includes/prod_short.md)] и готовы начать создание PowerApp.</span><span class="sxs-lookup"><span data-stu-id="e360c-121">At this point, you have successfully connected to your [!INCLUDE[prod_short](includes/prod_short.md)] data and are ready to begin building your PowerApp.</span></span> <span data-ttu-id="e360c-122">Можно добавить дополнительные экраны и подключить дополнительные данные из [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="e360c-122">You can add additional screens and connect to additional data from your [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="e360c-123">Дополнительные сведения см. в разделе [Создание приложения на основе холста из примера в Power Apps](/powerapps/maker/canvas-apps/open-and-run-a-sample-app).</span><span class="sxs-lookup"><span data-stu-id="e360c-123">For more information, see [Create a canvas app from a sample in Power Apps](/powerapps/maker/canvas-apps/open-and-run-a-sample-app).</span></span>  

<span data-ttu-id="e360c-124">После разработки и построения приложения можно поделиться им с коллегами.</span><span class="sxs-lookup"><span data-stu-id="e360c-124">When you have designed and built your app, you can share it with your colleagues.</span></span> <span data-ttu-id="e360c-125">Дополнительные сведения см. в разделе [Сохранение и публикация приложения на основе холста в Power Apps](/powerapps/maker/canvas-apps/save-publish-app).</span><span class="sxs-lookup"><span data-stu-id="e360c-125">For more information, see [Save and publish a canvas app in Power Apps](/powerapps/maker/canvas-apps/save-publish-app).</span></span>  

> [!NOTE]
> <span data-ttu-id="e360c-126">Если требуется подключиться к [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises, необходимо выбрать соединитель **Business Central (локальная версия)** на шаге 3.</span><span class="sxs-lookup"><span data-stu-id="e360c-126">If you want to connect to [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, then you must choose the **Business Central (on-premises)** connector in step 3.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e360c-127">См. также</span><span class="sxs-lookup"><span data-stu-id="e360c-127">See Also</span></span>

[<span data-ttu-id="e360c-128">Создание приложения на основе холста из шаблона в Power Apps</span><span class="sxs-lookup"><span data-stu-id="e360c-128">Create a canvas app from a template in Power Apps</span></span>](/powerapps/maker/canvas-apps/get-started-test-drive)  
[<span data-ttu-id="e360c-129">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="e360c-129">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="e360c-130">[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="e360c-130">[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span></span>  
[<span data-ttu-id="e360c-131">Начальные сведения по разработке соединительных приложений для Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="e360c-131">Getting Started Developing Connect Apps for Dynamics 365 Business Central</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  


[!INCLUDE[footer-include](includes/footer-banner.md)]