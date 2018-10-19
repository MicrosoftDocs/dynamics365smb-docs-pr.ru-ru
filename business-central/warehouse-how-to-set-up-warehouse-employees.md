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
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 90af049fe87640b7e444848102b21c2fb1f8461e
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-warehouse-employees"></a><span data-ttu-id="1a45b-103">Настройка работников склада</span><span class="sxs-lookup"><span data-stu-id="1a45b-103">Set Up Warehouse Employees</span></span>
<span data-ttu-id="1a45b-104">Каждый пользователь, который выполняет складские действия, должен быть настроен как работник склада, которому назначен один склад по умолчанию и могут быть назначены другие склады.</span><span class="sxs-lookup"><span data-stu-id="1a45b-104">Each user who performs warehouse activities must be set up as a warehouse employee assigned to one default location and potentially more non-default locations.</span></span> <span data-ttu-id="1a45b-105">Данная настройка пользователя фильтрует все складские действия в базе данных по складу сотрудника, чтобы сотрудник мог выполнять складские задачи только для склада по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1a45b-105">This user setup filters all warehouse activities across the database to the employee's location so that the employee can only perform the warehouse activities at the default location.</span></span> <span data-ttu-id="1a45b-106">Пользователю могут быть назначены дополнительные нестандартные склады, где работник может просматривать строки задач, но не выполнять их.</span><span class="sxs-lookup"><span data-stu-id="1a45b-106">A user can be assigned to additional non-default locations for which the employee can view activity lines but not perform the activities.</span></span>

## <a name="to-set-up-warehouse-employees"></a><span data-ttu-id="1a45b-107">Настройка работников склада</span><span class="sxs-lookup"><span data-stu-id="1a45b-107">To set up warehouse employees</span></span>  
1.  <span data-ttu-id="1a45b-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сотрудники склада**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="1a45b-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1a45b-109">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="1a45b-109">Choose the **New** action.</span></span>  
3. <span data-ttu-id="1a45b-110">Выберите поле **Код пользователя**, а затем выберите пользователя, которого необходимо добавить как работника склада.</span><span class="sxs-lookup"><span data-stu-id="1a45b-110">Select the **User ID** field, and then select the user to be added as a warehouse employee.</span></span> <span data-ttu-id="1a45b-111">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="1a45b-111">Choose the **OK** button.</span></span>  
6.  <span data-ttu-id="1a45b-112">В поле **Код склада** введите код склада, где будет работать пользователь.</span><span class="sxs-lookup"><span data-stu-id="1a45b-112">In the **Location Code** field, enter the code of the location where the user will be working.</span></span>  
7.  <span data-ttu-id="1a45b-113">Установите флажок **По умолчанию**, чтобы определить склад как единственный, где сотрудник может выполнять складские действия.</span><span class="sxs-lookup"><span data-stu-id="1a45b-113">Select the **Default** check box to define the location as the only location where the employee can perform warehouse activities.</span></span>  
8.  <span data-ttu-id="1a45b-114">Повторите эти шаги, чтобы назначить работникам склады или назначить нестандартные склады существующим работникам склада.</span><span class="sxs-lookup"><span data-stu-id="1a45b-114">Repeat these steps to assign other employees to locations or assign non-default locations to existing warehouse employees.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1a45b-115">См. также</span><span class="sxs-lookup"><span data-stu-id="1a45b-115">See Also</span></span>  
[<span data-ttu-id="1a45b-116">Управление складом</span><span class="sxs-lookup"><span data-stu-id="1a45b-116">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="1a45b-117">Наличие</span><span class="sxs-lookup"><span data-stu-id="1a45b-117">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="1a45b-118">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="1a45b-118">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="1a45b-119">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="1a45b-119">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="1a45b-120">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="1a45b-120">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="1a45b-121">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1a45b-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

