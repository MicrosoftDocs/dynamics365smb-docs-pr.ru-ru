---
title: Товарные документы в России
description: Российские улучшения включают товарные документы.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 8dde817ce360e193e1aad0167ad8472a343ab3f2
ms.sourcegitcommit: 319023e53627dbe8e68643908aacc6fd594a4957
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/04/2019
ms.locfileid: "2554467"
---
# <a name="item-documents"></a><span data-ttu-id="0d440-103">Товарные документы</span><span class="sxs-lookup"><span data-stu-id="0d440-103">Item Documents</span></span>

[!INCLUDE[prodshort](../../includes/prodshort.md)] <span data-ttu-id="0d440-104">включает несколько документов, которые можно использовать для управления складом.</span><span class="sxs-lookup"><span data-stu-id="0d440-104">includes several documents that you can use to manage your warehouse.</span></span> <span data-ttu-id="0d440-105">К ним относятся отчеты, который необходимо предоставлять официальным органам, такие как ТОРГ-29, акт приемки товаров ТОРГ-1 и расхождение при приемке ТОРГ-2.</span><span class="sxs-lookup"><span data-stu-id="0d440-105">This also includes reports that you must submit for official reporting, such as the Item Report TORG-29, Items Receipt Act TORG-1, and Receipt Deviations TORG-2 reports.</span></span>

<span data-ttu-id="0d440-106">Следующие типы документов полезны при управлении складом:</span><span class="sxs-lookup"><span data-stu-id="0d440-106">The following types of documents are useful for managing your warehouse:</span></span>

- <span data-ttu-id="0d440-107">Акт приемки товаров без счета поставщика — применяется для учета прихода товаров на основе качества, количества и стоимости.</span><span class="sxs-lookup"><span data-stu-id="0d440-107">Item receipt act without the vendor invoice - This is applied to the account receipt of items based on the quality, quantity, and cost.</span></span>
- <span data-ttu-id="0d440-108">Акт списания товаров — применяется для регистрации повреждений по таким причинам, как утрата качества товаров, которые не подлежат дальнейшей продаже.</span><span class="sxs-lookup"><span data-stu-id="0d440-108">Item writing-off act – This is applied to register damage for reasons such as the loss of quality of items that will no longer be sold.</span></span>
- <span data-ttu-id="0d440-109">Перемещение товара — применяется при приеме и поставке отгрузок для перемещения товаров в рамках организации.</span><span class="sxs-lookup"><span data-stu-id="0d440-109">Item transfer – This is applied to receipt and delivery shipments for transfer of items within the organization.</span></span>

## <a name="setting-up-warehouse-document-numbering"></a><span data-ttu-id="0d440-110">Настройка нумерации складских документов</span><span class="sxs-lookup"><span data-stu-id="0d440-110">Setting Up Warehouse Document Numbering</span></span>

<span data-ttu-id="0d440-111">В следующей процедуре показан порядок настройки нумерации складских документов.</span><span class="sxs-lookup"><span data-stu-id="0d440-111">The following procedure shows how to set up warehouse document numbering.</span></span>

1. <span data-ttu-id="0d440-112">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Запасы"**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="0d440-112">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="0d440-113">На экспресс-вкладке **Нумерация** укажите в следующих полях серии номеров документов.</span><span class="sxs-lookup"><span data-stu-id="0d440-113">On the **Numbering** FastTab, specify in the following fields the series of numbers for documents:</span></span>
   - <span data-ttu-id="0d440-114">**Серия номеров актов оприходования товаров**</span><span class="sxs-lookup"><span data-stu-id="0d440-114">**Item Receipt Nos**</span></span>
   - <span data-ttu-id="0d440-115">**Серия номеров учт. актов оприходования товаров**</span><span class="sxs-lookup"><span data-stu-id="0d440-115">**Posted Item receipt Nos**</span></span>
   - <span data-ttu-id="0d440-116">**Серия номеров актов списания товаров**</span><span class="sxs-lookup"><span data-stu-id="0d440-116">**Item Shipment Nos**</span></span>
   - <span data-ttu-id="0d440-117">**Серия номеров учт. актов списания товаров**</span><span class="sxs-lookup"><span data-stu-id="0d440-117">**Posted Item Shipment Nos**</span></span>

