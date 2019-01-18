---
title: "Способы устранения или обхода неполадок | Microsoft Docs"
description: "Узнайте, как обойти возможные проблемы, возникающие в Accountant Hub для Dynamics 365."
author: edupont04
ms.service: dynamics365-accountant
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, troubleshoot
ms.date: 10/23/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 0ebd99e9097e4c701038f3b8be7a07d1e80a4b31
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="troubleshooting-include-d365acclongincludesd365acclongmdmd"></a><span data-ttu-id="b3be2-103">Устранение неполадок в [!INCLUDE [d365acc_long](includes/d365acc_long_md.md)]</span><span class="sxs-lookup"><span data-stu-id="b3be2-103">Troubleshooting [!INCLUDE [d365acc_long](includes/d365acc_long_md.md)]</span></span>
[!INCLUDE [d365fin_early_release](includes/d365fin_early_release.md.md)]

<span data-ttu-id="b3be2-104">Регистрация в [!INCLUDE [d365acc](includes/d365acc_md.md)] проста и выполняется очень быстро.</span><span class="sxs-lookup"><span data-stu-id="b3be2-104">Signing up for [!INCLUDE [d365acc](includes/d365acc_md.md)] is easy and can be done very quickly.</span></span> <span data-ttu-id="b3be2-105">Добавлять клиентов на панель мониторинга также очень просто, однако в этой статье рассматриваются проблемы, которые могут при этом возникнуть.</span><span class="sxs-lookup"><span data-stu-id="b3be2-105">Adding clients to the dashboard is also easy, but this article addresses issues that you may have on the way.</span></span>

## <a name="what-email-address-can-i-use-with-include-d365accincludesd365accmdmd"></a><span data-ttu-id="b3be2-106">Какой адрес электронной почты можно использовать с [!INCLUDE [d365acc](includes/d365acc_md.md)]?</span><span class="sxs-lookup"><span data-stu-id="b3be2-106">What email address can I use with [!INCLUDE [d365acc](includes/d365acc_md.md)]?</span></span>
<span data-ttu-id="b3be2-107">[!INCLUDE [d365acc](includes/d365acc_md.md)] требует, чтобы для регистрации использовался рабочий или учебный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b3be2-107">[!INCLUDE [d365acc](includes/d365acc_md.md)] requires that you use a work or school email address to sign up.</span></span> <span data-ttu-id="b3be2-108">[!INCLUDE [d365acc](includes/d365acc_md.md)] не поддерживает адреса электронной почты, предоставленные общедоступными сервисами электронной почты и поставщиками услуг связи.</span><span class="sxs-lookup"><span data-stu-id="b3be2-108">[!INCLUDE [d365acc](includes/d365acc_md.md)] does not support email addresses provided by consumer email services or telecommunication providers.</span></span> <span data-ttu-id="b3be2-109">К таким адресам относятся outlook.com, hotmail.com, gmail.com и т. д.</span><span class="sxs-lookup"><span data-stu-id="b3be2-109">This includes outlook.com, hotmail.com, gmail.com, and others.</span></span>  

<span data-ttu-id="b3be2-110">При попытке зарегистрироваться с личного адреса электронной почты вы получите сообщение о том, что нужно использовать рабочий или учебный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b3be2-110">If you try to sign up with a personal email address, you will get a message indicating to use a work or school email address.</span></span>  

## <a name="why-cant-i-connect-to-my-clients-data"></a><span data-ttu-id="b3be2-111">Почему я не могу подключиться к данным своего клиента?</span><span class="sxs-lookup"><span data-stu-id="b3be2-111">Why can't I connect to my client's data?</span></span>
<span data-ttu-id="b3be2-112">Причин может быть несколько, в том числе:</span><span class="sxs-lookup"><span data-stu-id="b3be2-112">There can be a couple of reasons, including the following:</span></span>

- <span data-ttu-id="b3be2-113">URL-адрес в поле **URL-адрес клиента** не является действительным</span><span class="sxs-lookup"><span data-stu-id="b3be2-113">The URL in the **Client URL** field is not valid</span></span>  

  <span data-ttu-id="b3be2-114">Перейдите в окно **Управление клиентами**, откройте клиента, к которому вам не удается подключиться, и выберите **Проверить URL-адрес клиента**.</span><span class="sxs-lookup"><span data-stu-id="b3be2-114">Go to **Manage Clients**, open the client that you cannot connect to, and then choose **Test Client URL**.</span></span>  
- <span data-ttu-id="b3be2-115">Компания клиента в настоящее время не подключена в сети, например из-за обновления</span><span class="sxs-lookup"><span data-stu-id="b3be2-115">The client's company is currently offline, for example if it being upgraded</span></span>

  <span data-ttu-id="b3be2-116">На панели мониторинга выберите пункт меню **Инструменты** и выберите **Проверить ошибки**.</span><span class="sxs-lookup"><span data-stu-id="b3be2-116">In your dashboard, choose the **Tools** menu item, and then choose **Check Errors**.</span></span> <span data-ttu-id="b3be2-117">Откроется список с техническими подробностями; если вы видите ошибки, возможно, имеет смысл связаться с администратором.</span><span class="sxs-lookup"><span data-stu-id="b3be2-117">This opens a list with technical details, so you might want to contact your administrator if you're seeing errors.</span></span> <span data-ttu-id="b3be2-118">Например, сообщение об ошибке "Сервер отклонил учетные данные клиента" может говорить о том, что у вас нет доступа.</span><span class="sxs-lookup"><span data-stu-id="b3be2-118">For example, the error message "The server has rejected the client credentials" suggests that you do not have access.</span></span>  
