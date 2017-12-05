---
title: "Пример сценария. Определение динамических распределений на основе проданных товаров | Microsoft Docs"
description: "В этом разделе приведен пример, как определять распределения с помощью метода динамического распределения."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: d87e01cb987a019c6e71b50dcdeae55dc0375146
ms.contentlocale: ru-ru
ms.lasthandoff: 11/10/2017

---
# <a name="scenario-example-defining-dynamic-allocations-based-on-items-sold"></a><span data-ttu-id="f8011-103">Пример сценария. Определение динамических распределений на основе проданных товаров</span><span class="sxs-lookup"><span data-stu-id="f8011-103">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>
<span data-ttu-id="f8011-104">В этом разделе приведен пример, как определять распределения с помощью метода динамического распределения.</span><span class="sxs-lookup"><span data-stu-id="f8011-104">This topic shows an example of how to define allocations by using the dynamic allocation method.</span></span> <span data-ttu-id="f8011-105">В этом примере изменяется динамическое распределение себестоимости для места возникновения затрат ПРОДАЖИ с целью поддержки нового объекта затрат ИТ-ОБОРУДОВАНИЕ.</span><span class="sxs-lookup"><span data-stu-id="f8011-105">In the example, you change the dynamic allocation of the costs for the SALES cost center to support the new cost object IT EQUIPMENT.</span></span> <span data-ttu-id="f8011-106">Пакеты ИТ-ОБОРУДОВАНИЯ имеют номера товаров в диапазоне от 8904-W до 8924-W.</span><span class="sxs-lookup"><span data-stu-id="f8011-106">IT EQUIPMENT packages have item numbers in the range from 8904-W to 8924-W.</span></span> <span data-ttu-id="f8011-107">Показатели продаж за прошлый год используются для расчета долей.</span><span class="sxs-lookup"><span data-stu-id="f8011-107">You use the previous year’s sales figures to calculate the share.</span></span> <span data-ttu-id="f8011-108">Распределение учитывается по типу затрат 9903.</span><span class="sxs-lookup"><span data-stu-id="f8011-108">The allocation is posted to the helping cost type 9903.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="f8011-109">В примере используются демонстрационные данные в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f8011-109">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-define-dynamic-allocations-based-on-items-sold-in-the-previous-year"></a><span data-ttu-id="f8011-110">Определение динамических распределений на основе количества проданных товаров в предыдущем году</span><span class="sxs-lookup"><span data-stu-id="f8011-110">To define dynamic allocations based on items sold in the previous year</span></span>  

