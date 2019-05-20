---
title: Управление сервисным обслуживанием | Документы Майкрософт
description: Узнайте, как использовать функции, предназначенные для поддержки операций ремонтной мастерской и выездного обслуживания.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: bd37d6f2364ec1466e7d3d8769da13761587f1d8
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1251657"
---
# <a name="service-management"></a><span data-ttu-id="9cc5f-103">Сервисный центр</span><span class="sxs-lookup"><span data-stu-id="9cc5f-103">Service Management</span></span>
> [!NOTE]
> <span data-ttu-id="9cc5f-104">Функциональная возможность, описанная в этом разделе и его подразделах, отображается в пользовательском университете только при наличии функционального уровня **Premium**.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-104">Functionality described in this topic and sub topics is only visible in the user interface if you have the **Premium** experience.</span></span> <span data-ttu-id="9cc5f-105">Дополнительные сведения см. в разделе [Изменение набора отображаемых функций](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="9cc5f-105">For more information, see [Changing Which Features are Displayed](ui-experiences.md).</span></span>

<span data-ttu-id="9cc5f-106">Предоставление текущего обслуживания клиентам является важной составляющей любого бизнеса и одним из источников, способствующих повышению степени лояльности и удовлетворенности клиентов, в дополнение к прибыли.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-106">Providing ongoing service to customers is an important part of any business and one that can be a source of customer satisfaction and loyalty, in addition to revenue.</span></span> <span data-ttu-id="9cc5f-107">Однако управление и трассировку служб не всегда легко выполнять, поэтому в [!INCLUDE[d365fin](includes/d365fin_md.md)] предусмотрен набор вспомогательных инструментов.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-107">However, managing and tracking service is not always easy, and [!INCLUDE[d365fin](includes/d365fin_md.md)] provides a set of tools to help.</span></span> <span data-ttu-id="9cc5f-108">Эти средства предназначены для поддержки работы в условиях ремонтных мастерских и технического обслуживания в условиях эксплуатации. Их можно применять в таких бизнес-сценариях, как сложные системы сервисного обслуживания клиентов, обслуживание в процессе эксплуатации на производстве с применением спецификаций и оперативное управление работой большого числа технических специалистов с применением требований к управлению запчастями.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-108">These tools are designed to support repair shop and field service operations, and can be used in business scenarios such as complex customer service distribution systems, industrial service environments with bills of materials, and high volume dispatching of service technicians with requirements for spare parts management.</span></span>  

 <span data-ttu-id="9cc5f-109">Этими инструментами можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-109">With these tools you can accomplish the following:</span></span>  

* <span data-ttu-id="9cc5f-110">Планирование обращений в отдел обслуживания и настройка сервисных заказов.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-110">Schedule service calls and set up service orders.</span></span>  
* <span data-ttu-id="9cc5f-111">Трассировка запасных частей и поставок</span><span class="sxs-lookup"><span data-stu-id="9cc5f-111">Track repair parts and supplies.</span></span>  
* <span data-ttu-id="9cc5f-112">Назначение обслуживающего персонала на основе данных о квалификации и доступности.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-112">Assign service personnel based on skill and availability.</span></span>  
* <span data-ttu-id="9cc5f-113">Введите сервисные оценки и сервисные счета.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-113">Provide service estimates and service invoices.</span></span>  

<span data-ttu-id="9cc5f-114">Кроме этого, можно стандартизировать кодирование, настроить контракты, внедрить политику скидок и создать карты маршрутов для обслуживающего персонала.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-114">In addition, you can standardize coding, set up contracts, implement a discounting policy, and create route maps for service employees.</span></span>  

<span data-ttu-id="9cc5f-115">В общем случае, существует два аспекта сервисного управления: установка и настройка системы и ее использование для ценообразования, контрактов, заказов, оперативного управления обслуживающим персоналом и планирования задач.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-115">In general, there are two aspects to service management: configuring and setting up your system, and using it for pricing, contracts, orders, service personnel dispatch, and job scheduler.</span></span>  

<span data-ttu-id="9cc5f-116">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="9cc5f-117">**Задача**</span><span class="sxs-lookup"><span data-stu-id="9cc5f-117">**To**</span></span>|<span data-ttu-id="9cc5f-118">**Ссылка**</span><span class="sxs-lookup"><span data-stu-id="9cc5f-118">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="9cc5f-119">Настройка приложения «Сервисное управление», включая коды неисправности, политики, документы и шаблоны по умолчанию</span><span class="sxs-lookup"><span data-stu-id="9cc5f-119">Set up Service Management, including fault codes, policies, default documents and templates.</span></span>|[<span data-ttu-id="9cc5f-120">Настройка управления сервисным обслуживанием</span><span class="sxs-lookup"><span data-stu-id="9cc5f-120">Setting Up Service Management</span></span>](service-setup-service.md)|  
|<span data-ttu-id="9cc5f-121">Управление сервисной ценой, создание сервисных товаров и сведения о порядке мониторинга хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-121">Manage service pricing, create service items, and understand how to monitor progress.</span></span>|[<span data-ttu-id="9cc5f-122">Планирование сервисного обслуживания</span><span class="sxs-lookup"><span data-stu-id="9cc5f-122">Planning Service</span></span>](service-plan-service.md)|  
|<span data-ttu-id="9cc5f-123">Создание и управление контрактными соглашениями между организацией и клиентами.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-123">Create and manage contractual agreements between you and your customers.</span></span>|[<span data-ttu-id="9cc5f-124">Выполнение контрактов на обслуживание</span><span class="sxs-lookup"><span data-stu-id="9cc5f-124">Fulfilling Service Contracts</span></span>](service-fulfill-service-contracts.md)|  
|<span data-ttu-id="9cc5f-125">Предоставление сервисных услуг клиентам и выставление счетов по сервисным заказам.</span><span class="sxs-lookup"><span data-stu-id="9cc5f-125">Provide service to customers, and invoice service orders.</span></span>|[<span data-ttu-id="9cc5f-126">Предоставление услуги</span><span class="sxs-lookup"><span data-stu-id="9cc5f-126">Delivering Service</span></span>](service-deliver-service.md)|  

## <a name="see-also"></a><span data-ttu-id="9cc5f-127">См. также</span><span class="sxs-lookup"><span data-stu-id="9cc5f-127">See Also</span></span>  
<span data-ttu-id="9cc5f-128">[Управление дебиторской задолженностью](receivables-manage-receivables.md) </span><span class="sxs-lookup"><span data-stu-id="9cc5f-128">[Managing Receivables](receivables-manage-receivables.md) </span></span>  
<span data-ttu-id="9cc5f-129">[Работы](projects-how-create-jobs.md) </span><span class="sxs-lookup"><span data-stu-id="9cc5f-129">[Jobs](projects-how-create-jobs.md) </span></span>  
<span data-ttu-id="9cc5f-130">[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] ](index.md)</span><span class="sxs-lookup"><span data-stu-id="9cc5f-130">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] ](index.md)</span></span>

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
