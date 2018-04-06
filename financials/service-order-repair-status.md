---
title: "Настройка статусов для сервисных заказов и ремонтных работ | Документы Майкрософт"
description: "Необходимо настроить девять параметров статуса ремонта, которые указывают продвижение ремонта и обслуживания сервисных товаров в сервисных заказах."
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
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 8ffd5d6893b2b6c8ce7b7377c586f4f5414279b5
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-statuses-for-service-orders-and-repairs"></a><span data-ttu-id="bbc51-103">Как настраивать статусы для сервисных заказов и ремонтных работ</span><span class="sxs-lookup"><span data-stu-id="bbc51-103">Set Up Statuses for Service Orders and Repairs</span></span>
<span data-ttu-id="bbc51-104">Необходимо настроить параметры статуса ремонта, которые указывают продвижение ремонта и обслуживания сервисных товаров в сервисных заказах.</span><span class="sxs-lookup"><span data-stu-id="bbc51-104">You must set up repair status options that identify the progress of repair and maintenance of service items in service orders.</span></span> <span data-ttu-id="bbc51-105">Необходимо настроить по крайней мере девять параметров статуса ремонта, указывающих ситуации или действия, производимые с сервисными товарами.</span><span class="sxs-lookup"><span data-stu-id="bbc51-105">You must set up at least nine repair status options that identify situations or actions taken when servicing service items.</span></span>  

<span data-ttu-id="bbc51-106">Можно задать уровень приоритета для параметров статуса сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="bbc51-106">You can set the priority level for service order status options.</span></span> <span data-ttu-id="bbc51-107">Имеется четыре приоритета: "Высокий", "Выше Среднего", "Ниже Среднего" и "Низкий".</span><span class="sxs-lookup"><span data-stu-id="bbc51-107">There four priorities are High, Medium High, Medium Low, and Low.</span></span>  
  
<span data-ttu-id="bbc51-108">При изменении статуса ремонта сервисного товара в сервисном заказе статус сервисного заказа обновляется.</span><span class="sxs-lookup"><span data-stu-id="bbc51-108">When you change the repair status of a service item in a service order, the service order status is updated.</span></span> <span data-ttu-id="bbc51-109">Статус ремонта каждого сервисного товара связан со статусом сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="bbc51-109">The repair status of each service item is linked to the service order status.</span></span> <span data-ttu-id="bbc51-110">Если сервисные товары связаны с двумя или более параметрами статуса сервисного заказа, то выбирается статус сервисного заказа с наиболее высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="bbc51-110">If the service items are linked to two or more service order status options, the service order status with the highest priority is selected.</span></span>  

## <a name="to-set-up-a-repair-status"></a><span data-ttu-id="bbc51-111">Настройка статуса ремонта</span><span class="sxs-lookup"><span data-stu-id="bbc51-111">To set up a repair status</span></span>  
1. <span data-ttu-id="bbc51-112">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Статус ремонта**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="bbc51-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Repair Status**, and then choose the related link.</span></span> <span data-ttu-id="bbc51-113">2.</span><span class="sxs-lookup"><span data-stu-id="bbc51-113">2.</span></span> <span data-ttu-id="bbc51-114">Создать новый статус ремонта.</span><span class="sxs-lookup"><span data-stu-id="bbc51-114">Create a new repair status.</span></span>  
3. <span data-ttu-id="bbc51-115">Заполните поля **Код** и **Описание**.</span><span class="sxs-lookup"><span data-stu-id="bbc51-115">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="bbc51-116">В поле **Статус сервисного заказа** выберите статус заказа, с которым требуется связать статус ремонта.</span><span class="sxs-lookup"><span data-stu-id="bbc51-116">In the **Service Order Status** field, choose the order status to link the repair status to.</span></span> <span data-ttu-id="bbc51-117">В поле **Приоритет** отображается приоритет выбранного статуса сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="bbc51-117">The **Priority** field displays the priority of the service order status you have chosen.</span></span>  
5. <span data-ttu-id="bbc51-118">Выберите статус ремонта.</span><span class="sxs-lookup"><span data-stu-id="bbc51-118">Choose a repair status.</span></span> <span data-ttu-id="bbc51-119">Можно выбрать только один.</span><span class="sxs-lookup"><span data-stu-id="bbc51-119">You can choose only one.</span></span>  
6. <span data-ttu-id="bbc51-120">Выберите поле **Учет разрешен**, чтобы можно было учитывать сервисные заказы с этим статусом ремонта, включая сервисные товары.</span><span class="sxs-lookup"><span data-stu-id="bbc51-120">To be able to post service orders, including service items, with this repair status, choose the **Posting Allowed** field.</span></span>  
7. <span data-ttu-id="bbc51-121">Выберите флажок **Статус ожидания разрешен**, чтобы иметь возможность менять вручную параметр статуса сервисного заказа на **Ожидание** в сервисных заказах с этим статусом ремонта, включая сервисные товары.</span><span class="sxs-lookup"><span data-stu-id="bbc51-121">To be able to manually change the service order status option to **Pending** in service orders including service items with this repair status, choose the **Pending Status Allowed** check box.</span></span>  
8. <span data-ttu-id="bbc51-122">Выберите флажки **Статус В работе разрешен**, **Статус Завершено разрешен** и **Статус На удержании разрешен** таким же образом.</span><span class="sxs-lookup"><span data-stu-id="bbc51-122">Choose the **In Process Status Allowed**, **Finished Status Allowed**, and **On Hold Status Allowed** check boxes in the same way.</span></span>
  
## <a name="to-set-up-service-status-priorities"></a><span data-ttu-id="bbc51-123">Настройка приоритетов сервисных статусов</span><span class="sxs-lookup"><span data-stu-id="bbc51-123">To set up service status priorities</span></span>  
1. <span data-ttu-id="bbc51-124">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Статус сервисного заказа**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="bbc51-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Order Status**, and then choose the related link.</span></span>  
2. <span data-ttu-id="bbc51-125">Выберите статус сервисного заказа, которому необходимо назначить приоритет.</span><span class="sxs-lookup"><span data-stu-id="bbc51-125">Select the service order status you want to set a priority for.</span></span>  
3. <span data-ttu-id="bbc51-126">В поле **Приоритет** выберите тот приоритет, который хотите назначить этому статусу сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="bbc51-126">In the **Priority** field, choose the priority you want for this service order status.</span></span> <span data-ttu-id="bbc51-127">Повторите этот шаг для каждого статуса.</span><span class="sxs-lookup"><span data-stu-id="bbc51-127">Repeat this step for each status.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="bbc51-128">См. также</span><span class="sxs-lookup"><span data-stu-id="bbc51-128">See Also</span></span>  
[<span data-ttu-id="bbc51-129">Статус сервисного заказа и статус ремонта</span><span class="sxs-lookup"><span data-stu-id="bbc51-129">Understanding Service Order Status and Repair Status</span></span>]()  
[<span data-ttu-id="bbc51-130">Настройка управления сервисным обслуживанием</span><span class="sxs-lookup"><span data-stu-id="bbc51-130">Setting Up Service Management</span></span>](service-setup-service.md)  

