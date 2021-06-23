---
title: Сведения о проектировании — управление складом | Документация Майкрософт
description: Этот раздел содержит обзор дизайна, концепций и принципов, используемых в функциях управления складом в Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 7a0576ce3141c9c35933ac78e11c3bfdcb0ba7f8
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "6214607"
---
# <a name="design-details-warehouse-management"></a><span data-ttu-id="faf79-103">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="faf79-103">Design Details: Warehouse Management</span></span>
<span data-ttu-id="faf79-104">Этот документ содержит обзор концепций и принципов, использованных в функциях управления складом в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="faf79-104">This documentation gives an overview of the concepts and principles that are used in the Warehouse Management features in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="faf79-105">В ней описывается, как работают функции центрального склада и как управление складом интегрируется с другими функциями цепочки поставок.</span><span class="sxs-lookup"><span data-stu-id="faf79-105">It explains the design behind central warehouse features and how warehousing integrates with other supply chain features.</span></span>  

<span data-ttu-id="faf79-106">Чтобы различать разные уровни сложности складирования, в этом документе используется две общие группы — базовые и расширенные конфигурации складирования, описываемые в одноименных разделах.</span><span class="sxs-lookup"><span data-stu-id="faf79-106">To differentiate the different complexity levels of the warehousing, this documentation is divided into two general groups, Basic and Advanced warehouse configurations, indicated by section titles.</span></span> <span data-ttu-id="faf79-107">Эта простая дифференциация охватывает разные уровни сложности, как определено областями продукции и настройками склада.</span><span class="sxs-lookup"><span data-stu-id="faf79-107">This simple differentiation covers different complexity levels as defined by product granules and location setup.</span></span> <span data-ttu-id="faf79-108">Дополнительные сведения см. в разделе [Сведения о проектировании: настройка склада](design-details-warehouse-setup.md).</span><span class="sxs-lookup"><span data-stu-id="faf79-108">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="faf79-109">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="faf79-109">In This Section</span></span>  
[<span data-ttu-id="faf79-110">Сведения о проектировании: обзор склада</span><span class="sxs-lookup"><span data-stu-id="faf79-110">Design Details: Warehouse Overview</span></span>](design-details-warehouse-overview.md)  
[<span data-ttu-id="faf79-111">Сведения о проектировании: настройка склада</span><span class="sxs-lookup"><span data-stu-id="faf79-111">Design Details: Warehouse Setup</span></span>](design-details-warehouse-setup.md)  
[<span data-ttu-id="faf79-112">Сведения о проектировании: входящий складской поток</span><span class="sxs-lookup"><span data-stu-id="faf79-112">Design Details: Inbound Warehouse Flow</span></span>](design-details-inbound-warehouse-flow.md)  
[<span data-ttu-id="faf79-113">Сведения о проектировании: внутренние складские потоки</span><span class="sxs-lookup"><span data-stu-id="faf79-113">Design Details: Internal Warehouse Flows</span></span>](design-details-internal-warehouse-flows.md)  
[<span data-ttu-id="faf79-114">Сведения о проектировании: наличие на складе</span><span class="sxs-lookup"><span data-stu-id="faf79-114">Design Details: Availability in the Warehouse</span></span>](design-details-availability-in-the-warehouse.md)  
[<span data-ttu-id="faf79-115">Сведения о проектировании: исходящий складской поток</span><span class="sxs-lookup"><span data-stu-id="faf79-115">Design Details: Outbound Warehouse Flow</span></span>](design-details-outbound-warehouse-flow.md)  
[<span data-ttu-id="faf79-116">Сведения о проектировании: интеграция с запасом</span><span class="sxs-lookup"><span data-stu-id="faf79-116">Design Details: Integration with Inventory</span></span>](design-details-integration-with-inventory.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]