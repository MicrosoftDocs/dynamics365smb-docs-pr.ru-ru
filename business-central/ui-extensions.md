---
title: Установка расширений для настройки Business Central | Документация Майкрософт
description: Узнайте о добавлении функций и настройке Business Central путем установки расширений.
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: app, add-in, manifest, customize
ms.date: 08/12/2020
ms.author: edupont
ms.openlocfilehash: 2011728e8e036442418c6a2d8b51477b45b02d1e
ms.sourcegitcommit: 43284728c34b72ad1984a516273dc80e4cdc99ab
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2020
ms.locfileid: "3765925"
---
# <a name="customizing-business-central-using-extensions"></a><span data-ttu-id="c77a9-103">Настройка Business Central с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="c77a9-103">Customizing Business Central Using Extensions</span></span>

<span data-ttu-id="c77a9-104">Вы можете изменить [!INCLUDE[d365fin](includes/d365fin_md.md)] за счет установки расширений, которые добавляют функциональность, изменяют поведение или, например, предоставляют доступ к новым интернет-службам.</span><span class="sxs-lookup"><span data-stu-id="c77a9-104">You can change [!INCLUDE[d365fin](includes/d365fin_md.md)] by installing extensions that add functionality, changes behavior, or gives you access to new online services, for example.</span></span>

> [!NOTE]
> <span data-ttu-id="c77a9-105">Чтобы установить расширения из AppSource или добавить расширения для каждого арендатора, у вас должны быть соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="c77a9-105">To install extensions from AppSource or add per-tenant extensions, you must have the right permissions.</span></span> <span data-ttu-id="c77a9-106">Вы должны быть либо участником группы пользователей D365 EXTENSION MGMT, либо у вас должен быть установлен набор разрешений D365 EXTENSION MGMT.</span><span class="sxs-lookup"><span data-stu-id="c77a9-106">You must either be a member of the D365 EXTENSION MGMT user group or you must have the D365 EXTENSION MGMT permission set.</span></span> <span data-ttu-id="c77a9-107">Если вы являетесь администратором, вы можете назначать группы пользователей и разрешения другим пользователям в вашей компании.</span><span class="sxs-lookup"><span data-stu-id="c77a9-107">If you are an administrator, you can assign user groups and permissions to other users in your company.</span></span><br /><br />
<span data-ttu-id="c77a9-108">Чтобы использовать функциональную возможность, предоставляемую расширением, такую как открытие страниц, запуск отчетов, выбор действий и т. п., необходимо назначить наборы разрешений, которые устанавливаются как часть расширения.</span><span class="sxs-lookup"><span data-stu-id="c77a9-108">To use the functionality that is provided by an extension, such as opening pages, running reports, selecting actions, and so on, you must be assigned the permission sets that are installed as part of the extension.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="c77a9-109">Загрузка расширений для каждого арендатора и установка расширения AppSource не поддерживаются через страницу **Управление расширениями** для локальных установок.</span><span class="sxs-lookup"><span data-stu-id="c77a9-109">The upload of per-tenant extensions and the installation of AppSource extensions is not supported through the **Extension Management** page for on-premise installations.</span></span>

<span data-ttu-id="c77a9-110">При первом запуске [!INCLUDE[d365fin](includes/d365fin_md.md)] некоторые расширения уже установлены.</span><span class="sxs-lookup"><span data-stu-id="c77a9-110">When you first launch [!INCLUDE[d365fin](includes/d365fin_md.md)], some extensions are already installed for you.</span></span> <span data-ttu-id="c77a9-111">Со временем вам станут доступны дополнительные расширения, и вы сможете выбрать, хотите ли вы использовать эти расширения.</span><span class="sxs-lookup"><span data-stu-id="c77a9-111">Over time, more extensions will be made available to you, and you can then choose if you want to use the extension or not.</span></span>

<span data-ttu-id="c77a9-112">Например, корпорация Майкрософт предлагает расширение, которое обеспечивает интеграцию с PayPal Payments Standard.</span><span class="sxs-lookup"><span data-stu-id="c77a9-112">For example, Microsoft provides an extension that provides integration with PayPal Payments Standard.</span></span> <span data-ttu-id="c77a9-113">Это расширение установлено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c77a9-113">This extension is installed by default.</span></span>
<span data-ttu-id="c77a9-114">Но если появится другое расширение, предлагающее интеграцию с другой службой платежей, вы можете установить его и выбрать службу платежей для использования.</span><span class="sxs-lookup"><span data-stu-id="c77a9-114">But if another extension is made available that offers integration with another payment service, you can install the new extension and then choose which of the two services to use.</span></span>  

