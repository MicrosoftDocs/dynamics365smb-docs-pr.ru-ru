---
title: Документы запасов в России
description: Российские улучшения для документов запасов.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: dba547c2d5dbfacb1a795f1e6a654c766c673be2
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5781419"
---
# <a name="inventory-documents"></a><span data-ttu-id="b1782-103">Инвентарные документы</span><span class="sxs-lookup"><span data-stu-id="b1782-103">Inventory Documents</span></span>

[!INCLUDE[prod_short](../../includes/prod_short.md)] <span data-ttu-id="b1782-104">также включает отчеты, который необходимо предоставлять официальным органам, такие как акт списания ТОРГ-16, акт приемки товаров ТОРГ-1 и расхождение при приемке ТОРГ-2.</span><span class="sxs-lookup"><span data-stu-id="b1782-104">includes reports that you must submit for official reporting, such as the Write-off act TORG-16, Items Receipt Act TORG-1, and Receipt Deviations TORG-2 reports.</span></span>

## <a name="report-act-items-receipt-m-7-items-receipt-act-torg-1-and-receipt-deviations-torg-2-based-on-an-unposted-inventory-receipt"></a><span data-ttu-id="b1782-105">Отчет акта о приемке материалов M-7, акт о приемке товаров ТОРГ-1 и акт о расхождении по количеству и качеству при приемке товарно-материальных ценностей ТОРГ-2 на основе неучтенной приходной накладной</span><span class="sxs-lookup"><span data-stu-id="b1782-105">Report Act Items Receipt M-7, Items Receipt Act TORG-1, and Receipt Deviations TORG-2 Based on an Unposted Inventory Receipt</span></span>

<span data-ttu-id="b1782-106">В следующей процедуре описывается порядок создания следующих отчетов на основании документов приходной накладной, которые не были учтены.</span><span class="sxs-lookup"><span data-stu-id="b1782-106">The following procedure shows how to create a following reports based on inventory receipt documents that are not posted.</span></span>
- <span data-ttu-id="b1782-107">Акт о приемке материалов М-7</span><span class="sxs-lookup"><span data-stu-id="b1782-107">Act Items Receipt M-7</span></span>
- <span data-ttu-id="b1782-108">Акт о приемке товаров ТОРГ-1</span><span class="sxs-lookup"><span data-stu-id="b1782-108">Items Receipt Act TORG-1</span></span>
- <span data-ttu-id="b1782-109">Расхождение при приемке ТОРГ-2</span><span class="sxs-lookup"><span data-stu-id="b1782-109">Receipt Deviations TORG-2</span></span>

1. <span data-ttu-id="b1782-110">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Приходная накладная**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b1782-110">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Receipt**, and then choose the related link.</span></span>
2. <span data-ttu-id="b1782-111">Заполните поля.</span><span class="sxs-lookup"><span data-stu-id="b1782-111">Fill in the fields.</span></span> <span data-ttu-id="b1782-112">Дополнительные сведения см. в разделе [Подсчет и корректировка запасов с использованием документов](../../inventory-how-count-inventory-with-documents.md).</span><span class="sxs-lookup"><span data-stu-id="b1782-112">For more information, see [Count and Adjust Inventory Using Documents](../../inventory-how-count-inventory-with-documents.md).</span></span>
3. <span data-ttu-id="b1782-113">Выберите действие **Подписи сотрудников**, чтобы указать подпись ответственного лица.</span><span class="sxs-lookup"><span data-stu-id="b1782-113">Choose the **Employee Signatures** action to specify the signature of the person in charge.</span></span>
4. <span data-ttu-id="b1782-114">Введите значения в поля, описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b1782-114">Enter the fields described in the following table.</span></span>

    | <span data-ttu-id="b1782-115">Поле</span><span class="sxs-lookup"><span data-stu-id="b1782-115">Field</span></span>             | <span data-ttu-id="b1782-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b1782-116">Description</span></span>                                                  |
    | ----------------- | ------------------------------------------------------------ |
    | <span data-ttu-id="b1782-117">**Тип сотрудника**</span><span class="sxs-lookup"><span data-stu-id="b1782-117">**Employee Type**</span></span> | <span data-ttu-id="b1782-118">Определяет тип сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b1782-118">Specifies the type of the employee.</span></span>                          |
    | <span data-ttu-id="b1782-119">**Код сотрудника**</span><span class="sxs-lookup"><span data-stu-id="b1782-119">**Employee No.**</span></span>  | <span data-ttu-id="b1782-120">Задает номер сотрудника, который должен поставить свою подпись.</span><span class="sxs-lookup"><span data-stu-id="b1782-120">Specifies the employee number of the employee who must sign.</span></span> |
    | <span data-ttu-id="b1782-121">**Имя сотрудника**</span><span class="sxs-lookup"><span data-stu-id="b1782-121">**Employee Name**</span></span> | <span data-ttu-id="b1782-122">Задает значения, которые извлекаются из стандартных полей выбранной карточки **Карточка сотрудника**.</span><span class="sxs-lookup"><span data-stu-id="b1782-122">Specifies the values that are retrieved from the standard fields of the selected **Employee Card**.</span></span> |