- <span data-ttu-id="b3be2-119">Вы не получили от своего клиента сообщение электронной почты с приглашением в [!INCLUDE [d365fin](includes/d365fin_md.md)] клиента, не перешли по ссылке в сообщении или не приняли приглашение</span><span class="sxs-lookup"><span data-stu-id="b3be2-119">You have not received an email from your client that invites them to their [!INCLUDE [d365fin](includes/d365fin_md.md)], or you did not open the link in the email, or you did not accept the invitation</span></span>

  <span data-ttu-id="b3be2-120">Вы должны перейти по ссылке в приглашении и согласиться с действиями, в результате которых вы будете добавлены в [!INCLUDE [d365fin](includes/d365fin_md.md)] клиента.</span><span class="sxs-lookup"><span data-stu-id="b3be2-120">You must open the link in the invitation and accept the steps that adds you to your client's [!INCLUDE [d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b3be2-121">Без этого доступа к данным клиента у вас не будет.</span><span class="sxs-lookup"><span data-stu-id="b3be2-121">Until then, you do not have access to their data.</span></span>  
- <span data-ttu-id="b3be2-122">У вас есть доступ не ко всем компаниям в [!INCLUDE [d365fin](includes/d365fin_md.md)] вашего клиента</span><span class="sxs-lookup"><span data-stu-id="b3be2-122">You do not have access to all companies in your client's [!INCLUDE [d365fin](includes/d365fin_md.md)]</span></span>

  <span data-ttu-id="b3be2-123">У вашего клиента может быть несколько филиалов или компаний в [!INCLUDE [d365fin](includes/d365fin_md.md)], и ваше приглашение может включать в себя не все эти компании.</span><span class="sxs-lookup"><span data-stu-id="b3be2-123">Your client can have multiple business units or companies in [!INCLUDE [d365fin](includes/d365fin_md.md)], and your invitation does not always include all companies.</span></span> <span data-ttu-id="b3be2-124">Поговорите со своим клиентом, чтобы убедиться, что у вас есть доступ ко всем компаниям, с которыми вы должны работать.</span><span class="sxs-lookup"><span data-stu-id="b3be2-124">Work with your client to make sure that you have access to the companies that the client wants you to work in.</span></span>  

## <a name="why-doesnt-the-data-refresh-in-my-dashboard"></a><span data-ttu-id="b3be2-125">Почему на моей панели мониторинга не обновляются данные?</span><span class="sxs-lookup"><span data-stu-id="b3be2-125">Why doesn't the data refresh in my dashboard?</span></span>
<span data-ttu-id="b3be2-126">Когда вы добавляете клиента или запрашиваете обновление данных, [!INCLUDE [d365acc](includes/d365acc_md.md)] извлекает данные.</span><span class="sxs-lookup"><span data-stu-id="b3be2-126">When you add a client or request a refresh of the data, [!INCLUDE [d365acc](includes/d365acc_md.md)] fetches the data.</span></span> <span data-ttu-id="b3be2-127">Однако вы должны сами обновить страницу: например, выбрать действие "Заново отобразить все компании", обновить страницу браузера, перейти с панели мониторинга на другую страницу и затем вернуться и т. п.</span><span class="sxs-lookup"><span data-stu-id="b3be2-127">But you must refresh the page yourself, such as choosing the "Redisplay all companies" action, refresh the browser page, navigate away from the dashboard and then back again, or similar.</span></span> <span data-ttu-id="b3be2-128">Это известная проблема, которую мы планируем устранить в одном из будущих обновлений.</span><span class="sxs-lookup"><span data-stu-id="b3be2-128">This is a known issue that we are working on improving in a later update.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b3be2-129">См. также</span><span class="sxs-lookup"><span data-stu-id="b3be2-129">See Also</span></span>
<span data-ttu-id="b3be2-130">[Начало работы с [!INCLUDE[d365acc](includes/d365acc_md.md)]](get-started.md)</span><span class="sxs-lookup"><span data-stu-id="b3be2-130">[Get Started with [!INCLUDE[d365acc](includes/d365acc_md.md)]](get-started.md)</span></span>  
<span data-ttu-id="b3be2-131">[Добавление клиентов на панель мониторинга в [!INCLUDE[d365acc](includes/d365acc_md.md)]](add-client.md)</span><span class="sxs-lookup"><span data-stu-id="b3be2-131">[Add Clients to Your Dashboard in [!INCLUDE[d365acc](includes/d365acc_md.md)]](add-client.md)</span></span>  

