---
title: Практическое руководство. Настройка экспедиторов | Документация Майкрософт
description: Для каждого экспедитора можно задать код и указать соответствующую информацию.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 221578a174c6bd0dd87377340e97cd54a98d177b
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5778401"
---
# <a name="set-up-shipping-agents"></a><span data-ttu-id="5c3f5-103">Настройка экспедиторов</span><span class="sxs-lookup"><span data-stu-id="5c3f5-103">Set Up Shipping Agents</span></span>
<span data-ttu-id="5c3f5-104">Для каждого экспедитора можно задать код и указать соответствующую информацию.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-104">You can set up a code for each of your shipping agents and enter information about them.</span></span>  

<span data-ttu-id="5c3f5-105">Если для экспедитора указывается адрес Интернет и экспедитор предоставляет пакет услуг, связанных с трассировкой товара при помощи Интернет, можно использовать функцию автоматической трассировки посылок.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-105">If you enter an Internet address for the shipping agent, and the agent provides package tracking services on the Internet, you can use the automatic package tracking feature.</span></span> <span data-ttu-id="5c3f5-106">Дополнительные сведения см. в разделе [Трассировка посылок](sales-how-track-packages.md).</span><span class="sxs-lookup"><span data-stu-id="5c3f5-106">For more information, see [Track Packages](sales-how-track-packages.md).</span></span>

<span data-ttu-id="5c3f5-107">При настройке в заказах продажи экспедиторов можно также указать услуги, предоставляемые каждым экспедитором.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-107">When you set up shipping agents on your sales orders, you can also specify the services that each shipping agent offers.</span></span>  
<span data-ttu-id="5c3f5-108">Для каждого экспедитора можно настроить неограниченное количество услуг и по каждой услуге указать время отгрузки.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-108">For each shipping agent, you can set up an unlimited number of services, and you can specify a shipping time for each service.</span></span>  

<span data-ttu-id="5c3f5-109">После того, как для строки продажи задана услуга экспедитора, время отгрузки для услуги будет включаться в расчет сроков по заказу для данной строки.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-109">When you have assigned a shipping agent service to a sales order line, the shipping time of the service will be included in the order promising calculation, for that line.</span></span> <span data-ttu-id="5c3f5-110">Дополнительные сведения см. в разделе [Расчет сроков планирования заказов](sales-how-to-calculate-order-promising-dates.md).</span><span class="sxs-lookup"><span data-stu-id="5c3f5-110">For more information, see [Calculate Order Promising Dates](sales-how-to-calculate-order-promising-dates.md).</span></span>

## <a name="to-set-up-a-shipping-agent"></a><span data-ttu-id="5c3f5-111">Настройка экспедитора</span><span class="sxs-lookup"><span data-stu-id="5c3f5-111">To set up a shipping agent</span></span>  
1.  <span data-ttu-id="5c3f5-112">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Экспедиторы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shipping Agents**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5c3f5-113">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-113">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="5c3f5-114">.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-114">.</span></span>  
3.  <span data-ttu-id="5c3f5-115">Выберите действие **Услуги экспедитора**.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-115">Choose the **Shipping Agent Services** action.</span></span>
4. <span data-ttu-id="5c3f5-116">В поле **Услуги экспедитора** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-116">In the **Shipping Agent Services**, fill in the fields as necessary.</span></span>

> [!NOTE]  
>  <span data-ttu-id="5c3f5-117">Если удалить экспедитора из строки заказа, код услуги экспедитора для данной строки также будет удален.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-117">If you delete the shipping agent on the order line, the shipping agent service code is also deleted.</span></span> <span data-ttu-id="5c3f5-118">Производится пересчет содержимого полей, которые были частично связаны с данной услугой экспедитора.</span><span class="sxs-lookup"><span data-stu-id="5c3f5-118">The contents of fields that were based in part on the shipping agent service are recalculated.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5c3f5-119">См. также</span><span class="sxs-lookup"><span data-stu-id="5c3f5-119">See Also</span></span>
[<span data-ttu-id="5c3f5-120">Настройка методов отгрузки</span><span class="sxs-lookup"><span data-stu-id="5c3f5-120">Set Up Shipment Methods</span></span>](sales-how-set-up-shipment-methods.md)  
<span data-ttu-id="5c3f5-121">[Трассировка посылок](sales-how-track-packages.md)  </span><span class="sxs-lookup"><span data-stu-id="5c3f5-121">[Track Packages](sales-how-track-packages.md)  </span></span>  
[<span data-ttu-id="5c3f5-122">Управление складом</span><span class="sxs-lookup"><span data-stu-id="5c3f5-122">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="5c3f5-123">Запасы</span><span class="sxs-lookup"><span data-stu-id="5c3f5-123">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="5c3f5-124">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="5c3f5-124">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="5c3f5-125">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="5c3f5-125">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="5c3f5-126">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="5c3f5-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="5c3f5-127">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5c3f5-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]