5. <span data-ttu-id="b1782-123">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="b1782-123">Choose the **Print** action.</span></span>

## <a name="report-act-items-receipt-m-7-items-receipt-act-torg-1-and-receipt-deviations-torg-2-based-on-an-posted-inventory-receipt"></a><span data-ttu-id="b1782-124">Отчет акта о приемке материалов M-7, акт о приемке товаров ТОРГ-1 и акт о расхождении по количеству и качеству при приемке товарно-материальных ценностей ТОРГ-2 на основе учтенной приходной накладной</span><span class="sxs-lookup"><span data-stu-id="b1782-124">Report Act Items Receipt M-7, Items Receipt Act TORG-1, and Receipt Deviations TORG-2 Based on an Posted Inventory Receipt</span></span>

<span data-ttu-id="b1782-125">В следующей процедуре описывается порядок создания следующих отчетов на основании документов приходной накладной, которые не были учтены.</span><span class="sxs-lookup"><span data-stu-id="b1782-125">The following procedure shows how to create a following reports based on posted inventory receipt.</span></span>
- <span data-ttu-id="b1782-126">Акт о приемке материалов М-7</span><span class="sxs-lookup"><span data-stu-id="b1782-126">Act Items Receipt M-7</span></span>
- <span data-ttu-id="b1782-127">Акт о приемке товаров ТОРГ-1</span><span class="sxs-lookup"><span data-stu-id="b1782-127">Items Receipt Act TORG-1</span></span>
- <span data-ttu-id="b1782-128">Расхождение при приемке ТОРГ-2</span><span class="sxs-lookup"><span data-stu-id="b1782-128">Receipt Deviations TORG-2</span></span>

1. <span data-ttu-id="b1782-129">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенные приходные накладные**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b1782-129">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Inventory Receipts**, and then choose the related link.</span></span>
2. <span data-ttu-id="b1782-130">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="b1782-130">Choose the **Print** action.</span></span>

## <a name="report-item-write-off-act-torg-16-based-on-an-unposted-inventory-shipment"></a><span data-ttu-id="b1782-131">Отчет об акте списания товаров ТОРГ-16 на основании неучтенной расходной накладной</span><span class="sxs-lookup"><span data-stu-id="b1782-131">Report Item Write-off act TORG-16 Based on an Unposted Inventory Shipment</span></span>

<span data-ttu-id="b1782-132">В следующей процедуре описывается порядок создания отчета акта списания товаров ТОРГ-16 на основании документов расходной накладной, которые не были учтены.</span><span class="sxs-lookup"><span data-stu-id="b1782-132">The following procedure shows how to create a Item Write-off act TORG-16 report based on inventory shipment documents that are not posted.</span></span>

