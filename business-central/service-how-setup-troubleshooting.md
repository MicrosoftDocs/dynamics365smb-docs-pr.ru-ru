---
title: "Настройка процессов устранения неисправностей | Документы Майкрософт"
description: "Узнайте, как настраивать процессы, которые помогают представителям по сервисному обслуживанию выявлять и устранять неполадки в сервисных товарах."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, service item, troubleshoot, repairs, maintenance
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 24a4fa9811547acfd3372d3eaf7de7b9f1882c7d
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---

# <a name="setting-up-troubleshooting-for-service-items"></a><span data-ttu-id="6c86a-103">Настройка устранения неполадок для сервисных товаров</span><span class="sxs-lookup"><span data-stu-id="6c86a-103">Setting Up Troubleshooting for Service Items</span></span>
<span data-ttu-id="6c86a-104">Можно настроить руководства по устранению неполадок, которые помогают техническим специалистам устранять проблемы при обслуживании.</span><span class="sxs-lookup"><span data-stu-id="6c86a-104">You can set up troubleshooting guidelines that help technicians solve problems when providing service.</span></span> <span data-ttu-id="6c86a-105">Например, руководство может являться списком операций при выполнении ремонта или последовательностью вопросов, которые требуется задать о товарах.</span><span class="sxs-lookup"><span data-stu-id="6c86a-105">For example, guidelines might be a list of steps to perform a repair, or a series of questions to ask about the items.</span></span> <span data-ttu-id="6c86a-106">После настройки руководство по устранению неисправностей их можно назначить группам сервисных товаров, сервисным товарам или товарам.</span><span class="sxs-lookup"><span data-stu-id="6c86a-106">After you set up troubleshooting guidelines, you can assign them to service item groups, service items, and items.</span></span> <span data-ttu-id="6c86a-107">Для руководств предусмотрена иерархия наследования.</span><span class="sxs-lookup"><span data-stu-id="6c86a-107">There is an inheritance hierarchy for guidelines.</span></span> <span data-ttu-id="6c86a-108">Если назначить их группе сервисных товаров, включенных в эту группу товары будут наследовать эти руководства, если они не будут указаны для товаров.</span><span class="sxs-lookup"><span data-stu-id="6c86a-108">If you assign them to a service item group, the items included in the group will inherit the guidelines unless you specify them for the items.</span></span> <span data-ttu-id="6c86a-109">Аналогично, сервисные товары будут наследовать из товаров.</span><span class="sxs-lookup"><span data-stu-id="6c86a-109">Similarly, service items will inherit guidelines from items.</span></span>  

## <a name="to-set-up-troubleshooting-guidelines"></a><span data-ttu-id="6c86a-110">Настройка руководства по устранению проблем</span><span class="sxs-lookup"><span data-stu-id="6c86a-110">To set up troubleshooting guidelines</span></span>
1. <span data-ttu-id="6c86a-111">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Устранение неполадок**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6c86a-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Troubleshooting**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6c86a-112">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="6c86a-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-troubleshooting-guidelines-to-items-service-items-or-service-item-groups"></a><span data-ttu-id="6c86a-113">Назначение руководств по устранению неполадок товарам, сервисным товарам или группам сервисных товаров</span><span class="sxs-lookup"><span data-stu-id="6c86a-113">To assign troubleshooting guidelines to items, service items, or service item groups</span></span>
1. <span data-ttu-id="6c86a-114">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, **Сервисные товары** или **Группы сервисных товаров**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6c86a-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, **Service Items**, or **Service Item Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6c86a-115">Выберите соответствующий объект, затем выберите действие **Устранение неполадок**.</span><span class="sxs-lookup"><span data-stu-id="6c86a-115">Choose the relevant entity, and then choose the **Troubleshooting** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6c86a-116">См. также</span><span class="sxs-lookup"><span data-stu-id="6c86a-116">See Also</span></span>
[<span data-ttu-id="6c86a-117">Сервисный центр</span><span class="sxs-lookup"><span data-stu-id="6c86a-117">Service Management</span></span>](service-service.md)