## <a name="creating-an-item-receipt-act-without-a-vendor"></a><span data-ttu-id="0d440-118">Создание акта оприходования товаров без поставщика</span><span class="sxs-lookup"><span data-stu-id="0d440-118">Creating an Item Receipt Act Without a Vendor</span></span>

<span data-ttu-id="0d440-119">В следующей процедуре показан порядок создания акта оприходования товаров без поставщика.</span><span class="sxs-lookup"><span data-stu-id="0d440-119">The following procedure shows how to create an item receipt act without a vendor.</span></span>

1. <span data-ttu-id="0d440-120">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Акты оприходования товаров**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="0d440-120">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Receipts**, and then choose the related link.</span></span>

2. <span data-ttu-id="0d440-121">В заголовке окна **Акт оприходования товаров** заполните поля, описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0d440-121">In the header of the **Item Receipt** window, enter the fields described in the following table.</span></span>

   | <span data-ttu-id="0d440-122">Поле</span><span class="sxs-lookup"><span data-stu-id="0d440-122">Field</span></span>                               | <span data-ttu-id="0d440-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0d440-123">Description</span></span>                                                  |
   | ----------------------------------- | ------------------------------------------------------------ |
   | <span data-ttu-id="0d440-124">**Номер**</span><span class="sxs-lookup"><span data-stu-id="0d440-124">**No.**</span></span>                             | <span data-ttu-id="0d440-125">Определяет номер заголовка складского документа.</span><span class="sxs-lookup"><span data-stu-id="0d440-125">Specifies the warehouse document header number.</span></span>              |
   | <span data-ttu-id="0d440-126">**Описание учета**</span><span class="sxs-lookup"><span data-stu-id="0d440-126">**Posting Description**</span></span>             | <span data-ttu-id="0d440-127">Определяет описание учета.</span><span class="sxs-lookup"><span data-stu-id="0d440-127">Specifies the posting description.</span></span>                           |
   | <span data-ttu-id="0d440-128">**Код Склада**</span><span class="sxs-lookup"><span data-stu-id="0d440-128">**Location Code**</span></span>                   | <span data-ttu-id="0d440-129">Указывает значение кода, которое заполняется из списка складов.</span><span class="sxs-lookup"><span data-stu-id="0d440-129">Specifies the value code that is filled in from the Location list.</span></span> |
   | <span data-ttu-id="0d440-130">**Общая бизнес-группа**</span><span class="sxs-lookup"><span data-stu-id="0d440-130">**Gen. Bus. Posting Group**</span></span>         | <span data-ttu-id="0d440-131">Определяет код общей бизнес-группы.</span><span class="sxs-lookup"><span data-stu-id="0d440-131">Specifies the code of the general business posting group.</span></span>    |
   | <span data-ttu-id="0d440-132">**Дата учета**  **Дата документа**</span><span class="sxs-lookup"><span data-stu-id="0d440-132">**Posting Date**  **Document Date**</span></span> | <span data-ttu-id="0d440-133">Указывает рабочую дату, которая заполняется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0d440-133">Specifies the working date that is filled in by default.</span></span>     |
   | <span data-ttu-id="0d440-134">**Номер внешнего документа**</span><span class="sxs-lookup"><span data-stu-id="0d440-134">**External Document No.**</span></span>           | <span data-ttu-id="0d440-135">Введите номер первичного документа.</span><span class="sxs-lookup"><span data-stu-id="0d440-135">Enter the primary document number.</span></span>                           |
   | <span data-ttu-id="0d440-136">**Код менеджера**</span><span class="sxs-lookup"><span data-stu-id="0d440-136">**Purchaser Code**</span></span>                  | <span data-ttu-id="0d440-137">Указывает значение кода, которое выбирается из списка продавцов или менеджеров.</span><span class="sxs-lookup"><span data-stu-id="0d440-137">Specifies the value code that is selected from salespeople or purchasers.</span></span> |
   | <span data-ttu-id="0d440-138">**Корректировка**</span><span class="sxs-lookup"><span data-stu-id="0d440-138">**Correction**</span></span>                      | <span data-ttu-id="0d440-139">Определяет операцию как исправление.</span><span class="sxs-lookup"><span data-stu-id="0d440-139">Specifies if the entry is a correction.</span></span>                      |
   | <span data-ttu-id="0d440-140">**Статус**</span><span class="sxs-lookup"><span data-stu-id="0d440-140">**Status**</span></span>                          | <span data-ttu-id="0d440-141">Указывает состояние документа: "Открыт" или "Выпущен".</span><span class="sxs-lookup"><span data-stu-id="0d440-141">Specifies if the document is Open or Released.</span></span>               |

