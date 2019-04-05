---
title: Определение статических распределений на основе отношения распределений | Документы Майкрософт
description: 'Метод статического распределения основан на конкретном значении, таком как занятая площадь в квадратных метрах или заданное соотношение распределения (например, 5:2: 4).'
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
redirect_url: finance-define-and-allocate-costs
ms.openlocfilehash: d35fd5de7a0583c3864268d0749384322bf947ed
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "805195"
---
# <a name="scenario-example-defining-static-allocations-based-on-allocation-ratio"></a><span data-ttu-id="7d605-103">Пример сценария. Определение статических распределений на основе отношения распределений</span><span class="sxs-lookup"><span data-stu-id="7d605-103">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span></span>
<span data-ttu-id="7d605-104">Метод статического распределения основан на конкретном значении, таком как занятая площадь в квадратных метрах или заданное соотношение распределения (например, 5:2: 4).</span><span class="sxs-lookup"><span data-stu-id="7d605-104">Static allocation method is based on a definite value, such as square meters used, or an established allocation ratio such as 5:2:4.</span></span>  

<span data-ttu-id="7d605-105">В этом разделе описывается, как определить три новых объекта затрат цели распределения для места возникновения затрат ПРОД источника распределения с использованием принятого соотношения распределения 5:2:4.</span><span class="sxs-lookup"><span data-stu-id="7d605-105">This topic describes how to define three new allocation target cost objects for the allocation source PROD cost center using the established allocation ratio 5:2:4.</span></span> <span data-ttu-id="7d605-106">Три целевых объекта затрат: ПРИНАДЛЕЖНОСТИ, КРАСКА и ФИТИНГИ.</span><span class="sxs-lookup"><span data-stu-id="7d605-106">The three target cost objects are ACCESSO, PAINT, and FITTINGS.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="7d605-107">В примере используются демонстрационные данные в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="7d605-107">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-define-the-allocation-source-prod-cost-center-on-the-general-fasttab"></a><span data-ttu-id="7d605-108">Определение места возникновения затрат ПРОД по источнику распределения на экспресс-вкладке "Общее"</span><span class="sxs-lookup"><span data-stu-id="7d605-108">To define the allocation source PROD cost center on the General FastTab</span></span>  

1.  <span data-ttu-id="7d605-109">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Распределение затрат**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="7d605-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Allocation**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7d605-110">На странице **Распределение затрат** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="7d605-110">On the **Cost Allocation** page, choose the **New** action.</span></span>  
3.  <span data-ttu-id="7d605-111">В поле **ИД** нажмите кнопку ВВОД или введите идентификатор.</span><span class="sxs-lookup"><span data-stu-id="7d605-111">In the **ID** field, press Enter or enter an ID.</span></span>  
4.  <span data-ttu-id="7d605-112">В поле **Уровень** введите **1**.</span><span class="sxs-lookup"><span data-stu-id="7d605-112">In the **Level** field, enter **1**.</span></span>  
5.  <span data-ttu-id="7d605-113">В полях **Действительно с** и **Действительно по** введите соответствующие даты.</span><span class="sxs-lookup"><span data-stu-id="7d605-113">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span></span>  
6.  <span data-ttu-id="7d605-114">В поле **Код центра затрат** введите **ПРОИЗВ**.</span><span class="sxs-lookup"><span data-stu-id="7d605-114">In the **Cost Center Code** field, enter **PROD**.</span></span>  
7.  <span data-ttu-id="7d605-115">В поле **Кредит по типу затрат** введите тип затрат **9903**.</span><span class="sxs-lookup"><span data-stu-id="7d605-115">In the **Credit to Cost Type** field, enter the cost type **9903**.</span></span>  

## <a name="to-define-the-allocation-target-cost-objects-on-the-lines-fasttab"></a><span data-ttu-id="7d605-116">Определение объектов затрат по целям распределения на экспресс-вкладке "Строки"</span><span class="sxs-lookup"><span data-stu-id="7d605-116">To define the allocation target cost objects on the Lines FastTab</span></span>  

