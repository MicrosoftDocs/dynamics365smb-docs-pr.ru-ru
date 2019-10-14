---
title: Вопросы и ответы о функции "Что вы хотите сделать" | Документация Майкрософт
description: Эта статья содержит ответы на вопросы, которые наши партнеры и клиенты часто задают по поводу функции "Что вы хотите сделать".
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: find
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: 9fac8d546a24839ebaa0719d721d886c03001521
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2310760"
---
# <a name="tell-me-faq"></a><span data-ttu-id="fe1ed-103">Вопросы и ответы о функции "Что вы хотите сделать"</span><span class="sxs-lookup"><span data-stu-id="fe1ed-103">Tell Me FAQ</span></span>
<span data-ttu-id="fe1ed-104">В этой теме содержатся ответы на вопросы, которые часто задают наши продвинутые пользователи о функции "Что вы хотите сделать"</span><span class="sxs-lookup"><span data-stu-id="fe1ed-104">This topic answers questions that our advanced users often ask about the Tell Me feature.</span></span>

### <a name="are-all-actions-from-my-current-page-discoverable-in-tell-me"></a><span data-ttu-id="fe1ed-105">Все ли действия из текущей страницы могут быть обнаружены в функции "Что вы хотите сделать"?</span><span class="sxs-lookup"><span data-stu-id="fe1ed-105">Are all actions from my current page discoverable in Tell Me?</span></span>
<span data-ttu-id="fe1ed-106">Нет.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-106">No.</span></span> <span data-ttu-id="fe1ed-107">Действия в частях, таких как часть строк продажи или информационные панели, не отображаются в функции "Что вы хотите сделать".</span><span class="sxs-lookup"><span data-stu-id="fe1ed-107">Actions in parts, such as the Sales Lines part or FactBoxes, are not displayed in Tell Me.</span></span>

### <a name="are-the-results-in-tell-me-filtered-by-permissions"></a><span data-ttu-id="fe1ed-108">Фильтруются ли результаты функции "Что вы хотите сделать" по правам доступа?</span><span class="sxs-lookup"><span data-stu-id="fe1ed-108">Are the results in Tell Me filtered by permissions?</span></span>
<span data-ttu-id="fe1ed-109">Если пользователь не имеет AccessByPermissions, такие действия не отображаются.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-109">If the user does not have AccessByPermissions then actions are not displayed.</span></span> <span data-ttu-id="fe1ed-110">Однако страниц и отчеты появляются в результатах, но пользователю необходимо имеет право на получение доступа к ним.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-110">However, pages and reports appear in the results but require that the user has permission to access them.</span></span> <span data-ttu-id="fe1ed-111">Показывается сообщение, если пользователь не имеет прав на просмотр объекта.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-111">A message will display if the user does not have permission to view the object.</span></span>

### <a name="does-tell-me-display-content-from-my-customizations-or-installed-third-party-extensions"></a><span data-ttu-id="fe1ed-112">Показывает ли функция "Что вы хотите сделать" содержимое из моих настроек или установленных расширений третьих сторон?</span><span class="sxs-lookup"><span data-stu-id="fe1ed-112">Does Tell Me display content from my customizations or installed third-party extensions?</span></span>
<span data-ttu-id="fe1ed-113">Действия, страницы и отчеты, которые происходят из расширений, охватываются функцией "Что вы хотите сделать", но настроенная справочная документация не охватывается.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-113">Actions, pages, and reports that originate from extensions are picked up by Tell Me, but custom help documentation is not.</span></span> <span data-ttu-id="fe1ed-114">Технические сведения о том, как сделать настроенные страницы и отчеты обнаруживаемыми, см. в разделе [Добавление страниц и отчетов в поиск](/dynamics365/business-central/dev-itpro/developer/devenv-al-menusuite-functionality).</span><span class="sxs-lookup"><span data-stu-id="fe1ed-114">For technical information about how to make custom pages and reports discoverable, see [Adding Pages and Reports to Search](/dynamics365/business-central/dev-itpro/developer/devenv-al-menusuite-functionality).</span></span>

### <a name="what-makes-this-different-from-what-was-previously-known-as-page-search"></a><span data-ttu-id="fe1ed-115">Чем эта функция отличается от ранее известной функции поиска страниц?</span><span class="sxs-lookup"><span data-stu-id="fe1ed-115">What makes this different from what was previously known as Page Search?</span></span>
<span data-ttu-id="fe1ed-116">Поиск страниц эволюционировал в функцию "Что вы хотите сделать", чтобы помочь работать быстрее.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-116">Page Search has evolved into Tell Me to help you get work done quickly.</span></span> <span data-ttu-id="fe1ed-117">Поиск страниц мог помочь только переходить к страницам или отчетам.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-117">Page Search could only help you navigate to pages or reports.</span></span> <span data-ttu-id="fe1ed-118">На техническом уровне функция "Что вы хотите сделать" больше не основывается на концепции MenuSuite.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-118">At a technical level, Tell Me is no longer based on the legacy MenuSuite concept.</span></span>

