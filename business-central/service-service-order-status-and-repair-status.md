---
title: Статус сервисного заказа и ремонта
description: Поле "Статус" на странице "Сервисный заказ" и статус ремонта сервисного товара, представленный полем "Код статуса ремонта" на странице "Сервисный заказ", имеют определенную взаимозависимость в области приложения "Сервисное управление". Статус сервисного заказа отражает статус ремонта всех сервисных товаров данного сервисного заказа.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/15/2020
ms.author: edupont
ms.openlocfilehash: 9bbe3a4263250a7d06bfffa2019114eba72a31ca
ms.sourcegitcommit: 2d2dfb6c3eca1322835f0167dc7dab614346972e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2020
ms.locfileid: "4038622"
---
# <a name="service-order-status-and-repair-status"></a><span data-ttu-id="85792-104">Статус сервисного заказа и ремонта</span><span class="sxs-lookup"><span data-stu-id="85792-104">Service Order Status and Repair Status</span></span>

<span data-ttu-id="85792-105">Поле **Статус** на странице **Сервисный заказ** и статус ремонта сервисного товара, представленный полем **Код статуса ремонта** на странице **Сервисный заказ**, имеют определенную взаимозависимость в области приложения "Сервисное управление".</span><span class="sxs-lookup"><span data-stu-id="85792-105">The **Status** field on the **Service Order** page and the service item repair status, which is represented by the **Repair Status Code** field on the **Service Order** page have a certain relationship in Service Management.</span></span> <span data-ttu-id="85792-106">Статус сервисного заказа отражает статус ремонта всех сервисных товаров данного сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="85792-106">The service order status reflects the repair status of all the service items in the service order.</span></span>  

> [!NOTE]  
> <span data-ttu-id="85792-107">Эти два поля статуса не связаны с полем **Статус выпуска** в заголовке сервисного заказа, который управляет обработкой сервисных товаров на складе.</span><span class="sxs-lookup"><span data-stu-id="85792-107">These two status field are not related to the **Release Status** field on the service order header, which determines how the warehouse handles service items.</span></span>  

<span data-ttu-id="85792-108">При каждом изменении статуса ремонта сервисного товара в сервисном заказе его статус обновляется.</span><span class="sxs-lookup"><span data-stu-id="85792-108">Each time the repair status of a service item is changed in a service order, the status of the order is updated.</span></span> <span data-ttu-id="85792-109">Чтобы отобразить общий статус ремонта отдельных сервисных товаров, следует определить следующее:</span><span class="sxs-lookup"><span data-stu-id="85792-109">To display the status that reflects the overall repair status of the individual service items, you must specify the following:</span></span>  

* <span data-ttu-id="85792-110">Статус сервисного заказа, с которым связан статус ремонта.</span><span class="sxs-lookup"><span data-stu-id="85792-110">The service order status that each repair status is linked to.</span></span>  
* <span data-ttu-id="85792-111">Уровень приоритета каждого параметра статуса сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="85792-111">The level of priority of each service order status option.</span></span>  

<span data-ttu-id="85792-112">При преобразовании сервисного предложения в сервисный заказ статус ремонта каждого сервисного товара в заказе меняется на **Начальный**, а статус сервисного заказа меняется на **Ожидание**.</span><span class="sxs-lookup"><span data-stu-id="85792-112">When you convert a service quote to a service order, the repair status of each service item is changed in the order to **Initial** and the service order status is changed to **Pending**.</span></span>  

> [!NOTE]
> <span data-ttu-id="85792-113">Перед созданием заказов на обслуживание необходимо настроить статусы ремонта и приоритеты статусов обслуживания.</span><span class="sxs-lookup"><span data-stu-id="85792-113">Before you can create service orders, you must set up repair statuses and service status priorities.</span></span> <span data-ttu-id="85792-114">Дополнительные сведения см. в разделе [Настройка статусов для сервисных заказов и ремонтных работ](service-order-repair-status.md).</span><span class="sxs-lookup"><span data-stu-id="85792-114">For more information, see [Set Up Statuses for Service Orders and Repairs](service-order-repair-status.md).</span></span>

## <a name="specifying-service-order-status-for-repair-status"></a><span data-ttu-id="85792-115">Указание статуса сервисного заказа для определения статуса ремонта</span><span class="sxs-lookup"><span data-stu-id="85792-115">Specifying Service Order Status for Repair Status</span></span>

<span data-ttu-id="85792-116">Каждый статус ремонта связан с определённым статусом сервисного заказа. Параметры статуса сервисного заказа:</span><span class="sxs-lookup"><span data-stu-id="85792-116">Each repair status is linked to a particular service order status.</span></span> <span data-ttu-id="85792-117">Возможны следующие варианты статуса заказа на обслуживание:</span><span class="sxs-lookup"><span data-stu-id="85792-117">The options for the service order status are as follows:</span></span>

