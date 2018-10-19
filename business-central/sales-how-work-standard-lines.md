---
title: "Настройка стандартных строк для типовых продаж и покупок | Документы Майкрософт"
description: "Вы можете настроить строки покупок и продаж, которые вы регулярно осуществляете, а затем вставлять их в документы продажи и покупки, чтобы быстро заполнять строки стандартной информацией."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell, replenishment
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: df4f093ded0a55d45c40be15c5888035d6e3b2df
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="create-recurring-sales-and-purchase-lines"></a><span data-ttu-id="46649-103">Создание типовых строк продажи и покупки</span><span class="sxs-lookup"><span data-stu-id="46649-103">Create Recurring Sales and Purchase Lines</span></span>
<span data-ttu-id="46649-104">Если вам часто приходится создавать строки покупки и продажи с одинаковыми данными, вы можете настроить стандартные строки, которые затем можно вставлять в документы типовых продаж и покупок, например для типовых заказов на пополнение.</span><span class="sxs-lookup"><span data-stu-id="46649-104">If you often need to create sales and purchase lines with similar information, you can set up standard lines that you can then insert on recurring sales and purchase documents, for example, for recurring replenishment orders.</span></span>  

<span data-ttu-id="46649-105">Ниже приводится процедура работы со стандартными строками продажи.</span><span class="sxs-lookup"><span data-stu-id="46649-105">The following procedure shows how to work with standard sales lines.</span></span> <span data-ttu-id="46649-106">Она аналогична процедуре для стандартных строк покупки.</span><span class="sxs-lookup"><span data-stu-id="46649-106">It works in a similar way for standard purchase lines.</span></span>  

## <a name="to-set-up-standard-sales-lines"></a><span data-ttu-id="46649-107">Настройка стандартных строк продажи</span><span class="sxs-lookup"><span data-stu-id="46649-107">To set up standard sales lines</span></span>  
1. <span data-ttu-id="46649-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Строки стандартных продаж**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="46649-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Standard Sales Lines**, and then choose the related link.</span></span>  
2. <span data-ttu-id="46649-109">В окне **Стандартные коды продажи** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="46649-109">In the **Standard Sales Lines** window, choose the **New** action.</span></span>  
3. <span data-ttu-id="46649-110">На экспресс-вкладке **Общее** заполните необходимые поля.</span><span class="sxs-lookup"><span data-stu-id="46649-110">On the **General** FastTab, fill the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. <span data-ttu-id="46649-111">На экспресс-вкладке **Строки** заполните поля для подготовки строк продажи, которые отражают стандартные строки, которые ожидаются как типовые в документах продажи.</span><span class="sxs-lookup"><span data-stu-id="46649-111">On the **Lines** FastTab, enter information in the fields to prepare sales lines that reflect the standard lines that you expect to use as recurring lines on sales documents.</span></span>  

## <a name="to-insert-standard-sales-lines-on-a-sales-invoice"></a><span data-ttu-id="46649-112">Вставка стандартных строк продажи в счет продажи</span><span class="sxs-lookup"><span data-stu-id="46649-112">To insert standard sales lines on a sales invoice</span></span>
1. <span data-ttu-id="46649-113">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="46649-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="46649-114">Откройте счет продажи, в который требуется вставить одну или несколько стандартных строк.</span><span class="sxs-lookup"><span data-stu-id="46649-114">Open the sales invoice that you want to insert one or more standard sales lines on.</span></span>
3. <span data-ttu-id="46649-115">Выберите значение **Получить строки типовых продаж**.</span><span class="sxs-lookup"><span data-stu-id="46649-115">Choose the **Get Recurring Sales Lines** action.</span></span>
4. <span data-ttu-id="46649-116">В окне **Строки типовых продаж** нажмите кнопку выбора в поле **Код**, а затем выберите набор стандартных строк продажи.</span><span class="sxs-lookup"><span data-stu-id="46649-116">In the **Recurring Sales Lines** window, choose the lookup button in the **Code** field, and then select a set of standard sales lines.</span></span>

    > [!NOTE]
    > <span data-ttu-id="46649-117">Чтобы использовать типовые строки продажи, заданные вместе с пакетным заданием **Создание типовых счетов продажи**, необходимо также заполнить поля **Действует с даты** и **Действует до даты** в окне **Строки типовых продаж**.</span><span class="sxs-lookup"><span data-stu-id="46649-117">To use the recurring sales lines set together with the **Create Recurring Sales Invoices** batch job, you must also fill in the **Valid From Date** and **Valid To Date** fields in the **Recurring Sales Lines** window.</span></span> <span data-ttu-id="46649-118">Дополнительные сведения см. в разделе "Создание нескольких счетов продажи на основе стандартных строк продаж".</span><span class="sxs-lookup"><span data-stu-id="46649-118">For more information, see the "To create multiple sales invoices based on standard sales lines" section.</span></span>

