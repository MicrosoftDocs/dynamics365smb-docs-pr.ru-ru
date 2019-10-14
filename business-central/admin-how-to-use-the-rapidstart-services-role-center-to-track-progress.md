---
title: Использование ролевого центра "Внедряющий мастер служб RapidStart Services" | Документация Майкрософт
description: При использовании служб RapidStart Services рекомендуется отслеживать свою работу и использовать ролевой центр «Внедряющий мастер служб RapidStart Services», так как он предоставляет правильный контекст для вашей работы по конфигурации.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: /dynamics365/business-central/admin-set-up-company-configuration
ROBOTS: NOINDEX
ms.openlocfilehash: 908e460ae5a3fc8ecb804f27363a1cfad71d997c
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2307929"
---
# <a name="use-the-rapidstart-services-implementer-role-center"></a><span data-ttu-id="8fab3-103">Использование ролевого центра «Внедряющий мастер служб RapidStart Services»</span><span class="sxs-lookup"><span data-stu-id="8fab3-103">Use the RapidStart Services Implementer Role Center</span></span>
<span data-ttu-id="8fab3-104">При использовании служб RapidStart Services рекомендуется использовать ролевой центр «Внедряющий мастер служб RapidStart Services», так как он предоставляет правильный контекст для вашей работы по конфигурации.</span><span class="sxs-lookup"><span data-stu-id="8fab3-104">When you use RapidStart Services, we recommend that you use the RapidStart Services Implementer Role Center as it provides the correct context for your configuration work.</span></span> <span data-ttu-id="8fab3-105">Дополнительные сведения см. в разделе [Изменение роли](ui-change-basic-settings.md#to-change-the-role).</span><span class="sxs-lookup"><span data-stu-id="8fab3-105">For more information, see [To change the role](ui-change-basic-settings.md#to-change-the-role).</span></span>

<span data-ttu-id="8fab3-106">Во время работы вы можете назначить каждой таблице статус, который отражает текущее состояние работ.</span><span class="sxs-lookup"><span data-stu-id="8fab3-106">As you continue with your work, you can assign each table the status that reflects where you are in the process.</span></span> <span data-ttu-id="8fab3-107">В этом случае [!INCLUDE[d365fin](includes/d365fin_md.md)] отслеживает статус таблицы в части **Действия** в ролевом центре.</span><span class="sxs-lookup"><span data-stu-id="8fab3-107">[!INCLUDE[d365fin](includes/d365fin_md.md)] then keeps track of the table status in the **Activities** part on the Role Center.</span></span>  

<span data-ttu-id="8fab3-108">По умолчанию при добавлении таблицы в журнал конфигураций ее статус устанавливается пустым.</span><span class="sxs-lookup"><span data-stu-id="8fab3-108">By default, when you add a table to the configuration worksheet, its status is set to blank.</span></span> <span data-ttu-id="8fab3-109">Это означает, что конфигурация таблицы не началась.</span><span class="sxs-lookup"><span data-stu-id="8fab3-109">This means that configuration of the table has not begun.</span></span> <span data-ttu-id="8fab3-110">Это отражено в количестве **Не запущено** на плитке **Действия**.</span><span class="sxs-lookup"><span data-stu-id="8fab3-110">This is reflected in the **Not Started** count in the **Activities** tile.</span></span>  

## <a name="to-update-the-status-of-a-configuration-table"></a><span data-ttu-id="8fab3-111">Обновление статуса таблицы конфигурации</span><span class="sxs-lookup"><span data-stu-id="8fab3-111">To update the status of a configuration table</span></span>  
1.  <span data-ttu-id="8fab3-112">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал конфигураций**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="8fab3-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8fab3-113">Выберите действие **Изменить список**.</span><span class="sxs-lookup"><span data-stu-id="8fab3-113">Choose the **Edit List** action.</span></span>  
3.  <span data-ttu-id="8fab3-114">Выберите таблицу, а затем в поле **Статус** выберите подходящий статус.</span><span class="sxs-lookup"><span data-stu-id="8fab3-114">Select a table, and in the **Status** field, choose the appropriate status.</span></span>  
4.  <span data-ttu-id="8fab3-115">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="8fab3-115">Choose the **OK** button.</span></span>  

<span data-ttu-id="8fab3-116">При возврате в ролевой центр плитки в части **Действия** обновляются, чтобы отразить внесенные изменения.</span><span class="sxs-lookup"><span data-stu-id="8fab3-116">When you return to the Role Center, the tiles in the **Activities** part are updated to reflect your changes.</span></span>  

## <a name="to-track-the-status-of-a-configuration-project"></a><span data-ttu-id="8fab3-117">Трассировка статуса проекта конфигурации</span><span class="sxs-lookup"><span data-stu-id="8fab3-117">To track the status of a configuration project</span></span>  
- <span data-ttu-id="8fab3-118">Откройте ролевой центр RapidStart Services.</span><span class="sxs-lookup"><span data-stu-id="8fab3-118">Open the RapidStart Services Role Center.</span></span>  

<span data-ttu-id="8fab3-119">В разделе **Области конфигурации** отображается статистику завершения для областей и групп, которые вы настроили.</span><span class="sxs-lookup"><span data-stu-id="8fab3-119">In the **Configuration Areas** part, completion statistics are shown for the areas and groups that you have set up.</span></span> <span data-ttu-id="8fab3-120">Если не были заданы области или группы, то в этой части данные отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8fab3-120">If you have not set up any groups or areas, this part has no data.</span></span>  

## <a name="to-see-a-filtered-view-of-table-status"></a><span data-ttu-id="8fab3-121">Просмотр отфильтрованного представления статуса таблицы</span><span class="sxs-lookup"><span data-stu-id="8fab3-121">To see a filtered view of table status</span></span>  
1. <span data-ttu-id="8fab3-122">Выберите действие **Таблицы**.</span><span class="sxs-lookup"><span data-stu-id="8fab3-122">Choose the **Tables** action.</span></span>  
2. <span data-ttu-id="8fab3-123">Выберите подходящее представление с фильтром.</span><span class="sxs-lookup"><span data-stu-id="8fab3-123">Select the appropriate filtered view.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8fab3-124">См. также</span><span class="sxs-lookup"><span data-stu-id="8fab3-124">See Also</span></span>  
[<span data-ttu-id="8fab3-125">Настройка организации со службами RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="8fab3-125">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="8fab3-126">Администрация</span><span class="sxs-lookup"><span data-stu-id="8fab3-126">Administration</span></span>](admin-setup-and-administration.md)
