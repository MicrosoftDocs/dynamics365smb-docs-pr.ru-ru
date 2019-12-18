---
title: Создание карточки поставщика для регистрации нового поставщика | Документация Майкрософт
description: Узнайте. как создать карточку поставщика для регистрации нового поставщика.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 7ab77dd3c154c81172037e07fb6decf4ad907f5b
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2883098"
---
# <a name="register-new-vendors"></a><span data-ttu-id="b2887-103">Регистрация новых поставщиков</span><span class="sxs-lookup"><span data-stu-id="b2887-103">Register New Vendors</span></span>
<span data-ttu-id="b2887-104">Поставщики предоставляют продукцию, которую вы продаете.</span><span class="sxs-lookup"><span data-stu-id="b2887-104">Vendors provide the products that you sell.</span></span> <span data-ttu-id="b2887-105">Каждый поставщик, у которого производится покупка, должен быть зарегистрирован в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="b2887-105">Each vendor that you purchase from must be registered as a vendor card.</span></span>

<span data-ttu-id="b2887-106">Перед регистрацией новых поставщиков необходимо настроить различные коды покупки, которые можно будет выбирать при заполнении карточек поставщиков.</span><span class="sxs-lookup"><span data-stu-id="b2887-106">Before you can register new vendors, you must set up various purchase codes that you can select from when you fill vendor cards.</span></span> <span data-ttu-id="b2887-107">После создания всех необходимых основных данных можно выполнить дополнительную настройку поставщика, например определить приоритетность поставщика при осуществлении оплаты и указать товары, которые может поставлять этот или другие поставщики.</span><span class="sxs-lookup"><span data-stu-id="b2887-107">When all of the required master data is created, you can perform additional configuration of the vendor, such as prioritize the vendor for payment purposes and list items that the vendor and other vendors can supply.</span></span> <span data-ttu-id="b2887-108">Еще одна группа задач настройки поставщиков предназначена для записи соглашений по скидкам, ценам и способам оплаты.</span><span class="sxs-lookup"><span data-stu-id="b2887-108">Another group of setup tasks for vendors is to record your agreements concerning discounts, prices, and payment methods.</span></span> <span data-ttu-id="b2887-109">Дополнительные сведения см. в разделе [Настройка покупки](purchasing-setup-purchasing.md).</span><span class="sxs-lookup"><span data-stu-id="b2887-109">For more information, see [Setting Up Purchasing](purchasing-setup-purchasing.md).</span></span>

