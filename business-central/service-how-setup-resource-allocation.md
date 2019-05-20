---
title: Настройка распределения ресурсов | Документы Майкрософт
description: Узнайте, как система может помочь обеспечить, чтобы для сервисных работ назначались сотрудники с необходимыми навыками.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: resource, skill, service, zones
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: 7b7a01bc61d55379cd12563d1f31f331c3b4fd74
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1251957"
---
# <a name="set-up-resource-allocation"></a><span data-ttu-id="91ee2-103">Настройка распределения ресурсов</span><span class="sxs-lookup"><span data-stu-id="91ee2-103">Set Up Resource Allocation</span></span>
<span data-ttu-id="91ee2-104">Для обеспечения хорошего качества выполнения сервисной задачи важно найти квалифицированный ресурс, обладающий квалификацией для выполнения работы.</span><span class="sxs-lookup"><span data-stu-id="91ee2-104">To ensure that a service task is performed well, it's important to find a resource who is qualified to do the work.</span></span> <span data-ttu-id="91ee2-105">Можно настроить [!INCLUDE[d365fin](includes/d365fin_md.md)] таким образом, чтобы было легко выделить для работы сотрудника с требуемой квалификацией.</span><span class="sxs-lookup"><span data-stu-id="91ee2-105">You can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] so that it's easy to allocate someone who has the right skills for the job.</span></span> <span data-ttu-id="91ee2-106">В [!INCLUDE[d365fin](includes/d365fin_md.md)] это называется _распределением ресурсов_.</span><span class="sxs-lookup"><span data-stu-id="91ee2-106">In [!INCLUDE[d365fin](includes/d365fin_md.md)], we call this _resource allocation_.</span></span> <span data-ttu-id="91ee2-107">Ресурсы можно распределять на основе квалификации, доступности или по принадлежности к той же зоне обслуживания, что и клиент.</span><span class="sxs-lookup"><span data-stu-id="91ee2-107">You can allocate resources based on their skill, availability, or whether they are in the same service zone as the customer.</span></span> 

<span data-ttu-id="91ee2-108">Для использования распределения ресурсов необходимо настроить:</span><span class="sxs-lookup"><span data-stu-id="91ee2-108">To use resource allocation, you must set up:</span></span>  
  
* <span data-ttu-id="91ee2-109">Навыки, необходимые для ремонта и обслуживания сервисных товаров.</span><span class="sxs-lookup"><span data-stu-id="91ee2-109">The skills required to repair and maintain service items.</span></span> <span data-ttu-id="91ee2-110">Они назначаются сервисным товарам и ресурсам.</span><span class="sxs-lookup"><span data-stu-id="91ee2-110">You assign these to service items and resources.</span></span>  
* <span data-ttu-id="91ee2-111">Географические регионы, называемые зонами, которые вы определили для вашего рынка.</span><span class="sxs-lookup"><span data-stu-id="91ee2-111">Geographic regions, called zones, that you define for your market.</span></span> <span data-ttu-id="91ee2-112">Например, восточная, западная, центральная и т. д.</span><span class="sxs-lookup"><span data-stu-id="91ee2-112">For example, East, West, Central, and so on.</span></span> <span data-ttu-id="91ee2-113">Они назначаются клиентам и ресурсам.</span><span class="sxs-lookup"><span data-stu-id="91ee2-113">You assign these to customers and resources.</span></span>  
* <span data-ttu-id="91ee2-114">Требуется ли отображаться навыки и зоны, а также требуется ли отображать предупреждение, если кто-то выбирает неквалифицированный ресурс или ресурс, который не находится в зоне клиента.</span><span class="sxs-lookup"><span data-stu-id="91ee2-114">Whether to display resource skills and zones, and whether to display a warning if someone chooses unqualified resource, or a resource that is not in the customer zone.</span></span>  

## <a name="to-set-up-skills"></a><span data-ttu-id="91ee2-115">Настройка навыков</span><span class="sxs-lookup"><span data-stu-id="91ee2-115">To set up skills</span></span>
1. <span data-ttu-id="91ee2-116">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Квалификации**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="91ee2-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Skills**, and then choose the related link.</span></span>  
2. <span data-ttu-id="91ee2-117">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="91ee2-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-skills-to-service-items-and-resources"></a><span data-ttu-id="91ee2-118">Назначение квалификации сервисным товарам и ресурсам</span><span class="sxs-lookup"><span data-stu-id="91ee2-118">To assign skills to service items and resources</span></span>
1. <span data-ttu-id="91ee2-119">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сервисные товары** или **Ресурсы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="91ee2-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items** or **Resources**, and then choose the related link.</span></span>  
2. <span data-ttu-id="91ee2-120">Откройте карточку для сервисного товара или ресурса, затем выберите одно из следующего:</span><span class="sxs-lookup"><span data-stu-id="91ee2-120">Open the card for the service item or resource, and then choose one of the following:</span></span>  
  
    * <span data-ttu-id="91ee2-121">Для сервисных товаров выберите **Квалификация ресурсов**.</span><span class="sxs-lookup"><span data-stu-id="91ee2-121">For service items, choose **Resource Skills**.</span></span>  
    * <span data-ttu-id="91ee2-122">Для ресурсов выберите **Квалификация**.</span><span class="sxs-lookup"><span data-stu-id="91ee2-122">For resources, choose **Skills**.</span></span>  