### <a name="i-use-on-premises-included365finincludesd365fin_mdmd-does-that-include-tell-me"></a><span data-ttu-id="fe1ed-119">Я использую локальную версию [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="fe1ed-119">I use on-premises [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="fe1ed-120">Она включает функцию "Что вы хотите сделать"?</span><span class="sxs-lookup"><span data-stu-id="fe1ed-120">Does that include Tell Me?</span></span>
<span data-ttu-id="fe1ed-121">Можно использовать функцию "Что вы хотите сделать" в веб-клиенте локальной версии для поиска действий, страниц и отчетов, но не документации, или приложения и консультативные услуги в AppSource.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-121">You can use Tell Me in the on-premises Web Client to find actions, pages, and reports, but not documentation, or apps and consulting services on AppSource.</span></span>

### <a name="is-tell-me-available-for-all-form-factors"></a><span data-ttu-id="fe1ed-122">Доступна ли функция "Что вы хотите сделать" для всех форм-факторов?</span><span class="sxs-lookup"><span data-stu-id="fe1ed-122">Is Tell Me available for all form factors?</span></span>
<span data-ttu-id="fe1ed-123">Функция "Что вы хотите сделать" доступна только в веб-клиента или в приложении рабочего стола Windows.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-123">Tell Me is only available in the Web Client or Windows desktop app.</span></span>

### <a name="are-the-documentation-results-available-in-any-language"></a><span data-ttu-id="fe1ed-124">Результаты документации доступны на любом языке?</span><span class="sxs-lookup"><span data-stu-id="fe1ed-124">Are the documentation results available in any language?</span></span>
<span data-ttu-id="fe1ed-125">Статьи справки отображаются на языке, указанном в пункте **Мои настройки**, если справки доступна на этом языке.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-125">The help articles display in the language you have specified in **My Settings**, if help is available in that language.</span></span>

### <a name="why-dont-i-see-a-bookmark-icon-for-my-search-results"></a><span data-ttu-id="fe1ed-126">Почему я не вижу значка закладки для результатов поиска?</span><span class="sxs-lookup"><span data-stu-id="fe1ed-126">Why don't I see a bookmark icon for my search results?</span></span>
<span data-ttu-id="fe1ed-127">Значок закладки не отображается в окне "Что вы хотите сделать", когда для роли пользователя отключена персонализация.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-127">The bookmark icon is not displayed in the Tell Me window when personalization is disabled for a user role.</span></span>

### <a name="is-the-bookmark-icon-available-for-reports"></a><span data-ttu-id="fe1ed-128">Доступен ли значок закладки для отчетов?</span><span class="sxs-lookup"><span data-stu-id="fe1ed-128">Is the bookmark icon available for reports?</span></span>
<span data-ttu-id="fe1ed-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="fe1ed-129">No.</span></span> <span data-ttu-id="fe1ed-130">Добавить в закладки можно только ссылку на страницу или результаты поиска, которые отображаются в разделе **Страницы и задачи** окна "Что вы хотите сделать".</span><span class="sxs-lookup"><span data-stu-id="fe1ed-130">You can only bookmark a link to a page or any search results that are displayed in the **Pages and Tasks** section of the Tell Me window.</span></span>


## <a name="see-also"></a><span data-ttu-id="fe1ed-131">См. также</span><span class="sxs-lookup"><span data-stu-id="fe1ed-131">See Also</span></span>  
[<span data-ttu-id="fe1ed-132">Сохранение и персонализация представлений списков</span><span class="sxs-lookup"><span data-stu-id="fe1ed-132">Save and Personalize List Views</span></span>](ui-views.md)  
[<span data-ttu-id="fe1ed-133">Поиск страниц и информации с помощью функции "Что вы хотите сделать"</span><span class="sxs-lookup"><span data-stu-id="fe1ed-133">Finding Pages and Information with Tell Me</span></span>](ui-search.md)  
[<span data-ttu-id="fe1ed-134">Поиск страниц из обзора функций</span><span class="sxs-lookup"><span data-stu-id="fe1ed-134">Finding Pages from a Feature Overview</span></span>](ui-role-explorer.md)
