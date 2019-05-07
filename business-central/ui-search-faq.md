---
title: Вопросы и ответы о функции "Что вы хотите сделать" | Документы Майкрософт
description: Эта статья содержит ответы на вопросы, которые наши партнеры и клиенты часто задают по поводу функции "Что вы хотите сделать".
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: find
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: d04f78b31b9fb0403201cb9e5cb1f98f1ef935e1
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "937585"
---
# <a name="tell-me-faq"></a><span data-ttu-id="a7cc7-103">Вопросы и ответы о функции "Что вы хотите сделать"</span><span class="sxs-lookup"><span data-stu-id="a7cc7-103">Tell Me FAQ</span></span>
<span data-ttu-id="a7cc7-104">В этом разделе приводятся ответы на вопросы, которые опытные пользователи часто задают о новой функции "Что вы хотите сделать", которая заменила предыдущую функцию поиска страниц, известную под названием **Поиск страниц и отчетов**.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-104">This topic answers questions that our advanced users often ask about the new Tell Me feature, which has replaced the previous Page Search feature known as **Find Pages and Reports**.</span></span>

### <a name="are-all-actions-from-my-current-page-discoverable-in-tell-me"></a><span data-ttu-id="a7cc7-105">Все ли действия из текущей страницы могут быть обнаружены в функции "Что вы хотите сделать"?</span><span class="sxs-lookup"><span data-stu-id="a7cc7-105">Are all actions from my current page discoverable in Tell Me?</span></span>
<span data-ttu-id="a7cc7-106">Нет.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-106">No.</span></span> <span data-ttu-id="a7cc7-107">Действия в частях, таких как часть строк продажи или информационные панели, не отображаются в функции "Что вы хотите сделать".</span><span class="sxs-lookup"><span data-stu-id="a7cc7-107">Actions in parts, such as the Sales Lines part or FactBoxes, are not displayed in Tell Me.</span></span>

### <a name="are-the-results-in-tell-me-filtered-by-permissions"></a><span data-ttu-id="a7cc7-108">Фильтруются ли результаты функции "Что вы хотите сделать" по правам доступа?</span><span class="sxs-lookup"><span data-stu-id="a7cc7-108">Are the results in Tell Me filtered by permissions?</span></span>
<span data-ttu-id="a7cc7-109">Если пользователь не имеет AccessByPermissions, такие действия не отображаются.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-109">If the user does not have AccessByPermissions then actions are not displayed.</span></span> <span data-ttu-id="a7cc7-110">Однако страниц и отчеты появляются в результатах, но пользователю необходимо имеет право на получение доступа к ним.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-110">However, pages and reports appear in the results but require that the user has permission to access them.</span></span> <span data-ttu-id="a7cc7-111">Показывается сообщение, если пользователь не имеет прав на просмотр объекта.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-111">A message will display if the user does not have permission to view the object.</span></span>

### <a name="does-tell-me-display-content-from-my-customizations-or-installed-third-party-extensions"></a><span data-ttu-id="a7cc7-112">Показывает ли функция "Что вы хотите сделать" содержимое из моих настроек или установленных расширений третьих сторон?</span><span class="sxs-lookup"><span data-stu-id="a7cc7-112">Does Tell Me display content from my customizations or installed third-party extensions?</span></span>
<span data-ttu-id="a7cc7-113">Действия, страницы и отчеты, которые происходят из расширений, охватываются функцией "Что вы хотите сделать", но настроенная справочная документация не охватывается.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-113">Actions, pages, and reports that originate from extensions are picked up by Tell Me, but custom help documentation is not.</span></span> <span data-ttu-id="a7cc7-114">Технические сведения о том, как сделать настроенные страницы и отчеты обнаруживаемыми, см. в разделе [Добавление страниц и отчетов в поиск](/dynamics365/business-central/dev-itpro/developer/devenv-al-menusuite-functionality).</span><span class="sxs-lookup"><span data-stu-id="a7cc7-114">For technical information about how to make custom pages and reports discoverable, see [Adding Pages and Reports to Search](/dynamics365/business-central/dev-itpro/developer/devenv-al-menusuite-functionality).</span></span>

