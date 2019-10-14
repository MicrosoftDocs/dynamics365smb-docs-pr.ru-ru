---
title: Практическое руководство. Настройка методов отгрузки | Документация Майкрософт
description: Для предлагаемого метода отгрузки можно задать код и указать соответствующую информацию.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: incoterms
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: be65cd62cec984cd2571b6e88998dc169741f376
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2312080"
---
# <a name="set-up-shipment-methods"></a><span data-ttu-id="b54bd-103">Настройка методов отгрузки</span><span class="sxs-lookup"><span data-stu-id="b54bd-103">Set Up Shipment Methods</span></span>
<span data-ttu-id="b54bd-104">Зачастую методы отгрузки, называемые также ИНКОТЕРМС, зависят от товаров, клиентов и поставщиков.</span><span class="sxs-lookup"><span data-stu-id="b54bd-104">Shipment methods, also called incoterms, often depend on the items, the customers, and the vendors.</span></span> <span data-ttu-id="b54bd-105">Например, если клиент живет на острове, то товары могут быть ему отправлены или по воздуху, или морем.</span><span class="sxs-lookup"><span data-stu-id="b54bd-105">For example, if the customer lives on an island, they can choose to have items always shipped by air or always by sea.</span></span> <span data-ttu-id="b54bd-106">Некоторым клиентам может потребоваться доставка на следующий день.</span><span class="sxs-lookup"><span data-stu-id="b54bd-106">Some customers may require next day delivery.</span></span> <span data-ttu-id="b54bd-107">Другие могут захотеть забрать заказ.</span><span class="sxs-lookup"><span data-stu-id="b54bd-107">Some may want to pick up the order.</span></span> <span data-ttu-id="b54bd-108">В карточках клиента и поставщика определяется требуемый тип доставки.</span><span class="sxs-lookup"><span data-stu-id="b54bd-108">On the customer and vendor cards, you can specify what sort of delivery is desired.</span></span>

<span data-ttu-id="b54bd-109">Описание и код каждого метода отгрузки настраивается на странице **Методы отгрузки**.</span><span class="sxs-lookup"><span data-stu-id="b54bd-109">You set up the description and code for each shipment method on the **Shipment Methods** page.</span></span> <span data-ttu-id="b54bd-110">Например, можно настроить код ФОБ и ввести "Франко-борт" в поле **Описание**.</span><span class="sxs-lookup"><span data-stu-id="b54bd-110">For example, you can set up the code FOB, and enter Free on Board in the **Description** field.</span></span> <span data-ttu-id="b54bd-111">Затем код можно ввести в поля **Код метода отгрузки** по всей программе, например, в карточку клиента.</span><span class="sxs-lookup"><span data-stu-id="b54bd-111">You can then enter the code in **Shipment Method Code** fields elsewhere in the system, such as on a customer card.</span></span> <span data-ttu-id="b54bd-112">После этого при создании заказов, счетов, кредит-нот и т. д. программа будет вводить описание, представленное данным кодом.</span><span class="sxs-lookup"><span data-stu-id="b54bd-112">Then when you create new orders, invoices, credit memos, and so on, the system will enter the description represented by the code.</span></span> <span data-ttu-id="b54bd-113">При необходимости его можно изменить в документе.</span><span class="sxs-lookup"><span data-stu-id="b54bd-113">You can change it on the document as needed.</span></span>

## <a name="to-set-up-a-shipment-code"></a><span data-ttu-id="b54bd-114">Настройка кода отгрузки</span><span class="sxs-lookup"><span data-stu-id="b54bd-114">To set up a shipment code</span></span>
1. <span data-ttu-id="b54bd-115">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Методы отгрузки**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b54bd-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shipment Methods**, and then choose the related link.</span></span>
2. <span data-ttu-id="b54bd-116">На странице **Методы отгрузки** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="b54bd-116">On the **Shipment Methods** page, choose the **New** action.</span></span>
3. <span data-ttu-id="b54bd-117">В новой строке определите код и описание для метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="b54bd-117">On the new line, specify a code and description for the shipment method.</span></span>

## <a name="see-also"></a><span data-ttu-id="b54bd-118">См. также</span><span class="sxs-lookup"><span data-stu-id="b54bd-118">See Also</span></span>
[<span data-ttu-id="b54bd-119">Инкотермс</span><span class="sxs-lookup"><span data-stu-id="b54bd-119">Incoterms</span></span>](https://iccwbo.org/resources-for-business/incoterms-rules)  
[<span data-ttu-id="b54bd-120">Настройка экспедиторов</span><span class="sxs-lookup"><span data-stu-id="b54bd-120">Set Up Shipping Agents</span></span>](sales-how-to-set-up-shipping-agents.md)  
<span data-ttu-id="b54bd-121">[Трассировка посылок](sales-how-track-packages.md)  </span><span class="sxs-lookup"><span data-stu-id="b54bd-121">[Track Packages](sales-how-track-packages.md)  </span></span>  
[<span data-ttu-id="b54bd-122">Управление складом</span><span class="sxs-lookup"><span data-stu-id="b54bd-122">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="b54bd-123">Запасы</span><span class="sxs-lookup"><span data-stu-id="b54bd-123">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="b54bd-124">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="b54bd-124">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="b54bd-125">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="b54bd-125">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="b54bd-126">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="b54bd-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="b54bd-127">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b54bd-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