* <span data-ttu-id="85792-118">**Ожидание**</span><span class="sxs-lookup"><span data-stu-id="85792-118">**Pending**</span></span>
* <span data-ttu-id="85792-119">**В работе**</span><span class="sxs-lookup"><span data-stu-id="85792-119">**In Process**</span></span>
* <span data-ttu-id="85792-120">**На удержании**</span><span class="sxs-lookup"><span data-stu-id="85792-120">**On Hold**</span></span>
* <span data-ttu-id="85792-121">**Завершен**</span><span class="sxs-lookup"><span data-stu-id="85792-121">**Finished**</span></span>

<span data-ttu-id="85792-122">Возможны следующие варианты статуса ремонта:</span><span class="sxs-lookup"><span data-stu-id="85792-122">The repair status options are as follows:</span></span>

* <span data-ttu-id="85792-123">**Начальное**</span><span class="sxs-lookup"><span data-stu-id="85792-123">**Initial**</span></span>
* <span data-ttu-id="85792-124">**В работе**</span><span class="sxs-lookup"><span data-stu-id="85792-124">**In Process**</span></span>
* <span data-ttu-id="85792-125">**Ссылается**</span><span class="sxs-lookup"><span data-stu-id="85792-125">**Referred**</span></span>
* <span data-ttu-id="85792-126">**Частично обслужено**</span><span class="sxs-lookup"><span data-stu-id="85792-126">**Partly Serviced**</span></span>
* <span data-ttu-id="85792-127">**Предложение завершено**</span><span class="sxs-lookup"><span data-stu-id="85792-127">**Quote Finished**</span></span>
* <span data-ttu-id="85792-128">**Ожидание клиента**</span><span class="sxs-lookup"><span data-stu-id="85792-128">**Waiting for Customer**</span></span>
* <span data-ttu-id="85792-129">**Запчасти заказаны**</span><span class="sxs-lookup"><span data-stu-id="85792-129">**Spare Part Ordered**</span></span>
* <span data-ttu-id="85792-130">**Запчасти получены**</span><span class="sxs-lookup"><span data-stu-id="85792-130">**Spare Part Received**</span></span>
* <span data-ttu-id="85792-131">**Завершен**</span><span class="sxs-lookup"><span data-stu-id="85792-131">**Finished**</span></span>  

### <a name="pending"></a><span data-ttu-id="85792-132">Ожидание</span><span class="sxs-lookup"><span data-stu-id="85792-132">Pending</span></span>

<span data-ttu-id="85792-133">Статус сервисного заказа **Ожидание** указывает, что обслуживание может начаться или продолжиться в любое время.</span><span class="sxs-lookup"><span data-stu-id="85792-133">The service order status **Pending** indicates that the service can start or continue at any time.</span></span> <span data-ttu-id="85792-134">Поэтому параметры статуса ремонта **Начальный**, **Ссылается**, **Частично обслужен** и **Запчасти получены** могут быть связаны с этим статусом сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="85792-134">Therefore, the repair status options of **Initial**, **Referred**, **Partly Serviced**, and **Spare Part Received** can be linked to this service order status.</span></span>  

### <a name="in-process"></a><span data-ttu-id="85792-135">В работе</span><span class="sxs-lookup"><span data-stu-id="85792-135">In Process</span></span>

<span data-ttu-id="85792-136">Статус сервисного заказа **В работе** указывает, что идет процесс обслуживания.</span><span class="sxs-lookup"><span data-stu-id="85792-136">The service order status **In Process** indicates that the service is in process.</span></span> <span data-ttu-id="85792-137">Поэтому параметры статуса ремонта **В работе** и **Запчасти заказаны** могут быть связаны с этим статусом сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="85792-137">Therefore, the repair status options **In Process** and **Spare Part Ordered** can both be linked to this service order status.</span></span> <span data-ttu-id="85792-138">Если статус **Запчасти заказаны** связывается со статусом **В работе**, то статус **Запчасти получены** следует также связать с этим статусом сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="85792-138">If you link the **Spare Part Ordered** status to an **In Process** service order status, you must also link the **Spare Part Received** status to this service order status.</span></span>  

### <a name="on-hold"></a><span data-ttu-id="85792-139">На удержании</span><span class="sxs-lookup"><span data-stu-id="85792-139">On Hold</span></span>

<span data-ttu-id="85792-140">Статус сервисного заказа **На удержании** указывает, что обслуживание временно задержано, потому что вы ждете ответа клиента или запчастей, чтобы начать обслуживание.</span><span class="sxs-lookup"><span data-stu-id="85792-140">The service order status **On Hold** indicates that the service is temporarily on hold because you are waiting for a customer response or spare parts before the service can start.</span></span> <span data-ttu-id="85792-141">Поэтому параметры статуса ремонта **Предложение завершено**, **Запчасти заказаны** и **Ожидание клиента** могут быть связаны с этим статусом сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="85792-141">Therefore, the repair status options of **Quote Finished**, **Spare Part Ordered**, and **Waiting for Customer** can be linked to this service order status.</span></span>  

