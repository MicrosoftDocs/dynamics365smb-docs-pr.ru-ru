---
title: Практическое руководство. Учет потребления в пакетном режиме | Документация Майкрософт
description: Если выбран метод списания **Вручную**, учет компонентов производится вручную с использованием журнала потребления.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 0bf0a92d05b6c9ecb3d5a5ba054b4675680ad43c
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5391803"
---
# <a name="batch-post-production-consumption"></a><span data-ttu-id="bbeaa-103">Учет потребления для производства в пакетном режиме</span><span class="sxs-lookup"><span data-stu-id="bbeaa-103">Batch Post Production Consumption</span></span>
<span data-ttu-id="bbeaa-104">Если выбран метод списания **Вручную**, учет компонентов производится вручную с использованием журнала потребления.</span><span class="sxs-lookup"><span data-stu-id="bbeaa-104">If the flushing method is **Manual**, you must post the components manually, using a consumption journal.</span></span>

<span data-ttu-id="bbeaa-105">Можно также настроить систему для автоматического учета (*списания*) компонентов при запуске или завершении производственных заказов.</span><span class="sxs-lookup"><span data-stu-id="bbeaa-105">You can also set the system up to automatically post (*flush*) components when you start or finish production orders.</span></span> <span data-ttu-id="bbeaa-106">Дополнительные сведения см. в разделе [Включение списания компонентов в соответствии с производственным выпуском](production-how-to-flush-components-according-to-operation-output.md).</span><span class="sxs-lookup"><span data-stu-id="bbeaa-106">For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).</span></span>

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a><span data-ttu-id="bbeaa-107">Учет потребления для одной или нескольких строк производственного заказа</span><span class="sxs-lookup"><span data-stu-id="bbeaa-107">To post consumption for one or more production order lines</span></span>  
1.  <span data-ttu-id="bbeaa-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал потребления**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="bbeaa-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Consumption Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="bbeaa-109">Заполните поля данными производственного заказа и данными о потреблении.</span><span class="sxs-lookup"><span data-stu-id="bbeaa-109">Fill in the fields with the production order data and the consumption data.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    <span data-ttu-id="bbeaa-110">Если склад, на котором хранятся компоненты, настроен на использование ячеек, но не требует обработки подбора, присвойте код ячейки строке журнала для указания места на складе, откуда должны забираться товары.</span><span class="sxs-lookup"><span data-stu-id="bbeaa-110">If the warehouse location where the components are stored is set up to use bins but does not require pick processing, assign a bin code to the journal line to indicate where the items should be taken from in the warehouse.</span></span> <span data-ttu-id="bbeaa-111">Дополнительные сведения см. в разделе [Подбор для производства или сборки](warehouse-how-to-pick-for-production.md).</span><span class="sxs-lookup"><span data-stu-id="bbeaa-111">For more information, see [Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).</span></span>  
3.  <span data-ttu-id="bbeaa-112">Выберите действие **Учесть**, чтобы учесть потребление.</span><span class="sxs-lookup"><span data-stu-id="bbeaa-112">Choose the **Post** action to post the consumption.</span></span> <span data-ttu-id="bbeaa-113">Соответствующие операции в книге товаров уменьшаются.</span><span class="sxs-lookup"><span data-stu-id="bbeaa-113">The related item ledger entries are reduced.</span></span>

## <a name="see-also"></a><span data-ttu-id="bbeaa-114">См. также</span><span class="sxs-lookup"><span data-stu-id="bbeaa-114">See Also</span></span>  
<span data-ttu-id="bbeaa-115">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="bbeaa-115">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="bbeaa-116">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="bbeaa-116">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="bbeaa-117">[Планирование](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="bbeaa-117">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="bbeaa-118">Запасы</span><span class="sxs-lookup"><span data-stu-id="bbeaa-118">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="bbeaa-119">Покупки</span><span class="sxs-lookup"><span data-stu-id="bbeaa-119">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="bbeaa-120">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bbeaa-120">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]