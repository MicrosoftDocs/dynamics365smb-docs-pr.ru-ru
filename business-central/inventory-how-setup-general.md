---
title: Определение настройки общей информации по запасам
description: Описывает, как определить общую настройку запасов, чтобы вы могли управлять своим складом и запасами.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, stock
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 1430123f433cfc101e0ae94ce0598d9c0cdd58b2
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5785827"
---
# <a name="set-up-general-inventory-information"></a><span data-ttu-id="e4b3f-103">Настройка общей информации по запасам</span><span class="sxs-lookup"><span data-stu-id="e4b3f-103">Set Up General Inventory Information</span></span>

<span data-ttu-id="e4b3f-104">Можно указать общую информацию по запасам на странице **Настройка запасов**.</span><span class="sxs-lookup"><span data-stu-id="e4b3f-104">You specify your general inventory setup on the **Inventory Setup** page.</span></span>

## <a name="to-set-up-general-inventory-information"></a><span data-ttu-id="e4b3f-105">Настройка общей информации по запасам</span><span class="sxs-lookup"><span data-stu-id="e4b3f-105">To set up general inventory information</span></span>

1. <span data-ttu-id="e4b3f-106">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Запасы"**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e4b3f-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="e4b3f-107">На странице **Настройка запасов** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="e4b3f-107">On the **Inventory Setup** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="e4b3f-108">Для получения подробной информации о полях себестоимости, **Автомат. учет себест.**, **Учет ожидаемой себест.** и **Метод учета себестоимости по умолчанию** см. разделы [Выверка себестоимости товаров с главной книгой](finance-how-to-post-inventory-costs-to-the-general-ledger.md), [Сведения о проектировании: себестоимость запасов](design-details-inventory-costing.md) и [Сведения о проектировании: учет ожидаемой себестоимости](design-details-expected-cost-posting.md).</span><span class="sxs-lookup"><span data-stu-id="e4b3f-108">For detailed information about the costing fields, **Automatic Cost Posting**, **Expected Cost Posting to G/L**, and **Default Costing Method**, see [Reconcile Inventory Costs with the General Ledger](finance-how-to-post-inventory-costs-to-the-general-ledger.md), [Design Details: Inventory Costing](design-details-inventory-costing.md), and [Design Details: Expected Cost Posting](design-details-expected-cost-posting.md).</span></span> <span data-ttu-id="e4b3f-109">Для получения дополнительной информации об учете себестоимости в целом см. [Управление себестоимостью товаров](finance-manage-inventory-costs.md).</span><span class="sxs-lookup"><span data-stu-id="e4b3f-109">For more information about costing in general, see [Managing Inventory Costs](finance-manage-inventory-costs.md).</span></span>  

<span data-ttu-id="e4b3f-110">Если требуется учитывать в расчетах входящее время обработки склада при планирования заказов в строке покупки, для запаса и склада это можно задать на странице **Настройка модуля "Запасы"** в качестве поведения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e4b3f-110">If you want to include warehouse handling time in the order promising calculation on the purchase line, you can set it up as a default for the inventory, on the **Inventory Setup** page, and for your location.</span></span> <span data-ttu-id="e4b3f-111">Дополнительные сведения см. в разделе [Расчет сроков планирования заказов](sales-how-to-calculate-order-promising-dates.md).</span><span class="sxs-lookup"><span data-stu-id="e4b3f-111">For more information, see [Calculate Order Promising Dates](sales-how-to-calculate-order-promising-dates.md).</span></span>  

> [!NOTE]
> <span data-ttu-id="e4b3f-112">Переключатель **Автоматическая коррекция себестоимости** включен по умолчанию, чтобы гарантировать, что значения запасов всегда верны в главной книге, что, в свою очередь, поддерживает актуальность статистики продаж и прибыли.</span><span class="sxs-lookup"><span data-stu-id="e4b3f-112">The **Automatic Cost Adjustment** toggle is turned on by default to ensure that inventory values are always correct in the general ledger, which in turn keeps your sales and profit statistics up to date.</span></span> <span data-ttu-id="e4b3f-113">Любые изменения себестоимости из входящих операций, например операций для закупок или выпуска производства, назначаются соответствующим исходящим операциям, например продажам или перемещению.</span><span class="sxs-lookup"><span data-stu-id="e4b3f-113">Cost changes from inbound entries, such as those for purchases or production output, are assigned to the related outbound entries, such as sales or transfers.</span></span> <span data-ttu-id="e4b3f-114">Это полезно для новых клиентов [!INCLUDE[prod_short](includes/prod_short.md)] и малых предприятий с относительно низкими уровнями складских операций.</span><span class="sxs-lookup"><span data-stu-id="e4b3f-114">This is helpful for new [!INCLUDE[prod_short](includes/prod_short.md)] customers and small businesses with relatively low inventory transaction levels.</span></span> <span data-ttu-id="e4b3f-115">Однако по мере роста бизнеса и увеличения уровня запасов это может снизить производительность системы.</span><span class="sxs-lookup"><span data-stu-id="e4b3f-115">However, as a business grows and inventory levels increase, this can slow down system performance.</span></span> <span data-ttu-id="e4b3f-116">Чтобы свести к минимуму снижение производительности во время разноски, выберите параметр времени, чтобы определить, как далеко во времени от рабочей даты может произойти входящая транзакция, чтобы потенциально инициировать корректировку связанных записей исходящих значений.</span><span class="sxs-lookup"><span data-stu-id="e4b3f-116">To minimize reduced performance during posting, select a time option to define how far back in time from the work date an inbound transaction can occur to potentially trigger adjustment of related outbound value entries.</span></span> <span data-ttu-id="e4b3f-117">Кроме того, вы можете вручную корректировать затраты через регулярные промежутки времени с помощью пакетного задания «Коррекция себестоимости запасов».</span><span class="sxs-lookup"><span data-stu-id="e4b3f-117">Alternatively, you can manually adjust costs at regular intervals with the Adjust Cost - Item Entries batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="e4b3f-118">См. также</span><span class="sxs-lookup"><span data-stu-id="e4b3f-118">See Also</span></span>
[<span data-ttu-id="e4b3f-119">Настройка запасов</span><span class="sxs-lookup"><span data-stu-id="e4b3f-119">Set Up Inventory</span></span>](inventory-setup-inventory.md)  
<span data-ttu-id="e4b3f-120">[Сведения о проектировании: методы учета себестоимости](design-details-costing-methods.md)  </span><span class="sxs-lookup"><span data-stu-id="e4b3f-120">[Design Details: Costing Methods](design-details-costing-methods.md)  </span></span>  
[<span data-ttu-id="e4b3f-121">Управление запасами</span><span class="sxs-lookup"><span data-stu-id="e4b3f-121">Manage Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="e4b3f-122">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e4b3f-122">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="e4b3f-123">Изменение набора отображаемых функций</span><span class="sxs-lookup"><span data-stu-id="e4b3f-123">Change Which Features are Displayed</span></span>](ui-experiences.md)  
[<span data-ttu-id="e4b3f-124">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="e4b3f-124">General Business Functionality</span></span>](ui-across-business-areas.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]