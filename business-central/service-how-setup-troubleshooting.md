---
title: Настройка процессов устранения неисправностей | Документация Майкрософт
description: Узнайте, как настраивать процессы, которые помогают представителям по сервисному обслуживанию выявлять и устранять неполадки в сервисных товарах.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, service item, troubleshoot, repairs, maintenance
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 2e962552bf091e095a968f6f312e852e02aad8d6
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3195020"
---
# <a name="setting-up-troubleshooting-for-service-items"></a><span data-ttu-id="d7895-103">Настройка устранения неполадок для сервисных товаров</span><span class="sxs-lookup"><span data-stu-id="d7895-103">Setting Up Troubleshooting for Service Items</span></span>
<span data-ttu-id="d7895-104">Можно настроить руководства по устранению неполадок, которые помогают техническим специалистам устранять проблемы при обслуживании.</span><span class="sxs-lookup"><span data-stu-id="d7895-104">You can set up troubleshooting guidelines that help technicians solve problems when providing service.</span></span> <span data-ttu-id="d7895-105">Например, руководство может являться списком операций при выполнении ремонта или последовательностью вопросов, которые требуется задать о товарах.</span><span class="sxs-lookup"><span data-stu-id="d7895-105">For example, guidelines might be a list of steps to perform a repair, or a series of questions to ask about the items.</span></span> <span data-ttu-id="d7895-106">После настройки руководство по устранению неисправностей их можно назначить группам сервисных товаров, сервисным товарам или товарам.</span><span class="sxs-lookup"><span data-stu-id="d7895-106">After you set up troubleshooting guidelines, you can assign them to service item groups, service items, and items.</span></span> <span data-ttu-id="d7895-107">Для руководств предусмотрена иерархия наследования.</span><span class="sxs-lookup"><span data-stu-id="d7895-107">There is an inheritance hierarchy for guidelines.</span></span> <span data-ttu-id="d7895-108">Если назначить их группе сервисных товаров, включенных в эту группу товары будут наследовать эти руководства, если они не будут указаны для товаров.</span><span class="sxs-lookup"><span data-stu-id="d7895-108">If you assign them to a service item group, the items included in the group will inherit the guidelines unless you specify them for the items.</span></span> <span data-ttu-id="d7895-109">Аналогично, сервисные товары будут наследовать из товаров.</span><span class="sxs-lookup"><span data-stu-id="d7895-109">Similarly, service items will inherit guidelines from items.</span></span>  

## <a name="to-set-up-troubleshooting-guidelines"></a><span data-ttu-id="d7895-110">Настройка руководства по устранению проблем</span><span class="sxs-lookup"><span data-stu-id="d7895-110">To set up troubleshooting guidelines</span></span>
1. <span data-ttu-id="d7895-111">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Устранение проблем**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="d7895-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Troubleshooting**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d7895-112">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="d7895-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-troubleshooting-guidelines-to-items-service-items-or-service-item-groups"></a><span data-ttu-id="d7895-113">Назначение руководств по устранению неполадок товарам, сервисным товарам или группам сервисных товаров</span><span class="sxs-lookup"><span data-stu-id="d7895-113">To assign troubleshooting guidelines to items, service items, or service item groups</span></span>
1. <span data-ttu-id="d7895-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, **Сервисные товары** или **Группы сервисных товаров**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="d7895-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, **Service Items**, or **Service Item Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d7895-115">Выберите соответствующий объект, затем выберите действие **Устранение неполадок**.</span><span class="sxs-lookup"><span data-stu-id="d7895-115">Choose the relevant entity, and then choose the **Troubleshooting** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d7895-116">См. также</span><span class="sxs-lookup"><span data-stu-id="d7895-116">See Also</span></span>
[<span data-ttu-id="d7895-117">Управление сервисом</span><span class="sxs-lookup"><span data-stu-id="d7895-117">Service Management</span></span>](service-service.md)