### <a name="finished"></a><span data-ttu-id="85792-142">Завершен</span><span class="sxs-lookup"><span data-stu-id="85792-142">Finished</span></span>

<span data-ttu-id="85792-143">Статус сервисного заказа **Завершен** указывает, что сервис выполнен.</span><span class="sxs-lookup"><span data-stu-id="85792-143">The service order status **Finished** indicates that the service has been completed.</span></span> <span data-ttu-id="85792-144">Поэтому статус ремонта **Завершен** связан с этим статусом.</span><span class="sxs-lookup"><span data-stu-id="85792-144">Therefore, the **Finished** repair status is linked to this status.</span></span>  

## <a name="assigning-priority-to-service-order-status"></a><span data-ttu-id="85792-145">Назначение приоритета со статусом сервисного заказа</span><span class="sxs-lookup"><span data-stu-id="85792-145">Assigning Priority to Service Order Status</span></span>

<span data-ttu-id="85792-146">Если меняется статус ремонта сервисного товара, то определяются параметры статуса сервисного заказа, связанные с разными параметрами статуса ремонта всех сервисных товаров в заказе.</span><span class="sxs-lookup"><span data-stu-id="85792-146">When a repair status of a service item is changed, the service order status options linked to the different repair status options of all the service items in the order are identified.</span></span> <span data-ttu-id="85792-147">Если сервисные товары связаны с двумя или более параметрами статуса сервисного заказа, то выбирается статус сервисного заказа с наиболее высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="85792-147">If the service items are linked to two or more service order status options, the service order status option with the highest priority is selected.</span></span>  

<span data-ttu-id="85792-148">Вы должны решить, какой статус сервисного заказа содержит наиболее важную информацию о статусе сервисного заказа и назначить этому статусу наивысший приоритет, и т.д.</span><span class="sxs-lookup"><span data-stu-id="85792-148">You must decide which service order status contains the most important information about the status of the service order and assign that status the highest priority, and so on.</span></span>  

<span data-ttu-id="85792-149">Затем, когда вы создаете новый сервисный заказ и добавляете в него сервисные позиции, поле **Приоритет** в заголовке заказа на обслуживание обновляется на основе приоритетов для позиций обслуживания.</span><span class="sxs-lookup"><span data-stu-id="85792-149">Then, when you create a new service order and you add service items to it, the **Priority** field on the service order header is updated based on the priorities on the service items.</span></span>  

### <a name="example"></a><span data-ttu-id="85792-150">Пример</span><span class="sxs-lookup"><span data-stu-id="85792-150">Example</span></span>

<span data-ttu-id="85792-151">Типичное распределение уровней приоритета может быть следующим:</span><span class="sxs-lookup"><span data-stu-id="85792-151">A typical priority level assignment could be as follows:</span></span>  

* <span data-ttu-id="85792-152">«В работе» - «Высокий»</span><span class="sxs-lookup"><span data-stu-id="85792-152">In Process - High</span></span>  
* <span data-ttu-id="85792-153">"Ожидание" – "Выше среднего"</span><span class="sxs-lookup"><span data-stu-id="85792-153">Pending - Medium high</span></span>  
* <span data-ttu-id="85792-154">"На удержании" – "Ниже среднего"</span><span class="sxs-lookup"><span data-stu-id="85792-154">On Hold - Medium low</span></span>  
* <span data-ttu-id="85792-155">«Завершён» - «Низкий»</span><span class="sxs-lookup"><span data-stu-id="85792-155">Finished - Low</span></span>  

<span data-ttu-id="85792-156">Например, если один сервисный товар имеет статус ремонта **Начальный** (связанный со статусом сервисного заказа **Ожидание**), другой - **В работе** (связанный со статусом сервисного заказа **В работе**), а третий – **Запчасти заказаны** (связанный со статусом сервисного заказа **На удержании**), то тогда окончательный статус сервисного заказа будет **В работе**, поскольку он имеет наивысший приоритет.</span><span class="sxs-lookup"><span data-stu-id="85792-156">For example, if one service item has the repair status **Initial**, linked to the service order status **Pending**, another has the repair status **In Process**, linked to the service order status **In Process**, and a third has the repair status **Spare Part Ordered**, linked to the service order status **On Hold**, the resulting service order status will be **In Process** because this has the highest priority.</span></span>  

## <a name="see-also"></a><span data-ttu-id="85792-157">См. также</span><span class="sxs-lookup"><span data-stu-id="85792-157">See Also</span></span>

[<span data-ttu-id="85792-158">Настройка статусов для сервисных заказов и ремонтных работ</span><span class="sxs-lookup"><span data-stu-id="85792-158">Set Up Statuses for Service Orders and Repairs</span></span>](service-order-repair-status.md)  
[<span data-ttu-id="85792-159">Настройка управления сервисным обслуживанием</span><span class="sxs-lookup"><span data-stu-id="85792-159">Setting Up Service Management</span></span>](service-setup-service.md)  
