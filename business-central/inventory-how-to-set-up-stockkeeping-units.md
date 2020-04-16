---
title: Практическое руководство. Настройка единиц хранения | Документация Майкрософт
description: Единицы хранения используются для записи информации о товарах для кода конкретного склада или кода конкретного варианта.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 610939cb61c917d5319fc758e582c0d169d7f11b
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3182016"
---
# <a name="set-up-stockkeeping-units"></a><span data-ttu-id="b1e02-103">Настройка единиц хранения</span><span class="sxs-lookup"><span data-stu-id="b1e02-103">Set Up Stockkeeping Units</span></span>
<span data-ttu-id="b1e02-104">Единицы хранения используются для записи информации о товарах для кода конкретного склада или кода конкретного варианта.</span><span class="sxs-lookup"><span data-stu-id="b1e02-104">You can use stockkeeping units to record information about your items for a specific location or a specific variant code.</span></span>  

 <span data-ttu-id="b1e02-105">Единицы хранения являются дополнением к карточкам товара.</span><span class="sxs-lookup"><span data-stu-id="b1e02-105">Stockkeeping units are a supplement to item cards.</span></span> <span data-ttu-id="b1e02-106">Они не заменяют их, хотя связаны с ними.</span><span class="sxs-lookup"><span data-stu-id="b1e02-106">They do not replace them, although they are related to them.</span></span> <span data-ttu-id="b1e02-107">Единицы хранения позволяют различать для одного и того же товара информацию о товаре, предназначенном для конкретной площадки хранения (как складской комплекс или центр дистрибуции) или для конкретного варианта хранения (таких как различные номера полок и различная информация о пополнении).</span><span class="sxs-lookup"><span data-stu-id="b1e02-107">Stockkeeping units allow you to differentiate information about an item for a specific location, such as a warehouse or distribution center, or a specific variant, such as different shelf numbers and different replenishment information, for the same item.</span></span>  

## <a name="to-set-up-a-stockkeeping-unit"></a><span data-ttu-id="b1e02-108">Настройка единицы хранения</span><span class="sxs-lookup"><span data-stu-id="b1e02-108">To set up a stockkeeping unit</span></span>  

1.  <span data-ttu-id="b1e02-109">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Единицы хранения**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b1e02-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stockkeeping Units**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b1e02-110">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="b1e02-110">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="b1e02-111">Заполните поля в карточке.</span><span class="sxs-lookup"><span data-stu-id="b1e02-111">Fill in the fields on the card.</span></span> <span data-ttu-id="b1e02-112">Следующие поля являются обязательными: **Код товара**, **Код склада** и/или **Код варианта**.</span><span class="sxs-lookup"><span data-stu-id="b1e02-112">The following fields are required: **Item No.**, **Location Code**, and/or **Variant Code**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

<span data-ttu-id="b1e02-113">После настройки первой единицы хранения для товара устанавливается флажок **Есть единица хранения** в карточке **Товар**.</span><span class="sxs-lookup"><span data-stu-id="b1e02-113">When you have set up the first stockkeeping unit for an item, the **Stockkeeping Unit Exists** check box on the **Item** card is selected.</span></span>  

<span data-ttu-id="b1e02-114">Для создания нескольких единиц хранения для одного товара используется пакетное задание **Создание единицы хранения**.</span><span class="sxs-lookup"><span data-stu-id="b1e02-114">To create several stockkeeping units for an item, use the **Create Stockkeeping Unit** batch job.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="b1e02-115">Информация в карточке **Единица хранения** обладает более высоким приоритетом по сравнению с информацией в карточке **Товар**.</span><span class="sxs-lookup"><span data-stu-id="b1e02-115">The information on the **Stockkeeping Unit** card has priority over the **Item** card.</span></span>

> [!Warning]
> <span data-ttu-id="b1e02-116">Если номер SKU указывается при производстве, поле **Стандартная себестоимость** не используется для выставления счетов и коррекции фактической себестоимости производимого товара.</span><span class="sxs-lookup"><span data-stu-id="b1e02-116">If the SKU is supplied through production, then the **Standard Cost** field is not used when invoicing and adjusting the actual cost of the produced item.</span></span> <span data-ttu-id="b1e02-117">Вместо этого используется поле **Стандартная себестоимость** в карточке базового товара, и все отклонения рассчитываются на базе структуры себестоимости данного товара.</span><span class="sxs-lookup"><span data-stu-id="b1e02-117">Instead, the **Standard Cost** field on the underlying item card is used, and any variances are calculated against the cost shares of that item.</span></span><br /><br />
> <span data-ttu-id="b1e02-118">Поскольку производственные спецификации и маршрутизаций не могут быть назначены единицам хранения, себестоимость единиц будет свернута, а связанный расчет доль затрат также не будет доступен для единиц хранения.</span><span class="sxs-lookup"><span data-stu-id="b1e02-118">Because production BOMs and routing cannot be assigned to SKUs, then the unit cost roll-up and the related calculation of cost shares are also not available on SKUs.</span></span> <span data-ttu-id="b1e02-119">Дополнительные сведения см. в разделе [Расчет стандартной себестоимости](finance-about-calculating-standard-cost.md)</span><span class="sxs-lookup"><span data-stu-id="b1e02-119">For more information, see [About Calculating Standard Cost](finance-about-calculating-standard-cost.md)</span></span>

## <a name="see-also"></a><span data-ttu-id="b1e02-120">См. также</span><span class="sxs-lookup"><span data-stu-id="b1e02-120">See Also</span></span>  
[<span data-ttu-id="b1e02-121">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="b1e02-121">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="b1e02-122">Настройка управления складом</span><span class="sxs-lookup"><span data-stu-id="b1e02-122">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
[<span data-ttu-id="b1e02-123">Управление складом</span><span class="sxs-lookup"><span data-stu-id="b1e02-123">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="b1e02-124">Наличие</span><span class="sxs-lookup"><span data-stu-id="b1e02-124">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="b1e02-125">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="b1e02-125">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="b1e02-126">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="b1e02-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="b1e02-127">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b1e02-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
