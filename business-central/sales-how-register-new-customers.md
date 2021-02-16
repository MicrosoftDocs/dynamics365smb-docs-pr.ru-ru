---
title: Создание карточки клиента для регистрации нового клиента | Документация Майкрософт
description: Описывается процедура создания карточки клиента для регистрации информации о каждом новом клиенте, которому вы что-либо продаете.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: client
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 86527387653d198bc8cf6f7817058b5ff551e1d0
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4748323"
---
# <a name="register-new-customers"></a><span data-ttu-id="bc7aa-103">Регистрация новых клиентов</span><span class="sxs-lookup"><span data-stu-id="bc7aa-103">Register New Customers</span></span>

<span data-ttu-id="bc7aa-104">Клиенты — это источник доходов.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-104">Customers are the source of your income.</span></span> <span data-ttu-id="bc7aa-105">Необходимо зарегистрировать каждого клиента, которому осуществляется продажа, в карточке клиента.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-105">You must register each customer you sell to as a customer card.</span></span> <span data-ttu-id="bc7aa-106">Карточки клиентов содержат сведения, необходимые для продажи продуктов клиенту.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-106">Customer cards hold the information that is required to sell products to the customer.</span></span> <span data-ttu-id="bc7aa-107">Дополнительные сведения см. в разделах [Выставление счетов продажи](sales-how-invoice-sales.md) и [Регистрация новых товаров](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="bc7aa-107">For more information, see [Invoice Sales](sales-how-invoice-sales.md) and [Register New Items](inventory-how-register-new-items.md).</span></span>  

<span data-ttu-id="bc7aa-108">Перед регистрацией новых клиентов необходимо настроить различные коды продажи, которые можно будет выбирать при заполнении карточек клиентов.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-108">Before you can register new customers, you must set up various sales codes that you can select from when you fill in customer cards.</span></span> <span data-ttu-id="bc7aa-109">Дополнительные сведения см. в разделе [Настройка продаж](sales-setup-sales.md).</span><span class="sxs-lookup"><span data-stu-id="bc7aa-109">For more information, see [Setting Up Sales](sales-setup-sales.md).</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3PZsM]

## <a name="adding-new-customers"></a><span data-ttu-id="bc7aa-110">Добавление новых клиентов</span><span class="sxs-lookup"><span data-stu-id="bc7aa-110">Adding new customers</span></span>

<span data-ttu-id="bc7aa-111">Чтобы зарегистрировать нового клиента, необходимо заполнить карточку клиента.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-111">To register a new customer, you must fill in a customer card.</span></span> <span data-ttu-id="bc7aa-112">Вы можете создавать шаблоны для разных профилей клиентов или добавлять клиентов без шаблонов.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-112">You can establish templates for different customer profiles, or you can add customers without templates.</span></span>  

> [!NOTE]  
> <span data-ttu-id="bc7aa-113">Если существуют шаблоны клиентов для различных типов клиентов, при создании новой карточки клиента отобразится страница, с которой можно выбрать подходящий шаблон.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-113">If customer templates exist for different customer types, then a page appears when you create a new customer card from where you can select an appropriate template.</span></span> <span data-ttu-id="bc7aa-114">Если существует только один шаблон клиента, для создания новых карточек клиентов всегда используется этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-114">If only one customer template exists, then new customer cards always use that template.</span></span>  

### <a name="to-create-a-new-customer-card"></a><span data-ttu-id="bc7aa-115">Создание новой карточки клиента</span><span class="sxs-lookup"><span data-stu-id="bc7aa-115">To create a new customer card</span></span>

1. <span data-ttu-id="bc7aa-116">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиенты**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span></span>  
2. <span data-ttu-id="bc7aa-117">На странице **Клиенты** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-117">On the **Customers** page, choose the **New** action.</span></span>

    <span data-ttu-id="bc7aa-118">Если существует только один шаблон клиента, откроется новая карточка клиента, некоторые поля которой будут заполнены сведениями из шаблона.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-118">If only one customer template exists, then a new customer card opens with some fields filled with information from the template.</span></span>

    <span data-ttu-id="bc7aa-119">Если существует несколько шаблонов клиентов, будет открыта страница, на которой можно будет выбрать шаблон клиента.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-119">If more than one customer template exists, then a page opens from which you can select a customer template.</span></span> <span data-ttu-id="bc7aa-120">В этом случае выполните следующие два действия.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-120">In that case, follow the next two steps.</span></span>