3. <span data-ttu-id="0d440-142">В строках документа окна **Акт оприходования товаров** заполните поля, описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0d440-142">In the document lines of the **Item Receipt** window, enter the fields described in the following table.</span></span>

   | <span data-ttu-id="0d440-143">Поле</span><span class="sxs-lookup"><span data-stu-id="0d440-143">Field</span></span>                      | <span data-ttu-id="0d440-144">Описание</span><span class="sxs-lookup"><span data-stu-id="0d440-144">Description</span></span>                                                  |
   | -------------------------- | ------------------------------------------------------------ |
   | <span data-ttu-id="0d440-145">**Код товара**</span><span class="sxs-lookup"><span data-stu-id="0d440-145">**Item No.**</span></span>               | <span data-ttu-id="0d440-146">Указывает номер товара из таблицы "Список товаров".</span><span class="sxs-lookup"><span data-stu-id="0d440-146">Specifies the item number from the Item List table.</span></span>          |
   | <span data-ttu-id="0d440-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d440-147">**Description**</span></span>            | <span data-ttu-id="0d440-148">Определяет описание товара.</span><span class="sxs-lookup"><span data-stu-id="0d440-148">Specifies the item description.</span></span>                              |
   | <span data-ttu-id="0d440-149">**количество;**</span><span class="sxs-lookup"><span data-stu-id="0d440-149">**Quantity**</span></span>               | <span data-ttu-id="0d440-150">Определяет количество единиц товара.</span><span class="sxs-lookup"><span data-stu-id="0d440-150">Specifies the number of item units.</span></span>                          |
   | <span data-ttu-id="0d440-151">**Зарезерв. входящее кол-во**</span><span class="sxs-lookup"><span data-stu-id="0d440-151">**Reserve Quantity Inbnd**</span></span> | <span data-ttu-id="0d440-152">Указывает количество товара, зарезервированное на складе получателя.</span><span class="sxs-lookup"><span data-stu-id="0d440-152">Specifies the item quantity reserved at the warehouse of the receiver.</span></span> |
   | <span data-ttu-id="0d440-153">**Цена единицы**</span><span class="sxs-lookup"><span data-stu-id="0d440-153">**Unit Amount**</span></span>            | <span data-ttu-id="0d440-154">Определяет цену единицы товара.</span><span class="sxs-lookup"><span data-stu-id="0d440-154">Specifies the price of a unit item.</span></span>                          |
   | <span data-ttu-id="0d440-155">**Косвенные затраты (%)**</span><span class="sxs-lookup"><span data-stu-id="0d440-155">**Indirect Cost %**</span></span>        | <span data-ttu-id="0d440-156">Определяет процент косвенных затрат.</span><span class="sxs-lookup"><span data-stu-id="0d440-156">Specifies the indirect cost percent.</span></span>                         |
   | <span data-ttu-id="0d440-157">**Себестоимость единицы**</span><span class="sxs-lookup"><span data-stu-id="0d440-157">**Unit Cost**</span></span>              | <span data-ttu-id="0d440-158">Определяет себестоимость единицы товара в строке прихода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="0d440-158">Specifies the item unit cost of the receipt shipment line.</span></span>   |
   | <span data-ttu-id="0d440-159">**Сумма**</span><span class="sxs-lookup"><span data-stu-id="0d440-159">**Amount**</span></span>                 | <span data-ttu-id="0d440-160">Определяет сумму транзакции.</span><span class="sxs-lookup"><span data-stu-id="0d440-160">Specifies the transaction amount.</span></span>                            |
   | <span data-ttu-id="0d440-161">**Код единицы измерения**</span><span class="sxs-lookup"><span data-stu-id="0d440-161">**Unit of Measure Code**</span></span>   | <span data-ttu-id="0d440-162">Определяет код единицы измерения полученных товаров.</span><span class="sxs-lookup"><span data-stu-id="0d440-162">Specifies the unit of measure code for the received items.</span></span>   |

