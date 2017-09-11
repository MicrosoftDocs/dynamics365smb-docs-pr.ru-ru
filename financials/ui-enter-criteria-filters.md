---
title: "Определение критериев поиска в фильтрах | Документы Майкрософт"
description: "Описывается порядок работы с фильтрами, например с быстрым фильтром, для уточнения результатов поиска данных."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 86ca45493081d9dbd229548f7c560e1df4e1c7c3
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="entering-criteria-in-filters"></a><span data-ttu-id="0d05b-103">Ввод критериев в фильтрах</span><span class="sxs-lookup"><span data-stu-id="0d05b-103">Entering Criteria in Filters</span></span>
<span data-ttu-id="0d05b-104">Если необходимо выполнить поиск данных, таких как название клиента, адреса или товарные группы, вводятся критерии.</span><span class="sxs-lookup"><span data-stu-id="0d05b-104">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="0d05b-105">В критериях поиска можно использовать все цифры и буквы, которые вводятся в соответствующие поля.</span><span class="sxs-lookup"><span data-stu-id="0d05b-105">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="0d05b-106">Кроме того, для дополнительной фильтрации результатов можно использовать специальные символы.</span><span class="sxs-lookup"><span data-stu-id="0d05b-106">In addition, you can use special symbols to further filter the results.</span></span>

## <a name="searching-using-the-quick-filter"></a><span data-ttu-id="0d05b-107">Поиск с помощью экспресс-фильтра</span><span class="sxs-lookup"><span data-stu-id="0d05b-107">Searching using the Quick Filter</span></span>
<span data-ttu-id="0d05b-108">Вы можете добавить фильтры на все страницы с помощью экспресс-фильтра.</span><span class="sxs-lookup"><span data-stu-id="0d05b-108">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="0d05b-109">Экспресс-фильтр включается при выборе значка лупы в правом верхнем углу страницы.</span><span class="sxs-lookup"><span data-stu-id="0d05b-109">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="0d05b-110">Данный тип фильтра используется для быстрого ввода критериев.</span><span class="sxs-lookup"><span data-stu-id="0d05b-110">This filtering type is used for a fast entry of criteria.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="0d05b-111">Экспресс-фильтр обеспечивает удобный доступ к фильтруемым данным путем ввода простого текста, а также множество вариантов указания критериев поиска.</span><span class="sxs-lookup"><span data-stu-id="0d05b-111">The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="0d05b-112">В зависимости от того, введен ли обычный текст или текст с символами, поведение экспресс-фильтра отличается.</span><span class="sxs-lookup"><span data-stu-id="0d05b-112">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  

* <span data-ttu-id="0d05b-113">Если в критериях поиска ввести обычный текст, критерии поиска будут рассматриваться без учета регистра и будет выполняться поиск определенного текста.</span><span class="sxs-lookup"><span data-stu-id="0d05b-113">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
* <span data-ttu-id="0d05b-114">Если в критериях поиска ввести тест с символами, критерии поиска будут рассматриваться с учетом регистра и будет выполняться поиск точного текста.</span><span class="sxs-lookup"><span data-stu-id="0d05b-114">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="0d05b-115">Критерии экспресс-фильтра</span><span class="sxs-lookup"><span data-stu-id="0d05b-115">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="0d05b-116">Критерии поиска</span><span class="sxs-lookup"><span data-stu-id="0d05b-116">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="0d05b-117">Интерпретируется как…</span><span class="sxs-lookup"><span data-stu-id="0d05b-117">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="0d05b-118">Возвращает…</span><span class="sxs-lookup"><span data-stu-id="0d05b-118">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="0d05b-119">man</span><span class="sxs-lookup"><span data-stu-id="0d05b-119">man</span></span></TD>
    <TD><span data-ttu-id="0d05b-120">@&#42;man&#42;</span><span class="sxs-lookup"><span data-stu-id="0d05b-120">@&#42;man&#42;</span></span></TD>
    <TD><span data-ttu-id="0d05b-121">Все записи, содержащие текст <b>man</b>, без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="0d05b-121">All records that contain the text <b>man</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="0d05b-122">se</span><span class="sxs-lookup"><span data-stu-id="0d05b-122">se</span></span></TD>
    <TD><span data-ttu-id="0d05b-123">@&#42;se&#42;</span><span class="sxs-lookup"><span data-stu-id="0d05b-123">@&#42;se&#42;</span></span></TD>
    <TD><span data-ttu-id="0d05b-124">Все записи, содержащие текст <b>se</b>, без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="0d05b-124">All records that contain the text <b>se</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="0d05b-125">Man&#42;</span><span class="sxs-lookup"><span data-stu-id="0d05b-125">Man&#42;</span></span></TD>
    <TD><span data-ttu-id="0d05b-126">Начинается с <b>Man</b> с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="0d05b-126">Starts with <b>Man</b> and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="0d05b-127">Все записи, которые начинаются с текста <b>Man</b>.</span><span class="sxs-lookup"><span data-stu-id="0d05b-127">All records that start with the text <b>Man</b>.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="0d05b-128">'man'</span><span class="sxs-lookup"><span data-stu-id="0d05b-128">'man'</span></span></TD>
    <TD><span data-ttu-id="0d05b-129">Точный текст с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="0d05b-129">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="0d05b-130">Все записи, которые в точности соответствуют <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="0d05b-130">All records that match <b>man</b> exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="0d05b-131">@man*</span><span class="sxs-lookup"><span data-stu-id="0d05b-131">@man*</span></span> </TD>
    <TD><span data-ttu-id="0d05b-132">Начинается на man без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="0d05b-132">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="0d05b-133">Все записи, которые начинаются на <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="0d05b-133">All records that start with <b>man</b>.</span></span></TD>
  </TR>
    <TR>
    <TD><span data-ttu-id="0d05b-134">@&#42;man</span><span class="sxs-lookup"><span data-stu-id="0d05b-134">@&#42;man</span></span></TD>
    <TD><span data-ttu-id="0d05b-135">Заканчивается на man без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="0d05b-135">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="0d05b-136">Все записи, которые заканчиваются на <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="0d05b-136">All records that end with <b>man</b>.</span></span></TD>
  </TR>
</TABLE>

> [!NOTE]  
>   <span data-ttu-id="0d05b-137">Нельзя использовать подстановочные символы при фильтрации в полях перечислений, например в поле **Статус** заказов на продажу.</span><span class="sxs-lookup"><span data-stu-id="0d05b-137">You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="0d05b-138">Чтобы ввести фильтр для данного типа поля, можно ввести в качестве параметра фильтра числовое значение.</span><span class="sxs-lookup"><span data-stu-id="0d05b-138">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="0d05b-139">Например, в поле **Статус** в заказе на продажу, которое имеет значения **Открыть**, **Выпущено**, **Ожидает утверждения** и **Ожидает предоплаты**, используйте значения **0**, **1**, **2**, и **3** для фильтрации этих параметров.</span><span class="sxs-lookup"><span data-stu-id="0d05b-139">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0d05b-140">См. также</span><span class="sxs-lookup"><span data-stu-id="0d05b-140">See Also</span></span>
<span data-ttu-id="0d05b-141">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0d05b-141">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

