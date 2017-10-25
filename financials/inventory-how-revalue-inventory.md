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
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: cfccd4f4ac6e2599ebc4b53b43163f4dfcc4d0ef
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-revalue-inventory"></a><span data-ttu-id="3da3a-103">Практическое руководство. Переоценка запасов</span><span class="sxs-lookup"><span data-stu-id="3da3a-103">How to: Revalue Inventory</span></span>
<span data-ttu-id="3da3a-104">Чтобы повысить или понизить стоимость изделия или конкретной учтенной товарной операции, нужно воспользоваться журналом переоценки.</span><span class="sxs-lookup"><span data-stu-id="3da3a-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span></span>

## <a name="to-revalue-inventory"></a><span data-ttu-id="3da3a-105">Переоценка запасов</span><span class="sxs-lookup"><span data-stu-id="3da3a-105">To revalue inventory</span></span>
1. <span data-ttu-id="3da3a-106">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журнал переоценки**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3da3a-106">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Revaluation Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="3da3a-107">Выберите действие **Расчет стоимости запасов**.</span><span class="sxs-lookup"><span data-stu-id="3da3a-107">Choose the **Calculate Inventory Value** action.</span></span>
3. <span data-ttu-id="3da3a-108">В окне **Расчет стоимости запасов** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="3da3a-108">In the **Calculate Inventory Value** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="3da3a-109">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="3da3a-109">Choose the **OK** button.</span></span>
5. <span data-ttu-id="3da3a-110">В каждой строке в окне **Журнал переоценки** в поле **Себестоимость единицы (переоценка)** введите новую себестоимость единицы.</span><span class="sxs-lookup"><span data-stu-id="3da3a-110">On each line in the **Revaluation Journal** window, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span></span> <span data-ttu-id="3da3a-111">Можно также ввести новую общую сумму в поле **Стоимость запасов (переоценка)**.</span><span class="sxs-lookup"><span data-stu-id="3da3a-111">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span></span>

    <span data-ttu-id="3da3a-112">Соответствующие поля обновляются автоматически.</span><span class="sxs-lookup"><span data-stu-id="3da3a-112">The relevant fields are automatically updated.</span></span> <span data-ttu-id="3da3a-113">Следует учесть, что в поле **Сумма** отражается фактическое изменение в значении склада для выбранных учтенных товарных операций.</span><span class="sxs-lookup"><span data-stu-id="3da3a-113">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span></span> <span data-ttu-id="3da3a-114">Там подсчитывается разница между полями **Стоимость запасов (расчетная)** и **Стоимость запасов (переоценка)**.</span><span class="sxs-lookup"><span data-stu-id="3da3a-114">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span></span>
6. <span data-ttu-id="3da3a-115">После того как будут заполнены все строки в журнале переоценки, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="3da3a-115">When you have completed all lines in the revaluation journal, choose the **Post** action.</span></span>

<span data-ttu-id="3da3a-116">Создаются новые операции стоимости, которые отражают учтенную переоценку.</span><span class="sxs-lookup"><span data-stu-id="3da3a-116">New value entries are now created to reflect the revaluations that you have posted.</span></span> <span data-ttu-id="3da3a-117">Новые значения можно просмотреть в соответствующей карточке товара.</span><span class="sxs-lookup"><span data-stu-id="3da3a-117">You can see the new values on the respective item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="3da3a-118">См. также</span><span class="sxs-lookup"><span data-stu-id="3da3a-118">See Also</span></span>
[<span data-ttu-id="3da3a-119">Сведения о проектировании: переоценка</span><span class="sxs-lookup"><span data-stu-id="3da3a-119">Design Details: Revaluation</span></span>](design-details-revaluation.md)  
[<span data-ttu-id="3da3a-120">Наличие</span><span class="sxs-lookup"><span data-stu-id="3da3a-120">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="3da3a-121">Продажи</span><span class="sxs-lookup"><span data-stu-id="3da3a-121">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="3da3a-122">Покупки</span><span class="sxs-lookup"><span data-stu-id="3da3a-122">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="3da3a-123">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3da3a-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