4. <span data-ttu-id="0d440-163">В окне **Акт оприходования товаров** выберите действие **Подписи сотрудников**, чтобы указать подпись ответственного лица.</span><span class="sxs-lookup"><span data-stu-id="0d440-163">In the **Item Receipt** window, choose the **Employee Signatures** action to specify the signature of the person in charge.</span></span>

5. <span data-ttu-id="0d440-164">Введите значения в поля, описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0d440-164">Enter the fields described in the following table.</span></span>

   | <span data-ttu-id="0d440-165">Поле</span><span class="sxs-lookup"><span data-stu-id="0d440-165">Field</span></span>             | <span data-ttu-id="0d440-166">Описание</span><span class="sxs-lookup"><span data-stu-id="0d440-166">Description</span></span>                                                  |
   | ----------------- | ------------------------------------------------------------ |
   | <span data-ttu-id="0d440-167">**Тип сотрудника**</span><span class="sxs-lookup"><span data-stu-id="0d440-167">**Employee Type**</span></span> | <span data-ttu-id="0d440-168">Определяет тип сотрудника.</span><span class="sxs-lookup"><span data-stu-id="0d440-168">Specifies the type of the employee.</span></span>                          |
   | <span data-ttu-id="0d440-169">**Код сотрудника**</span><span class="sxs-lookup"><span data-stu-id="0d440-169">**Employee No.**</span></span>  | <span data-ttu-id="0d440-170">Задает номер сотрудника, который должен поставить свою подпись.</span><span class="sxs-lookup"><span data-stu-id="0d440-170">Specifies the employee number of the employee who must sign.</span></span> |
   | <span data-ttu-id="0d440-171">**Имя сотрудника**</span><span class="sxs-lookup"><span data-stu-id="0d440-171">**Employee Name**</span></span> | <span data-ttu-id="0d440-172">Задает значения, которые извлекаются из стандартных полей выбранной карточки **Карточка сотрудника**.</span><span class="sxs-lookup"><span data-stu-id="0d440-172">Specifies the values that are retrieved from the standard fields of the selected **Employee Card**.</span></span> |

6. <span data-ttu-id="0d440-173">Для печати отчета **Акт оприходования товаров** из окна **Акт оприходования товаров** выберите действие **Товарный документ**.</span><span class="sxs-lookup"><span data-stu-id="0d440-173">To print an **Item Receipt** report from the **Item Receipt** window, choose the **Item Document** action.</span></span>

7. <span data-ttu-id="0d440-174">Нажмите кнопку **Печать**.</span><span class="sxs-lookup"><span data-stu-id="0d440-174">Choose the **Print** button.</span></span>

<span data-ttu-id="0d440-175">Следующие функции доступны в окне **Акт оприходования товара**.</span><span class="sxs-lookup"><span data-stu-id="0d440-175">The following functions are available in the **Item Receipt** window.</span></span>

