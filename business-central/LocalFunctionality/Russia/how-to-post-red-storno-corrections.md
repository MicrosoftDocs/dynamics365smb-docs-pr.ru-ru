---
title: Учет коррекций "красный сторно" в России
description: Российские улучшения включают учет коррекций "красный сторно".
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 2ccf62bc2f78e717a31585086c822cab81c91bfe
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771280"
---
# <a name="post-red-storno-corrections"></a><span data-ttu-id="54c5f-103">Учет коррекций "красный сторно"</span><span class="sxs-lookup"><span data-stu-id="54c5f-103">Post Red Storno Corrections</span></span>

<span data-ttu-id="54c5f-104">Можно настраивать склад на использование одного столбца для первоначального и корректирующего учета.</span><span class="sxs-lookup"><span data-stu-id="54c5f-104">You can set up inventory to use the same column for original and corrective postings.</span></span> <span data-ttu-id="54c5f-105">Эта функция часто называется *красный сторно*.</span><span class="sxs-lookup"><span data-stu-id="54c5f-105">This is often referred to as *red storno*.</span></span> <span data-ttu-id="54c5f-106">Учет "красный сторно" можно использовать для учета следующих операций склада:</span><span class="sxs-lookup"><span data-stu-id="54c5f-106">You can use red storno posting to post the following inventory entries:</span></span>

- <span data-ttu-id="54c5f-107">Корректирующие операции в журнале товаров.</span><span class="sxs-lookup"><span data-stu-id="54c5f-107">Corrective entries in the item journal.</span></span>
- <span data-ttu-id="54c5f-108">Сторнирование товарных документов, таких как акты оприходования и акты списания товаров.</span><span class="sxs-lookup"><span data-stu-id="54c5f-108">Reversal of item documents such as item receipts and item shipments.</span></span>
- <span data-ttu-id="54c5f-109">Учет журналов переоценки или реклассификации товаров.</span><span class="sxs-lookup"><span data-stu-id="54c5f-109">Posting item revaluation or item reclassification journals.</span></span>
- <span data-ttu-id="54c5f-110">Периодические корректировки себестоимости товара.</span><span class="sxs-lookup"><span data-stu-id="54c5f-110">Periodic adjustments of item costs.</span></span>

> [!NOTE]
> <span data-ttu-id="54c5f-111">Функцию "красный сторно" необходимо включить в окне **Настройка модуля "Запасы"**, прежде чем можно будет учитывать корректирующие операции.</span><span class="sxs-lookup"><span data-stu-id="54c5f-111">You must enable red storno in the **Inventory Setup** window before you can post corrective entries.</span></span> <span data-ttu-id="54c5f-112">Дополнительные сведения см. в разделе [Настройка модуля "Запасы"](Inventory-Setup.md).</span><span class="sxs-lookup"><span data-stu-id="54c5f-112">For more information, see [Inventory Setup](Inventory-Setup.md).</span></span>  

## <a name="to-post-corrective-entries-in-the-item-journal"></a><span data-ttu-id="54c5f-113">Учет корректирующих операций в журнале товаров</span><span class="sxs-lookup"><span data-stu-id="54c5f-113">To post corrective entries in the item journal</span></span>

1. <span data-ttu-id="54c5f-114">Выберите значок ![Поиск страницы или отчета](), введите **Журнал товаров**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="54c5f-114">Choose the ![Search for Page or Report]() icon, enter **Item Journal**, and then choose the related link.</span></span>

2. <span data-ttu-id="54c5f-115">Введите значения в поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="54c5f-115">Fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="54c5f-116">Поле</span><span class="sxs-lookup"><span data-stu-id="54c5f-116">Field</span></span>          | <span data-ttu-id="54c5f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="54c5f-117">Description</span></span>                                                  |
   | :------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="54c5f-118">**Тип операции**</span><span class="sxs-lookup"><span data-stu-id="54c5f-118">**Entry Type**</span></span> | <span data-ttu-id="54c5f-119">Выберите тот же тип операции, что и для первоначального учета.</span><span class="sxs-lookup"><span data-stu-id="54c5f-119">Select the same entry type as the original posting.</span></span>          |
   | <span data-ttu-id="54c5f-120">**количество;**</span><span class="sxs-lookup"><span data-stu-id="54c5f-120">**Quantity**</span></span>   | <span data-ttu-id="54c5f-121">Введите количество со знаком, противоположным первоначальному учету, например **-4**.</span><span class="sxs-lookup"><span data-stu-id="54c5f-121">Enter the quantity with the opposite sign of the original posting, such as **-4**.</span></span> |
   | <span data-ttu-id="54c5f-122">**Красное сторно**</span><span class="sxs-lookup"><span data-stu-id="54c5f-122">**Red Storno**</span></span> | <span data-ttu-id="54c5f-123">Выберите для учета в качестве корректирующего учета.</span><span class="sxs-lookup"><span data-stu-id="54c5f-123">Select to post as a corrective posting.</span></span>                      |

   <span data-ttu-id="54c5f-124">Также необходимо выбрать соответствующие операции в полях **Примен. к операции** или **Примен. из операции**.</span><span class="sxs-lookup"><span data-stu-id="54c5f-124">You must also select the appropriate entries in the **Applies-to Entry** or **Applies-from Entry** fields.</span></span>

3. <span data-ttu-id="54c5f-125">Учтите журнал.</span><span class="sxs-lookup"><span data-stu-id="54c5f-125">Post the journal.</span></span>

<span data-ttu-id="54c5f-126">Коррекция учитывается, и учитывается вся корреспонденция счета главной книги, которая была настроена.</span><span class="sxs-lookup"><span data-stu-id="54c5f-126">The correction is posted, and any general ledger account correspondence that you have set up will be considered.</span></span>

