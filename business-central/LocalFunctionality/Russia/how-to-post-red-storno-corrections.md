---
title: Учет коррекций "красный сторно" в России
description: Российские улучшения включают учет коррекций "красный сторно".
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 825ea58ceb7bd76c5c26291850111a77f773f994
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3921228"
---
# <a name="post-red-storno-corrections"></a><span data-ttu-id="79a42-103">Учет коррекций "красный сторно"</span><span class="sxs-lookup"><span data-stu-id="79a42-103">Post Red Storno Corrections</span></span>

<span data-ttu-id="79a42-104">Можно настраивать склад на использование одного столбца для первоначального и корректирующего учета.</span><span class="sxs-lookup"><span data-stu-id="79a42-104">You can set up inventory to use the same column for original and corrective postings.</span></span> <span data-ttu-id="79a42-105">Эта функция часто называется *красный сторно*.</span><span class="sxs-lookup"><span data-stu-id="79a42-105">This is often referred to as *red storno*.</span></span> <span data-ttu-id="79a42-106">Учет "красный сторно" можно использовать для учета следующих операций склада:</span><span class="sxs-lookup"><span data-stu-id="79a42-106">You can use red storno posting to post the following inventory entries:</span></span>

- <span data-ttu-id="79a42-107">Корректирующие операции в журнале товаров.</span><span class="sxs-lookup"><span data-stu-id="79a42-107">Corrective entries in the item journal.</span></span>
- <span data-ttu-id="79a42-108">Сторнирование товарных документов, таких как акты оприходования и акты списания товаров.</span><span class="sxs-lookup"><span data-stu-id="79a42-108">Reversal of item documents such as item receipts and item shipments.</span></span>
- <span data-ttu-id="79a42-109">Учет журналов переоценки или реклассификации товаров.</span><span class="sxs-lookup"><span data-stu-id="79a42-109">Posting item revaluation or item reclassification journals.</span></span>
- <span data-ttu-id="79a42-110">Периодические корректировки себестоимости товара.</span><span class="sxs-lookup"><span data-stu-id="79a42-110">Periodic adjustments of item costs.</span></span>

> [!NOTE]
> <span data-ttu-id="79a42-111">Функцию "красный сторно" необходимо включить в окне **Настройка модуля "Запасы"**, прежде чем можно будет учитывать корректирующие операции.</span><span class="sxs-lookup"><span data-stu-id="79a42-111">You must enable red storno in the **Inventory Setup** window before you can post corrective entries.</span></span> <span data-ttu-id="79a42-112">Дополнительные сведения см. в разделе [Настройка модуля "Запасы"](Inventory-Setup.md).</span><span class="sxs-lookup"><span data-stu-id="79a42-112">For more information, see [Inventory Setup](Inventory-Setup.md).</span></span>  

## <a name="to-post-corrective-entries-in-the-item-journal"></a><span data-ttu-id="79a42-113">Учет корректирующих операций в журнале товаров</span><span class="sxs-lookup"><span data-stu-id="79a42-113">To post corrective entries in the item journal</span></span>

1. <span data-ttu-id="79a42-114">Выберите значок ![Поиск страницы или отчета](), введите **Журнал товаров**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="79a42-114">Choose the ![Search for Page or Report]() icon, enter **Item Journal**, and then choose the related link.</span></span>

2. <span data-ttu-id="79a42-115">Введите значения в поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="79a42-115">Fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="79a42-116">Поле</span><span class="sxs-lookup"><span data-stu-id="79a42-116">Field</span></span>          | <span data-ttu-id="79a42-117">Описание</span><span class="sxs-lookup"><span data-stu-id="79a42-117">Description</span></span>                                                  |
   | :------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="79a42-118">**Тип операции**</span><span class="sxs-lookup"><span data-stu-id="79a42-118">**Entry Type**</span></span> | <span data-ttu-id="79a42-119">Выберите тот же тип операции, что и для первоначального учета.</span><span class="sxs-lookup"><span data-stu-id="79a42-119">Select the same entry type as the original posting.</span></span>          |
   | <span data-ttu-id="79a42-120">**количество;**</span><span class="sxs-lookup"><span data-stu-id="79a42-120">**Quantity**</span></span>   | <span data-ttu-id="79a42-121">Введите количество со знаком, противоположным первоначальному учету, например **-4**.</span><span class="sxs-lookup"><span data-stu-id="79a42-121">Enter the quantity with the opposite sign of the original posting, such as **-4**.</span></span> |
   | <span data-ttu-id="79a42-122">**Красное сторно**</span><span class="sxs-lookup"><span data-stu-id="79a42-122">**Red Storno**</span></span> | <span data-ttu-id="79a42-123">Выберите для учета в качестве корректирующего учета.</span><span class="sxs-lookup"><span data-stu-id="79a42-123">Select to post as a corrective posting.</span></span>                      |

   <span data-ttu-id="79a42-124">Также необходимо выбрать соответствующие операции в полях **Примен. к операции** или **Примен. из операции**.</span><span class="sxs-lookup"><span data-stu-id="79a42-124">You must also select the appropriate entries in the **Applies-to Entry** or **Applies-from Entry** fields.</span></span>

3. <span data-ttu-id="79a42-125">Учтите журнал.</span><span class="sxs-lookup"><span data-stu-id="79a42-125">Post the journal.</span></span>

<span data-ttu-id="79a42-126">Коррекция учитывается, и учитывается вся корреспонденция счета главной книги, которая была настроена.</span><span class="sxs-lookup"><span data-stu-id="79a42-126">The correction is posted, and any general ledger account correspondence that you have set up will be considered.</span></span>