## <a name="to-set-up-zones"></a><span data-ttu-id="91ee2-123">Настройка зон</span><span class="sxs-lookup"><span data-stu-id="91ee2-123">To set up zones</span></span>
1. <span data-ttu-id="91ee2-124">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Зоны**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="91ee2-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Zones**, and then choose the related link.</span></span>  
2. <span data-ttu-id="91ee2-125">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="91ee2-125">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-zones-to-customers-and-resources"></a><span data-ttu-id="91ee2-126">Назначение зон клиентам и ресурсам</span><span class="sxs-lookup"><span data-stu-id="91ee2-126">To assign zones to customers and resources</span></span> 
1. <span data-ttu-id="91ee2-127">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиенты** или **Ресурсы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="91ee2-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers** or **Resources**, and then choose the related link.</span></span>  
2. <span data-ttu-id="91ee2-128">Откройте карточку для сервисного товара или ресурса, затем выберите одно из следующего:</span><span class="sxs-lookup"><span data-stu-id="91ee2-128">Open the card for the service item or resource, and then choose one of the following:</span></span>  
  
    * <span data-ttu-id="91ee2-129">Для клиентов выберите зону в поле **Код сервисной зоны**.</span><span class="sxs-lookup"><span data-stu-id="91ee2-129">For customers, choose a zone in the **Service Zone Code** field.</span></span>  
    * <span data-ttu-id="91ee2-130">Для ресурсов выберите действие **Сервисные зоны**.</span><span class="sxs-lookup"><span data-stu-id="91ee2-130">For resources, choose the **Service Zones** action.</span></span>  

## <a name="to-specify-what-to-show-when-a-resource-is-chosen"></a><span data-ttu-id="91ee2-131">Указание, что должно отображаться при выборе ресурса</span><span class="sxs-lookup"><span data-stu-id="91ee2-131">To specify what to show when a resource is chosen</span></span>
1. <span data-ttu-id="91ee2-132">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка сервиса**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="91ee2-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Setup**, and then choose the related link.</span></span> 
2. <span data-ttu-id="91ee2-133">В поле **Параметр квалификации ресурсов** выберите один из вариантов, описанных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="91ee2-133">In the **Resource Skills Option** field, choose one of the options described in the following table.</span></span>  
  
    |<span data-ttu-id="91ee2-134">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="91ee2-134">**Option**</span></span>|<span data-ttu-id="91ee2-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="91ee2-135">**Description**</span></span>|  
    |------------|-------------|  
    |<span data-ttu-id="91ee2-136">Отображаемый код</span><span class="sxs-lookup"><span data-stu-id="91ee2-136">Code Shown</span></span> | <span data-ttu-id="91ee2-137">Отображается только код.</span><span class="sxs-lookup"><span data-stu-id="91ee2-137">Displays the code only.</span></span>|  
    |<span data-ttu-id="91ee2-138">Отображаемое предупреждение</span><span class="sxs-lookup"><span data-stu-id="91ee2-138">Warning Displayed</span></span> | <span data-ttu-id="91ee2-139">Отображается информация и выводится предупреждение при выборе ресурса, не имеющего требуемой квалификации.</span><span class="sxs-lookup"><span data-stu-id="91ee2-139">Shows the information and displays a warning if you choose a resource that is not qualified.</span></span>|  
    |<span data-ttu-id="91ee2-140">Не используется</span><span class="sxs-lookup"><span data-stu-id="91ee2-140">Not Used</span></span> | <span data-ttu-id="91ee2-141">Не отображает эту информацию.</span><span class="sxs-lookup"><span data-stu-id="91ee2-141">Does not show this information.</span></span>|  

## <a name="to-update-resource-capacity"></a><span data-ttu-id="91ee2-142">Обновление производственной мощности ресурсов</span><span class="sxs-lookup"><span data-stu-id="91ee2-142">To update resource capacity</span></span>  
<span data-ttu-id="91ee2-143">Может потребоваться изменить производственную мощность ресурсов.</span><span class="sxs-lookup"><span data-stu-id="91ee2-143">You may need to change the capacity of resources.</span></span>  
  