<span data-ttu-id="c77a9-115">Управление расширениями осуществляется на странице **Управление расширениями**.</span><span class="sxs-lookup"><span data-stu-id="c77a9-115">You manage the extensions on the **Extension Management** page.</span></span> <span data-ttu-id="c77a9-116">Эта страница доступна с начальной страницы.</span><span class="sxs-lookup"><span data-stu-id="c77a9-116">You can access this page from Home.</span></span> <span data-ttu-id="c77a9-117">Также можно выбрать значок **Поиск страницы или отчета** ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать") в правом верхнем углу, ввести **Расширение**, а затем выбрать соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="c77a9-117">Alternatively, choose the **Search for Page or Report** icon ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") in the top right corner, enter **Extension**, and then choose the related link.</span></span> <span data-ttu-id="c77a9-118">Дополнительные сведения см. в разделе [Установка и удаление расширений](ui-extensions-install-uninstall.md).</span><span class="sxs-lookup"><span data-stu-id="c77a9-118">For more information, see [Installing and Uninstalling Extensions](ui-extensions-install-uninstall.md).</span></span>

> [!NOTE]  
> <span data-ttu-id="c77a9-119">Если вы считаете, что у вас должен быть доступ к расширению, но вы не можете найти его функциональные возможности, проверьте страницу **Управление расширениями**. Если расширение не указано в списке, вы можете установить его, как описано в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="c77a9-119">If you think you should have access to an extension but you cannot find its functionality, check the **Extension Management** page - if the extension is not listed there, you can install it as described in the following section.</span></span>  

> [!NOTE]  
> <span data-ttu-id="c77a9-120">Новые расширения не становятся доступными в AppSource сразу после объявления об обновлении.</span><span class="sxs-lookup"><span data-stu-id="c77a9-120">New extensions are not available in AppSource immediately after we announce an update.</span></span> <span data-ttu-id="c77a9-121">Следить за выходом новых расширений можно на сайте [AppSource.microsoft.com](https://go.microsoft.com/fwlink/?linkid=2081646).</span><span class="sxs-lookup"><span data-stu-id="c77a9-121">You can keep an eye out for the extensions at  [AppSource.microsoft.com](https://go.microsoft.com/fwlink/?linkid=2081646).</span></span>

## <a name="see-also"></a><span data-ttu-id="c77a9-122">См. также</span><span class="sxs-lookup"><span data-stu-id="c77a9-122">See Also</span></span>

[<span data-ttu-id="c77a9-123">Расширение Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="c77a9-123">Extending Dynamics 365 Business Central</span></span>](about-develop-extensions.md)  
[<span data-ttu-id="c77a9-124">Расширения для Business Central от других поставщиков</span><span class="sxs-lookup"><span data-stu-id="c77a9-124">Business Central Extensions by Other Providers</span></span>](ui-extensions-other.md)  
[<span data-ttu-id="c77a9-125">Настройка службы Envestnet Yodlee Bank Feeds</span><span class="sxs-lookup"><span data-stu-id="c77a9-125">Set Up the Envestnet Yodlee Bank Feeds Service</span></span>](bank-how-setup-bank-statement-service.md)  
[<span data-ttu-id="c77a9-126">Включение платежей клиентов через PayPal</span><span class="sxs-lookup"><span data-stu-id="c77a9-126">Enable Customer Payment Through PayPal</span></span>](sales-how-enable-payment-service-extensions.md)  
[<span data-ttu-id="c77a9-127">Миграция бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="c77a9-127">Migrating Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
[<span data-ttu-id="c77a9-128">Настройка расширения "Почтовые индексы Великобритании GetAddress.io"</span><span class="sxs-lookup"><span data-stu-id="c77a9-128">Setting Up the GetAddress.io UK Postal Code extension</span></span>](LocalFunctionality/UnitedKingdom/uk-setup-postal-code-service.md)  
<span data-ttu-id="c77a9-129">[Расширения [!INCLUDE[d365fin](includes/d365fin_md.md)] от других поставщиков](ui-extensions-other.md)</span><span class="sxs-lookup"><span data-stu-id="c77a9-129">[[!INCLUDE[d365fin](includes/d365fin_md.md)] Extensions by Other Providers](ui-extensions-other.md)</span></span>  
[<span data-ttu-id="c77a9-130">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="c77a9-130">Getting Started</span></span>](product-get-started.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
