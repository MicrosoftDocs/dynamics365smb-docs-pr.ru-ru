---
title: Оптимизация Outlook для входящего рабочего почтового ящика
description: Узнайте о том, что вы можете сделать, чтобы улучшить работу с "Входящие" для бизнеса в Microsoft Outlook.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Outlook, Microsoft 365, inbox, business inbox, WebView2, Edge, addin, add-in
ms.date: 05/12/2021
ms.author: jswymer
ms.openlocfilehash: 2fee1782057d0f45319e4d12d715c2e1e0d3d4a6
ms.sourcegitcommit: 61e279b253370cdf87b7bc1ee0f927e4f0521344
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "6064860"
---
# <a name="optimizing-outlook-for-your-business-inbox"></a><span data-ttu-id="6bf88-103">Оптимизация Outlook для входящего рабочего почтового ящика</span><span class="sxs-lookup"><span data-stu-id="6bf88-103">Optimizing Outlook for Your Business Inbox</span></span> 

<span data-ttu-id="6bf88-104">В этой статье рассказывается о том, что вы можете сделать, чтобы максимально использовать возможности "Входящие" для бизнеса в Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="6bf88-104">This article discusses things you can do to get the best possible experience with the Business Inbox in Microsoft Outlook.</span></span> 

## <a name="update-outlook"></a><span data-ttu-id="6bf88-105">Обновить Outlook</span><span class="sxs-lookup"><span data-stu-id="6bf88-105">Update Outlook</span></span>

<span data-ttu-id="6bf88-106">Обновите Outlook до версии 2012 или новее.</span><span class="sxs-lookup"><span data-stu-id="6bf88-106">Update to Outlook version 2012 or newer.</span></span>

> [!NOTE]
> <span data-ttu-id="6bf88-107">Если вы не можете обновить Outlook до версии 2012 или более поздней, убедитесь, что вы обновили хотя бы до версии 1905.</span><span class="sxs-lookup"><span data-stu-id="6bf88-107">If you are unable to update Outlook to version 2012 or later, make sure that you at least update to version 1905.</span></span> <span data-ttu-id="6bf88-108">Это предотвращает запуск надстройки Outlook с использованием устаревших компонентов Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="6bf88-108">This prevents the Outlook Add-in from running using legacy Internet Explorer components</span></span>

### <a name="how-to-check-your-version-of-outlook"></a><span data-ttu-id="6bf88-109">Как проверить свою версию Outlook</span><span class="sxs-lookup"><span data-stu-id="6bf88-109">How to check your version of Outlook</span></span>

<span data-ttu-id="6bf88-110">Независимо от того, используете ли вы Office 2019 или Microsoft 365, следуйте этому руководству службы поддержки Microsoft, чтобы узнать, какая у вас версия Outlook:</span><span class="sxs-lookup"><span data-stu-id="6bf88-110">Whether you use Office 2019 or Microsoft 365, follow this Microsoft Support guide to check which version of Outlook you have:</span></span>  

