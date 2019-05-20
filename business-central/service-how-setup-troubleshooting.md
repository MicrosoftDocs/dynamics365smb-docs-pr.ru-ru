---
title: Настройка процессов устранения неисправностей | Документы Майкрософт
description: Узнайте, как настраивать процессы, которые помогают представителям по сервисному обслуживанию выявлять и устранять неполадки в сервисных товарах.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, service item, troubleshoot, repairs, maintenance
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 2dfa02f0054cab20605281bb1cc580b522b893fd
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1251266"
---
# <a name="setting-up-troubleshooting-for-service-items"></a><span data-ttu-id="fb47f-103">Настройка устранения неполадок для сервисных товаров</span><span class="sxs-lookup"><span data-stu-id="fb47f-103">Setting Up Troubleshooting for Service Items</span></span>
<span data-ttu-id="fb47f-104">Можно настроить руководства по устранению неполадок, которые помогают техническим специалистам устранять проблемы при обслуживании.</span><span class="sxs-lookup"><span data-stu-id="fb47f-104">You can set up troubleshooting guidelines that help technicians solve problems when providing service.</span></span> <span data-ttu-id="fb47f-105">Например, руководство может являться списком операций при выполнении ремонта или последовательностью вопросов, которые требуется задать о товарах.</span><span class="sxs-lookup"><span data-stu-id="fb47f-105">For example, guidelines might be a list of steps to perform a repair, or a series of questions to ask about the items.</span></span> <span data-ttu-id="fb47f-106">После настройки руководство по устранению неисправностей их можно назначить группам сервисных товаров, сервисным товарам или товарам.</span><span class="sxs-lookup"><span data-stu-id="fb47f-106">After you set up troubleshooting guidelines, you can assign them to service item groups, service items, and items.</span></span> <span data-ttu-id="fb47f-107">Для руководств предусмотрена иерархия наследования.</span><span class="sxs-lookup"><span data-stu-id="fb47f-107">There is an inheritance hierarchy for guidelines.</span></span> <span data-ttu-id="fb47f-108">Если назначить их группе сервисных товаров, включенных в эту группу товары будут наследовать эти руководства, если они не будут указаны для товаров.</span><span class="sxs-lookup"><span data-stu-id="fb47f-108">If you assign them to a service item group, the items included in the group will inherit the guidelines unless you specify them for the items.</span></span> <span data-ttu-id="fb47f-109">Аналогично, сервисные товары будут наследовать из товаров.</span><span class="sxs-lookup"><span data-stu-id="fb47f-109">Similarly, service items will inherit guidelines from items.</span></span>  

## <a name="to-set-up-troubleshooting-guidelines"></a><span data-ttu-id="fb47f-110">Настройка руководства по устранению проблем</span><span class="sxs-lookup"><span data-stu-id="fb47f-110">To set up troubleshooting guidelines</span></span>
1. <span data-ttu-id="fb47f-111">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Устранение неполадок**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fb47f-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Troubleshooting**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fb47f-112">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="fb47f-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-troubleshooting-guidelines-to-items-service-items-or-service-item-groups"></a><span data-ttu-id="fb47f-113">Назначение руководств по устранению неполадок товарам, сервисным товарам или группам сервисных товаров</span><span class="sxs-lookup"><span data-stu-id="fb47f-113">To assign troubleshooting guidelines to items, service items, or service item groups</span></span>
1. <span data-ttu-id="fb47f-114">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, **Сервисные товары** или **Группы сервисных товаров**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fb47f-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, **Service Items**, or **Service Item Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fb47f-115">Выберите соответствующий объект, затем выберите действие **Устранение неполадок**.</span><span class="sxs-lookup"><span data-stu-id="fb47f-115">Choose the relevant entity, and then choose the **Troubleshooting** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fb47f-116">См. также</span><span class="sxs-lookup"><span data-stu-id="fb47f-116">See Also</span></span>
[<span data-ttu-id="fb47f-117">Сервисный центр</span><span class="sxs-lookup"><span data-stu-id="fb47f-117">Service Management</span></span>](service-service.md)