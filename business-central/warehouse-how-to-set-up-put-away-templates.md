---
title: Как настраивать шаблоны размещения | Документы Майкрософт
description: С помощью функции расширенного подбора и размещения в любой момент времени отыскивается наиболее подходящая для товаров ячейка в соответствии с шаблоном размещения, настроенным для склада, заданными рейтингами ячеек и максимальными и минимальными количествами, заданными для фиксированных ячеек.
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
ms.openlocfilehash: 83ae54e61c5881cce9a58c6684bbf82c4b3ad750
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "804355"
---
# <a name="set-up-put-away-templates"></a><span data-ttu-id="67fd9-103">Настройка шаблонов размещения</span><span class="sxs-lookup"><span data-stu-id="67fd9-103">Set Up Put-away Templates</span></span>
<span data-ttu-id="67fd9-104">С помощью функции расширенного подбора и размещения в любой момент времени отыскивается наиболее подходящая для товаров ячейка в соответствии с шаблоном размещения, настроенным для склада, заданными рейтингами ячеек и максимальными и минимальными количествами, заданными для фиксированных ячеек.</span><span class="sxs-lookup"><span data-stu-id="67fd9-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span></span>  

<span data-ttu-id="67fd9-105">Возможно настроить несколько шаблонов размещения и выбрать один из них для управления размещениями на всем складе.</span><span class="sxs-lookup"><span data-stu-id="67fd9-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span></span> <span data-ttu-id="67fd9-106">Также шаблон размещения возможно выбрать для каждого товара или единицы хранения, имеющих особые условия размещения.</span><span class="sxs-lookup"><span data-stu-id="67fd9-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span></span>  

## <a name="to-set-up-put-away-templates"></a><span data-ttu-id="67fd9-107">Настройка шаблонов размещения</span><span class="sxs-lookup"><span data-stu-id="67fd9-107">To set up put-away templates</span></span>  
1.  <span data-ttu-id="67fd9-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Шаблоны размещения**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="67fd9-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Put-away Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="67fd9-109">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="67fd9-109">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="67fd9-110">Введите код, являющийся уникальным идентификатором создаваемого шаблона.</span><span class="sxs-lookup"><span data-stu-id="67fd9-110">Enter a code that is the unique identifier of the template you are about to create.</span></span>  
4.  <span data-ttu-id="67fd9-111">При необходимости введите краткое описание.</span><span class="sxs-lookup"><span data-stu-id="67fd9-111">Enter a short description, if you wish.</span></span>  
5.  <span data-ttu-id="67fd9-112">Заполните первую строку требованиями, которые должны выполняться в первую очередь при предложении размещения.</span><span class="sxs-lookup"><span data-stu-id="67fd9-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span></span>  
6.  <span data-ttu-id="67fd9-113">Заполните вторую строку требованиями, которые определяют второй вариант выбора при поиске ячейки для размещения.</span><span class="sxs-lookup"><span data-stu-id="67fd9-113">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span></span> <span data-ttu-id="67fd9-114">Вторая строка используется только в том случае, если ячейка, соответствующая требованиям первой строки, не найдена.</span><span class="sxs-lookup"><span data-stu-id="67fd9-114">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span></span>  
7.  <span data-ttu-id="67fd9-115">Продолжайте заполнять строки, пока полностью не опишете приемлемое расположение ячеек, используемых в процессе размещения.</span><span class="sxs-lookup"><span data-stu-id="67fd9-115">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span></span>  
8.  <span data-ttu-id="67fd9-116">В последней строке шаблона размещения установите флажок **Найти плавающую ячейку**.</span><span class="sxs-lookup"><span data-stu-id="67fd9-116">On the last line in the put-away template, select the **Find Floating Bin** check box.</span></span>  

<span data-ttu-id="67fd9-117">Можно создавать различные шаблоны размещения и использовать их в соответствии с индивидуальными требованиями.</span><span class="sxs-lookup"><span data-stu-id="67fd9-117">You can create various put-away templates and then apply them as you see fit.</span></span> <span data-ttu-id="67fd9-118">В первую очередь выполняется обращение к шаблону размещения, выбранному для товара или единицы хранения, при наличии таковых.</span><span class="sxs-lookup"><span data-stu-id="67fd9-118">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span></span> <span data-ttu-id="67fd9-119">Если данные поля не заполнены, то используется шаблон размещения, выбранный для склада на экспресс-вкладке **Политики ячеек** в карточке склада.</span><span class="sxs-lookup"><span data-stu-id="67fd9-119">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span></span>  

## <a name="see-also"></a><span data-ttu-id="67fd9-120">См. также</span><span class="sxs-lookup"><span data-stu-id="67fd9-120">See Also</span></span>  
[<span data-ttu-id="67fd9-121">Управление складом</span><span class="sxs-lookup"><span data-stu-id="67fd9-121">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="67fd9-122">Наличие</span><span class="sxs-lookup"><span data-stu-id="67fd9-122">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="67fd9-123">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="67fd9-123">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="67fd9-124">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="67fd9-124">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="67fd9-125">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="67fd9-125">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="67fd9-126">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="67fd9-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
