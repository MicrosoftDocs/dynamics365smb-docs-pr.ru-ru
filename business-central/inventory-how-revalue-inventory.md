---
title: Создание новых операций стоимости для товаров на складе | Документы Майкрософт
description: Описывается, как повысить или понизить операции стоимости одного или нескольких товаров в запасах путем учета текущей вычисленной стоимости.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: costing, inventory cost, value entries
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 602381b34a057120cc53deca4dd293f939777dc5
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1243093"
---
# <a name="revalue-inventory"></a><span data-ttu-id="7c469-103">Переоценка запасов</span><span class="sxs-lookup"><span data-stu-id="7c469-103">Revalue Inventory</span></span>
<span data-ttu-id="7c469-104">Чтобы повысить или понизить стоимость изделия или конкретной учтенной товарной операции, нужно воспользоваться журналом переоценки.</span><span class="sxs-lookup"><span data-stu-id="7c469-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span></span>

## <a name="to-revalue-inventory"></a><span data-ttu-id="7c469-105">Переоценка запасов</span><span class="sxs-lookup"><span data-stu-id="7c469-105">To revalue inventory</span></span>
1. <span data-ttu-id="7c469-106">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал переоценки**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="7c469-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Revaluation Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="7c469-107">Выберите действие **Расчет стоимости запасов**.</span><span class="sxs-lookup"><span data-stu-id="7c469-107">Choose the **Calculate Inventory Value** action.</span></span>
3. <span data-ttu-id="7c469-108">На странице **Расчет стоимости запасов** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="7c469-108">On the **Calculate Inventory Value** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="7c469-109">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="7c469-109">Choose the **OK** button.</span></span>
5. <span data-ttu-id="7c469-110">В каждой строке на странице **Журнал переоценки** в поле **Себестоимость единицы (переоценка)** введите новую себестоимость единицы.</span><span class="sxs-lookup"><span data-stu-id="7c469-110">On each line on the **Revaluation Journal** page, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span></span> <span data-ttu-id="7c469-111">Можно также ввести новую общую сумму в поле **Стоимость запасов (переоценка)**.</span><span class="sxs-lookup"><span data-stu-id="7c469-111">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span></span>

    <span data-ttu-id="7c469-112">Соответствующие поля обновляются автоматически.</span><span class="sxs-lookup"><span data-stu-id="7c469-112">The relevant fields are automatically updated.</span></span> <span data-ttu-id="7c469-113">Следует учесть, что в поле **Сумма** отражается фактическое изменение в значении склада для выбранных учтенных товарных операций.</span><span class="sxs-lookup"><span data-stu-id="7c469-113">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span></span> <span data-ttu-id="7c469-114">Там подсчитывается разница между полями **Стоимость запасов (расчетная)** и **Стоимость запасов (переоценка)**.</span><span class="sxs-lookup"><span data-stu-id="7c469-114">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span></span>
6. <span data-ttu-id="7c469-115">После того как будут заполнены все строки в журнале переоценки, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="7c469-115">When you have completed all lines in the revaluation journal, choose the **Post** action.</span></span>

<span data-ttu-id="7c469-116">Создаются новые операции стоимости, которые отражают учтенную переоценку.</span><span class="sxs-lookup"><span data-stu-id="7c469-116">New value entries are now created to reflect the revaluations that you have posted.</span></span> <span data-ttu-id="7c469-117">Новые значения можно просмотреть в соответствующей карточке товара.</span><span class="sxs-lookup"><span data-stu-id="7c469-117">You can see the new values on the respective item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="7c469-118">См. также</span><span class="sxs-lookup"><span data-stu-id="7c469-118">See Also</span></span>
[<span data-ttu-id="7c469-119">Сведения о проектировании: переоценка</span><span class="sxs-lookup"><span data-stu-id="7c469-119">Design Details: Revaluation</span></span>](design-details-revaluation.md)  
[<span data-ttu-id="7c469-120">Наличие</span><span class="sxs-lookup"><span data-stu-id="7c469-120">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="7c469-121">Продажи</span><span class="sxs-lookup"><span data-stu-id="7c469-121">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="7c469-122">Покупки</span><span class="sxs-lookup"><span data-stu-id="7c469-122">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="7c469-123">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7c469-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