| <span data-ttu-id="0d440-176">Функция</span><span class="sxs-lookup"><span data-stu-id="0d440-176">Function</span></span>                         | <span data-ttu-id="0d440-177">Описание</span><span class="sxs-lookup"><span data-stu-id="0d440-177">Description</span></span>                 |
| -------------------------------- | ----------------------------|
| <span data-ttu-id="0d440-178">Изменение статуса документа</span><span class="sxs-lookup"><span data-stu-id="0d440-178">Changing document status</span></span>         | <span data-ttu-id="0d440-179">Документы можно открыть или выпустить для следующего этапа обработки.</span><span class="sxs-lookup"><span data-stu-id="0d440-179">Documents can be open or released for the next processing stage.</span></span> <span data-ttu-id="0d440-180">Выберите действие **Выпустить** или **Открыть повторно**.</span><span class="sxs-lookup"><span data-stu-id="0d440-180">Choose the **Release** or the **Reopen** action.</span></span> |
| <span data-ttu-id="0d440-181">Резервирование строк документа</span><span class="sxs-lookup"><span data-stu-id="0d440-181">Reservation of document lines</span></span>    | <span data-ttu-id="0d440-182">Товары можно зарезервировать из строки документа.</span><span class="sxs-lookup"><span data-stu-id="0d440-182">Items can be reserved from the document line.</span></span> <span data-ttu-id="0d440-183">Выберите действие **Резервировать**.</span><span class="sxs-lookup"><span data-stu-id="0d440-183">Choose the **Reserve** action.</span></span> |
| <span data-ttu-id="0d440-184">Расчет коррекции склада</span><span class="sxs-lookup"><span data-stu-id="0d440-184">Warehouse adjustment calculation</span></span> | <span data-ttu-id="0d440-185">Относится только к коррекции количества товаров в складских ячейках. Эта функция доступна только тогда, когда на складке используется расширенная комплектация и размещение.</span><span class="sxs-lookup"><span data-stu-id="0d440-185">Refers only to item quantity corrections in the warehouse bins. This is accessible only if advanced picking and placing is used in the warehouse.</span></span> |
| <span data-ttu-id="0d440-186">Учет документа</span><span class="sxs-lookup"><span data-stu-id="0d440-186">Document posting</span></span>                 | <span data-ttu-id="0d440-187">Выберите действие **Учет**, чтобы выполнить следующую операцию:   -   **Учет** Учет акта оприходования товара.</span><span class="sxs-lookup"><span data-stu-id="0d440-187">Choose the **Post** action to perform the following:   -   **Post** Post the item receipt.</span></span> <span data-ttu-id="0d440-188">Создается учтенный акт оприходования товара.</span><span class="sxs-lookup"><span data-stu-id="0d440-188">The posted item receipt is created.</span></span><span data-ttu-id="0d440-189"> -   **Учет и печать** Учет акта оприходования и печать тестового отчета.</span><span class="sxs-lookup"><span data-stu-id="0d440-189"> -   **Post and Print** Post the receipt and print the test report.</span></span> |

## <a name="analysis-of-a-posted-document-item-receipt-without-a-vendor"></a><span data-ttu-id="0d440-190">Анализ учтенного акта оприходования товара без поставщика</span><span class="sxs-lookup"><span data-stu-id="0d440-190">Analysis of a Posted Document Item Receipt Without a Vendor</span></span>

<span data-ttu-id="0d440-191">В следующей процедуре показан порядок анализа учтенного акта оприходования товаров без поставщика.</span><span class="sxs-lookup"><span data-stu-id="0d440-191">The following procedure shows how to analyze a posted document item receipt without a vendor.</span></span>

1. <span data-ttu-id="0d440-192">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенные акты оприходования товара**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="0d440-192">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Item Receipts**, and then choose the related link.</span></span>

   > [!NOTE]
   > <span data-ttu-id="0d440-193">В учтенном акте оприходования товаров отображается вся информация из приходной накладной.</span><span class="sxs-lookup"><span data-stu-id="0d440-193">The posted item receipt displays all the information from the item receipt.</span></span>

