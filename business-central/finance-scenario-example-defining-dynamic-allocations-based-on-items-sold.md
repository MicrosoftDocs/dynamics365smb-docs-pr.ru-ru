---
title: Пример сценария. Определение динамических распределений на основе проданных товаров | Документация Майкрософт
description: В этом разделе приведен пример, как определять распределения с помощью метода динамического распределения.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: finance-define-and-allocate-costs
ms.openlocfilehash: 905dc15b2c29c4a97f2bf73b9970750b47995720
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301784"
---
# <a name="scenario-example-defining-dynamic-allocations-based-on-items-sold"></a><span data-ttu-id="53f1b-103">Пример сценария. Определение динамических распределений на основе проданных товаров</span><span class="sxs-lookup"><span data-stu-id="53f1b-103">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>
<span data-ttu-id="53f1b-104">В этом разделе приведен пример, как определять распределения с помощью метода динамического распределения.</span><span class="sxs-lookup"><span data-stu-id="53f1b-104">This topic shows an example of how to define allocations by using the dynamic allocation method.</span></span> <span data-ttu-id="53f1b-105">В этом примере изменяется динамическое распределение себестоимости для места возникновения затрат ПРОДАЖИ с целью поддержки нового объекта затрат ИТ-ОБОРУДОВАНИЕ.</span><span class="sxs-lookup"><span data-stu-id="53f1b-105">In the example, you change the dynamic allocation of the costs for the SALES cost center to support the new cost object IT EQUIPMENT.</span></span> <span data-ttu-id="53f1b-106">Пакеты ИТ-ОБОРУДОВАНИЯ имеют номера товаров в диапазоне от 8904-W до 8924-W.</span><span class="sxs-lookup"><span data-stu-id="53f1b-106">IT EQUIPMENT packages have item numbers in the range from 8904-W to 8924-W.</span></span> <span data-ttu-id="53f1b-107">Показатели продаж за прошлый год используются для расчета долей.</span><span class="sxs-lookup"><span data-stu-id="53f1b-107">You use the previous year’s sales figures to calculate the share.</span></span> <span data-ttu-id="53f1b-108">Распределение учитывается по типу затрат 9903.</span><span class="sxs-lookup"><span data-stu-id="53f1b-108">The allocation is posted to the helping cost type 9903.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="53f1b-109">В примере используются демонстрационные данные в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="53f1b-109">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-define-dynamic-allocations-based-on-items-sold-in-the-previous-year"></a><span data-ttu-id="53f1b-110">Определение динамических распределений на основе количества проданных товаров в предыдущем году</span><span class="sxs-lookup"><span data-stu-id="53f1b-110">To define dynamic allocations based on items sold in the previous year</span></span>  