1.  <span data-ttu-id="7d605-117">В первой строке, в поле **Тип назначения затрат** укажите **9903**.</span><span class="sxs-lookup"><span data-stu-id="7d605-117">On the first line, in the **Target Cost Type** field, enter **9903**.</span></span>  
2.  <span data-ttu-id="7d605-118">В первой строке, в поле **Целевой объект затрат** выберите **ACCESSO**.</span><span class="sxs-lookup"><span data-stu-id="7d605-118">On the first line, in the **Target Cost Object** field, select **ACCESSO**.</span></span>  
3.  <span data-ttu-id="7d605-119">На первой строке в поле **Тип назначения распределения** выберите **Все затраты**, чтобы определить способ распределения всех начисленных средств.</span><span class="sxs-lookup"><span data-stu-id="7d605-119">On the first line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
4.  <span data-ttu-id="7d605-120">В первой строке в поле **База** выберите **Статический**, чтобы использовать метод статического распределения.</span><span class="sxs-lookup"><span data-stu-id="7d605-120">On the first line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
5.  <span data-ttu-id="7d605-121">В первой строке в поле **Доля** введите соотношение распределения **5**.</span><span class="sxs-lookup"><span data-stu-id="7d605-121">On the first line, in the **Share** field, enter the allocation ratio **5**.</span></span>  
6.  <span data-ttu-id="7d605-122">Во второй строке в поле **Тип назначения затрат** укажите **9903**.</span><span class="sxs-lookup"><span data-stu-id="7d605-122">On the second line, in the **Target Cost Type** field, enter **9903**.</span></span>  
7.  <span data-ttu-id="7d605-123">Во второй строке в поле **Целевой объект затрат** выберите **PAINT**.</span><span class="sxs-lookup"><span data-stu-id="7d605-123">On the second line, in the **Target Cost Object** field, select **PAINT**.</span></span>  
8.  <span data-ttu-id="7d605-124">На второй строке в поле **Тип назначения распределения** выберите **Все затраты**, чтобы определить способ распределения всех начисленных средств.</span><span class="sxs-lookup"><span data-stu-id="7d605-124">On the second line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
9. <span data-ttu-id="7d605-125">Во второй строке в поле **База** выберите **Статический**, чтобы использовать метод статического распределения.</span><span class="sxs-lookup"><span data-stu-id="7d605-125">On the second line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
10. <span data-ttu-id="7d605-126">Во второй строке в поле **Доля** введите соотношение распределения **2**.</span><span class="sxs-lookup"><span data-stu-id="7d605-126">On the second line, in the **Share** field, enter the allocation ratio **2**.</span></span>  
11. <span data-ttu-id="7d605-127">В третьей строке в поле **Тип назначения затрат** укажите **9903**.</span><span class="sxs-lookup"><span data-stu-id="7d605-127">On the third line, in the **Target Cost Type** field, enter **9903**.</span></span>  
12. <span data-ttu-id="7d605-128">В третьей строке в поле **Целевой объект затрат** выберите **FITTINGS**.</span><span class="sxs-lookup"><span data-stu-id="7d605-128">On the third line, in the **Target Cost Object** field, select **FITTINGS**.</span></span>  
13. <span data-ttu-id="7d605-129">В третьей строке в поле **Тип назначения распределения** выберите **Все затраты**, чтобы определить способ распределения всех начисленных средств.</span><span class="sxs-lookup"><span data-stu-id="7d605-129">On the third line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
14. <span data-ttu-id="7d605-130">В третьей строке в поле **База** выберите **Статический**, чтобы использовать метод статического распределения.</span><span class="sxs-lookup"><span data-stu-id="7d605-130">On the third line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
15. <span data-ttu-id="7d605-131">В третьей строке в поле **Доля** введите соотношение распределения **4**.</span><span class="sxs-lookup"><span data-stu-id="7d605-131">On the third line, in the **Share** field, enter the allocation ratio **4**.</span></span>  

> [!IMPORTANT]  
>  [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="7d605-132">автоматически вычисляет поле **Процент** с помощью процента, который зависит от всех трех соотношений распределения, которые вводятся в поле **Доля** для всех трех строк.</span><span class="sxs-lookup"><span data-stu-id="7d605-132">automatically calculates the **Percent** field using a percentage rate that is dependent on all three allocation ratios that are entered in the **Share** field for all three lines.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7d605-133">См. также</span><span class="sxs-lookup"><span data-stu-id="7d605-133">See Also</span></span>  
[<span data-ttu-id="7d605-134">Определение и распределение затрат</span><span class="sxs-lookup"><span data-stu-id="7d605-134">Defining and Allocating Costs</span></span>](finance-define-and-allocate-costs.md)   
