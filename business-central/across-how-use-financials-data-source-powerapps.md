---
title: Использование данных для создания приложения | Документация Майкрософт
description: Данные Business Central можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания бизнес-приложения с помощью PowerApps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Odata, Power App, SOAP
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: 4b8005154afb988cf25c6a04b7beeaafd199afca
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2305031"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-powerapps"></a><span data-ttu-id="794ee-103">Подключение к данным Business Central для создания бизнес-приложения с помощью PowerApps</span><span class="sxs-lookup"><span data-stu-id="794ee-103">Connecting to Your Business Central Data to Build a Business App Using PowerApps</span></span>
<span data-ttu-id="794ee-104">Данные [!INCLUDE[d365fin](includes/d365fin_md.md)] можно сделать доступными в качестве источника данных в PowerApps.</span><span class="sxs-lookup"><span data-stu-id="794ee-104">You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in PowerApps.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="794ee-105">Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в PowerApps.</span><span class="sxs-lookup"><span data-stu-id="794ee-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with PowerApps.</span></span>  

## <a name="to-add-included365finincludesd365fin_mdmd-as-a-data-source-in-powerapps"></a><span data-ttu-id="794ee-106">Добавление [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных в PowerApps</span><span class="sxs-lookup"><span data-stu-id="794ee-106">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in PowerApps</span></span>
1. <span data-ttu-id="794ee-107">В браузере перейдите к [powerapps.microsoft.com](https://powerapps.microsoft.com/en-us/) и выполните вход.</span><span class="sxs-lookup"><span data-stu-id="794ee-107">In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/en-us/), and then sign in.</span></span>
2. <span data-ttu-id="794ee-108">На домашней странице выберите **Приложения**, **Создать приложение** и **Холст**, чтобы создать новое приложение на основе холста.</span><span class="sxs-lookup"><span data-stu-id="794ee-108">On the Home page, choose the **Apps**, **Create an app** and **Canvas** to create a new canvas app.</span></span> <span data-ttu-id="794ee-109">Это приложение будет разработано для использования на мобильных устройствах, но также можно выбрать для использования другой шаблон.</span><span class="sxs-lookup"><span data-stu-id="794ee-109">This app will be designed for use on a mobile device, but you can also choose to use another template.</span></span>

    <span data-ttu-id="794ee-110">Следующий шаг создания PowerApp — выбор данных.</span><span class="sxs-lookup"><span data-stu-id="794ee-110">The next step to create a PowerApp is to select your data.</span></span> <span data-ttu-id="794ee-111">Щелкните значок стрелки, а затем выберите параметр **Новое подключение** в левом верхнем углу страницы.</span><span class="sxs-lookup"><span data-stu-id="794ee-111">Choose the Arrow icon then choose the **New connection** option in the upper left side of the page.</span></span>
3. <span data-ttu-id="794ee-112">В списке доступных соединений выберите **Business Central**, затем нажмите кнопку **Создать**.</span><span class="sxs-lookup"><span data-stu-id="794ee-112">In the list of available connections, choose **Business Central**, and then choose the **Create** button.</span></span>

    <span data-ttu-id="794ee-113">PowerApps подключится к вашему экземпляру [!INCLUDE [prodshort](includes/prodshort.md)] с использованием учетных данных, с которыми вы выполнили вход.</span><span class="sxs-lookup"><span data-stu-id="794ee-113">PowerApps will connect to your [!INCLUDE [prodshort](includes/prodshort.md)] using the credentials that you are signed in with.</span></span> <span data-ttu-id="794ee-114">Если вы не являетесь администратором [!INCLUDE [prodshort](includes/prodshort.md)], может потребоваться выполнить вход с другой учетной записью.</span><span class="sxs-lookup"><span data-stu-id="794ee-114">If you are not an administrator of your [!INCLUDE [prodshort](includes/prodshort.md)], you may have to sign in with another account.</span></span>  

4.  <span data-ttu-id="794ee-115">PowerApps отобразит список *сред и организаций*, доступных в [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="794ee-115">PowerApps will display a list of *Environments and companies* that are available from [!INCLUDE [prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="794ee-116">Выберите среду и организацию, содержащую данные, к которым вы хотите подключиться.</span><span class="sxs-lookup"><span data-stu-id="794ee-116">Choose the environment and company that contains the data you want to connect to.</span></span> <span data-ttu-id="794ee-117">Далее вы увидите список API.</span><span class="sxs-lookup"><span data-stu-id="794ee-117">Next, you will be presented with a list of APIs.</span></span> <span data-ttu-id="794ee-118">Выберите **API**, к которому вы ходите подключиться.</span><span class="sxs-lookup"><span data-stu-id="794ee-118">Select the **API** you want to connect to.</span></span>

<span data-ttu-id="794ee-119">Эти так называемые таблицы являются частью API-интерфейса [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="794ee-119">These so-called tables are part of the [!INCLUDE [prodshort](includes/prodshort.md)] API.</span></span> <span data-ttu-id="794ee-120">Настраивать конечные точки вам не нужно — соединитель [!INCLUDE [prodshort](includes/prodshort.md)] для PowerApps делает это автоматически.</span><span class="sxs-lookup"><span data-stu-id="794ee-120">You do not have to configure the end points yourself - the [!INCLUDE [prodshort](includes/prodshort.md)] connector for PowerApps does it for you.</span></span>  

    If you want to include data from other tables in [!INCLUDE [prodshort](includes/prodshort.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE [prodshort](includes/prodshort.md)] and then consume that custom API through a custom connector in PowerApps. For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).  

<span data-ttu-id="794ee-121">На этом шаге вы успешно подключились с данным [!INCLUDE [prodshort](includes/prodshort.md)] и готовы начать создание PowerApp.</span><span class="sxs-lookup"><span data-stu-id="794ee-121">At this point, you have successfully connected to your [!INCLUDE [prodshort](includes/prodshort.md)] data and are ready to begin building your PowerApp.</span></span> <span data-ttu-id="794ee-122">Можно добавить дополнительные экраны и подключить дополнительные данные из [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="794ee-122">You can add additional screens and connect to additional data from your [!INCLUDE [prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="794ee-123">Дополнительные сведения см. в разделе [Создание приложения на основе холста из шаблона в PowerApps](/powerapps/maker/canvas-apps/get-started-test-drive).</span><span class="sxs-lookup"><span data-stu-id="794ee-123">For more information, see [Create a canvas app from a template in PowerApps](/powerapps/maker/canvas-apps/get-started-test-drive).</span></span>  

<span data-ttu-id="794ee-124">После разработки и построения приложения можно поделиться им с коллегами.</span><span class="sxs-lookup"><span data-stu-id="794ee-124">When you have designed and built your app, you can share it with your colleagues.</span></span> <span data-ttu-id="794ee-125">Дополнительные сведения см. в разделе [Сохранение и публикация приложения на основе холста в PowerApps](/powerapps/maker/canvas-apps/save-publish-app).</span><span class="sxs-lookup"><span data-stu-id="794ee-125">For more information, see [Save and publish a canvas app in PowerApps](/powerapps/maker/canvas-apps/save-publish-app).</span></span>  

> [!NOTE]
> <span data-ttu-id="794ee-126">Если требуется подключиться к [!INCLUDE [prodshort](includes/prodshort.md)] On-Premises, необходимо выбрать соединитель **Business Central (локальная версия)** на шаге 3.</span><span class="sxs-lookup"><span data-stu-id="794ee-126">If you want to connect to [!INCLUDE [prodshort](includes/prodshort.md)] on-premises, then you must choose the **Business Central (on-premises)** connector in step 3.</span></span>  

## <a name="see-also"></a><span data-ttu-id="794ee-127">См. также</span><span class="sxs-lookup"><span data-stu-id="794ee-127">See Also</span></span>

[<span data-ttu-id="794ee-128">Создание приложения на основе холста из шаблона в PowerApps</span><span class="sxs-lookup"><span data-stu-id="794ee-128">Create a canvas app from a template in PowerApps</span></span>](/powerapps/maker/canvas-apps/get-started-test-drive)  
[<span data-ttu-id="794ee-129">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="794ee-129">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="794ee-130">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="794ee-130">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="794ee-131">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="794ee-131">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="794ee-132">Финансы</span><span class="sxs-lookup"><span data-stu-id="794ee-132">Finance</span></span>](finance.md)  
[<span data-ttu-id="794ee-133">Начальные сведения по разработке соединительных приложений для Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="794ee-133">Getting Started Developing Connect Apps for Dynamics 365 Business Central</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  
