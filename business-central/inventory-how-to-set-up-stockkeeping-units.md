---
title: Практическое руководство. Настройка единиц хранения | Документы Майкрософт
description: Единицы хранения используются для записи информации о товарах для кода конкретного склада или кода конкретного варианта.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 50bf3695a135652ec422bb187f1ff2fef06f3a35
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1239387"
---
# <a name="set-up-stockkeeping-units"></a><span data-ttu-id="46adc-103">Настройка единиц хранения</span><span class="sxs-lookup"><span data-stu-id="46adc-103">Set Up Stockkeeping Units</span></span>
<span data-ttu-id="46adc-104">Единицы хранения используются для записи информации о товарах для кода конкретного склада или кода конкретного варианта.</span><span class="sxs-lookup"><span data-stu-id="46adc-104">You can use stockkeeping units to record information about your items for a specific location or a specific variant code.</span></span>  

 <span data-ttu-id="46adc-105">Единицы хранения являются дополнением к карточкам товара.</span><span class="sxs-lookup"><span data-stu-id="46adc-105">Stockkeeping units are a supplement to item cards.</span></span> <span data-ttu-id="46adc-106">Они не заменяют их, хотя связаны с ними.</span><span class="sxs-lookup"><span data-stu-id="46adc-106">They do not replace them, although they are related to them.</span></span> <span data-ttu-id="46adc-107">Единицы хранения позволяют различать для одного и того же товара информацию о товаре, предназначенном для конкретной площадки хранения (как складской комплекс или центр дистрибуции) или для конкретного варианта хранения (таких как различные номера полок и различная информация о пополнении).</span><span class="sxs-lookup"><span data-stu-id="46adc-107">Stockkeeping units allow you to differentiate information about an item for a specific location, such as a warehouse or distribution center, or a specific variant, such as different shelf numbers and different replenishment information, for the same item.</span></span>  

## <a name="to-set-up-a-stockkeeping-unit"></a><span data-ttu-id="46adc-108">Настройка единицы хранения</span><span class="sxs-lookup"><span data-stu-id="46adc-108">To set up a stockkeeping unit</span></span>  

1.  <span data-ttu-id="46adc-109">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Единицы хранения**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="46adc-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stockkeeping Units**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="46adc-110">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="46adc-110">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="46adc-111">Заполните поля в карточке.</span><span class="sxs-lookup"><span data-stu-id="46adc-111">Fill in the fields on the card.</span></span> <span data-ttu-id="46adc-112">Следующие поля являются обязательными: **Код товара**, **Код склада** и/или **Код варианта**.</span><span class="sxs-lookup"><span data-stu-id="46adc-112">The following fields are required: **Item No.**, **Location Code**, and/or **Variant Code**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

<span data-ttu-id="46adc-113">После настройки первой единицы хранения для товара устанавливается флажок **Есть единица хранения** в карточке **Товар**.</span><span class="sxs-lookup"><span data-stu-id="46adc-113">When you have set up the first stockkeeping unit for an item, the **Stockkeeping Unit Exists** check box on the **Item** card is selected.</span></span>  

<span data-ttu-id="46adc-114">Для создания нескольких единиц хранения для одного товара используется пакетное задание **Создание единицы хранения**.</span><span class="sxs-lookup"><span data-stu-id="46adc-114">To create several stockkeeping units for an item, use the **Create Stockkeeping Unit** batch job.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="46adc-115">Информация в карточке **Единица хранения** обладает более высоким приоритетом по сравнению с информацией в карточке **Товар**.</span><span class="sxs-lookup"><span data-stu-id="46adc-115">The information on the **Stockkeeping Unit** card has priority over the **Item** card.</span></span>

> [!Warning]
> <span data-ttu-id="46adc-116">Если номер SKU указывается при производстве, поле **Стандартная себестоимость** не используется для выставления счетов и коррекции фактической себестоимости производимого товара.</span><span class="sxs-lookup"><span data-stu-id="46adc-116">If the SKU is supplied through production, then the **Standard Cost** field is not used when invoicing and adjusting the actual cost of the produced item.</span></span> <span data-ttu-id="46adc-117">Вместо этого используется поле **Стандартная себестоимость** в карточке базового товара, и все отклонения рассчитываются на базе структуры себестоимости данного товара.</span><span class="sxs-lookup"><span data-stu-id="46adc-117">Instead, the **Standard Cost** field on the underlying item card is used, and any variances are calculated against the cost shares of that item.</span></span><br /><br />
> <span data-ttu-id="46adc-118">Поскольку производственные спецификации и маршрутизаций не могут быть назначены единицам хранения, себестоимость единиц будет свернута, а связанный расчет доль затрат также не будет доступен для единиц хранения.</span><span class="sxs-lookup"><span data-stu-id="46adc-118">Because production BOMs and routing cannot be assigned to SKUs, then the unit cost roll-up and the related calculation of cost shares are also not available on SKUs.</span></span> <span data-ttu-id="46adc-119">Дополнительные сведения см. в разделе [Расчет стандартной себестоимости](finance-about-calculating-standard-cost.md)</span><span class="sxs-lookup"><span data-stu-id="46adc-119">For more information, see [About Calculating Standard Cost](finance-about-calculating-standard-cost.md)</span></span>

## <a name="see-also"></a><span data-ttu-id="46adc-120">См. также</span><span class="sxs-lookup"><span data-stu-id="46adc-120">See Also</span></span>  
[<span data-ttu-id="46adc-121">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="46adc-121">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="46adc-122">Настройка управления складом</span><span class="sxs-lookup"><span data-stu-id="46adc-122">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
[<span data-ttu-id="46adc-123">Управление складом</span><span class="sxs-lookup"><span data-stu-id="46adc-123">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="46adc-124">Наличие</span><span class="sxs-lookup"><span data-stu-id="46adc-124">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="46adc-125">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="46adc-125">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="46adc-126">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="46adc-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="46adc-127">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="46adc-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
