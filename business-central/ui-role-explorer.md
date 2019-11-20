---
title: Просмотр страниц для роли и и навигация по ним | Документация Майкрософт
description: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 11/06/2019
ms.author: sgroespe
ms.openlocfilehash: c0cd3a1d72b466946f8efcd4774a1629c21af6d0
ms.sourcegitcommit: 2a6d629cf290645606356b714a77ef2872bdec64
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/07/2019
ms.locfileid: "2774799"
---
# <a name="finding-pages-with-the-role-explorer"></a><span data-ttu-id="81782-102">Поиск страниц с помощью обозревателя ролей</span><span class="sxs-lookup"><span data-stu-id="81782-102">Finding Pages with the Role Explorer</span></span>
<span data-ttu-id="81782-103">Вы можете получить обзор всех бизнес-функций, доступных для вашей роли, а также для других ролей.</span><span class="sxs-lookup"><span data-stu-id="81782-103">You can get an overview of all the business features that are available for your role, and for other roles if you go a step further.</span></span> <span data-ttu-id="81782-104">В следующей документации этот обзор функций называется *обозреватель ролей*.</span><span class="sxs-lookup"><span data-stu-id="81782-104">In the following documentation, this feature overview is referred to as the *role explorer*.</span></span>

<span data-ttu-id="81782-105">Каждый элемент в обозревателе ролей представляет собой действие, которое открывает страницу.</span><span class="sxs-lookup"><span data-stu-id="81782-105">Each element on the role explorer is an action that opens a page.</span></span> <span data-ttu-id="81782-106">Соответственно, вы также можете использовать обозреватель ролей в качестве средства навигации по [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="81782-106">Accordingly, you can also use the role explorer as a means to navigate in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

<span data-ttu-id="81782-107">Открыть обозреватель ролей можно из ролевого центра и со всех страниц списка, а также из окна **Что вы хотите сделать**.</span><span class="sxs-lookup"><span data-stu-id="81782-107">You can open the role explorer from the Role Center and all list pages and from the **Tell Me** window.</span></span>

- <span data-ttu-id="81782-108">В ролевом центре или на любой странице списка выберите кнопку ![Кнопка меню](media/ui_menu_button.png "Кнопка меню") справа от панели навигации или нажмите Shift+F12.</span><span class="sxs-lookup"><span data-stu-id="81782-108">On your Role Center or any list page, choose the ![Menu button](media/ui_menu_button.png "Menu button") button to the right of the navigation bar, or press Shift+F12.</span></span>
- <span data-ttu-id="81782-109">В окне **Что вы хотите сделать** выберите действие под ссылкой **обозревателем ролей** в нижней части окна.</span><span class="sxs-lookup"><span data-stu-id="81782-109">In the **Tell Me** window, choose the **exploring** action at the bottom.</span></span>

<span data-ttu-id="81782-110">Чтобы получить обзор бизнес-функций, доступных для всех других ролей, в дополнение к вашей собственной, выберите действие **Смотреть все** на странице, которая представляет обозреватель ролей.</span><span class="sxs-lookup"><span data-stu-id="81782-110">To get an overview of business feature that are available for all other roles, in addition to your own, choose the **Explore all** action on the page that presents the role explorer.</span></span>

> [!NOTE]
> <span data-ttu-id="81782-111">Только действия ролевого центра для профилей, где установлен флажок **Показать в обозревателе ролей**, будет отображаться в расширенной версии обозревателя ролей (показано с действием **Смотреть все**).</span><span class="sxs-lookup"><span data-stu-id="81782-111">Only Role Center actions for profiles where the **Show in Role Explorer** check box is selected will appear on the extended version of the role explorer (shown with the **Explore all** action).</span></span> <span data-ttu-id="81782-112">Дополнительные сведения см. в разделе [Управление профилями](admin-users-profiles-roles.md).</span><span class="sxs-lookup"><span data-stu-id="81782-112">For more information, see [Manage Profiles](admin-users-profiles-roles.md).</span></span>

## <a name="to-expandcollapse-nodes-on-the-role-explorer"></a><span data-ttu-id="81782-113">Чтобы развернуть/свернуть узлы в обозревателе ролей</span><span class="sxs-lookup"><span data-stu-id="81782-113">To expand/collapse nodes on the role explorer</span></span>
<span data-ttu-id="81782-114">Действия, которые открывают страницы, организованы под узлами, названными по названию функций или областей приложения.</span><span class="sxs-lookup"><span data-stu-id="81782-114">The actions that open pages are organized under nodes named after the features or application areas.</span></span> <span data-ttu-id="81782-115">Каждый узел можно свернуть или развернуть по отдельности, и вы можете свернуть/развернуть все узлы вместе.</span><span class="sxs-lookup"><span data-stu-id="81782-115">Each node can be collapsed or expanded individually and you can collapse/expand all nodes together.</span></span>

- <span data-ttu-id="81782-116">Чтобы развернуть/свернуть узел, выберите узел.</span><span class="sxs-lookup"><span data-stu-id="81782-116">To expand/collapse a node, choose the node.</span></span> <span data-ttu-id="81782-117">Это относится к узлам верхнего уровня и подузлам.</span><span class="sxs-lookup"><span data-stu-id="81782-117">This applies to top-level nodes and sub nodes.</span></span>
- <span data-ttu-id="81782-118">Чтобы развернуть/свернуть все узлы верхнего уровня на странице, выберите действие **Развернуть** или **Свернуть** в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="81782-118">To expand/collapse all top-level nodes on the page, choose the **Expand** or **Collapse** action in the top-right corner.</span></span>
- <span data-ttu-id="81782-119">Чтобы развернуть/свернуть узел верхнего уровня и все подчиненные узлы под ним, нажмите клавиши Ctrl+Shift, когда вы выбираете действие **Развернуть** или **Свернуть** в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="81782-119">To expand/collapse a top-level node and all sub nodes under it, press the Ctrl+Shift keys while you choose the **Expand** or **Collapse** action in the top-right corner.</span></span>

## <a name="see-also"></a><span data-ttu-id="81782-120">См. также</span><span class="sxs-lookup"><span data-stu-id="81782-120">See Also</span></span>
[<span data-ttu-id="81782-121">Поиск страниц и информации с помощью функции "Что вы хотите сделать"</span><span class="sxs-lookup"><span data-stu-id="81782-121">Finding Pages and Information with Tell Me</span></span>](ui-search.md)  
[<span data-ttu-id="81782-122">Управление профилями</span><span class="sxs-lookup"><span data-stu-id="81782-122">Manage Profiles</span></span>](admin-users-profiles-roles.md)  
<span data-ttu-id="81782-123">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="81782-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