### <a name="what-makes-this-different-from-what-was-previously-known-as-page-search"></a><span data-ttu-id="a7cc7-115">Чем эта функция отличается от ранее известной функции поиска страниц?</span><span class="sxs-lookup"><span data-stu-id="a7cc7-115">What makes this different from what was previously known as Page Search?</span></span>
<span data-ttu-id="a7cc7-116">Поиск страниц эволюционировал в функцию "Что вы хотите сделать", чтобы помочь работать быстрее.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-116">Page Search has evolved into Tell Me to help you get work done quickly.</span></span> <span data-ttu-id="a7cc7-117">Поиск страниц мог помочь только переходить к страницам или отчетам.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-117">Page Search could only help you navigate to pages or reports.</span></span> <span data-ttu-id="a7cc7-118">На техническом уровне функция "Что вы хотите сделать" больше не основывается на концепции MenuSuite.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-118">At a technical level, Tell Me is no longer based on the legacy MenuSuite concept.</span></span>

### <a name="i-use-on-premises-included365finincludesd365finmdmd-does-that-include-tell-me"></a><span data-ttu-id="a7cc7-119">Я использую локальную версию [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a7cc7-119">I use on-premises [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="a7cc7-120">Она включает функцию "Что вы хотите сделать"?</span><span class="sxs-lookup"><span data-stu-id="a7cc7-120">Does that include Tell Me?</span></span>
<span data-ttu-id="a7cc7-121">Можно использовать функцию "Что вы хотите сделать" в веб-клиенте локальной версии для поиска действий, страниц и отчетов, но не документации, или приложения и консультативные услуги в AppSource.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-121">You can use Tell Me in the on-premises Web Client to find actions, pages, and reports, but not documentation, or apps and consulting services on AppSource.</span></span> <span data-ttu-id="a7cc7-122">Пользователи, подключающиеся к [!INCLUDE[d365fin](includes/d365fin_md.md)] из клиента Dynamics NAV, продолжат использовать поиск страниц.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-122">Users connecting to [!INCLUDE[d365fin](includes/d365fin_md.md)] from the Dynamics NAV client continue to use Page Search.</span></span>

### <a name="is-tell-me-available-for-all-form-factors"></a><span data-ttu-id="a7cc7-123">Доступна ли функция "Что вы хотите сделать" для всех форм-факторов?</span><span class="sxs-lookup"><span data-stu-id="a7cc7-123">Is Tell Me available for all form factors?</span></span>
<span data-ttu-id="a7cc7-124">Функция "Что вы хотите сделать" доступна только в веб-клиента или в приложении рабочего стола Windows.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-124">Tell Me is only available in the Web Client or Windows desktop app.</span></span>

### <a name="are-the-documentation-results-available-in-any-language"></a><span data-ttu-id="a7cc7-125">Результаты документации доступны на любом языке?</span><span class="sxs-lookup"><span data-stu-id="a7cc7-125">Are the documentation results available in any language?</span></span>
<span data-ttu-id="a7cc7-126">Статьи справки отображаются на языке, указанном в пункте **Мои настройки**, если справки доступна на этом языке.</span><span class="sxs-lookup"><span data-stu-id="a7cc7-126">The help articles display in the language you have specified in **My Settings**, if help is available in that language.</span></span>

## <a name="see-also"></a><span data-ttu-id="a7cc7-127">См. также</span><span class="sxs-lookup"><span data-stu-id="a7cc7-127">See Also</span></span>  
[<span data-ttu-id="a7cc7-128">Обнаружение функций и информации</span><span class="sxs-lookup"><span data-stu-id="a7cc7-128">Finding Features and Information</span></span>](ui-search.md)
