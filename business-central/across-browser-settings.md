---
title: Настройка браузера
description: Описывается, как настроить браузеры для работы с решением Business Central и продуктами, которые с ним интегрируются.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, web client, troubleshooting, errors
ms.date: 01/08/2021
ms.author: jswymer
ms.openlocfilehash: 17b41653b1b5934e98c82ce8a35430e7b6a5c0d0
ms.sourcegitcommit: 1aac2c5f6773151c011dc1e4069c84d79fe5bda8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "4839962"
---
# <a name="setting-up-and-troubleshooting-your-browser-to-work-with-business-central-web-client"></a><span data-ttu-id="241ba-103">Настройка и устранение неполадок браузера для работы с веб-клиентом Business Central</span><span class="sxs-lookup"><span data-stu-id="241ba-103">Setting Up and Troubleshooting Your Browser to Work With Business Central Web Client</span></span>

<span data-ttu-id="241ba-104">В этой статье объясняется, как настроить браузер так, чтобы [!INCLUDE[web_client](includes/web_client.md)] и все его функции работали правильно.</span><span class="sxs-lookup"><span data-stu-id="241ba-104">This article explains how to set up your browser so that the [!INCLUDE[web_client](includes/web_client.md)] and all its features work properly.</span></span> <span data-ttu-id="241ba-105">Прочтите эту статью, если у вас возникли проблемы с открытием [!INCLUDE[web_client](includes/web_client.md)], потому что некоторые проблемы могут быть вызваны настройками вашего браузера.</span><span class="sxs-lookup"><span data-stu-id="241ba-105">Read this article if you're having problems opening the [!INCLUDE[web_client](includes/web_client.md)], because some problems may be caused by your browser's settings.</span></span>

<span data-ttu-id="241ba-106">В статье подробно рассказывается о настройке Microsoft Edge, но требования для JavaScript, файлов cookie и всплывающих окон одинаковы для всех поддерживаемых браузеров.</span><span class="sxs-lookup"><span data-stu-id="241ba-106">The article provides details for setting up Microsoft Edge, but the requirements for JavaScript, cookies, and pop-ups are the same for all supported browsers.</span></span> <span data-ttu-id="241ba-107">Для других браузеров обратитесь к инструкциям производителя.</span><span class="sxs-lookup"><span data-stu-id="241ba-107">For other browsers, refer to the instructions provided by the manufacturer.</span></span>  

## <a name="use-a-supported-browser"></a><span data-ttu-id="241ba-108">Использование поддерживаемого браузера</span><span class="sxs-lookup"><span data-stu-id="241ba-108">Use a supported browser</span></span>

