---
title: Практическое руководство. Настройка экспедиторов | Документация Майкрософт
description: Для каждого экспедитора можно задать код и указать соответствующую информацию.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: d6a4bac4d540a65cc164029b23b063c8c9dbc1fb
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3192662"
---
# <a name="set-up-shipping-agents"></a><span data-ttu-id="7e1d2-103">Настройка экспедиторов</span><span class="sxs-lookup"><span data-stu-id="7e1d2-103">Set Up Shipping Agents</span></span>
<span data-ttu-id="7e1d2-104">Для каждого экспедитора можно задать код и указать соответствующую информацию.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-104">You can set up a code for each of your shipping agents and enter information about them.</span></span>  

<span data-ttu-id="7e1d2-105">Если для экспедитора указывается адрес Интернет и экспедитор предоставляет пакет услуг, связанных с трассировкой товара при помощи Интернет, можно использовать функцию автоматической трассировки посылок.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-105">If you enter an Internet address for the shipping agent, and the agent provides package tracking services on the Internet, you can use the automatic package tracking feature.</span></span> <span data-ttu-id="7e1d2-106">Дополнительные сведения см. в разделе [Трассировка посылок](sales-how-track-packages.md).</span><span class="sxs-lookup"><span data-stu-id="7e1d2-106">For more information, see [Track Packages](sales-how-track-packages.md).</span></span>

<span data-ttu-id="7e1d2-107">При настройке в заказах продажи экспедиторов можно также указать услуги, предоставляемые каждым экспедитором.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-107">When you set up shipping agents on your sales orders, you can also specify the services that each shipping agent offers.</span></span>  
<span data-ttu-id="7e1d2-108">Для каждого экспедитора можно настроить неограниченное количество услуг и по каждой услуге указать время отгрузки.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-108">For each shipping agent, you can set up an unlimited number of services, and you can specify a shipping time for each service.</span></span>  

<span data-ttu-id="7e1d2-109">После того, как для строки продажи задана услуга экспедитора, время отгрузки для услуги будет включаться в расчет сроков по заказу для данной строки.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-109">When you have assigned a shipping agent service to a sales order line, the shipping time of the service will be included in the order promising calculation, for that line.</span></span> <span data-ttu-id="7e1d2-110">Дополнительные сведения см. в разделе [Расчет сроков планирования заказов](sales-how-to-calculate-order-promising-dates.md).</span><span class="sxs-lookup"><span data-stu-id="7e1d2-110">For more information, see [Calculate Order Promising Dates](sales-how-to-calculate-order-promising-dates.md).</span></span>

## <a name="to-set-up-a-shipping-agent"></a><span data-ttu-id="7e1d2-111">Настройка экспедитора</span><span class="sxs-lookup"><span data-stu-id="7e1d2-111">To set up a shipping agent</span></span>  
1.  <span data-ttu-id="7e1d2-112">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Экспедиторы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shipping Agents**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7e1d2-113">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-113">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="7e1d2-114">.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-114">.</span></span>  
3.  <span data-ttu-id="7e1d2-115">Выберите действие **Услуги экспедитора**.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-115">Choose the **Shipping Agent Services** action.</span></span>
4. <span data-ttu-id="7e1d2-116">В поле **Услуги экспедитора** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-116">In the **Shipping Agent Services**, fill in the fields as necessary.</span></span>

> [!NOTE]  
>  <span data-ttu-id="7e1d2-117">Если удалить экспедитора из строки заказа, код услуги экспедитора для данной строки также будет удален.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-117">If you delete the shipping agent on the order line, the shipping agent service code is also deleted.</span></span> <span data-ttu-id="7e1d2-118">Производится пересчет содержимого полей, которые были частично связаны с данной услугой экспедитора.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-118">The contents of fields that were based in part on the shipping agent service are recalculated.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7e1d2-119">См. также</span><span class="sxs-lookup"><span data-stu-id="7e1d2-119">See Also</span></span>
[<span data-ttu-id="7e1d2-120">Настройка методов отгрузки</span><span class="sxs-lookup"><span data-stu-id="7e1d2-120">Set Up Shipment Methods</span></span>](sales-how-set-up-shipment-methods.md)  
<span data-ttu-id="7e1d2-121">[Трассировка посылок](sales-how-track-packages.md)  </span><span class="sxs-lookup"><span data-stu-id="7e1d2-121">[Track Packages](sales-how-track-packages.md)  </span></span>  
[<span data-ttu-id="7e1d2-122">Управление складом</span><span class="sxs-lookup"><span data-stu-id="7e1d2-122">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="7e1d2-123">Запасы</span><span class="sxs-lookup"><span data-stu-id="7e1d2-123">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="7e1d2-124">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="7e1d2-124">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="7e1d2-125">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="7e1d2-125">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="7e1d2-126">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="7e1d2-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="7e1d2-127">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7e1d2-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
