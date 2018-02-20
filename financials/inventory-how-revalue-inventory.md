---
title: "Создание новых операций стоимости для товаров на складе | Документы Майкрософт"
description: "Описывается, как повысить или понизить операции стоимости одного или нескольких товаров в запасах путем учета текущей вычисленной стоимости."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: costing, inventory cost, value entries
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 8460dac8478fa101a255d93110578fa9ea20516f
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="revalue-inventory"></a><span data-ttu-id="92245-103">Переоценка запасов</span><span class="sxs-lookup"><span data-stu-id="92245-103">Revalue Inventory</span></span>
<span data-ttu-id="92245-104">Чтобы повысить или понизить стоимость изделия или конкретной учтенной товарной операции, нужно воспользоваться журналом переоценки.</span><span class="sxs-lookup"><span data-stu-id="92245-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span></span>

## <a name="to-revalue-inventory"></a><span data-ttu-id="92245-105">Переоценка запасов</span><span class="sxs-lookup"><span data-stu-id="92245-105">To revalue inventory</span></span>
1. <span data-ttu-id="92245-106">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журнал переоценки**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="92245-106">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Revaluation Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="92245-107">Выберите действие **Расчет стоимости запасов**.</span><span class="sxs-lookup"><span data-stu-id="92245-107">Choose the **Calculate Inventory Value** action.</span></span>
3. <span data-ttu-id="92245-108">В окне **Расчет стоимости запасов** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="92245-108">In the **Calculate Inventory Value** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="92245-109">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="92245-109">Choose the **OK** button.</span></span>
5. <span data-ttu-id="92245-110">В каждой строке в окне **Журнал переоценки** в поле **Себестоимость единицы (переоценка)** введите новую себестоимость единицы.</span><span class="sxs-lookup"><span data-stu-id="92245-110">On each line in the **Revaluation Journal** window, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span></span> <span data-ttu-id="92245-111">Можно также ввести новую общую сумму в поле **Стоимость запасов (переоценка)**.</span><span class="sxs-lookup"><span data-stu-id="92245-111">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span></span>

    <span data-ttu-id="92245-112">Соответствующие поля обновляются автоматически.</span><span class="sxs-lookup"><span data-stu-id="92245-112">The relevant fields are automatically updated.</span></span> <span data-ttu-id="92245-113">Следует учесть, что в поле **Сумма** отражается фактическое изменение в значении склада для выбранных учтенных товарных операций.</span><span class="sxs-lookup"><span data-stu-id="92245-113">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span></span> <span data-ttu-id="92245-114">Там подсчитывается разница между полями **Стоимость запасов (расчетная)** и **Стоимость запасов (переоценка)**.</span><span class="sxs-lookup"><span data-stu-id="92245-114">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span></span>
6. <span data-ttu-id="92245-115">После того как будут заполнены все строки в журнале переоценки, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="92245-115">When you have completed all lines in the revaluation journal, choose the **Post** action.</span></span>

<span data-ttu-id="92245-116">Создаются новые операции стоимости, которые отражают учтенную переоценку.</span><span class="sxs-lookup"><span data-stu-id="92245-116">New value entries are now created to reflect the revaluations that you have posted.</span></span> <span data-ttu-id="92245-117">Новые значения можно просмотреть в соответствующей карточке товара.</span><span class="sxs-lookup"><span data-stu-id="92245-117">You can see the new values on the respective item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="92245-118">См. также</span><span class="sxs-lookup"><span data-stu-id="92245-118">See Also</span></span>
[<span data-ttu-id="92245-119">Сведения о проектировании: переоценка</span><span class="sxs-lookup"><span data-stu-id="92245-119">Design Details: Revaluation</span></span>](design-details-revaluation.md)  
[<span data-ttu-id="92245-120">Наличие</span><span class="sxs-lookup"><span data-stu-id="92245-120">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="92245-121">Продажи</span><span class="sxs-lookup"><span data-stu-id="92245-121">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="92245-122">Покупки</span><span class="sxs-lookup"><span data-stu-id="92245-122">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="92245-123">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="92245-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