2. <span data-ttu-id="0d440-194">Выберите действие **Сортировка**, чтобы отсортировать список выбранных для печати документов по возрастанию или по убыванию.</span><span class="sxs-lookup"><span data-stu-id="0d440-194">Choose the **Sort** action to sort the list of documents selected for printing in ascending or descending order.</span></span>

3. <span data-ttu-id="0d440-195">Нажмите кнопку **Печать**.</span><span class="sxs-lookup"><span data-stu-id="0d440-195">Choose the **Print** button.</span></span>

## <a name="creating-an-item-writing-off-act"></a><span data-ttu-id="0d440-196">Создание акта списания товаров</span><span class="sxs-lookup"><span data-stu-id="0d440-196">Creating an Item Writing-Off Act</span></span>

<span data-ttu-id="0d440-197">В следующей процедуре показан порядок создания акта списания товаров.</span><span class="sxs-lookup"><span data-stu-id="0d440-197">The following procedure shows how to create an item writing-off act.</span></span>

1. <span data-ttu-id="0d440-198">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Акты списания товаров**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="0d440-198">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Shipments**, and then choose the related link.</span></span>

2. <span data-ttu-id="0d440-199">В заголовке окна **Акт списания товаров** заполните поля.</span><span class="sxs-lookup"><span data-stu-id="0d440-199">On the header of the **Item Shipment** window, enter the fields.</span></span> <span data-ttu-id="0d440-200">Эти поля идентичны полям окна **Акт оприходования товаров**.</span><span class="sxs-lookup"><span data-stu-id="0d440-200">These fields are the same as those on the **Item Receipt** window.</span></span>

3. <span data-ttu-id="0d440-201">В строках документа окна **Акт списания товаров** заполните поля.</span><span class="sxs-lookup"><span data-stu-id="0d440-201">In the document lines of the **Item Shipment** window, enter the fields.</span></span> <span data-ttu-id="0d440-202">Эти поля идентичны полям окна **Акт оприходования товаров**, за исключением следующего.</span><span class="sxs-lookup"><span data-stu-id="0d440-202">These fields are the same as those on the **Item Receipt** window except for the following:</span></span>

    - <span data-ttu-id="0d440-203">Поле **Косвенные затраты** доступно только в окне **Акт оприходования товаров**.</span><span class="sxs-lookup"><span data-stu-id="0d440-203">The **Indirect Cost** field is available only in the **Item Receipt** window.</span></span>
    - <span data-ttu-id="0d440-204">Поля, описанные в следующей таблице, доступны только в окне **Акт списания товаров**.</span><span class="sxs-lookup"><span data-stu-id="0d440-204">The fields in the following table are available only in the **Item Shipment** window.</span></span>

    | <span data-ttu-id="0d440-205">Поле</span><span class="sxs-lookup"><span data-stu-id="0d440-205">Field</span></span>                      | <span data-ttu-id="0d440-206">Описание</span><span class="sxs-lookup"><span data-stu-id="0d440-206">Description</span></span>                                                  |
    | -------------------------- | ------------------------------------------------------------ |
    | <span data-ttu-id="0d440-207">**Номер ОС**</span><span class="sxs-lookup"><span data-stu-id="0d440-207">**FA No.**</span></span>                 | <span data-ttu-id="0d440-208">Указывает основное средство для списания товаров и материалов.</span><span class="sxs-lookup"><span data-stu-id="0d440-208">Specifies the fixed asset to write off items and materials.</span></span>  |
    | <span data-ttu-id="0d440-209">**Код книги амортизации**</span><span class="sxs-lookup"><span data-stu-id="0d440-209">**Depreciation Book Code**</span></span> | <span data-ttu-id="0d440-210">Указывает книгу амортизации основных средств, в которую будут добавлены дополнительные затраты.</span><span class="sxs-lookup"><span data-stu-id="0d440-210">Specifies the fixed asset depreciation book to which the additional cost will be added.</span></span> |