1.  <span data-ttu-id="f8011-111">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Распределение затрат**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f8011-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Allocations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f8011-112">В окне **Распределение затрат** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="f8011-112">In the **Cost Allocation** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="f8011-113">В поле **ИД** нажмите кнопку ВВОД или введите идентификатор.</span><span class="sxs-lookup"><span data-stu-id="f8011-113">In the **ID** field, press Enter or enter an ID.</span></span>  
4.  <span data-ttu-id="f8011-114">В поле **Уровень** введите **1**.</span><span class="sxs-lookup"><span data-stu-id="f8011-114">In the **Level** field, enter **1**.</span></span>  
5.  <span data-ttu-id="f8011-115">В полях **Действительно с** и **Действительно по** введите соответствующие даты.</span><span class="sxs-lookup"><span data-stu-id="f8011-115">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span></span>  
6.  <span data-ttu-id="f8011-116">В поле **Код центра затрат** введите **ПРОДАЖИ**.</span><span class="sxs-lookup"><span data-stu-id="f8011-116">In the **Cost Center Code** field, enter **SALES**.</span></span>  
7.  <span data-ttu-id="f8011-117">В поле **Кредит по типу затрат** введите тип затрат **9903**.</span><span class="sxs-lookup"><span data-stu-id="f8011-117">In the **Credit to Cost Type** field, enter the cost type **9903**.</span></span>  
8.  <span data-ttu-id="f8011-118">В поле **Кредит по типу затрат** введите тип затрат **9903**.</span><span class="sxs-lookup"><span data-stu-id="f8011-118">In the **Target Cost Type** field, enter the cost type **9903**.</span></span>  
9. <span data-ttu-id="f8011-119">В поле **Целевой объект затрат** выберите **Создать**, чтобы создать новый объект затрат "ИТ-ОБОРУДОВАНИЕ" и заполните все нужные поля.</span><span class="sxs-lookup"><span data-stu-id="f8011-119">In the **Target Cost Object** field, choose **New** to create a new cost object IT EQUIPMENT and fill in fields as necessary.</span></span> <span data-ttu-id="f8011-120">Выберите **ИТ-ОБОРУДОВАНИЕ**.</span><span class="sxs-lookup"><span data-stu-id="f8011-120">Select **IT EQUIPMENT**.</span></span> <span data-ttu-id="f8011-121">Оставьте поле **Целевой центр затрат** пустым.</span><span class="sxs-lookup"><span data-stu-id="f8011-121">Leave the **Target Cost Center** field blank.</span></span>  
10. <span data-ttu-id="f8011-122">В поле **Тип назначения распределения** выберите **Все затраты**, чтобы определить способ распределения всех накопленных затрат.</span><span class="sxs-lookup"><span data-stu-id="f8011-122">In the **Allocation Target Type** field, select **All Costs** to define how all accumulated costs are allocated.</span></span>  
11. <span data-ttu-id="f8011-123">В поле **База** выберите базу распределения **Товаров продано (сумма)**.</span><span class="sxs-lookup"><span data-stu-id="f8011-123">In the **Base** field, select the allocation base **Items Sold (Amount)**.</span></span>  
12. <span data-ttu-id="f8011-124">В поле **Фильтр по номеру** введите **8904-W..8924-W**.</span><span class="sxs-lookup"><span data-stu-id="f8011-124">In the **No. Filter** field, enter **8904-W..8924-W**.</span></span>  
13. <span data-ttu-id="f8011-125">В поле **Код фильтра по дате** введите **Прошлый год**.</span><span class="sxs-lookup"><span data-stu-id="f8011-125">In the **Date Filter Code** field, enter **Last Year**.</span></span>  
14. <span data-ttu-id="f8011-126">Для расчета доли выберите действие **Вычислить ключ распределения**.</span><span class="sxs-lookup"><span data-stu-id="f8011-126">Choose the **Calculate Allocation Key** action to calculate the share.</span></span>  

    > [!IMPORTANT]  
    >  [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="f8011-127"> использует показатели продаж предыдущих лет для расчета акции стоимостью 1596,50 рублей со ста процентами для пакетов ИТ-ОБОРУДОВАНИЕ.</span><span class="sxs-lookup"><span data-stu-id="f8011-127"> uses the previous years’ sales figures to calculate a share of 1596.50 LCY with 100 percent for the IT EQUIPMENT packages.</span></span> <span data-ttu-id="f8011-128">Это означает, что все товары, проданные в прошлом году, будут распределены в объект затрат "ИТ-ОБОРУДОВАНИЕ".</span><span class="sxs-lookup"><span data-stu-id="f8011-128">This means that all of the items sold last year will be allocated to the cost object IT EQUIPMENT.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f8011-129">См. также</span><span class="sxs-lookup"><span data-stu-id="f8011-129">See Also</span></span>  
 <span data-ttu-id="f8011-130">[Настройка фильтров для базы динамического распределения](finance-setting-filters-for-dynamic-allocation-bases.md) </span><span class="sxs-lookup"><span data-stu-id="f8011-130">[Setting Filters for Dynamic Allocation Bases](finance-setting-filters-for-dynamic-allocation-bases.md) </span></span>  
 <span data-ttu-id="f8011-131">[Практическое руководство. Настройка источника и целей распределения](finance-how-to-set-up-allocation-source-and-targets.md) </span><span class="sxs-lookup"><span data-stu-id="f8011-131">[How to: Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span></span>  
 <span data-ttu-id="f8011-132">[Определение и распределение затрат](finance-define-and-allocate-costs.md) </span><span class="sxs-lookup"><span data-stu-id="f8011-132">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span></span>  
 <span data-ttu-id="f8011-133">[Терминология в учете затрат](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="f8011-133">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="f8011-134">Об учете затрат</span><span class="sxs-lookup"><span data-stu-id="f8011-134">About Cost Accounting</span></span>](finance-about-cost-accounting.md)