1. <span data-ttu-id="91ee2-144">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Производственная мощность ресурсов**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="91ee2-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Capacity**, and then choose the related link.</span></span>  
2. <span data-ttu-id="91ee2-145">Выберите ресурс, затем выберите действие **Установить произв. мощность**.</span><span class="sxs-lookup"><span data-stu-id="91ee2-145">Choose the resource, and then choose the **Set Capacity** action.</span></span>  
3. <span data-ttu-id="91ee2-146">Внесите изменения, затем выберите **Обновить произв. мощность**.</span><span class="sxs-lookup"><span data-stu-id="91ee2-146">Make the changes, and then choose **Update Capacity**.</span></span>  

## <a name="to-update-skills-for-items-service-items-or-service-item-groups"></a><span data-ttu-id="91ee2-147">Обновление квалификации для товаров, сервисных товаров или групп сервисных товаров</span><span class="sxs-lookup"><span data-stu-id="91ee2-147">To update skills for items, service items, or service item groups</span></span>
<span data-ttu-id="91ee2-148">Если нужно изменить коды квалификации, назначенные товарам, например с **ПЦ** на **ППК**, это можно сделать для товара, сервисного товара или всех товаров в группе сервисных товаров.</span><span class="sxs-lookup"><span data-stu-id="91ee2-148">If you want to change the skill codes assigned to items, for example from **PC** to **PCS**, you can do so either for an item, service item, or for all items in a service item group.</span></span>  
  
1. <span data-ttu-id="91ee2-149">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, **Сервисные товары** или **Группа сервисных товаров**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="91ee2-149">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items** or **Service Item**, or **Service Item Group**, and then choose the related link.</span></span>  
2. <span data-ttu-id="91ee2-150">Выберите объект для обновления, затем выберите действие **Квалификация ресурсов**.</span><span class="sxs-lookup"><span data-stu-id="91ee2-150">Choose the entity to update, and then choose the **Resource Skills** action.</span></span>  
3. <span data-ttu-id="91ee2-151">В поле **Код квалификации** строки, в которой нужно изменить код, выберите необходимый код квалификации.</span><span class="sxs-lookup"><span data-stu-id="91ee2-151">On the line with the code to be changed, in the **Skill Code** field, choose the relevant skill code.</span></span>  
4.  <span data-ttu-id="91ee2-152">Если имеются связанные с товаром сервисные товары, откроется следующее диалоговое окно с двумя вариантами действий.</span><span class="sxs-lookup"><span data-stu-id="91ee2-152">If the item has associated service items, a dialog box opens with the following two options:</span></span>  
  
    * <span data-ttu-id="91ee2-153">Изменить коды квалификации на выбранное значение: выберите этот параметр, если требуется заменить существующий код квалификации на новый для всех связанных сервисных товаров.</span><span class="sxs-lookup"><span data-stu-id="91ee2-153">Change the skill codes to the selected value: Select this option if you want to replace the old skill code with the new one on all the related service items.</span></span>  
    * <span data-ttu-id="91ee2-154">Удалить коды квалификации или обновить их связь: выберите это параметр, если требуется изменить код квалификации только для данного товара.</span><span class="sxs-lookup"><span data-stu-id="91ee2-154">Delete the skill codes or update their relation: Select this option if you want to change the skill code on this item only.</span></span> <span data-ttu-id="91ee2-155">Код квалификации связанных сервисных товаров будет переопределен, то есть будет обновлено поле **Кем назначено**.</span><span class="sxs-lookup"><span data-stu-id="91ee2-155">The skill code on the related service items will be reassigned, that is, the **Assigned From** field will be updated.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="91ee2-156">См. также</span><span class="sxs-lookup"><span data-stu-id="91ee2-156">See Also</span></span>
[<span data-ttu-id="91ee2-157">Распределение ресурсов</span><span class="sxs-lookup"><span data-stu-id="91ee2-157">Allocate Resources</span></span>](service-how-to-allocate-resources.md)  
[<span data-ttu-id="91ee2-158">Настройка рабочих часов и часов работы сервиса</span><span class="sxs-lookup"><span data-stu-id="91ee2-158">Set Up Work Hours and Service Hours</span></span>](service-how-setup-work-service-hours.md)  
[<span data-ttu-id="91ee2-159">Настройка отчетности по неисправностям</span><span class="sxs-lookup"><span data-stu-id="91ee2-159">Set Up Fault Reporting</span></span>](service-how-setup-fault-reporting.md)  
[<span data-ttu-id="91ee2-160">Настройка кодов для стандартных сервисов</span><span class="sxs-lookup"><span data-stu-id="91ee2-160">Set Up Codes for Standard Services</span></span>](service-how-setup-service-coding.md)  
 