[<span data-ttu-id="6bf88-111">О Office: какую версию Office я использую?</span><span class="sxs-lookup"><span data-stu-id="6bf88-111">About Office: What version of Office am I using?</span></span>](https://support.microsoft.com/office/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19)

### <a name="how-to-update-outlook"></a><span data-ttu-id="6bf88-112">Как обновить Outlook</span><span class="sxs-lookup"><span data-stu-id="6bf88-112">How to update Outlook</span></span>

<span data-ttu-id="6bf88-113">Чтобы обновить Outlook до последней версии, следуйте этому руководству службы поддержки Microsoft или обратитесь к администратору:</span><span class="sxs-lookup"><span data-stu-id="6bf88-113">To update Outlook to the latest version, follow this Microsoft Support guide or contact your administrator:</span></span>

[<span data-ttu-id="6bf88-114">Установить обновления Office</span><span class="sxs-lookup"><span data-stu-id="6bf88-114">Install Office updates</span></span>](https://support.microsoft.com/office/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5)

## <a name="install-microsoft-edge-webview2"></a><span data-ttu-id="6bf88-115">Установите Microsoft Edge WebView2</span><span class="sxs-lookup"><span data-stu-id="6bf88-115">Install Microsoft Edge WebView2</span></span>

<span data-ttu-id="6bf88-116">Убедитесь, что Microsoft Edge WebView2 установлен на вашем устройстве.</span><span class="sxs-lookup"><span data-stu-id="6bf88-116">Ensure that Microsoft Edge WebView2 is installed on your device.</span></span>

### <a name="how-to-check-if-microsoft-edge-webview2-is-installed"></a><span data-ttu-id="6bf88-117">Как проверить, установлен ли Microsoft Edge WebView2</span><span class="sxs-lookup"><span data-stu-id="6bf88-117">How to check if Microsoft Edge WebView2 is installed</span></span> 

<span data-ttu-id="6bf88-118">Чтобы проверить, установлен ли Microsoft Edge WebView2 на компьютере, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="6bf88-118">To check if you have Microsoft Edge WebView2 installed on a computer, do the following steps:</span></span>

<span data-ttu-id="6bf88-119">В меню «Пуск»:</span><span class="sxs-lookup"><span data-stu-id="6bf88-119">From Start menu:</span></span>

1. <span data-ttu-id="6bf88-120">Выберите **Пуск** ![Запуск Windows](media/windows-start-icon.png "Значок &quot;Пуск Windows&quot;") > **Параметры** ![Параметры Windows](media/windows-settings-icon.png "Значок настроек Windows") > **Приложения и функции**.</span><span class="sxs-lookup"><span data-stu-id="6bf88-120">Choose **Start** ![Windows Start](media/windows-start-icon.png "Windows Start icon") > **Settings** ![Windows Settings](media/windows-settings-icon.png "Windows Settings icon") > **Apps & Features**.</span></span>
2. <span data-ttu-id="6bf88-121">Введите **WebView2** в поле поиска.</span><span class="sxs-lookup"><span data-stu-id="6bf88-121">In the search box, type **WebView2**.</span></span> <span data-ttu-id="6bf88-122">Если Microsoft Edge WebView2 установлен, вы увидите запись с названием **Среда выполнения Microsoft Edge WebView2**.</span><span class="sxs-lookup"><span data-stu-id="6bf88-122">If Microsoft Edge WebView2 is installed, you'll see an entry called **Microsoft Edge WebView2 Runtime**.</span></span>

<span data-ttu-id="6bf88-123">На панели управления:</span><span class="sxs-lookup"><span data-stu-id="6bf88-123">From Control Panel:</span></span>

1. <span data-ttu-id="6bf88-124">В поле поиска рядом с **Пуск** ![Запуск Windows](media/windows-start-icon.png "Значок &quot;Пуск Windows&quot;") введите **Панель управления**, а затем выберите результат.</span><span class="sxs-lookup"><span data-stu-id="6bf88-124">In the search box next to **Start** ![Windows Start](media/windows-start-icon.png "Windows Start icon"), type **Control Panel**, and then select the result.</span></span>
2. <span data-ttu-id="6bf88-125">Выберите **Программ** > **Программы и компоненты**.</span><span class="sxs-lookup"><span data-stu-id="6bf88-125">Choose **Programs** > **Programs and Features**.</span></span>
3. <span data-ttu-id="6bf88-126">Введите **WebView2** в поле поиска.</span><span class="sxs-lookup"><span data-stu-id="6bf88-126">In the search box, type **WebView2**.</span></span> <span data-ttu-id="6bf88-127">Если Microsoft Edge WebView2 установлен, вы увидите запись с названием **Среда выполнения Microsoft Edge WebView2**.</span><span class="sxs-lookup"><span data-stu-id="6bf88-127">If Microsoft Edge WebView2 is installed, you'll see an entry called **Microsoft Edge WebView2 Runtime**.</span></span>

### <a name="how-to-install-microsoft-edge-webview2"></a><span data-ttu-id="6bf88-128">Как установить Microsoft Edge WebView2</span><span class="sxs-lookup"><span data-stu-id="6bf88-128">How to install Microsoft Edge WebView2</span></span> 

1. <span data-ttu-id="6bf88-129">В браузере перейдите в [https://developer.microsoft.com/microsoft-edge/webview2/](https://developer.microsoft.com/microsoft-edge/webview2/).</span><span class="sxs-lookup"><span data-stu-id="6bf88-129">Using your browser, go to [https://developer.microsoft.com/microsoft-edge/webview2/](https://developer.microsoft.com/microsoft-edge/webview2/).</span></span>
2. <span data-ttu-id="6bf88-130">Выберите **Загрузить**.</span><span class="sxs-lookup"><span data-stu-id="6bf88-130">Choose **Download**.</span></span>
3. <span data-ttu-id="6bf88-131">Задайте **Выбрать архитектуру**, чтобы соответствовать вашей системе.</span><span class="sxs-lookup"><span data-stu-id="6bf88-131">Set **Select Architecture** to match your system.</span></span>
4. <span data-ttu-id="6bf88-132">Выберите **Загрузить**.</span><span class="sxs-lookup"><span data-stu-id="6bf88-132">Choose **Download**.</span></span>

> [!NOTE]
> <span data-ttu-id="6bf88-133">В вашей организации могут быть ограничения на то, какие компоненты могут быть установлены на вашем устройстве.</span><span class="sxs-lookup"><span data-stu-id="6bf88-133">Your organization may have restriction on which components can be installed on your device.</span></span> <span data-ttu-id="6bf88-134">Обратитесь за помощью к администратору.</span><span class="sxs-lookup"><span data-stu-id="6bf88-134">Contact your administrator for assistance.</span></span>

## <a name="use-a-supported-browser"></a><span data-ttu-id="6bf88-135">Использование поддерживаемого браузера</span><span class="sxs-lookup"><span data-stu-id="6bf88-135">Use a supported browser</span></span>

<span data-ttu-id="6bf88-136">Рассмотрите возможность использования Outlook для Интернета в одном из браузеров, поддерживаемых Business Central.</span><span class="sxs-lookup"><span data-stu-id="6bf88-136">Consider using Outlook for the Web in one of the browsers supported by Business Central.</span></span> <span data-ttu-id="6bf88-137">Список поддерживаемых браузеров см. в [Минимальные требования для использования Business Central](product-requirements.md#browsers).</span><span class="sxs-lookup"><span data-stu-id="6bf88-137">For a list of supported browsers, see [Minimum Requirements for Using Business Central](product-requirements.md#browsers).</span></span>

## <a name="see-also"></a><span data-ttu-id="6bf88-138">См. также</span><span class="sxs-lookup"><span data-stu-id="6bf88-138">See Also</span></span>

[<span data-ttu-id="6bf88-139">Подготовьтесь к ведению бизнеса</span><span class="sxs-lookup"><span data-stu-id="6bf88-139">Getting Ready for Doing Business</span></span>](ui-get-ready-business.md)  
[<span data-ttu-id="6bf88-140">Получение Business Central на моем мобильном устройстве</span><span class="sxs-lookup"><span data-stu-id="6bf88-140">Getting Business Central on my Mobile Device</span></span>](install-mobile-app.md)  
[<span data-ttu-id="6bf88-141">Отправка документов по электронной почте</span><span class="sxs-lookup"><span data-stu-id="6bf88-141">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
[<span data-ttu-id="6bf88-142">Финансы</span><span class="sxs-lookup"><span data-stu-id="6bf88-142">Finance</span></span>](finance.md)  
[<span data-ttu-id="6bf88-143">Продажи</span><span class="sxs-lookup"><span data-stu-id="6bf88-143">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="6bf88-144">Покупки</span><span class="sxs-lookup"><span data-stu-id="6bf88-144">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="6bf88-145">Минимальные требования для Outlook</span><span class="sxs-lookup"><span data-stu-id="6bf88-145">Minimum Requirements for Outlook</span></span>](product-requirements.md#outlook)  
[<span data-ttu-id="6bf88-146">Использование надстроек в Outlook в Интернете</span><span class="sxs-lookup"><span data-stu-id="6bf88-146">Using add-ins in Outlook on the web</span></span>](https://support.office.com/article/Using-Add-ins-in-Outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce?appver=OWB150)  


[!INCLUDE[footer-include](includes/footer-banner.md)]