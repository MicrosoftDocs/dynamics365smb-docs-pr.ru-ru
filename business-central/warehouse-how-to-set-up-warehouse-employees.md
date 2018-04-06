---
title: "Как настраивать работников склада | Документы Майкрософт"
description: "Каждый пользователь, который выполняет складские действия, должен быть настроен как работник склада, которому назначен один склад по умолчанию и могут быть назначены другие склады."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: ed9622aae938e4876fc9537702b8f43b84764950
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-warehouse-employees"></a><span data-ttu-id="069d9-103">Настройка работников склада</span><span class="sxs-lookup"><span data-stu-id="069d9-103">Set Up Warehouse Employees</span></span>
<span data-ttu-id="069d9-104">Каждый пользователь, который выполняет складские действия, должен быть настроен как работник склада, которому назначен один склад по умолчанию и могут быть назначены другие склады.</span><span class="sxs-lookup"><span data-stu-id="069d9-104">Each user who performs warehouse activities must be set up as a warehouse employee assigned to one default location and potentially more non-default locations.</span></span> <span data-ttu-id="069d9-105">Данная настройка пользователя фильтрует все складские действия в базе данных по складу сотрудника, чтобы сотрудник мог выполнять складские задачи только для склада по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="069d9-105">This user setup filters all warehouse activities across the database to the employee's location so that the employee can only perform the warehouse activities at the default location.</span></span> <span data-ttu-id="069d9-106">Пользователю могут быть назначены дополнительные нестандартные склады, где работник может просматривать строки задач, но не выполнять их.</span><span class="sxs-lookup"><span data-stu-id="069d9-106">A user can be assigned to additional non-default locations for which the employee can view activity lines but not perform the activities.</span></span>

## <a name="to-set-up-warehouse-employees"></a><span data-ttu-id="069d9-107">Настройка работников склада</span><span class="sxs-lookup"><span data-stu-id="069d9-107">To set up warehouse employees</span></span>  
1.  <span data-ttu-id="069d9-108">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Сотрудники склада**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="069d9-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
2. <span data-ttu-id="069d9-109">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="069d9-109">Choose the **New** action.</span></span>  
3. <span data-ttu-id="069d9-110">Выберите поле **Код пользователя**, а затем выберите пользователя, которого необходимо добавить как работника склада.</span><span class="sxs-lookup"><span data-stu-id="069d9-110">Select the **User ID** field, and then select the user to be added as a warehouse employee.</span></span> <span data-ttu-id="069d9-111">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="069d9-111">Choose the **OK** button.</span></span>  
6.  <span data-ttu-id="069d9-112">В поле **Код склада** введите код склада, где будет работать пользователь.</span><span class="sxs-lookup"><span data-stu-id="069d9-112">In the **Location Code** field, enter the code of the location where the user will be working.</span></span>  
7.  <span data-ttu-id="069d9-113">Установите флажок **По умолчанию**, чтобы определить склад как единственный, где сотрудник может выполнять складские действия.</span><span class="sxs-lookup"><span data-stu-id="069d9-113">Select the **Default** check box to define the location as the only location where the employee can perform warehouse activities.</span></span>  
8.  <span data-ttu-id="069d9-114">Повторите эти шаги, чтобы назначить работникам склады или назначить нестандартные склады существующим работникам склада.</span><span class="sxs-lookup"><span data-stu-id="069d9-114">Repeat these steps to assign other employees to locations or assign non-default locations to existing warehouse employees.</span></span>  

## <a name="see-also"></a><span data-ttu-id="069d9-115">См. также</span><span class="sxs-lookup"><span data-stu-id="069d9-115">See Also</span></span>  
[<span data-ttu-id="069d9-116">Управление складом</span><span class="sxs-lookup"><span data-stu-id="069d9-116">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="069d9-117">Наличие</span><span class="sxs-lookup"><span data-stu-id="069d9-117">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="069d9-118">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="069d9-118">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="069d9-119">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="069d9-119">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="069d9-120">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="069d9-120">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="069d9-121">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="069d9-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

