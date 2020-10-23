---
title: Настройка кодов для стандартных сервисов | Документация Майкрософт
description: Узнайте, как настроить коды для часто выполняемых сервисных работ.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, service item, service order, repairs, maintenance
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 2db9480789e90b15e0a9d4e737817d3b8ff3b3c9
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3925834"
---
# <a name="set-up-standard-service-codes"></a><span data-ttu-id="fe9a5-103">Настройка стандартных сервисных кодов</span><span class="sxs-lookup"><span data-stu-id="fe9a5-103">Set Up Standard Service Codes</span></span>

<span data-ttu-id="fe9a5-104">При выполнении типичных сервисных операций часто необходимо создавать сервисные документы, в которых сервисные строки содержат похожую информацию.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-104">When you perform typical service, you often have to create service documents that use service lines that contain similar information.</span></span> <span data-ttu-id="fe9a5-105">Чтобы упростить создание этих строк, можно настроить стандартные сервисные коды, имеющие заранее заданный набор сервисных строк.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-105">To make it easy to create these lines, you can set up standard service codes that have a predefined set of service lines.</span></span> <span data-ttu-id="fe9a5-106">При выборе кода в сервисном документе эти строки вводятся автоматически.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-106">When you choose the code on a service document, the lines are entered automatically.</span></span> <span data-ttu-id="fe9a5-107">Можно настроить любое количество стандартных сервисных кодов, и с каждым кодом можно связать неограниченное количество сервисных строк различных типов, включая товар, ресурс, себестоимость или стандартный текст.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-107">You can set up any number of standard service codes, and each code can have an unlimited number of service lines of different types, including item, resource, cost, or standard text linked to it.</span></span> <span data-ttu-id="fe9a5-108">Сервисные строки для каждого стандартного сервисного кода создаются на карточке **Стандартный сервисный код**.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-108">You create service lines of each standard service code on the **Standard Service Code** card.</span></span> <span data-ttu-id="fe9a5-109">Можно присвоить стандартные сервисные коды группам сервисных товаров на странице **Станд. коды групп серв. товаров**.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-109">You then assign standard service codes to service item groups on the **Standard Serv. Item Gr. Codes** page.</span></span> <span data-ttu-id="fe9a5-110">Позднее при создании сервисного документа можно использовать действие **Получить стандартные коды сервиса** для добавления сервисных строк.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-110">Later, when you create a service document, you can use the **Get Standard Service Codes** action to add service lines.</span></span>  
  
> [!Tip]
> <span data-ttu-id="fe9a5-111">Можно использовать эту же концепцию для создания строк в документах продажи и покупки.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-111">You can use the same concept to create lines on sales and purchase documents.</span></span> <span data-ttu-id="fe9a5-112">Дополнительные сведения см. в разделе [Создание типовых строк продажи и покупки](sales-how-work-standard-lines.md).</span><span class="sxs-lookup"><span data-stu-id="fe9a5-112">For more information, see [Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md).</span></span>  
  
## <a name="to-set-up-a-standard-service-code"></a><span data-ttu-id="fe9a5-113">Настройка стандартного сервисного кода</span><span class="sxs-lookup"><span data-stu-id="fe9a5-113">To set up a standard service code</span></span>

1. <span data-ttu-id="fe9a5-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Стандартные сервисные коды**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Standard Service Codes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fe9a5-115">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="fe9a5-116">Заполните строки сервиса, связанные с данным сервисным кодом.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-116">Fill in the service lines linked to this service code.</span></span>  

## <a name="to-assign-a-standard-service-code-to-a-service-item-group"></a><span data-ttu-id="fe9a5-117">Присвоение стандартного сервисного кода группе сервисных товаров</span><span class="sxs-lookup"><span data-stu-id="fe9a5-117">To assign a standard service code to a service item group</span></span>

1. <span data-ttu-id="fe9a5-118">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Группы сервисных товаров**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service item Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fe9a5-119">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-119">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="fe9a5-120">Заполните строки сервиса, связанные с данным сервисным кодом.</span><span class="sxs-lookup"><span data-stu-id="fe9a5-120">Fill in the service lines linked to this service code.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fe9a5-121">См. также</span><span class="sxs-lookup"><span data-stu-id="fe9a5-121">See Also</span></span>

[<span data-ttu-id="fe9a5-122">Управление сервисом</span><span class="sxs-lookup"><span data-stu-id="fe9a5-122">Service Management</span></span>](service-service.md)