4. <span data-ttu-id="0d440-211">В окне **Акт списания товаров** выберите действие **Подписи сотрудников**, чтобы указать подпись ответственного лица.</span><span class="sxs-lookup"><span data-stu-id="0d440-211">In the **Item Shipment** window, choose the **Employee Signatures** actionm to specify the signature of the person in charge.</span></span>

5. <span data-ttu-id="0d440-212">Введите значения в поля, описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0d440-212">Enter the fields described in the following table.</span></span>

    | <span data-ttu-id="0d440-213">Поле</span><span class="sxs-lookup"><span data-stu-id="0d440-213">Field</span></span>             | <span data-ttu-id="0d440-214">Описание</span><span class="sxs-lookup"><span data-stu-id="0d440-214">Description</span></span>                                                  |
    | ----------------- | ------------------------------------------------------------ |
    | <span data-ttu-id="0d440-215">**Тип сотрудника**</span><span class="sxs-lookup"><span data-stu-id="0d440-215">**Employee Type**</span></span> | <span data-ttu-id="0d440-216">Определяет тип сотрудника.</span><span class="sxs-lookup"><span data-stu-id="0d440-216">Specifies the type of the employee.</span></span>                          |
    | <span data-ttu-id="0d440-217">**Код сотрудника**</span><span class="sxs-lookup"><span data-stu-id="0d440-217">**Employee No.**</span></span>  | <span data-ttu-id="0d440-218">Задает номер сотрудника, который должен поставить свою подпись.</span><span class="sxs-lookup"><span data-stu-id="0d440-218">Specifies the employee number of the employee who must sign.</span></span> |
    | <span data-ttu-id="0d440-219">**Имя сотрудника**</span><span class="sxs-lookup"><span data-stu-id="0d440-219">**Employee Name**</span></span> | <span data-ttu-id="0d440-220">Задает значения, которые извлекаются из стандартных полей выбранной карточки **Карточка сотрудника**.</span><span class="sxs-lookup"><span data-stu-id="0d440-220">Specifies the values that are retrieved from the standard fields of the selected **Employee Card**.</span></span> |

6. <span data-ttu-id="0d440-221">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="0d440-221">Choose the **Print** action.</span></span>

<span data-ttu-id="0d440-222">Функции, доступные в окне **Акт списания товаров**, совпадают с функциями, доступными в окне **Акт оприходования товаров**.</span><span class="sxs-lookup"><span data-stu-id="0d440-222">The functions available in the **Item Shipment** window are same as those in the **Item Receipt** window.</span></span>

## <a name="analysis-of-a-posted-document-item-writing-off-act"></a><span data-ttu-id="0d440-223">Анализ учтенного акта списания товара</span><span class="sxs-lookup"><span data-stu-id="0d440-223">Analysis of a Posted Document Item Writing-Off Act</span></span>

<span data-ttu-id="0d440-224">В следующей процедуре показан порядок анализа учтенного акта списания товаров.</span><span class="sxs-lookup"><span data-stu-id="0d440-224">The following procedure shows how to analyze a posted document item writing-off act.</span></span>

1. <span data-ttu-id="0d440-225">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенные акты списания товара**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="0d440-225">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Item Shipments**, and then choose the related link.</span></span>

  > [!NOTE]
  > <span data-ttu-id="0d440-226">В учтенном акте списания товаров отображается вся информация из расходной накладной.</span><span class="sxs-lookup"><span data-stu-id="0d440-226">The posted item shipment displays all the information from the item shipment.</span></span>

2. <span data-ttu-id="0d440-227">Выберите действие **Сортировка**, чтобы отсортировать список выбранных для печати документов по возрастанию или по убыванию.</span><span class="sxs-lookup"><span data-stu-id="0d440-227">Choose the **Sort** action to sort the list of documents selected for printing in ascending or descending order.</span></span>