## <a name="to-reverse-item-documents"></a><span data-ttu-id="79a42-127">Сторнирование товарных документов</span><span class="sxs-lookup"><span data-stu-id="79a42-127">To reverse item documents</span></span>

1. <span data-ttu-id="79a42-128">Для сторнирования акта оприходования товаров выберите значок ![Поиск страницы или отчета](), введите **Акты оприходования товаров**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="79a42-128">To reverse an item receipt, Choose the ![Search for Page or Report]() icon, enter **Item Receipt**, and then choose the related link.</span></span>

   <span data-ttu-id="79a42-129">Для сторнирования акта списания товаров выберите значок ![Поиск страницы или отчета](), введите **Акты списания товаров**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="79a42-129">To reverse an item shipment, Choose the ![Search for Page or Report]() icon, enter **Item Shipment**, and then choose the related link.</span></span>

2. <span data-ttu-id="79a42-130">На экспресс-вкладке **Общее** установите флажок **Корректировка**.</span><span class="sxs-lookup"><span data-stu-id="79a42-130">On the **General** FastTab, select the **Correction** check box.</span></span>

3. <span data-ttu-id="79a42-131">Выберите действие **Копировать документ**.</span><span class="sxs-lookup"><span data-stu-id="79a42-131">Choose the **Copy Document** action.</span></span>

4. <span data-ttu-id="79a42-132">В окне **Копировать документ** установите соответствующие фильтры, затем выберите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="79a42-132">In the **Copy Document** window, set the appropriate filters, and then choose the **OK** button.</span></span>

5. <span data-ttu-id="79a42-133">Внесите необходимые изменения в количество и суммы.</span><span class="sxs-lookup"><span data-stu-id="79a42-133">Make the needed changes to quantity and amounts.</span></span>

   <span data-ttu-id="79a42-134">Также необходимо выбрать соответствующие операции в полях **Примен. к операции** или **Примен. из операции**.</span><span class="sxs-lookup"><span data-stu-id="79a42-134">You must also select the appropriate entries in the **Applies-to Entry** or **Applies-from Entry** fields.</span></span> <span data-ttu-id="79a42-135">Эти поля определяют неправильно учтенный документ.</span><span class="sxs-lookup"><span data-stu-id="79a42-135">These fields identify the incorrectly posted document.</span></span>

6. <span data-ttu-id="79a42-136">Выполните учет журнала.</span><span class="sxs-lookup"><span data-stu-id="79a42-136">Post the document.</span></span>

## <a name="to-post-item-revaluation-or-item-reclassification-journals"></a><span data-ttu-id="79a42-137">Учет журналов переоценки или реклассификации товаров</span><span class="sxs-lookup"><span data-stu-id="79a42-137">To post item revaluation or item reclassification journals</span></span> 

1. <span data-ttu-id="79a42-138">Для учета переоценки товаров выберите значок ![Поиск страницы или отчета](), введите **Журнал переоценки**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="79a42-138">To post an item revaluation, Choose the ![Search for Page or Report]() icon, enter **Revaluation Journal**, and then choose the related link.</span></span>

   <span data-ttu-id="79a42-139">Для учета реклассификации товаров выберите значок ![Поиск страницы или отчета](), введите **Журнал реклассификации товаров**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="79a42-139">To post an item reclassification, Choose the ![Search for Page or Report]() icon, enter **Item Reclass Journal**, and then choose the related link.</span></span>

2. <span data-ttu-id="79a42-140">Введите значения в поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="79a42-140">Fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="79a42-141">Поле</span><span class="sxs-lookup"><span data-stu-id="79a42-141">Field</span></span>                  | <span data-ttu-id="79a42-142">Описание</span><span class="sxs-lookup"><span data-stu-id="79a42-142">Description</span></span>                                                  |
   | :--------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="79a42-143">**Применяемая операция**</span><span class="sxs-lookup"><span data-stu-id="79a42-143">**Applies-to Entry**</span></span>   | <span data-ttu-id="79a42-144">Указывает товарную операцию, для которой требуется выполнить переоценку или реклассификацию.</span><span class="sxs-lookup"><span data-stu-id="79a42-144">Specifies the item entry that you want to revalue or reclassify.</span></span> |
   | <span data-ttu-id="79a42-145">**Примен. из операции**</span><span class="sxs-lookup"><span data-stu-id="79a42-145">**Applies-from Entry**</span></span> | <span data-ttu-id="79a42-146">Указывает товарную операцию, для которой требуется выполнить переоценку или реклассификацию.</span><span class="sxs-lookup"><span data-stu-id="79a42-146">Specifies the item entry that you want to revalue or reclassify.</span></span> |
   | <span data-ttu-id="79a42-147">**Красное сторно**</span><span class="sxs-lookup"><span data-stu-id="79a42-147">**Red Storno**</span></span>         | <span data-ttu-id="79a42-148">Выберите для учета в качестве корректирующего учета.</span><span class="sxs-lookup"><span data-stu-id="79a42-148">Select to post as a corrective posting.</span></span>                      |

3. <span data-ttu-id="79a42-149">Выполните учет журнала.</span><span class="sxs-lookup"><span data-stu-id="79a42-149">Post the document.</span></span>

## <a name="see-also"></a><span data-ttu-id="79a42-150">См. также</span><span class="sxs-lookup"><span data-stu-id="79a42-150">See Also</span></span>

[<span data-ttu-id="79a42-151">Настройка запасов</span><span class="sxs-lookup"><span data-stu-id="79a42-151">Setting Up Inventory</span></span>](Inventory-Setup.md)  
