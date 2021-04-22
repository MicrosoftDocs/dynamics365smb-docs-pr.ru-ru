---
title: Учет в пакетном режиме выпуска продукции и времени работы
description: Выходное количество представляет собой ход работы в виде количества готовой продукции и использованной мощности работы или производственного центра.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 923f68b13619013dd54062438c66192a682868bc
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5787881"
---
# <a name="batch-post-output-and-run-times"></a><span data-ttu-id="9b56b-103">Учет в пакетном режиме выпуска продукции и времени работы</span><span class="sxs-lookup"><span data-stu-id="9b56b-103">Batch Post Output and Run Times</span></span>
<span data-ttu-id="9b56b-104">Выходное количество представляет собой ход работы в виде количества готовой продукции и использованной мощности работы или производственного центра.</span><span class="sxs-lookup"><span data-stu-id="9b56b-104">The output quantity represents the work progress in the form of the finished quantity and used capacity of work or machine center.</span></span>

<span data-ttu-id="9b56b-105">Можно использовать журнал выпуска для следующих целей:</span><span class="sxs-lookup"><span data-stu-id="9b56b-105">You can use the output journal to:</span></span>
*  <span data-ttu-id="9b56b-106">Корректировка запасов в связи с выпуском завершенных товаров с производства.</span><span class="sxs-lookup"><span data-stu-id="9b56b-106">Adjust inventory in connection with output of finished items from production.</span></span>
*  <span data-ttu-id="9b56b-107">Регистрация количества и брака для каждой операции в производственной технологической карте.</span><span class="sxs-lookup"><span data-stu-id="9b56b-107">Register quantities and scrap for each operation in production routing.</span></span>
*  <span data-ttu-id="9b56b-108">Регистрация времени наладки и работы для рабочих и производственных центров.</span><span class="sxs-lookup"><span data-stu-id="9b56b-108">Register setup and run time for work and machine centers.</span></span>

> [!NOTE]
> <span data-ttu-id="9b56b-109">Если используется производственная технологическая карта, запасы обновляются только при учете количества выхода в последней операции.</span><span class="sxs-lookup"><span data-stu-id="9b56b-109">If production routing are used, the inventory is updated only when you post output quantity on the last operation.</span></span>

<span data-ttu-id="9b56b-110">С помощью окна **Производственный журнал** можно также выполнять такие же задачи в окне **Журнал выхода продукции** и в это же время выполнять связанные задачи учета потребления.</span><span class="sxs-lookup"><span data-stu-id="9b56b-110">With the **Production Journal** window, you can perform the same tasks as in the **Output Journal** window and at the same time perform the related consumption posting tasks.</span></span> <span data-ttu-id="9b56b-111">Дополнительные сведения см. в разделе [Регистрация потребления и выхода для одной строки запущенного производственного заказа](production-how-to-register-consumption-and-output.md).</span><span class="sxs-lookup"><span data-stu-id="9b56b-111">For more information, see [Register Consumption and Output for One Released Production order line](production-how-to-register-consumption-and-output.md).</span></span>

## <a name="to-post-output-quantities-andor-register-run-times-for-one-or-more-production-order-lines"></a><span data-ttu-id="9b56b-112">Для учета количества выпущенной продукции и/или регистрации длительности операций для одной или нескольких строк производственного заказа</span><span class="sxs-lookup"><span data-stu-id="9b56b-112">To post output quantities and/or register run times for one or more production order lines</span></span>
1. <span data-ttu-id="9b56b-113">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал выхода продукции**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="9b56b-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9b56b-114">Заполните поля данными производственного заказа и данными о выпуске продукции и/или длительности операций.</span><span class="sxs-lookup"><span data-stu-id="9b56b-114">Fill in the fields with the production order data and the output data and/or run time.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
  
    <span data-ttu-id="9b56b-115">Вы можете использовать функцию **Раскрыть маршрут** для создания строк журнала из производственных заказов.</span><span class="sxs-lookup"><span data-stu-id="9b56b-115">You can use the **Explode Routing** function to generate journal lines from production orders.</span></span>
  
4. <span data-ttu-id="9b56b-116">Если операция была завершена, выберите поле **Завершен**.</span><span class="sxs-lookup"><span data-stu-id="9b56b-116">If the operation has been completed, select the **Finished** field.</span></span>  
5. <span data-ttu-id="9b56b-117">Выберите действие **Учесть**, чтобы учесть операции.</span><span class="sxs-lookup"><span data-stu-id="9b56b-117">Choose the **Post** action to post the operations.</span></span> 
 
<span data-ttu-id="9b56b-118">Операции в книге производственных мощностей обновляются для используемых производственных или машинных центров с учетом информации о времени и количестве выпуска и брака.</span><span class="sxs-lookup"><span data-stu-id="9b56b-118">Capacity ledger entries are updated for the used work or machine centers with information about time and quantity of output and scrap.</span></span> <span data-ttu-id="9b56b-119">Если вы учли последнюю операцию, товар будет добавлен в запасы.</span><span class="sxs-lookup"><span data-stu-id="9b56b-119">If you posted the last operation, the item will be added to the inventory.</span></span> 

## <a name="see-also"></a><span data-ttu-id="9b56b-120">См. также</span><span class="sxs-lookup"><span data-stu-id="9b56b-120">See Also</span></span>  
<span data-ttu-id="9b56b-121">[Учет брака/отходов вручную](production-how-to-post-scrap.md)
[Сторнирование учета выхода](production-how-to-reverse-output-posting.md)
[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="9b56b-121">[Post Scrap Manually](production-how-to-post-scrap.md)
[Reverse Output Posting](production-how-to-reverse-output-posting.md)
[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="9b56b-122">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="9b56b-122">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="9b56b-123">[Планирование](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="9b56b-123">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="9b56b-124">Запасы</span><span class="sxs-lookup"><span data-stu-id="9b56b-124">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="9b56b-125">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9b56b-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]
