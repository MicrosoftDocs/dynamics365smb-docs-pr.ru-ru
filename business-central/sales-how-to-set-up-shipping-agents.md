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
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: b1c5b0940998531601f0ab1c604c31328ce2bd66
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2882858"
---
# <a name="set-up-shipping-agents"></a><span data-ttu-id="e33d0-103">Настройка экспедиторов</span><span class="sxs-lookup"><span data-stu-id="e33d0-103">Set Up Shipping Agents</span></span>
<span data-ttu-id="e33d0-104">Для каждого экспедитора можно задать код и указать соответствующую информацию.</span><span class="sxs-lookup"><span data-stu-id="e33d0-104">You can set up a code for each of your shipping agents and enter information about them.</span></span>  

<span data-ttu-id="e33d0-105">Если для экспедитора указывается адрес Интернет и экспедитор предоставляет пакет услуг, связанных с трассировкой товара при помощи Интернет, можно использовать функцию автоматической трассировки посылок.</span><span class="sxs-lookup"><span data-stu-id="e33d0-105">If you enter an Internet address for the shipping agent, and the agent provides package tracking services on the Internet, you can use the automatic package tracking feature.</span></span> <span data-ttu-id="e33d0-106">Дополнительные сведения см. в разделе [Трассировка посылок](sales-how-track-packages.md).</span><span class="sxs-lookup"><span data-stu-id="e33d0-106">For more information, see [Track Packages](sales-how-track-packages.md).</span></span>

<span data-ttu-id="e33d0-107">При настройке в заказах продажи экспедиторов можно также указать услуги, предоставляемые каждым экспедитором.</span><span class="sxs-lookup"><span data-stu-id="e33d0-107">When you set up shipping agents on your sales orders, you can also specify the services that each shipping agent offers.</span></span>  
<span data-ttu-id="e33d0-108">Для каждого экспедитора можно настроить неограниченное количество услуг и по каждой услуге указать время отгрузки.</span><span class="sxs-lookup"><span data-stu-id="e33d0-108">For each shipping agent, you can set up an unlimited number of services, and you can specify a shipping time for each service.</span></span>  

<span data-ttu-id="e33d0-109">После того, как для строки продажи задана услуга экспедитора, время отгрузки для услуги будет включаться в расчет сроков по заказу для данной строки.</span><span class="sxs-lookup"><span data-stu-id="e33d0-109">When you have assigned a shipping agent service to a sales order line, the shipping time of the service will be included in the order promising calculation, for that line.</span></span> <span data-ttu-id="e33d0-110">Дополнительные сведения см. в разделе [Расчет сроков планирования заказов](sales-how-to-calculate-order-promising-dates.md).</span><span class="sxs-lookup"><span data-stu-id="e33d0-110">For more information, see [Calculate Order Promising Dates](sales-how-to-calculate-order-promising-dates.md).</span></span>

## <a name="to-set-up-a-shipping-agent"></a><span data-ttu-id="e33d0-111">Настройка экспедитора</span><span class="sxs-lookup"><span data-stu-id="e33d0-111">To set up a shipping agent</span></span>  
1.  <span data-ttu-id="e33d0-112">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Экспедиторы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e33d0-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shipping Agents**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e33d0-113">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="e33d0-113">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="e33d0-114">.</span><span class="sxs-lookup"><span data-stu-id="e33d0-114">.</span></span>  
3.  <span data-ttu-id="e33d0-115">Выберите действие **Услуги экспедитора**.</span><span class="sxs-lookup"><span data-stu-id="e33d0-115">Choose the **Shipping Agent Services** action.</span></span>
4. <span data-ttu-id="e33d0-116">В поле **Услуги экспедитора** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="e33d0-116">In the **Shipping Agent Services**, fill in the fields as necessary.</span></span>

> [!NOTE]  
>  <span data-ttu-id="e33d0-117">Если удалить экспедитора из строки заказа, код услуги экспедитора для данной строки также будет удален.</span><span class="sxs-lookup"><span data-stu-id="e33d0-117">If you delete the shipping agent on the order line, the shipping agent service code is also deleted.</span></span> <span data-ttu-id="e33d0-118">Производится пересчет содержимого полей, которые были частично связаны с данной услугой экспедитора.</span><span class="sxs-lookup"><span data-stu-id="e33d0-118">The contents of fields that were based in part on the shipping agent service are recalculated.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e33d0-119">См. также</span><span class="sxs-lookup"><span data-stu-id="e33d0-119">See Also</span></span>
[<span data-ttu-id="e33d0-120">Настройка методов отгрузки</span><span class="sxs-lookup"><span data-stu-id="e33d0-120">Set Up Shipment Methods</span></span>](sales-how-set-up-shipment-methods.md)  
<span data-ttu-id="e33d0-121">[Трассировка посылок](sales-how-track-packages.md)  </span><span class="sxs-lookup"><span data-stu-id="e33d0-121">[Track Packages](sales-how-track-packages.md)  </span></span>  
[<span data-ttu-id="e33d0-122">Управление складом</span><span class="sxs-lookup"><span data-stu-id="e33d0-122">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="e33d0-123">Запасы</span><span class="sxs-lookup"><span data-stu-id="e33d0-123">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="e33d0-124">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="e33d0-124">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="e33d0-125">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="e33d0-125">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="e33d0-126">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="e33d0-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="e33d0-127">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e33d0-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
