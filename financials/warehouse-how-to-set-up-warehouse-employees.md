---
title: "Как настраивать работников склада | Документы Майкрософт"
description: "Каждый пользователь, который выполняет складские действия, должен быть настроен как работник склада, которому назначен один склад по умолчанию и могут быть назначены другие склады."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 6fb0aa48352bc35c2e9ee399a3d0b17032a5ed7e
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-warehouse-employees"></a><span data-ttu-id="8590d-103">Практическое руководство. Настройка работников склада</span><span class="sxs-lookup"><span data-stu-id="8590d-103">How to: Set Up Warehouse Employees</span></span>
<span data-ttu-id="8590d-104">Каждый пользователь, который выполняет складские действия, должен быть настроен как работник склада, которому назначен один склад по умолчанию и могут быть назначены другие склады.</span><span class="sxs-lookup"><span data-stu-id="8590d-104">Each user who performs warehouse activities must be set up as a warehouse employee assigned to one default location and potentially more non-default locations.</span></span> <span data-ttu-id="8590d-105">Данная настройка пользователя фильтрует все складские действия в базе данных по складу сотрудника, чтобы сотрудник мог выполнять складские задачи только для склада по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8590d-105">This user setup filters all warehouse activities across the database to the employee's location so that the employee can only perform the warehouse activities at the default location.</span></span> <span data-ttu-id="8590d-106">Пользователю могут быть назначены дополнительные нестандартные склады, где работник может просматривать строки задач, но не выполнять их.</span><span class="sxs-lookup"><span data-stu-id="8590d-106">A user can be assigned to additional non-default locations for which the employee can view activity lines but not perform the activities.</span></span>

## <a name="to-set-up-warehouse-employees"></a><span data-ttu-id="8590d-107">Настройка работников склада</span><span class="sxs-lookup"><span data-stu-id="8590d-107">To set up warehouse employees</span></span>  
1.  <span data-ttu-id="8590d-108">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Сотрудники склада**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="8590d-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8590d-109">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="8590d-109">Choose the **New** action.</span></span>  
3. <span data-ttu-id="8590d-110">Выберите поле **Код пользователя**, а затем выберите пользователя, которого необходимо добавить как работника склада.</span><span class="sxs-lookup"><span data-stu-id="8590d-110">Select the **User ID** field, and then select the user to be added as a warehouse employee.</span></span> <span data-ttu-id="8590d-111">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="8590d-111">Choose the **OK** button.</span></span>  
6.  <span data-ttu-id="8590d-112">В поле **Код склада** введите код склада, где будет работать пользователь.</span><span class="sxs-lookup"><span data-stu-id="8590d-112">In the **Location Code** field, enter the code of the location where the user will be working.</span></span>  
7.  <span data-ttu-id="8590d-113">Установите флажок **По умолчанию**, чтобы определить склад как единственный, где сотрудник может выполнять складские действия.</span><span class="sxs-lookup"><span data-stu-id="8590d-113">Select the **Default** check box to define the location as the only location where the employee can perform warehouse activities.</span></span>  
8.  <span data-ttu-id="8590d-114">Повторите эти шаги, чтобы назначить работникам склады или назначить нестандартные склады существующим работникам склада.</span><span class="sxs-lookup"><span data-stu-id="8590d-114">Repeat these steps to assign other employees to locations or assign non-default locations to existing warehouse employees.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8590d-115">См. также</span><span class="sxs-lookup"><span data-stu-id="8590d-115">See Also</span></span>  
[<span data-ttu-id="8590d-116">Управление складом</span><span class="sxs-lookup"><span data-stu-id="8590d-116">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="8590d-117">Наличие</span><span class="sxs-lookup"><span data-stu-id="8590d-117">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="8590d-118">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="8590d-118">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="8590d-119">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="8590d-119">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="8590d-120">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="8590d-120">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="8590d-121">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8590d-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