1. <span data-ttu-id="b1782-133">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Отгрузочная накладная**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b1782-133">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Shipment**, and then choose the related link.</span></span>
2. <span data-ttu-id="b1782-134">Заполните поля.</span><span class="sxs-lookup"><span data-stu-id="b1782-134">Fill in the fields.</span></span> <span data-ttu-id="b1782-135">Дополнительные сведения см. в разделе [Подсчет и корректировка запасов с использованием документов](../../inventory-how-count-inventory-with-documents.md).</span><span class="sxs-lookup"><span data-stu-id="b1782-135">For more information, see [Count and Adjust Inventory Using Documents](../../inventory-how-count-inventory-with-documents.md).</span></span>
3. <span data-ttu-id="b1782-136">Выберите действие **Подписи сотрудников**, чтобы указать подпись ответственного лица.</span><span class="sxs-lookup"><span data-stu-id="b1782-136">Choose the **Employee Signatures** action to specify the signature of the person in charge.</span></span>
4. <span data-ttu-id="b1782-137">Введите значения в поля, описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b1782-137">Enter the fields described in the following table.</span></span>

    | <span data-ttu-id="b1782-138">Поле</span><span class="sxs-lookup"><span data-stu-id="b1782-138">Field</span></span>             | <span data-ttu-id="b1782-139">Описание</span><span class="sxs-lookup"><span data-stu-id="b1782-139">Description</span></span>                                                  |
    | ----------------- | ------------------------------------------------------------ |
    | <span data-ttu-id="b1782-140">**Тип сотрудника**</span><span class="sxs-lookup"><span data-stu-id="b1782-140">**Employee Type**</span></span> | <span data-ttu-id="b1782-141">Определяет тип сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b1782-141">Specifies the type of the employee.</span></span>                          |
    | <span data-ttu-id="b1782-142">**Код сотрудника**</span><span class="sxs-lookup"><span data-stu-id="b1782-142">**Employee No.**</span></span>  | <span data-ttu-id="b1782-143">Задает номер сотрудника, который должен поставить свою подпись.</span><span class="sxs-lookup"><span data-stu-id="b1782-143">Specifies the employee number of the employee who must sign.</span></span> |
    | <span data-ttu-id="b1782-144">**Имя сотрудника**</span><span class="sxs-lookup"><span data-stu-id="b1782-144">**Employee Name**</span></span> | <span data-ttu-id="b1782-145">Задает значения, которые извлекаются из стандартных полей выбранной карточки **Карточка сотрудника**.</span><span class="sxs-lookup"><span data-stu-id="b1782-145">Specifies the values that are retrieved from the standard fields of the selected **Employee Card**.</span></span> |

5. <span data-ttu-id="b1782-146">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="b1782-146">Choose the **Print** action.</span></span>

## <a name="report-item-write-off-act-torg-16-based-on-an-posted-inventory-shipment"></a><span data-ttu-id="b1782-147">Отчет об акте списания товаров ТОРГ-16 на основании учтенной расходной накладной</span><span class="sxs-lookup"><span data-stu-id="b1782-147">Report Item Write-off act TORG-16 Based on an posted Inventory Shipment</span></span>

<span data-ttu-id="b1782-148">В следующей процедуре описывается порядок создания отчета акта списания товаров ТОРГ-16 на основании учтенной расходной накладной.</span><span class="sxs-lookup"><span data-stu-id="b1782-148">The following procedure shows how to create a Item Write-off act TORG-16 report based on a posted inventory shipments.</span></span>

1. <span data-ttu-id="b1782-149">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Акты списания товаров**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b1782-149">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Shipments**, and then choose the related link.</span></span>
2. <span data-ttu-id="b1782-150">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="b1782-150">Choose the **Print** action.</span></span>

<span data-ttu-id="b1782-151">Функции, доступные в окне **Акт списания товаров**, совпадают с функциями, доступными в окне **Акт оприходования товаров**.</span><span class="sxs-lookup"><span data-stu-id="b1782-151">The functions available in the **Item Shipment** window are same as those in the **Item Receipt** window.</span></span>

## <a name="report-transfer-order-torg-13-based-on-an-unposted-transfer-document"></a><span data-ttu-id="b1782-152">Накладная на перемещение ТОРГ-13 на основании неучтенного документа перемещения</span><span class="sxs-lookup"><span data-stu-id="b1782-152">Report Transfer Order TORG-13 Based on an Unposted Transfer Document</span></span>

<span data-ttu-id="b1782-153">В следующей процедуре описывается порядок создания отчета по заказу на перемещение ТОРГ-13 на основании документов на перемещение, которые не были учтены.</span><span class="sxs-lookup"><span data-stu-id="b1782-153">The following procedure shows how to create a Transfer Order TORG-13 report based on transfer documents that are not posted.</span></span>