5. <span data-ttu-id="46649-119">Нажмите кнопку **ОК**, чтобы вставить в счет стандартные строки продажи, которые можно потом использовать их повторно или изменить.</span><span class="sxs-lookup"><span data-stu-id="46649-119">Choose the **OK** button to insert the standard sales lines on the invoice where you can reuse them as is or edit the information.</span></span>

## <a name="to-create-multiple-sales-invoices-based-on-standard-sales-lines"></a><span data-ttu-id="46649-120">Создание нескольких счетов продажи на основе стандартных строк продаж</span><span class="sxs-lookup"><span data-stu-id="46649-120">To create multiple sales invoices based on standard sales lines</span></span>
<span data-ttu-id="46649-121">Можно использовать пакетное задание **Создание типовых счетов продажи** для создания счетов продаж в соответствии со стандартными строками продаж, которые назначены клиентам, и с учетными датами в пределах дат "Действительно с" и "Действительно по", указанных в стандартных строках продажи.</span><span class="sxs-lookup"><span data-stu-id="46649-121">You can use the **Create Recurring Sales Invoices** batch job to create sales invoices according to standard sales lines that are assigned to the customers and with posting dates within the valid-from and valid-to dates that you specify on the standard sales lines.</span></span>

> [!NOTE]
> <span data-ttu-id="46649-122">В окне **Строки типовых продаж** также можно также определять метод оплаты прямого дебета и поручение прямого дебетования.</span><span class="sxs-lookup"><span data-stu-id="46649-122">In the **Recurring Sales Lines** window, you can also specify a direct-debit payment method and a direct-debit mandate.</span></span> <span data-ttu-id="46649-123">Счета продажи, созданные с помощью пакетного задания **Создание типовых счетов продажи**, затем будут включать информацию, необходимую для получения платежей по счетам продажи с прямым дебетом SEPA.</span><span class="sxs-lookup"><span data-stu-id="46649-123">The sales invoices that are created with the **Create Recurring Sales Inv.** batch job will then include information required to collect payment for the sales invoices with SEPA direct debit.</span></span> <span data-ttu-id="46649-124">Дополнительные сведения см. в разделе [Сбор платежей с прямым дебетованием SEPA](finance-collect-payments-with-sepa-direct-debit.md).</span><span class="sxs-lookup"><span data-stu-id="46649-124">For more information, see [Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md).</span></span>

1. <span data-ttu-id="46649-125">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Создание типовых счетов продажи**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="46649-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Create Recurring Sales Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="46649-126">В окне **Создание типовых счетов продажи** заполните поля по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="46649-126">In the **Create Recurring Sales Invoices** window, fill in the fields as necessary.</span></span>
3. <span data-ttu-id="46649-127">В поле фильтра **Код** введите код для стандартных строк продажи, назначенных клиенту, для которого требуется создать счета продаж.</span><span class="sxs-lookup"><span data-stu-id="46649-127">In the **Code** filter field, enter the code for standard sales lines that are assigned to a customer that you want to create sales invoices for.</span></span>
4. <span data-ttu-id="46649-128">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="46649-128">Choose the **OK** button.</span></span>

<span data-ttu-id="46649-129">Для клиентов создаются счета продажи с указанным стандартным клиентским кодом продажи, а также всеми заданными сведениями о прямом дебете для учета на определенную дату.</span><span class="sxs-lookup"><span data-stu-id="46649-129">Sales invoices are created for the customers with the specified standard customer sales code, and any specified direct-debit information, for posting on the specified date.</span></span>

## <a name="see-also"></a><span data-ttu-id="46649-130">См. также</span><span class="sxs-lookup"><span data-stu-id="46649-130">See Also</span></span>  
[<span data-ttu-id="46649-131">Продажи</span><span class="sxs-lookup"><span data-stu-id="46649-131">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="46649-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="46649-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

