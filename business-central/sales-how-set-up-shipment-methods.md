---
title: Настройка методов отгрузки
description: Для предлагаемого метода отгрузки можно задать код и указать соответствующую информацию.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: incoterms
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 8390c95083eb02c208e97f0309a725e8ec4d7730
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5778576"
---
# <a name="set-up-shipment-methods"></a><span data-ttu-id="c3d89-103">Настройка методов отгрузки</span><span class="sxs-lookup"><span data-stu-id="c3d89-103">Set Up Shipment Methods</span></span>

<span data-ttu-id="c3d89-104">Часто методы отгрузки зависят от товаров, клиентов и поставщиков.</span><span class="sxs-lookup"><span data-stu-id="c3d89-104">Shipment methods often depend on the items, the customers, and the vendors.</span></span> <span data-ttu-id="c3d89-105">Например, если клиент живет на острове, то товары могут быть ему отправлены или по воздуху, или морем.</span><span class="sxs-lookup"><span data-stu-id="c3d89-105">For example, if the customer lives on an island, they can choose to have items always shipped by air or always by sea.</span></span> <span data-ttu-id="c3d89-106">Некоторым клиентам может потребоваться доставка на следующий день.</span><span class="sxs-lookup"><span data-stu-id="c3d89-106">Some customers may require next day delivery.</span></span> <span data-ttu-id="c3d89-107">Другие могут захотеть забрать заказ.</span><span class="sxs-lookup"><span data-stu-id="c3d89-107">Some may want to pick up the order.</span></span> <span data-ttu-id="c3d89-108">В карточках клиента и поставщика определяется требуемый тип доставки.</span><span class="sxs-lookup"><span data-stu-id="c3d89-108">On the customer and vendor cards, you can specify what sort of delivery is desired.</span></span>

<span data-ttu-id="c3d89-109">Описание и код каждого метода отгрузки настраивается на странице **Методы отгрузки**.</span><span class="sxs-lookup"><span data-stu-id="c3d89-109">You set up the description and code for each shipment method on the **Shipment Methods** page.</span></span> <span data-ttu-id="c3d89-110">Например, можно настроить код ФОБ и ввести "Франко-борт" в поле **Описание**.</span><span class="sxs-lookup"><span data-stu-id="c3d89-110">For example, you can set up the code FOB, and enter Free on Board in the **Description** field.</span></span> <span data-ttu-id="c3d89-111">Затем код можно ввести в поля **Код метода отгрузки** по всей программе, например, в карточку клиента.</span><span class="sxs-lookup"><span data-stu-id="c3d89-111">You can then enter the code in **Shipment Method Code** fields elsewhere in the system, such as on a customer card.</span></span> <span data-ttu-id="c3d89-112">После этого при создании заказов, счетов, кредит-нот и т. д. программа будет вводить описание, представленное данным кодом.</span><span class="sxs-lookup"><span data-stu-id="c3d89-112">Then when you create new orders, invoices, credit memos, and so on, the system will enter the description represented by the code.</span></span> <span data-ttu-id="c3d89-113">При необходимости его можно изменить в документе.</span><span class="sxs-lookup"><span data-stu-id="c3d89-113">You can change it on the document as needed.</span></span>

## <a name="to-set-up-a-shipment-method"></a><span data-ttu-id="c3d89-114">Настройка метода отгрузки</span><span class="sxs-lookup"><span data-stu-id="c3d89-114">To set up a shipment method</span></span>

1. <span data-ttu-id="c3d89-115">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Методы отгрузки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="c3d89-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shipment Methods**, and then choose the related link.</span></span>
2. <span data-ttu-id="c3d89-116">На странице **Методы отгрузки** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="c3d89-116">On the **Shipment Methods** page, choose the **New** action.</span></span>
3. <span data-ttu-id="c3d89-117">В новой строке определите код и описание для метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="c3d89-117">On the new line, specify a code and description for the shipment method.</span></span>

> [!TIP]
> <span data-ttu-id="c3d89-118">Если вы используете Инкотермс, настройте способы отгрузки для соответствующих правил Инкотермс.</span><span class="sxs-lookup"><span data-stu-id="c3d89-118">If you use Incoterms, set up shipment methods to represent the relevant Incoterms rules.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c3d89-119">См. также</span><span class="sxs-lookup"><span data-stu-id="c3d89-119">See Also</span></span>

[<span data-ttu-id="c3d89-120">Настройка экспедиторов</span><span class="sxs-lookup"><span data-stu-id="c3d89-120">Set Up Shipping Agents</span></span>](sales-how-to-set-up-shipping-agents.md)  
[<span data-ttu-id="c3d89-121">Трассировка посылок</span><span class="sxs-lookup"><span data-stu-id="c3d89-121">Track Packages</span></span>](sales-how-track-packages.md)  
[<span data-ttu-id="c3d89-122">Управление складом</span><span class="sxs-lookup"><span data-stu-id="c3d89-122">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="c3d89-123">Запасы</span><span class="sxs-lookup"><span data-stu-id="c3d89-123">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="c3d89-124">Настройка управления складом</span><span class="sxs-lookup"><span data-stu-id="c3d89-124">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
[<span data-ttu-id="c3d89-125">Управление сборкой</span><span class="sxs-lookup"><span data-stu-id="c3d89-125">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="c3d89-126">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="c3d89-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="c3d89-127">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c3d89-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="c3d89-128">Инкотермс на iccwbo.org</span><span class="sxs-lookup"><span data-stu-id="c3d89-128">Incoterms on iccwbo.org</span></span>](https://iccwbo.org/resources-for-business/incoterms-rules)  

[!INCLUDE[footer-include](includes/footer-banner.md)]