---
title: "Создание карточки клиента для регистрации нового клиента | Документы Майкрософт"
description: "Описывается процедура создания карточки клиента для регистрации информации о каждом новом клиенте, которому вы что-либо продаете."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: client
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: a03575bce7d1029e47f2aa1a46d5d0dcf585ab2a
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="register-new-customers"></a><span data-ttu-id="c02a8-103">Регистрация новых клиентов</span><span class="sxs-lookup"><span data-stu-id="c02a8-103">Register New Customers</span></span>
<span data-ttu-id="c02a8-104">Клиенты — это источник доходов.</span><span class="sxs-lookup"><span data-stu-id="c02a8-104">Customers are the source of your income.</span></span> <span data-ttu-id="c02a8-105">Необходимо зарегистрировать каждого клиента, которому осуществляется продажа, в карточке клиента.</span><span class="sxs-lookup"><span data-stu-id="c02a8-105">You must register each customer you sell to as a customer card.</span></span> <span data-ttu-id="c02a8-106">Карточки клиентов содержат сведения, необходимые для продажи продуктов клиенту.</span><span class="sxs-lookup"><span data-stu-id="c02a8-106">Customer cards hold the information that is required to sell products to the customer.</span></span> <span data-ttu-id="c02a8-107">Дополнительные сведения см. в разделах [Выставление счетов продажи](sales-how-invoice-sales.md) и [Регистрация новых товаров](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="c02a8-107">For more information, see [Invoice Sales](sales-how-invoice-sales.md) and [Register New Items](inventory-how-register-new-items.md).</span></span>  

<span data-ttu-id="c02a8-108">Перед регистрацией новых клиентов необходимо настроить различные коды продажи, которые можно будет выбирать при заполнении карточек клиентов.</span><span class="sxs-lookup"><span data-stu-id="c02a8-108">Before you can register new customers, you must set up various sales codes that you can select from when you fill in customer cards.</span></span> <span data-ttu-id="c02a8-109">Дополнительные сведения см. в разделе [Настройка продаж](sales-setup-sales.md).</span><span class="sxs-lookup"><span data-stu-id="c02a8-109">For more information, see [Setting Up Sales](sales-setup-sales.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="c02a8-110">Если существуют шаблоны клиентов для различных типов клиентов, при создании новой карточки клиента отобразится окно, из которого можно выбрать подходящий шаблон.</span><span class="sxs-lookup"><span data-stu-id="c02a8-110">If customer templates exist for different customer types, then a window appears when you create a new customer card from where you can select an appropriate template.</span></span> <span data-ttu-id="c02a8-111">Если существует только один шаблон клиента, для создания новых карточек клиентов всегда используется этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="c02a8-111">If only one customer template exists, then new customer cards always use that template.</span></span>

## <a name="to-create-a-new-customer-card"></a><span data-ttu-id="c02a8-112">Создание новой карточки клиента</span><span class="sxs-lookup"><span data-stu-id="c02a8-112">To create a new customer card</span></span>
1. <span data-ttu-id="c02a8-113">На начальной странице выберите действие **Клиенты**, чтобы открыть список существующих клиентов.</span><span class="sxs-lookup"><span data-stu-id="c02a8-113">On the Home page, choose the **Customers** action to open the list of existing customers.</span></span>  
2. <span data-ttu-id="c02a8-114">В окне **Клиенты** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="c02a8-114">In the **Customers** window, choose the **New** action.</span></span>

    <span data-ttu-id="c02a8-115">Если существует только один шаблон клиента, откроется новая карточка клиента, некоторые поля которой будут заполнены сведениями из шаблона.</span><span class="sxs-lookup"><span data-stu-id="c02a8-115">If only one customer template exists, then a new customer card opens with some fields filled with information from the template.</span></span>

    <span data-ttu-id="c02a8-116">Если существует несколько шаблонов клиентов, будет открыто окно, в котором можно будет выбрать шаблон клиента.</span><span class="sxs-lookup"><span data-stu-id="c02a8-116">If more than one customer template exists, then a window opens from which you can select a customer template.</span></span> <span data-ttu-id="c02a8-117">В этом случае выполните следующие два действия.</span><span class="sxs-lookup"><span data-stu-id="c02a8-117">In that case, follow the next two steps.</span></span>
3. <span data-ttu-id="c02a8-118">В окне **Выбор шаблона для нового клиента** выберите шаблон, который требуется использовать для новой карточки клиента.</span><span class="sxs-lookup"><span data-stu-id="c02a8-118">In the **Select a template for a new customer** window, choose the template that you want to use for the new customer card.</span></span>
4. <span data-ttu-id="c02a8-119">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="c02a8-119">Choose the **OK** button.</span></span> <span data-ttu-id="c02a8-120">Откроется новая карточка клиента, некоторые поля которой будут заполнены сведениями из шаблона.</span><span class="sxs-lookup"><span data-stu-id="c02a8-120">A new customer card opens with some fields filled with information from the template.</span></span>  
5. <span data-ttu-id="c02a8-121">Заполните или измените поля в карточке клиента по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="c02a8-121">Proceed to fill or change fields on the customer card as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="c02a8-122">На экспресс-вкладке **Цены продажи** вы можете увидеть специальные цены или скидки, предоставляемые для клиента при соблюдении определенных критериев, например по товару, минимальному количеству заказа или дате окончания.</span><span class="sxs-lookup"><span data-stu-id="c02a8-122">On the **Sales Prices** FastTab, you can view special prices or discounts that you grant for the customer if certain criteria are met, such as item, minimum order quantity, or ending date.</span></span> <span data-ttu-id="c02a8-123">Каждая строка представляет специальную цену или скидку строки.</span><span class="sxs-lookup"><span data-stu-id="c02a8-123">Each row represents a special price or line discount.</span></span> <span data-ttu-id="c02a8-124">В каждом столбце представлен критерий, который необходимо применить, чтобы гарантировать специальную цену, введенную в поле **Цена за единицу**, или скидку строки, вводимую в поле **Скидка строки %**.</span><span class="sxs-lookup"><span data-stu-id="c02a8-124">Each column represents a criterion that must apply to warrant the special price that you enter in the **Unit Price** field, or the line discount that you enter in the **Line Discount %** field.</span></span> <span data-ttu-id="c02a8-125">Дополнительные сведения см. в разделе [Регистрация соглашений о цене продажи, скидках и платежах](sales-how-record-sales-price-discount-payment-agreements.md).</span><span class="sxs-lookup"><span data-stu-id="c02a8-125">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span></span>

<span data-ttu-id="c02a8-126">Теперь клиент зарегистрирован, и карточка клиента готова к использованию в документах продажи.</span><span class="sxs-lookup"><span data-stu-id="c02a8-126">The customer is now registered, and the customer card is ready to be used on sales documents.</span></span>

<span data-ttu-id="c02a8-127">Если эту карточку клиента требуется использовать в качестве шаблона при создании новых карточек клиентов, ее можно сохранить в качестве шаблона.</span><span class="sxs-lookup"><span data-stu-id="c02a8-127">If you want to use this customer card as a template when you create new customer cards, you can save it as a template.</span></span> <span data-ttu-id="c02a8-128">Дополнительные сведения см. в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="c02a8-128">For more information, see the following section.</span></span>

## <a name="to-save-the-customer-card-as-a-template"></a><span data-ttu-id="c02a8-129">Сохранение карточки клиента в качестве шаблона</span><span class="sxs-lookup"><span data-stu-id="c02a8-129">To save the customer card as a template</span></span>
1. <span data-ttu-id="c02a8-130">В окне **Карточка клиента** выберите действие **Сохранить как шаблон**.</span><span class="sxs-lookup"><span data-stu-id="c02a8-130">In the **Customer Card** window, choose the **Save as Template** action.</span></span> <span data-ttu-id="c02a8-131">Окно **Шаблон клиента** открывается с карточкой клиента в виде шаблона.</span><span class="sxs-lookup"><span data-stu-id="c02a8-131">The **Customer Template** window opens showing the customer card as a template.</span></span>
2. <span data-ttu-id="c02a8-132">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="c02a8-132">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="c02a8-133">Для повторного использования измерений в шаблонах, выберите действие **Измерения**.</span><span class="sxs-lookup"><span data-stu-id="c02a8-133">To reuse dimensions in templates, choose the **Dimensions** action.</span></span> <span data-ttu-id="c02a8-134">Открывается окно **Шаблоны измерений** с отображением кодов измерений, настроенных для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="c02a8-134">The **Dimension Templates** window opens showing any dimension codes that are set up for the customer.</span></span>
4. <span data-ttu-id="c02a8-135">Измените или введите коды измерений, которые будут применяться к новым карточкам клиентов, созданным с помощью шаблона.</span><span class="sxs-lookup"><span data-stu-id="c02a8-135">Edit or enter dimension codes that will apply to new customer cards created by using the template.</span></span>  
5. <span data-ttu-id="c02a8-136">Заполнив шаблон нового клиента, нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="c02a8-136">When you have completed the new customer template, choose the **OK** button.</span></span>

<span data-ttu-id="c02a8-137">Шаблон клиента добавляется в список шаблонов клиентов, чтобы можно было использовать его для создания новых карточек клиентов.</span><span class="sxs-lookup"><span data-stu-id="c02a8-137">The customer template is added to the list of customer templates, so that you can use it to create new customer cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="c02a8-138">См. также</span><span class="sxs-lookup"><span data-stu-id="c02a8-138">See Also</span></span>
<span data-ttu-id="c02a8-139">[Sales](sales-manage-sales.md)  </span><span class="sxs-lookup"><span data-stu-id="c02a8-139">[Sales](sales-manage-sales.md)  </span></span>  
<span data-ttu-id="c02a8-140">[Настройка продаж](sales-setup-sales.md)  </span><span class="sxs-lookup"><span data-stu-id="c02a8-140">[Setting Up Sales](sales-setup-sales.md)  </span></span>  
<span data-ttu-id="c02a8-141">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c02a8-141">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

