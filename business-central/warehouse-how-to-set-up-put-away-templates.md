---
title: Как настраивать шаблоны размещения | Документация Майкрософт
description: С помощью функции расширенного подбора и размещения в любой момент времени отыскивается наиболее подходящая для товаров ячейка в соответствии с шаблоном размещения, настроенным для склада, заданными рейтингами ячеек и максимальными и минимальными количествами, заданными для фиксированных ячеек.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/24/2020
ms.author: sgroespe
ms.openlocfilehash: 46dc891937ec4046a0403ca418296d1d7ee24a99
ms.sourcegitcommit: 3e9c89f90db5eaed599630299353300621fe4007
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "3529317"
---
# <a name="set-up-put-away-templates"></a><span data-ttu-id="92da5-103">Настройка шаблонов размещения</span><span class="sxs-lookup"><span data-stu-id="92da5-103">Set Up Put-away Templates</span></span>

<span data-ttu-id="92da5-104">С помощью функции расширенного подбора и размещения в любой момент времени отыскивается наиболее подходящая для товаров ячейка в соответствии с шаблоном размещения, настроенным для склада, заданными рейтингами ячеек и максимальными и минимальными количествами, заданными для фиксированных ячеек.</span><span class="sxs-lookup"><span data-stu-id="92da5-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span></span>  

<span data-ttu-id="92da5-105">Возможно настроить несколько шаблонов размещения и выбрать один из них для управления размещениями на всем складе.</span><span class="sxs-lookup"><span data-stu-id="92da5-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span></span> <span data-ttu-id="92da5-106">Также шаблон размещения возможно выбрать для каждого товара или единицы хранения, имеющих особые условия размещения.</span><span class="sxs-lookup"><span data-stu-id="92da5-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span></span>  

## <a name="to-set-up-put-away-templates"></a><span data-ttu-id="92da5-107">Настройка шаблонов размещения</span><span class="sxs-lookup"><span data-stu-id="92da5-107">To set up put-away templates</span></span>

1. <span data-ttu-id="92da5-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Шаблоны размещения**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="92da5-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Put-away Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="92da5-109">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="92da5-109">Choose the **New** action.</span></span>  
3. <span data-ttu-id="92da5-110">Введите код, являющийся уникальным идентификатором создаваемого шаблона.</span><span class="sxs-lookup"><span data-stu-id="92da5-110">Enter a code that is the unique identifier of the template you are about to create.</span></span>  
4. <span data-ttu-id="92da5-111">При необходимости введите краткое описание.</span><span class="sxs-lookup"><span data-stu-id="92da5-111">Enter a short description, if you wish.</span></span>  
5. <span data-ttu-id="92da5-112">Заполните первую строку требованиями, которые должны выполняться в первую очередь при предложении размещения.</span><span class="sxs-lookup"><span data-stu-id="92da5-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span></span>

    <span data-ttu-id="92da5-113">Например, если вы хотите, чтобы метод размещения по умолчанию основывался на фиксированных ячейках, выберите поле **Найти фиксированную ячейку**.</span><span class="sxs-lookup"><span data-stu-id="92da5-113">For example, if want the default put-away method to be based on fixed bins, then choose the **Find Fixed Bin** field.</span></span> [!INCLUDE[tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  
6. <span data-ttu-id="92da5-114">Заполните вторую строку требованиями, которые определяют второй вариант выбора при поиске ячейки для размещения.</span><span class="sxs-lookup"><span data-stu-id="92da5-114">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span></span> <span data-ttu-id="92da5-115">Вторая строка используется только в том случае, если ячейка, соответствующая требованиям первой строки, не найдена.</span><span class="sxs-lookup"><span data-stu-id="92da5-115">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span></span>  
7. <span data-ttu-id="92da5-116">Продолжайте заполнять строки, пока полностью не опишете приемлемое расположение ячеек, используемых в процессе размещения.</span><span class="sxs-lookup"><span data-stu-id="92da5-116">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span></span>  
8. <span data-ttu-id="92da5-117">В последней строке шаблона размещения установите флажок **Найти плавающую ячейку**.</span><span class="sxs-lookup"><span data-stu-id="92da5-117">On the last line in the put-away template, select the **Find Floating Bin** check box.</span></span>  

<span data-ttu-id="92da5-118">Можно создавать различные шаблоны размещения и использовать их в соответствии с индивидуальными требованиями.</span><span class="sxs-lookup"><span data-stu-id="92da5-118">You can create various put-away templates and then apply them as you see fit.</span></span> <span data-ttu-id="92da5-119">В первую очередь выполняется обращение к шаблону размещения, выбранному для товара или единицы хранения, при наличии таковых.</span><span class="sxs-lookup"><span data-stu-id="92da5-119">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span></span> <span data-ttu-id="92da5-120">Если данные поля не заполнены, то используется шаблон размещения, выбранный для склада на экспресс-вкладке **Политики ячеек** в карточке склада.</span><span class="sxs-lookup"><span data-stu-id="92da5-120">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span></span>  

## <a name="see-also"></a><span data-ttu-id="92da5-121">См. также</span><span class="sxs-lookup"><span data-stu-id="92da5-121">See Also</span></span>

[<span data-ttu-id="92da5-122">Управление складом</span><span class="sxs-lookup"><span data-stu-id="92da5-122">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="92da5-123">Наличие</span><span class="sxs-lookup"><span data-stu-id="92da5-123">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="92da5-124">Настройка управления складом</span><span class="sxs-lookup"><span data-stu-id="92da5-124">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
[<span data-ttu-id="92da5-125">Управление сборкой</span><span class="sxs-lookup"><span data-stu-id="92da5-125">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="92da5-126">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="92da5-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="92da5-127">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="92da5-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
