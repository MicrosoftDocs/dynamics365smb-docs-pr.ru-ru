---
title: Настройка статусов для сервисных заказов и ремонтных работ | Документация Майкрософт
description: Необходимо настроить девять параметров статуса ремонта, которые указывают продвижение ремонта и обслуживания сервисных товаров в сервисных заказах.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 0c4dd1916f60c424d93d4e225aa87830d34a1fff
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3915240"
---
# <a name="set-up-statuses-for-service-orders-and-repairs"></a><span data-ttu-id="1bd26-103">Как настраивать статусы для сервисных заказов и ремонтных работ</span><span class="sxs-lookup"><span data-stu-id="1bd26-103">Set Up Statuses for Service Orders and Repairs</span></span>
<span data-ttu-id="1bd26-104">Необходимо настроить параметры статуса ремонта, которые указывают продвижение ремонта и обслуживания сервисных товаров в сервисных заказах.</span><span class="sxs-lookup"><span data-stu-id="1bd26-104">You must set up repair status options that identify the progress of repair and maintenance of service items in service orders.</span></span> <span data-ttu-id="1bd26-105">Необходимо настроить по крайней мере девять параметров статуса ремонта, указывающих ситуации или действия, производимые с сервисными товарами.</span><span class="sxs-lookup"><span data-stu-id="1bd26-105">You must set up at least nine repair status options that identify situations or actions taken when servicing service items.</span></span>  

<span data-ttu-id="1bd26-106">Можно задать уровень приоритета для параметров статуса сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="1bd26-106">You can set the priority level for service order status options.</span></span> <span data-ttu-id="1bd26-107">Имеется четыре приоритета: "Высокий", "Выше Среднего", "Ниже Среднего" и "Низкий".</span><span class="sxs-lookup"><span data-stu-id="1bd26-107">There four priorities are High, Medium High, Medium Low, and Low.</span></span>  

<span data-ttu-id="1bd26-108">При изменении статуса ремонта сервисного товара в сервисном заказе статус сервисного заказа обновляется.</span><span class="sxs-lookup"><span data-stu-id="1bd26-108">When you change the repair status of a service item in a service order, the service order status is updated.</span></span> <span data-ttu-id="1bd26-109">Статус ремонта каждого сервисного товара связан со статусом сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="1bd26-109">The repair status of each service item is linked to the service order status.</span></span> <span data-ttu-id="1bd26-110">Если сервисные товары связаны с двумя или более параметрами статуса сервисного заказа, то выбирается статус сервисного заказа с наиболее высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="1bd26-110">If the service items are linked to two or more service order status options, the service order status with the highest priority is selected.</span></span>  

## <a name="to-set-up-a-repair-status"></a><span data-ttu-id="1bd26-111">Настройка статуса ремонта</span><span class="sxs-lookup"><span data-stu-id="1bd26-111">To set up a repair status</span></span>  
1. <span data-ttu-id="1bd26-112">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Статус ремонта**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1bd26-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Repair Status**, and then choose the related link.</span></span>
2. <span data-ttu-id="1bd26-113">Создать новый статус ремонта.</span><span class="sxs-lookup"><span data-stu-id="1bd26-113">Create a new repair status.</span></span>  
3. <span data-ttu-id="1bd26-114">Заполните поля **Код** и **Описание**.</span><span class="sxs-lookup"><span data-stu-id="1bd26-114">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="1bd26-115">В поле **Статус сервисного заказа** выберите статус заказа, с которым требуется связать статус ремонта.</span><span class="sxs-lookup"><span data-stu-id="1bd26-115">In the **Service Order Status** field, choose the order status to link the repair status to.</span></span> <span data-ttu-id="1bd26-116">В поле **Приоритет** отображается приоритет выбранного статуса сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="1bd26-116">The **Priority** field displays the priority of the service order status you have chosen.</span></span>  
5. <span data-ttu-id="1bd26-117">Выберите статус ремонта.</span><span class="sxs-lookup"><span data-stu-id="1bd26-117">Choose a repair status.</span></span> <span data-ttu-id="1bd26-118">Можно выбрать только один.</span><span class="sxs-lookup"><span data-stu-id="1bd26-118">You can choose only one.</span></span>  
6. <span data-ttu-id="1bd26-119">Выберите поле **Учет разрешен**, чтобы можно было учитывать сервисные заказы с этим статусом ремонта, включая сервисные товары.</span><span class="sxs-lookup"><span data-stu-id="1bd26-119">To be able to post service orders, including service items, with this repair status, choose the **Posting Allowed** field.</span></span>  
7. <span data-ttu-id="1bd26-120">Выберите флажок **Статус ожидания разрешен**, чтобы иметь возможность менять вручную параметр статуса сервисного заказа на **Ожидание** в сервисных заказах с этим статусом ремонта, включая сервисные товары.</span><span class="sxs-lookup"><span data-stu-id="1bd26-120">To be able to manually change the service order status option to **Pending** in service orders including service items with this repair status, choose the **Pending Status Allowed** check box.</span></span>  
8. <span data-ttu-id="1bd26-121">Выберите флажки **Статус В работе разрешен**, **Статус Завершено разрешен** и **Статус На удержании разрешен** таким же образом.</span><span class="sxs-lookup"><span data-stu-id="1bd26-121">Choose the **In Process Status Allowed**, **Finished Status Allowed**, and **On Hold Status Allowed** check boxes in the same way.</span></span>
  
## <a name="to-set-up-service-status-priorities"></a><span data-ttu-id="1bd26-122">Настройка приоритетов сервисных статусов</span><span class="sxs-lookup"><span data-stu-id="1bd26-122">To set up service status priorities</span></span>  
1. <span data-ttu-id="1bd26-123">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Статус сервисного заказа**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1bd26-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Order Status**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1bd26-124">Выберите статус сервисного заказа, которому необходимо назначить приоритет.</span><span class="sxs-lookup"><span data-stu-id="1bd26-124">Select the service order status you want to set a priority for.</span></span>  
3. <span data-ttu-id="1bd26-125">В поле **Приоритет** выберите тот приоритет, который хотите назначить этому статусу сервисного заказа.</span><span class="sxs-lookup"><span data-stu-id="1bd26-125">In the **Priority** field, choose the priority you want for this service order status.</span></span> <span data-ttu-id="1bd26-126">Повторите этот шаг для каждого статуса.</span><span class="sxs-lookup"><span data-stu-id="1bd26-126">Repeat this step for each status.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1bd26-127">См. также</span><span class="sxs-lookup"><span data-stu-id="1bd26-127">See Also</span></span>  
[<span data-ttu-id="1bd26-128">Статус сервисного заказа и ремонта</span><span class="sxs-lookup"><span data-stu-id="1bd26-128">Service Order Status and Repair Status</span></span>](service-service-order-status-and-repair-status.md)  
[<span data-ttu-id="1bd26-129">Настройка управления сервисным обслуживанием</span><span class="sxs-lookup"><span data-stu-id="1bd26-129">Setting Up Service Management</span></span>](service-setup-service.md)  