1.  <span data-ttu-id="53f1b-111">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Распределение затрат**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="53f1b-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Allocations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="53f1b-112">На странице **Распределение затрат** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="53f1b-112">On the **Cost Allocation** page, choose the **New** action.</span></span>  
3.  <span data-ttu-id="53f1b-113">В поле **ИД** нажмите кнопку ВВОД или введите идентификатор.</span><span class="sxs-lookup"><span data-stu-id="53f1b-113">In the **ID** field, press Enter or enter an ID.</span></span>  
4.  <span data-ttu-id="53f1b-114">В поле **Уровень** введите **1**.</span><span class="sxs-lookup"><span data-stu-id="53f1b-114">In the **Level** field, enter **1**.</span></span>  
5.  <span data-ttu-id="53f1b-115">В полях **Действительно с** и **Действительно по** введите соответствующие даты.</span><span class="sxs-lookup"><span data-stu-id="53f1b-115">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span></span>  
6.  <span data-ttu-id="53f1b-116">В поле **Код центра затрат** введите **ПРОДАЖИ**.</span><span class="sxs-lookup"><span data-stu-id="53f1b-116">In the **Cost Center Code** field, enter **SALES**.</span></span>  
7.  <span data-ttu-id="53f1b-117">В поле **Кредит по типу затрат** введите тип затрат **9903**.</span><span class="sxs-lookup"><span data-stu-id="53f1b-117">In the **Credit to Cost Type** field, enter the cost type **9903**.</span></span>  
8.  <span data-ttu-id="53f1b-118">В поле **Кредит по типу затрат** введите тип затрат **9903**.</span><span class="sxs-lookup"><span data-stu-id="53f1b-118">In the **Target Cost Type** field, enter the cost type **9903**.</span></span>  
9. <span data-ttu-id="53f1b-119">В поле **Целевой объект затрат** выберите **Создать**, чтобы создать новый объект затрат "ИТ-ОБОРУДОВАНИЕ" и заполните все нужные поля.</span><span class="sxs-lookup"><span data-stu-id="53f1b-119">In the **Target Cost Object** field, choose **New** to create a new cost object IT EQUIPMENT and fill in fields as necessary.</span></span> <span data-ttu-id="53f1b-120">Выберите **ИТ-ОБОРУДОВАНИЕ**.</span><span class="sxs-lookup"><span data-stu-id="53f1b-120">Select **IT EQUIPMENT**.</span></span> <span data-ttu-id="53f1b-121">Оставьте поле **Целевой центр затрат** пустым.</span><span class="sxs-lookup"><span data-stu-id="53f1b-121">Leave the **Target Cost Center** field blank.</span></span>  
10. <span data-ttu-id="53f1b-122">В поле **Тип назначения распределения** выберите **Все затраты**, чтобы определить способ распределения всех накопленных затрат.</span><span class="sxs-lookup"><span data-stu-id="53f1b-122">In the **Allocation Target Type** field, select **All Costs** to define how all accumulated costs are allocated.</span></span>  
11. <span data-ttu-id="53f1b-123">В поле **База** выберите базу распределения **Товаров продано (сумма)**.</span><span class="sxs-lookup"><span data-stu-id="53f1b-123">In the **Base** field, select the allocation base **Items Sold (Amount)**.</span></span>  
12. <span data-ttu-id="53f1b-124">В поле **Фильтр по номеру** введите **8904-W..8924-W**.</span><span class="sxs-lookup"><span data-stu-id="53f1b-124">In the **No. Filter** field, enter **8904-W..8924-W**.</span></span>  
13. <span data-ttu-id="53f1b-125">В поле **Код фильтра по дате** введите **Прошлый год**.</span><span class="sxs-lookup"><span data-stu-id="53f1b-125">In the **Date Filter Code** field, enter **Last Year**.</span></span>  
14. <span data-ttu-id="53f1b-126">Для расчета доли выберите действие **Вычислить ключ распределения**.</span><span class="sxs-lookup"><span data-stu-id="53f1b-126">Choose the **Calculate Allocation Key** action to calculate the share.</span></span>  

    > [!IMPORTANT]  
    >  [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="53f1b-127">использует показатели продаж предыдущих лет для расчета акции стоимостью 1596,50 рублей со ста процентами для пакетов ИТ-ОБОРУДОВАНИЕ.</span><span class="sxs-lookup"><span data-stu-id="53f1b-127">uses the previous years’ sales figures to calculate a share of 1596.50 LCY with 100 percent for the IT EQUIPMENT packages.</span></span> <span data-ttu-id="53f1b-128">Это означает, что все товары, проданные в прошлом году, будут распределены в объект затрат "ИТ-ОБОРУДОВАНИЕ".</span><span class="sxs-lookup"><span data-stu-id="53f1b-128">This means that all of the items sold last year will be allocated to the cost object IT EQUIPMENT.</span></span>  

## <a name="see-also"></a><span data-ttu-id="53f1b-129">См. также</span><span class="sxs-lookup"><span data-stu-id="53f1b-129">See Also</span></span>  
[<span data-ttu-id="53f1b-130">Определение и распределение затрат</span><span class="sxs-lookup"><span data-stu-id="53f1b-130">Defining and Allocating Costs</span></span>](finance-define-and-allocate-costs.md)  
<span data-ttu-id="53f1b-131">[Терминология в учете затрат](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="53f1b-131">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="53f1b-132">Об учете затрат</span><span class="sxs-lookup"><span data-stu-id="53f1b-132">About Cost Accounting</span></span>](finance-about-cost-accounting.md)