<span data-ttu-id="b2887-110">Карточки поставщиков содержат информацию, необходимую для приобретения продукции у поставщика.</span><span class="sxs-lookup"><span data-stu-id="b2887-110">Vendor cards hold the information that is required to buy products from the vendor.</span></span> <span data-ttu-id="b2887-111">Дополнительные сведения см. в разделах [Регистрация покупок](purchasing-how-record-purchases.md) и [Регистрация новых товаров](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="b2887-111">For more information, see [Record Purchases](purchasing-how-record-purchases.md) and [Register New Items](inventory-how-register-new-items.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="b2887-112">Если существуют шаблоны поставщиков для различных типов поставщиков, при создании новой карточки поставщика отобразится страница, с которой можно выбрать подходящий шаблон.</span><span class="sxs-lookup"><span data-stu-id="b2887-112">If vendor templates exist for different vendor types, then a page appears when you create a new vendor card from where you can select an appropriate template.</span></span> <span data-ttu-id="b2887-113">Если существует только один шаблон поставщика, для создания новых карточек поставщиков всегда используется этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="b2887-113">If only one vendor template exists, then new vendor cards always use that template.</span></span>
<br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE3PZtd]

## <a name="to-create-a-new-vendor-card"></a><span data-ttu-id="b2887-114">Создание новой карточки поставщика</span><span class="sxs-lookup"><span data-stu-id="b2887-114">To create a new vendor card</span></span>
1. <span data-ttu-id="b2887-115">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Поставщики**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b2887-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b2887-116">На странице **Поставщики** выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="b2887-116">On the **Vendors** page, Choose **New**.</span></span>

    <span data-ttu-id="b2887-117">Если существует несколько шаблонов поставщиков, будет открыта страница, на которой можно будет выбрать шаблон поставщика.</span><span class="sxs-lookup"><span data-stu-id="b2887-117">If more than one vendor template exists, then a page opens from which you can select a vendor template.</span></span> <span data-ttu-id="b2887-118">В этом случае выполните следующие два действия.</span><span class="sxs-lookup"><span data-stu-id="b2887-118">In that case, follow the next two steps.</span></span>
3. <span data-ttu-id="b2887-119">На странице **Выбор шаблона для нового поставщика** выберите шаблон, который требуется использовать для новой карточки поставщика.</span><span class="sxs-lookup"><span data-stu-id="b2887-119">On the **Select a template for a new vendor** page, choose the template that you want to use for the new vendor card.</span></span>
4. <span data-ttu-id="b2887-120">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="b2887-120">Choose the **OK** button.</span></span> <span data-ttu-id="b2887-121">Откроется новая карточка поставщика, некоторые поля которой будут заполнены сведениями из шаблона.</span><span class="sxs-lookup"><span data-stu-id="b2887-121">A new vendor card opens with some fields filled with information from the template.</span></span>
5. <span data-ttu-id="b2887-122">Заполните или измените поля в карточке поставщика по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="b2887-122">Proceed to fill or change fields on the vendor card as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   <span data-ttu-id="b2887-123">Если неизвестен адрес выставления счета, который будет использоваться для каждого счета от поставщика, не следует заполнять поле **Получатель оплаты**.</span><span class="sxs-lookup"><span data-stu-id="b2887-123">If you do not know the invoicing address that will be used for every invoice from a vendor, do not fill in the **Pay-to** field.</span></span> <span data-ttu-id="b2887-124">Вместо этого выберите код поставщика после того, как сформированы предложение по покупке, заказ или заголовок счета.</span><span class="sxs-lookup"><span data-stu-id="b2887-124">Instead, choose the pay-to vendor number after you have set up a purchase quote, order, or invoice header.</span></span>

<span data-ttu-id="b2887-125">Теперь поставщик зарегистрирован, и карточка поставщика готова к использованию в документах покупки.</span><span class="sxs-lookup"><span data-stu-id="b2887-125">The vendor is now registered, and the vendor card is ready to be used on purchase documents.</span></span>

<span data-ttu-id="b2887-126">Если эту карточку поставщика требуется использовать в качестве шаблона при создании новых карточек поставщиков, ее можно сохранить в качестве шаблона поставщика.</span><span class="sxs-lookup"><span data-stu-id="b2887-126">If you want to use this vendor card as a template when you create new vendor cards, you can save it as a vendor template.</span></span> <span data-ttu-id="b2887-127">Дополнительные сведения см. в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="b2887-127">For more information, see the following section.</span></span>

## <a name="to-save-the-vendor-card-as-a-template"></a><span data-ttu-id="b2887-128">Сохранение карточки поставщика в качестве шаблона</span><span class="sxs-lookup"><span data-stu-id="b2887-128">To save the vendor card as a template</span></span>
1. <span data-ttu-id="b2887-129">На странице **Карточка поставщика** выберите действие **Сохранить как шаблон**.</span><span class="sxs-lookup"><span data-stu-id="b2887-129">On the **Vendor Card** page, choose the **Save as Template** action.</span></span> <span data-ttu-id="b2887-130">Откроется страница **Шаблон поставщика**, на которой карточка поставщика будет показана в качестве шаблона.</span><span class="sxs-lookup"><span data-stu-id="b2887-130">The **Vendor Template** page opens showing the vendor card as a template.</span></span>
2. <span data-ttu-id="b2887-131">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="b2887-131">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="b2887-132">Для повторного использования измерений в шаблонах, выберите действие **Измерения**.</span><span class="sxs-lookup"><span data-stu-id="b2887-132">To reuse dimensions in templates, choose the **Dimensions** action.</span></span> <span data-ttu-id="b2887-133">Открывается страница **Шаблоны измерений** с отображением кодов измерений, настроенных для этого поставщика.</span><span class="sxs-lookup"><span data-stu-id="b2887-133">The **Dimension Templates** page opens showing any dimension codes that are set up for the vendor.</span></span>
4. <span data-ttu-id="b2887-134">Измените или введите коды измерений, которые будут применяться к новым карточкам поставщиков, созданным с помощью шаблона.</span><span class="sxs-lookup"><span data-stu-id="b2887-134">Edit or enter dimension codes that will apply to new vendor cards created by using the template.</span></span>
5. <span data-ttu-id="b2887-135">Заполнив шаблон нового поставщика, нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="b2887-135">When you have completed the new vendor template, choose the **OK** button.</span></span>  
   <span data-ttu-id="b2887-136">Шаблон поставщика добавляется в список шаблонов поставщиков, чтобы можно было использовать его для создания новых карточек поставщиков.</span><span class="sxs-lookup"><span data-stu-id="b2887-136">The vendor template is added to the list of vendor templates, so that you can use it to create new vendor cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="b2887-137">См. также</span><span class="sxs-lookup"><span data-stu-id="b2887-137">See Also</span></span>
[<span data-ttu-id="b2887-138">Объединение повторяющихся записей</span><span class="sxs-lookup"><span data-stu-id="b2887-138">Merge Duplicate Records</span></span>](sales-how-merge-duplicate-records.md)  
[<span data-ttu-id="b2887-139">Создание серий номеров</span><span class="sxs-lookup"><span data-stu-id="b2887-139">Create Number Series</span></span>](ui-create-number-series.md)  
[<span data-ttu-id="b2887-140">Покупки</span><span class="sxs-lookup"><span data-stu-id="b2887-140">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="b2887-141">[Регистрация покупок](purchasing-how-record-purchases.md) </span><span class="sxs-lookup"><span data-stu-id="b2887-141">[Record Purchases](purchasing-how-record-purchases.md) </span></span>  
<span data-ttu-id="b2887-142">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b2887-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
