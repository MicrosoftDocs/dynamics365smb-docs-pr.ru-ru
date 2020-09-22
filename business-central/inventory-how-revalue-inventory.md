---
title: Создание новых операций стоимости для товаров на складе | Документация Майкрософт
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
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 3570d5e7347745763c8d8e18dfdf65166e7839e0
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3782047"
---
# <a name="revalue-inventory"></a><span data-ttu-id="ac64e-103">Переоценка запасов</span><span class="sxs-lookup"><span data-stu-id="ac64e-103">Revalue Inventory</span></span>
<span data-ttu-id="ac64e-104">Чтобы повысить или понизить стоимость изделия или конкретной учтенной товарной операции, нужно воспользоваться журналом переоценки.</span><span class="sxs-lookup"><span data-stu-id="ac64e-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span></span>

## <a name="to-revalue-inventory"></a><span data-ttu-id="ac64e-105">Переоценка запасов</span><span class="sxs-lookup"><span data-stu-id="ac64e-105">To revalue inventory</span></span>
1. <span data-ttu-id="ac64e-106">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал переоценки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="ac64e-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Revaluation Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="ac64e-107">Выберите действие **Расчет стоимости запасов**.</span><span class="sxs-lookup"><span data-stu-id="ac64e-107">Choose the **Calculate Inventory Value** action.</span></span>
3. <span data-ttu-id="ac64e-108">На странице **Расчет стоимости запасов** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="ac64e-108">On the **Calculate Inventory Value** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="ac64e-109">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="ac64e-109">Choose the **OK** button.</span></span>
5. <span data-ttu-id="ac64e-110">В каждой строке на странице **Журнал переоценки** в поле **Себестоимость единицы (переоценка)** введите новую себестоимость единицы.</span><span class="sxs-lookup"><span data-stu-id="ac64e-110">On each line on the **Revaluation Journal** page, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span></span> <span data-ttu-id="ac64e-111">Можно также ввести новую общую сумму в поле **Стоимость запасов (переоценка)**.</span><span class="sxs-lookup"><span data-stu-id="ac64e-111">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span></span>

    <span data-ttu-id="ac64e-112">Соответствующие поля обновляются автоматически.</span><span class="sxs-lookup"><span data-stu-id="ac64e-112">The relevant fields are automatically updated.</span></span> <span data-ttu-id="ac64e-113">Следует учесть, что в поле **Сумма** отражается фактическое изменение в значении склада для выбранных учтенных товарных операций.</span><span class="sxs-lookup"><span data-stu-id="ac64e-113">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span></span> <span data-ttu-id="ac64e-114">Там подсчитывается разница между полями **Стоимость запасов (расчетная)** и **Стоимость запасов (переоценка)**.</span><span class="sxs-lookup"><span data-stu-id="ac64e-114">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span></span>
6. <span data-ttu-id="ac64e-115">После того как будут заполнены все строки в журнале переоценки, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="ac64e-115">When you have completed all lines in the revaluation journal, choose the **Post** action.</span></span>

<span data-ttu-id="ac64e-116">Создаются новые операции стоимости, которые отражают учтенную переоценку.</span><span class="sxs-lookup"><span data-stu-id="ac64e-116">New value entries are now created to reflect the revaluations that you have posted.</span></span> <span data-ttu-id="ac64e-117">Новые значения можно просмотреть в соответствующей карточке товара.</span><span class="sxs-lookup"><span data-stu-id="ac64e-117">You can see the new values on the respective item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="ac64e-118">См. также</span><span class="sxs-lookup"><span data-stu-id="ac64e-118">See Also</span></span>
[<span data-ttu-id="ac64e-119">Сведения о проектировании: переоценка</span><span class="sxs-lookup"><span data-stu-id="ac64e-119">Design Details: Revaluation</span></span>](design-details-revaluation.md)  
[<span data-ttu-id="ac64e-120">Запасы</span><span class="sxs-lookup"><span data-stu-id="ac64e-120">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="ac64e-121">Продажи</span><span class="sxs-lookup"><span data-stu-id="ac64e-121">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="ac64e-122">Покупки</span><span class="sxs-lookup"><span data-stu-id="ac64e-122">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="ac64e-123">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ac64e-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