3. <span data-ttu-id="bc7aa-121">На странице **Выбор шаблона для нового клиента** выберите шаблон, который требуется использовать для новой карточки клиента.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-121">On the **Select a template for a new customer** page, choose the template that you want to use for the new customer card.</span></span>
4. <span data-ttu-id="bc7aa-122">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-122">Choose the **OK** button.</span></span> <span data-ttu-id="bc7aa-123">Откроется новая карточка клиента, некоторые поля которой будут заполнены сведениями из шаблона.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-123">A new customer card opens with some fields filled with information from the template.</span></span>  
5. <span data-ttu-id="bc7aa-124">Заполните или измените поля в карточке клиента по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-124">Proceed to fill or change fields on the customer card as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="bc7aa-125">На экспресс-вкладке **Цены продажи** вы можете увидеть специальные цены или скидки, предоставляемые для клиента при соблюдении определенных критериев, например по товару, минимальному количеству заказа или дате окончания.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-125">On the **Sales Prices** FastTab, you can view special prices or discounts that you grant for the customer if certain criteria are met, such as item, minimum order quantity, or ending date.</span></span> <span data-ttu-id="bc7aa-126">Каждая строка представляет специальную цену или скидку строки.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-126">Each row represents a special price or line discount.</span></span> <span data-ttu-id="bc7aa-127">В каждом столбце представлен критерий, который необходимо применить, чтобы гарантировать специальную цену, введенную в поле **Цена за единицу**, или скидку строки, вводимую в поле **Скидка строки %**.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-127">Each column represents a criterion that must apply to warrant the special price that you enter in the **Unit Price** field, or the line discount that you enter in the **Line Discount %** field.</span></span> <span data-ttu-id="bc7aa-128">Дополнительные сведения см. в разделе [Регистрация соглашений о цене продажи, скидках и платежах](sales-how-record-sales-price-discount-payment-agreements.md).</span><span class="sxs-lookup"><span data-stu-id="bc7aa-128">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span></span>

<span data-ttu-id="bc7aa-129">Теперь клиент зарегистрирован, и карточка клиента готова к использованию в документах продажи.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-129">The customer is now registered, and the customer card is ready to be used on sales documents.</span></span>

<span data-ttu-id="bc7aa-130">Если эту карточку клиента требуется использовать в качестве шаблона при создании новых карточек клиентов, ее можно сохранить в качестве шаблона.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-130">If you want to use this customer card as a template when you create new customer cards, you can save it as a template.</span></span> <span data-ttu-id="bc7aa-131">Дополнительные сведения см. в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-131">For more information, see the following section.</span></span>  

### <a name="to-save-the-customer-card-as-a-template"></a><span data-ttu-id="bc7aa-132">Сохранение карточки клиента в качестве шаблона</span><span class="sxs-lookup"><span data-stu-id="bc7aa-132">To save the customer card as a template</span></span>

1. <span data-ttu-id="bc7aa-133">На странице **Карточка клиента** выберите действие **Сохранить как шаблон**.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-133">On the **Customer Card** page, choose the **Save as Template** action.</span></span> <span data-ttu-id="bc7aa-134">Страница **Шаблон клиента** открывается с карточкой клиента в виде шаблона.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-134">The **Customer Template** page opens showing the customer card as a template.</span></span>
2. <span data-ttu-id="bc7aa-135">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-135">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="bc7aa-136">Для повторного использования измерений в шаблонах, выберите действие **Измерения**.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-136">To reuse dimensions in templates, choose the **Dimensions** action.</span></span> <span data-ttu-id="bc7aa-137">Открывается страница **Шаблоны измерений** с отображением кодов измерений, настроенных для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-137">The **Dimension Templates** page opens showing any dimension codes that are set up for the customer.</span></span>
4. <span data-ttu-id="bc7aa-138">Измените или введите коды измерений, которые будут применяться к новым карточкам клиентов, созданным с помощью шаблона.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-138">Edit or enter dimension codes that will apply to new customer cards created by using the template.</span></span>  
5. <span data-ttu-id="bc7aa-139">Заполнив шаблон нового клиента, нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-139">When you have completed the new customer template, choose the **OK** button.</span></span>

<span data-ttu-id="bc7aa-140">Шаблон клиента добавляется в список шаблонов клиентов, чтобы можно было использовать его для создания новых карточек клиентов.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-140">The customer template is added to the list of customer templates, so that you can use it to create new customer cards.</span></span>

## <a name="deleting-customer-cards"></a><span data-ttu-id="bc7aa-141">Удаление карточек клиентов</span><span class="sxs-lookup"><span data-stu-id="bc7aa-141">Deleting customer cards</span></span>

<span data-ttu-id="bc7aa-142">Если вы учли транзакцию для клиента, удалить карточку нельзя, потому что операции книги могут быть необходимы для аудита.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-142">If you have posted a transaction for a customer, you cannot delete the card because the ledger entries may be needed for auditing.</span></span> <span data-ttu-id="bc7aa-143">Для удаления карточек клиентов с операциями книги обратитесь к своему партнеру Майкрософт, который может сделать это посредством кода.</span><span class="sxs-lookup"><span data-stu-id="bc7aa-143">To delete customer cards with ledger entries, contact your Microsoft partner to do so through code.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bc7aa-144">См. также</span><span class="sxs-lookup"><span data-stu-id="bc7aa-144">See Also</span></span>

[<span data-ttu-id="bc7aa-145">Определение способов оплаты</span><span class="sxs-lookup"><span data-stu-id="bc7aa-145">Defining Payment Methods</span></span>](finance-payment-methods.md)  
[<span data-ttu-id="bc7aa-146">Объединение повторяющихся записей</span><span class="sxs-lookup"><span data-stu-id="bc7aa-146">Merge Duplicate Records</span></span>](sales-how-merge-duplicate-records.md)  
[<span data-ttu-id="bc7aa-147">Создание серий номеров</span><span class="sxs-lookup"><span data-stu-id="bc7aa-147">Create Number Series</span></span>](ui-create-number-series.md)  
[<span data-ttu-id="bc7aa-148">Продажи</span><span class="sxs-lookup"><span data-stu-id="bc7aa-148">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="bc7aa-149">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="bc7aa-149">Setting Up Sales</span></span>](sales-setup-sales.md)  
<span data-ttu-id="bc7aa-150">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bc7aa-150">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