## <a name="to-reverse-item-documents"></a><span data-ttu-id="54c5f-127">Сторнирование товарных документов</span><span class="sxs-lookup"><span data-stu-id="54c5f-127">To reverse item documents</span></span>

1. <span data-ttu-id="54c5f-128">Для сторнирования акта оприходования товаров выберите значок ![Поиск страницы или отчета](), введите **Акты оприходования товаров**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="54c5f-128">To reverse an item receipt, Choose the ![Search for Page or Report]() icon, enter **Item Receipt**, and then choose the related link.</span></span>

   <span data-ttu-id="54c5f-129">Для сторнирования акта списания товаров выберите значок ![Поиск страницы или отчета](), введите **Акты списания товаров**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="54c5f-129">To reverse an item shipment, Choose the ![Search for Page or Report]() icon, enter **Item Shipment**, and then choose the related link.</span></span>

2. <span data-ttu-id="54c5f-130">На экспресс-вкладке **Общее** установите флажок **Корректировка**.</span><span class="sxs-lookup"><span data-stu-id="54c5f-130">On the **General** FastTab, select the **Correction** check box.</span></span>

3. <span data-ttu-id="54c5f-131">Выберите действие **Копировать документ**.</span><span class="sxs-lookup"><span data-stu-id="54c5f-131">Choose the **Copy Document** action.</span></span>

4. <span data-ttu-id="54c5f-132">В окне **Копировать документ** установите соответствующие фильтры, затем выберите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="54c5f-132">In the **Copy Document** window, set the appropriate filters, and then choose the **OK** button.</span></span>

5. <span data-ttu-id="54c5f-133">Внесите необходимые изменения в количество и суммы.</span><span class="sxs-lookup"><span data-stu-id="54c5f-133">Make the needed changes to quantity and amounts.</span></span>

   <span data-ttu-id="54c5f-134">Также необходимо выбрать соответствующие операции в полях **Примен. к операции** или **Примен. из операции**.</span><span class="sxs-lookup"><span data-stu-id="54c5f-134">You must also select the appropriate entries in the **Applies-to Entry** or **Applies-from Entry** fields.</span></span> <span data-ttu-id="54c5f-135">Эти поля определяют неправильно учтенный документ.</span><span class="sxs-lookup"><span data-stu-id="54c5f-135">These fields identify the incorrectly posted document.</span></span>

6. <span data-ttu-id="54c5f-136">Выполните учет журнала.</span><span class="sxs-lookup"><span data-stu-id="54c5f-136">Post the document.</span></span>

## <a name="to-post-item-revaluation-or-item-reclassification-journals"></a><span data-ttu-id="54c5f-137">Учет журналов переоценки или реклассификации товаров</span><span class="sxs-lookup"><span data-stu-id="54c5f-137">To post item revaluation or item reclassification journals</span></span> 

1. <span data-ttu-id="54c5f-138">Для учета переоценки товаров выберите значок ![Поиск страницы или отчета](), введите **Журнал переоценки**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="54c5f-138">To post an item revaluation, Choose the ![Search for Page or Report]() icon, enter **Revaluation Journal**, and then choose the related link.</span></span>

   <span data-ttu-id="54c5f-139">Для учета реклассификации товаров выберите значок ![Поиск страницы или отчета](), введите **Журнал реклассификации товаров**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="54c5f-139">To post an item reclassification, Choose the ![Search for Page or Report]() icon, enter **Item Reclass Journal**, and then choose the related link.</span></span>

2. <span data-ttu-id="54c5f-140">Введите значения в поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="54c5f-140">Fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="54c5f-141">Поле</span><span class="sxs-lookup"><span data-stu-id="54c5f-141">Field</span></span>                  | <span data-ttu-id="54c5f-142">Описание</span><span class="sxs-lookup"><span data-stu-id="54c5f-142">Description</span></span>                                                  |
   | :--------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="54c5f-143">**Применяемая операция**</span><span class="sxs-lookup"><span data-stu-id="54c5f-143">**Applies-to Entry**</span></span>   | <span data-ttu-id="54c5f-144">Указывает товарную операцию, для которой требуется выполнить переоценку или реклассификацию.</span><span class="sxs-lookup"><span data-stu-id="54c5f-144">Specifies the item entry that you want to revalue or reclassify.</span></span> |
   | <span data-ttu-id="54c5f-145">**Примен. из операции**</span><span class="sxs-lookup"><span data-stu-id="54c5f-145">**Applies-from Entry**</span></span> | <span data-ttu-id="54c5f-146">Указывает товарную операцию, для которой требуется выполнить переоценку или реклассификацию.</span><span class="sxs-lookup"><span data-stu-id="54c5f-146">Specifies the item entry that you want to revalue or reclassify.</span></span> |
   | <span data-ttu-id="54c5f-147">**Красное сторно**</span><span class="sxs-lookup"><span data-stu-id="54c5f-147">**Red Storno**</span></span>         | <span data-ttu-id="54c5f-148">Выберите для учета в качестве корректирующего учета.</span><span class="sxs-lookup"><span data-stu-id="54c5f-148">Select to post as a corrective posting.</span></span>                      |

3. <span data-ttu-id="54c5f-149">Выполните учет журнала.</span><span class="sxs-lookup"><span data-stu-id="54c5f-149">Post the document.</span></span>

## <a name="see-also"></a><span data-ttu-id="54c5f-150">См. также</span><span class="sxs-lookup"><span data-stu-id="54c5f-150">See Also</span></span>

[<span data-ttu-id="54c5f-151">Настройка запасов</span><span class="sxs-lookup"><span data-stu-id="54c5f-151">Setting Up Inventory</span></span>](Inventory-Setup.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]