<span data-ttu-id="241ba-109">Убедитесь, что вы используете один из поддерживаемых браузеров.</span><span class="sxs-lookup"><span data-stu-id="241ba-109">Make sure to use a one of the supported browsers.</span></span> <span data-ttu-id="241ba-110">См. раздел [Минимальные требования для использования Business Central](product-requirements.md#recommended-browsers).</span><span class="sxs-lookup"><span data-stu-id="241ba-110">See [Minimum Requirements for Using Business Central](product-requirements.md#recommended-browsers).</span></span>  

## <a name="allow-javascript-from-business-central"></a><span data-ttu-id="241ba-111">Разрешение JavaScript из Business Central</span><span class="sxs-lookup"><span data-stu-id="241ba-111">Allow JavaScript from Business Central</span></span>

<span data-ttu-id="241ba-112">*Проблема:*</span><span class="sxs-lookup"><span data-stu-id="241ba-112">*Problem:*</span></span>

<span data-ttu-id="241ba-113">Если браузер не поддерживает JavaScript, вы увидите сообщение **NotSupported/DisabledJavaScript** в адресной строке и сообщение **Ошибка HTTP 404.0 — не найдено** при попытке открыть [!INCLUDE[prod_short](includes/prod_short.md)], и</span><span class="sxs-lookup"><span data-stu-id="241ba-113">If the browser doesn't allow JavaScript, you'll see **NotSupported/DisabledJavaScript** in the address bar and an **HTTP Error 404.0 - Not Found** message when you try to open [!INCLUDE[prod_short](includes/prod_short.md)], and the</span></span> 

<!-- http://localhost:8080/NotSupported/DisabledJavaScript HTTP Error 404.0 - Not Found
The resource you are looking for has been removed, had its name changed, or is temporarily unavailable. -->

<span data-ttu-id="241ba-114">*Исправление:*</span><span class="sxs-lookup"><span data-stu-id="241ba-114">*Fix:*</span></span>

1. <span data-ttu-id="241ba-115">В Microsoft Edge перейдите к пункту **Настройки** > **Файлы cookie и разрешения сайтов** > **JavaScript**.</span><span class="sxs-lookup"><span data-stu-id="241ba-115">In Microsoft Edge, go to **Settings** > **Cookies and site permissions** > **JavaScript**.</span></span>
2. <span data-ttu-id="241ba-116">Выполните один из следующих шагов.</span><span class="sxs-lookup"><span data-stu-id="241ba-116">Do one of the following steps.</span></span> <span data-ttu-id="241ba-117">Выберите шаг, рекомендованный вашей организацией:</span><span class="sxs-lookup"><span data-stu-id="241ba-117">Choose the step that is recommended by your organization:</span></span>

    - <span data-ttu-id="241ba-118">Переместите выключатель **Разрешено** влево (Выкл.).</span><span class="sxs-lookup"><span data-stu-id="241ba-118">Move the **Allowed** toggle to the left (Off).</span></span> <span data-ttu-id="241ba-119">Затем выберите **Добавить** и введите адрес (URL) для [!INCLUDE[prod_short](includes/prod_short.md)] в поле **Сайт**.</span><span class="sxs-lookup"><span data-stu-id="241ba-119">Then, select **Add** and type the address (URL) for [!INCLUDE[prod_short](includes/prod_short.md)] in the **Site** box.</span></span> <span data-ttu-id="241ba-120">Выберите **Добавить**, когда будете готовы.</span><span class="sxs-lookup"><span data-stu-id="241ba-120">Select **Add** when done.</span></span>
    - <span data-ttu-id="241ba-121">Переместите выключатель **Разрешено** вправо (Вкл.).</span><span class="sxs-lookup"><span data-stu-id="241ba-121">Move the **Allowed** toggle to the right (On).</span></span>

## <a name="allow-cookies-from-business-central"></a><span data-ttu-id="241ba-122">Разрешение файлов cookie из Business Central</span><span class="sxs-lookup"><span data-stu-id="241ba-122">Allow cookies from Business Central</span></span>

<span data-ttu-id="241ba-123">*Проблема:*</span><span class="sxs-lookup"><span data-stu-id="241ba-123">*Problem:*</span></span>

<span data-ttu-id="241ba-124">Если браузер не разрешает файлы cookie, вы получите следующую ошибку:</span><span class="sxs-lookup"><span data-stu-id="241ba-124">If the browser doesn't allow cookies, you'll get the following error:</span></span>

<span data-ttu-id="241ba-125">**К сожалению, страница не найдена. Пожалуйста, проверьте адрес и попробуйте снова.**</span><span class="sxs-lookup"><span data-stu-id="241ba-125">**Sorry, the page could not be found. Please check the address and try again.**</span></span> 

<span data-ttu-id="241ba-126">*Исправление:*</span><span class="sxs-lookup"><span data-stu-id="241ba-126">*Fix:*</span></span>

1. <span data-ttu-id="241ba-127">В Microsoft Edge перейдите к пункту **Настройки** > **Файлы cookie и разрешения сайтов** > **Файлы cookie и данные сайта**.</span><span class="sxs-lookup"><span data-stu-id="241ba-127">In Microsoft Edge, go to **Settings** > **Cookies and site permissions** > **Cookies and site data**.</span></span>
2. <span data-ttu-id="241ba-128">Переместите выключатель **Разрешить сайтам сохранять и читать данные файлов cookie** вправо (Вкл.).</span><span class="sxs-lookup"><span data-stu-id="241ba-128">Move the **Allow sites to save and read cookie data** toggle to the right (On).</span></span>  

## <a name="allow-pop-ups-from-business-central"></a><a name="popup"></a><span data-ttu-id="241ba-129">Разрешение всплывающих окон из Business Central</span><span class="sxs-lookup"><span data-stu-id="241ba-129">Allow pop-ups from Business Central</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="241ba-130">интегрируется с несколькими продуктами.</span><span class="sxs-lookup"><span data-stu-id="241ba-130">integrates with several products.</span></span> <span data-ttu-id="241ba-131">В некоторых случаях, например, с Microsoft Teams, [!INCLUDE[prod_short](includes/prod_short.md)] открывается во всплывающем окне внутри продукта.</span><span class="sxs-lookup"><span data-stu-id="241ba-131">In some cases, like with Microsoft Teams, [!INCLUDE[prod_short](includes/prod_short.md)] opens, or "pop-ups", within the product.</span></span> <span data-ttu-id="241ba-132">Эта возможность требует, чтобы ваш браузер разрешал всплывающие окна из [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="241ba-132">This capability requires that your browser allows pop-ups from [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

<span data-ttu-id="241ba-133">*Проблема:*</span><span class="sxs-lookup"><span data-stu-id="241ba-133">*Problem:*</span></span>

<span data-ttu-id="241ba-134">Если всплывающие окна для [!INCLUDE[prod_short](includes/prod_short.md)] блокируются, вы получите сообщение, подобное следующему:</span><span class="sxs-lookup"><span data-stu-id="241ba-134">If pop-ups for [!INCLUDE[prod_short](includes/prod_short.md)] are being blocked, you get a message similar to the following message:</span></span>

<span data-ttu-id="241ba-135">**Что-то пошло не так. Ваш браузер может блокировать всплывающие окна, необходимые Business Central.**</span><span class="sxs-lookup"><span data-stu-id="241ba-135">**Something went wrong. Your browser may be blocking pop-ups needed by Business Central.**</span></span>

<!--
Something went wrong
Your browser may be blocking pop-ups needed by Business Central.

Change your browser settings to allow pop-ups or allow this for trusted domains, then try again.
If these settings are managed for your organization, you should contact your administrator for assistance.

Try again
-->
<span data-ttu-id="241ba-136">*Исправление:*</span><span class="sxs-lookup"><span data-stu-id="241ba-136">*Fix:*</span></span>

1. <span data-ttu-id="241ba-137">В Microsoft Edge перейдите к пункту **Настройки** > **Файлы cookie и разрешения сайтов** > **Всплывающие окна и перенаправления**.</span><span class="sxs-lookup"><span data-stu-id="241ba-137">In Microsoft Edge, go to **Settings** > **Cookies and site permissions** > **Pop-ups and redirects**.</span></span>
2. <span data-ttu-id="241ba-138">Переместите выключатель **Блокировать** вправо (Вкл.).</span><span class="sxs-lookup"><span data-stu-id="241ba-138">Move the **Blocked** toggle to the right (On).</span></span>
3. <span data-ttu-id="241ba-139">Выберите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="241ba-139">Select **Add**.</span></span> <span data-ttu-id="241ba-140">В поле **Сайт** введите `https://businesscentral.dynamics.com`, затем выберите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="241ba-140">In the **Site** box, type `https://businesscentral.dynamics.com`, then select **Add**.</span></span>

## <a name="see-also"></a><span data-ttu-id="241ba-141">См. также</span><span class="sxs-lookup"><span data-stu-id="241ba-141">See Also</span></span>

[<span data-ttu-id="241ba-142">Устранение неполадок Teams</span><span class="sxs-lookup"><span data-stu-id="241ba-142">Troubleshooting Teams</span></span>](admin-teams-troubleshooting.md)  