1. <span data-ttu-id="b1782-154">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на перемещение**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b1782-154">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="b1782-155">Заполните поля.</span><span class="sxs-lookup"><span data-stu-id="b1782-155">Fill in the fields.</span></span> <span data-ttu-id="b1782-156">Дополнительные сведения см. в разделе [Перемещение запасов между складами](../../inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="b1782-156">For more information, see [Transfer Inventory Between Locations](../../inventory-how-transfer-between-locations.md).</span></span>
3. <span data-ttu-id="b1782-157">Выберите действие **Подписи сотрудников**, чтобы указать подпись ответственного лица.</span><span class="sxs-lookup"><span data-stu-id="b1782-157">Choose the **Employee Signatures** action to specify the signature of the person in charge.</span></span>
4. <span data-ttu-id="b1782-158">Введите значения в поля, описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b1782-158">Enter the fields described in the following table.</span></span>

    | <span data-ttu-id="b1782-159">Поле</span><span class="sxs-lookup"><span data-stu-id="b1782-159">Field</span></span>             | <span data-ttu-id="b1782-160">Описание</span><span class="sxs-lookup"><span data-stu-id="b1782-160">Description</span></span>                                                  |
    | ----------------- | ------------------------------------------------------------ |
    | <span data-ttu-id="b1782-161">**Тип сотрудника**</span><span class="sxs-lookup"><span data-stu-id="b1782-161">**Employee Type**</span></span> | <span data-ttu-id="b1782-162">Определяет тип сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b1782-162">Specifies the type of the employee.</span></span>                          |
    | <span data-ttu-id="b1782-163">**Код сотрудника**</span><span class="sxs-lookup"><span data-stu-id="b1782-163">**Employee No.**</span></span>  | <span data-ttu-id="b1782-164">Задает номер сотрудника, который должен поставить свою подпись.</span><span class="sxs-lookup"><span data-stu-id="b1782-164">Specifies the employee number of the employee who must sign.</span></span> |
    | <span data-ttu-id="b1782-165">**Имя сотрудника**</span><span class="sxs-lookup"><span data-stu-id="b1782-165">**Employee Name**</span></span> | <span data-ttu-id="b1782-166">Задает значения, которые извлекаются из стандартных полей выбранной карточки **Карточка сотрудника**.</span><span class="sxs-lookup"><span data-stu-id="b1782-166">Specifies the values that are retrieved from the standard fields of the selected **Employee Card**.</span></span> |

5. <span data-ttu-id="b1782-167">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="b1782-167">Choose the **Print** action.</span></span>

## <a name="report-transfer-order-torg-13-based-on-a-posted-transfer-document---transfer-receipt"></a><span data-ttu-id="b1782-168">Накладная на перемещение ТОРГ-13 на основании учтенного документа перемещения - "Приходная накладная на перемещение"</span><span class="sxs-lookup"><span data-stu-id="b1782-168">Report Transfer Order TORG-13 Based on a Posted Transfer Document - Transfer Receipt</span></span>

<span data-ttu-id="b1782-169">В следующей процедуре описан порядок создания отчета на основе учтенного документа перемещения, называемого приходной накладной на перемещение.</span><span class="sxs-lookup"><span data-stu-id="b1782-169">The following procedure shows how to create a report based on a posted transfer document called a transfer receipt.</span></span>

1. <span data-ttu-id="b1782-170">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенная прих. накладная на перемещение**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b1782-170">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Transfer Receipt**, and then choose the related link.</span></span>
2. <span data-ttu-id="b1782-171">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="b1782-171">Choose the **Print** action.</span></span>

## <a name="report-transfer-order-torg-13-based-on-a-posted-transfer-document---transfer-shipment"></a><span data-ttu-id="b1782-172">Накладная на перемещение ТОРГ-13 на основании учтенного документа перемещения - "Расходная накладная на перемещение"</span><span class="sxs-lookup"><span data-stu-id="b1782-172">Report Transfer Order TORG-13 Based on a Posted Transfer Document - Transfer Shipment</span></span>

<span data-ttu-id="b1782-173">В следующей процедуре описан порядок создания отчета на основе учтенного документа перемещения, называемого расходной накладной на перемещение.</span><span class="sxs-lookup"><span data-stu-id="b1782-173">The following procedure shows how to create a report based on a posted transfer document called a transfer shipment.</span></span>

1. <span data-ttu-id="b1782-174">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенные расх. накладные на перемещение**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b1782-174">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Transfer Shipments**, and then choose the related link.</span></span>
2. <span data-ttu-id="b1782-175">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="b1782-175">Choose the **Print** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="b1782-176">См. также</span><span class="sxs-lookup"><span data-stu-id="b1782-176">See Also</span></span>

[<span data-ttu-id="b1782-177">Товары Настройка</span><span class="sxs-lookup"><span data-stu-id="b1782-177">Inventory Setup</span></span>](Inventory-Setup.md)  
[<span data-ttu-id="b1782-178">Акты обязательств по товару</span><span class="sxs-lookup"><span data-stu-id="b1782-178">Item Obligatory Acts</span></span>](Item-Obligatory-Acts.md)  
[<span data-ttu-id="b1782-179">Оборотная ведомость для товаров по ГК</span><span class="sxs-lookup"><span data-stu-id="b1782-179">Item General Ledger Turnover</span></span>](Item-General-Ledger-Turnover.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]