3. <span data-ttu-id="0d440-228">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="0d440-228">Choose the **Print** action.</span></span>

## <a name="report-transfer-order-torg-13-based-on-an-unposted-transfer-document"></a><span data-ttu-id="0d440-229">Накладная на перемещение ТОРГ-13 на основании неучтенного документа перемещения</span><span class="sxs-lookup"><span data-stu-id="0d440-229">Report Transfer Order TORG-13 Based on an Unposted Transfer Document</span></span>

<span data-ttu-id="0d440-230">В следующей процедуре описывается порядок создания отчета по заказу на перемещение ТОРГ-13 на основании документов на перемещение, которые не были учтены.</span><span class="sxs-lookup"><span data-stu-id="0d440-230">The following procedure shows how to create a Transfer Order TORG-13 report based on transfer documents that are not posted.</span></span>

1. <span data-ttu-id="0d440-231">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на перемещение**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="0d440-231">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer Orders**, and then choose the related link.</span></span>

   <span data-ttu-id="0d440-232">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="0d440-232">Choose the **Print** action.</span></span>

## <a name="report-transfer-order-torg-13-based-on-a-posted-transfer-document---transfer-receipt"></a><span data-ttu-id="0d440-233">Накладная на перемещение ТОРГ-13 на основании учтенного документа перемещения - "Приходная накладная на перемещение"</span><span class="sxs-lookup"><span data-stu-id="0d440-233">Report Transfer Order TORG-13 Based on a Posted Transfer Document - Transfer Receipt</span></span>

<span data-ttu-id="0d440-234">В следующей процедуре описан порядок создания отчета на основе учтенного документа перемещения, называемого приходной накладной на перемещение.</span><span class="sxs-lookup"><span data-stu-id="0d440-234">The following procedure shows how to create a report based on a posted transfer document called a transfer receipt.</span></span>

1. <span data-ttu-id="0d440-235">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенная приходная накладная на перемещение**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="0d440-235">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Transfer Receipt**, and then choose the related link.</span></span>
2. <span data-ttu-id="0d440-236">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="0d440-236">Choose the **Print** action.</span></span>

## <a name="report-transfer-order-torg-13-based-on-a-posted-transfer-document---transfer-shipment"></a><span data-ttu-id="0d440-237">Накладная на перемещение ТОРГ-13 на основании учтенного документа перемещения - "Расходная накладная на перемещение"</span><span class="sxs-lookup"><span data-stu-id="0d440-237">Report Transfer Order TORG-13 Based on a Posted Transfer Document - Transfer Shipment</span></span>

<span data-ttu-id="0d440-238">В следующей процедуре описан порядок создания отчета на основе учтенного документа перемещения, называемого расходной накладной на перемещение.</span><span class="sxs-lookup"><span data-stu-id="0d440-238">The following procedure shows how to create a report based on a posted transfer document called a transfer shipment.</span></span>

1. <span data-ttu-id="0d440-239">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенная расходная накладная на перемещение**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="0d440-239">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Transfer Shipments**, and then choose the related link.</span></span>

   <span data-ttu-id="0d440-240">Выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="0d440-240">Choose the **Print** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="0d440-241">См. также</span><span class="sxs-lookup"><span data-stu-id="0d440-241">See Also</span></span>

[<span data-ttu-id="0d440-242">Товары Настройка</span><span class="sxs-lookup"><span data-stu-id="0d440-242">Inventory Setup</span></span>](Inventory-Setup.md)  
[<span data-ttu-id="0d440-243">Акты обязательств по товару</span><span class="sxs-lookup"><span data-stu-id="0d440-243">Item Obligatory Acts</span></span>](Item-Obligatory-Acts.md)  
[<span data-ttu-id="0d440-244">Оборотная ведомость для товаров по ГК</span><span class="sxs-lookup"><span data-stu-id="0d440-244">Item General Ledger Turnover</span></span>](Item-General-Ledger-Turnover.md)  
