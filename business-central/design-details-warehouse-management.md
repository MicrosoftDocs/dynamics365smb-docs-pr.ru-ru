---
title: Сведения о проектировании — управление складом | Документация Майкрософт
description: Этот раздел содержит обзор дизайна, концепций и принципов, используемых в функциях управления складом в Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: efd4d06d0d16b81ca3640af46a797c359098cc08
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2306676"
---
# <a name="design-details-warehouse-management"></a><span data-ttu-id="d84f1-103">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="d84f1-103">Design Details: Warehouse Management</span></span>
<span data-ttu-id="d84f1-104">Этот документ содержит обзор концепций и принципов, использованных в функциях управления складом в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="d84f1-104">This documentation gives an overview of the concepts and principles that are used in the Warehouse Management features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="d84f1-105">В ней описывается, как работают функции центрального склада и как управление складом интегрируется с другими функциями цепочки поставок.</span><span class="sxs-lookup"><span data-stu-id="d84f1-105">It explains the design behind central warehouse features and how warehousing integrates with other supply chain features.</span></span>  

<span data-ttu-id="d84f1-106">Чтобы различать разные уровни сложности складирования, в этом документе используется две общие группы — базовые и расширенные конфигурации складирования, описываемые в одноименных разделах.</span><span class="sxs-lookup"><span data-stu-id="d84f1-106">To differentiate the different complexity levels of the warehousing, this documentation is divided into two general groups, Basic and Advanced warehouse configurations, indicated by section titles.</span></span> <span data-ttu-id="d84f1-107">Эта простая дифференциация охватывает разные уровни сложности, как определено областями продукции и настройками склада.</span><span class="sxs-lookup"><span data-stu-id="d84f1-107">This simple differentiation covers different complexity levels as defined by product granules and location setup.</span></span> <span data-ttu-id="d84f1-108">Дополнительные сведения см. в разделе [Сведения о проектировании: настройка склада](design-details-warehouse-setup.md).</span><span class="sxs-lookup"><span data-stu-id="d84f1-108">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="d84f1-109">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="d84f1-109">In This Section</span></span>  
[<span data-ttu-id="d84f1-110">Сведения о проектировании: обзор склада</span><span class="sxs-lookup"><span data-stu-id="d84f1-110">Design Details: Warehouse Overview</span></span>](design-details-warehouse-overview.md)  
[<span data-ttu-id="d84f1-111">Сведения о проектировании: настройка склада</span><span class="sxs-lookup"><span data-stu-id="d84f1-111">Design Details: Warehouse Setup</span></span>](design-details-warehouse-setup.md)  
[<span data-ttu-id="d84f1-112">Сведения о проектировании: входящий складской поток</span><span class="sxs-lookup"><span data-stu-id="d84f1-112">Design Details: Inbound Warehouse Flow</span></span>](design-details-inbound-warehouse-flow.md)  
[<span data-ttu-id="d84f1-113">Сведения о проектировании: внутренние складские потоки</span><span class="sxs-lookup"><span data-stu-id="d84f1-113">Design Details: Internal Warehouse Flows</span></span>](design-details-internal-warehouse-flows.md)  
[<span data-ttu-id="d84f1-114">Сведения о проектировании: наличие на складе</span><span class="sxs-lookup"><span data-stu-id="d84f1-114">Design Details: Availability in the Warehouse</span></span>](design-details-availability-in-the-warehouse.md)  
[<span data-ttu-id="d84f1-115">Сведения о проектировании: исходящий складской поток</span><span class="sxs-lookup"><span data-stu-id="d84f1-115">Design Details: Outbound Warehouse Flow</span></span>](design-details-outbound-warehouse-flow.md)  
[<span data-ttu-id="d84f1-116">Сведения о проектировании: интеграция с запасом</span><span class="sxs-lookup"><span data-stu-id="d84f1-116">Design Details: Integration with Inventory</span></span>](design-details-integration-with-inventory.md)
