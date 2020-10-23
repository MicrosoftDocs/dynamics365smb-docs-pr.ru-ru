---
title: Использование XML-схем для определения обмена данными
description: Используйте XML-схемы для настройки платформы обмена документами.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: d2e600f3b2da20540e224cb1405a50adc4a31f25
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3924957"
---
# <a name="use-xml-schemas-to-prepare-data-exchange-definitions"></a><span data-ttu-id="5bd54-103">Использование XML-схем для определения обмена данными</span><span class="sxs-lookup"><span data-stu-id="5bd54-103">Use XML Schemas to Prepare Data Exchange Definitions</span></span>

<span data-ttu-id="5bd54-104">Чтобы разрешить импорт или экспорт данных в файл в формате XML с использованием платформы обмена данными в [!INCLUDE[d365fin](includes/d365fin_md.md)], можно воспользоваться XML-схемами для определения элементов данных, которыми можно обмениваться с [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5bd54-104">To enable import/export of data in XML files through the data exchange framework in [!INCLUDE[d365fin](includes/d365fin_md.md)], you can use XML schemas to define which data elements you want to exchange with [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="5bd54-105">Эта работа выполняется на странице **Средство просмотра схем XML** путем загрузки файла XML-схемы. Для этого нужно выбрать соответствующие элементы данных, затем инициализировать определение обмена данными.</span><span class="sxs-lookup"><span data-stu-id="5bd54-105">You perform this work on the **XML Schema Viewer** page by loading the XML schema file, selecting the relevant data elements, and then initializing a data exchange definition.</span></span>  

 <span data-ttu-id="5bd54-106">Когда вы определили, какие элементы данных требуется включить на основе схемы XML, можно использовать действие **Создать определение обмена данными**, чтобы инициализировать определение обмена данными на основании выбранных элементов данных, которую затем можно закончить в структуре обмена данными.</span><span class="sxs-lookup"><span data-stu-id="5bd54-106">When you have defined which data elements to include based on the XML schema, you can use the **Generate Data Exchange Definition** action to initialize a data exchange definition based on the selected data elements, which you then complete in the Data Exchange Framework.</span></span> <span data-ttu-id="5bd54-107">В результате создается запись на странице **Определения учета обмена**, где затем определяется, какие элементы в файле сопоставляются полям в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5bd54-107">This creates a record on the **Posting Exchange Definition** page where you continue by defining which elements in the file map to which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="5bd54-108">Дополнительные сведения см. в разделе [Настройка определений обмена данными](across-how-to-set-up-data-exchange-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="5bd54-108">For more information, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

 <span data-ttu-id="5bd54-109">Этот раздел содержит следующие процедуры:</span><span class="sxs-lookup"><span data-stu-id="5bd54-109">This topic contains the following procedures:</span></span>  

- <span data-ttu-id="5bd54-110">загрузка файла XML-схемы</span><span class="sxs-lookup"><span data-stu-id="5bd54-110">To load an XML schema file</span></span>  

- <span data-ttu-id="5bd54-111">Выбор или удаление узлов в XML-схеме</span><span class="sxs-lookup"><span data-stu-id="5bd54-111">To select or clear nodes in an XML schema</span></span>  

- <span data-ttu-id="5bd54-112">Создание определения обмена данными на базе XML-схемы</span><span class="sxs-lookup"><span data-stu-id="5bd54-112">To generate a data exchange definition that is based on an XML schema</span></span>  

## <a name="to-load-an-xml-schema-file"></a><span data-ttu-id="5bd54-113">загрузка файла XML-схемы</span><span class="sxs-lookup"><span data-stu-id="5bd54-113">To load an XML schema file</span></span>

1. <span data-ttu-id="5bd54-114">Убедитесь, что доступен соответствующий файл XML-схемы.</span><span class="sxs-lookup"><span data-stu-id="5bd54-114">Make sure that the relevant XML schema file is available.</span></span> <span data-ttu-id="5bd54-115">Расширение файла – XSD.</span><span class="sxs-lookup"><span data-stu-id="5bd54-115">The file extension is .xsd.</span></span>  

2. <span data-ttu-id="5bd54-116">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Схемы XML**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="5bd54-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **XML Schemas**, and then choose the related link.</span></span>  

3. <span data-ttu-id="5bd54-117">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="5bd54-117">Choose the **New** action.</span></span>  

4. <span data-ttu-id="5bd54-118">Заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="5bd54-118">Fill the fields as described in the following table.</span></span>  

    |<span data-ttu-id="5bd54-119">Поле</span><span class="sxs-lookup"><span data-stu-id="5bd54-119">Field</span></span>|<span data-ttu-id="5bd54-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd54-120">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5bd54-121">**Код**</span><span class="sxs-lookup"><span data-stu-id="5bd54-121">**Code**</span></span>|<span data-ttu-id="5bd54-122">Указание кода для определения XML-схемы.</span><span class="sxs-lookup"><span data-stu-id="5bd54-122">Specify a code to identify the XML schema.</span></span>|  
    |<span data-ttu-id="5bd54-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5bd54-123">**Description**</span></span>|<span data-ttu-id="5bd54-124">Указание описания XML-схемы.</span><span class="sxs-lookup"><span data-stu-id="5bd54-124">Specify a description of the XML schema.</span></span>|  

     <span data-ttu-id="5bd54-125">В поле **Целевое пространство имен** задается любое пространство имен из файла XML-схемы, загруженного для соответствующей строки.</span><span class="sxs-lookup"><span data-stu-id="5bd54-125">The **Target Namespace** field specifies any namespace in the XML schema file that has been loaded for the line.</span></span>  

5. <span data-ttu-id="5bd54-126">Выберите действие **Схема загрузки**, затем выберите файл схемы XML.</span><span class="sxs-lookup"><span data-stu-id="5bd54-126">Choose the **Load Schema** action, and then select the XML schema file.</span></span>  

     <span data-ttu-id="5bd54-127">Если файл загружен, остальные поля в строке заполняются сведениями из этого файла, а также устанавливается флажок **Схема загружена**.</span><span class="sxs-lookup"><span data-stu-id="5bd54-127">When the file is loaded, the rest of the fields on the line are filled with information from the file, and the **Schema is Loaded** check box is selected.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="5bd54-128">Дерево загруженной XML-схемы по умолчанию свернуто.</span><span class="sxs-lookup"><span data-stu-id="5bd54-128">The tree of the loaded XML schema is collapsed by default.</span></span> <span data-ttu-id="5bd54-129">Можно развернуть каждый узел нажатием кнопки **+** на нем.</span><span class="sxs-lookup"><span data-stu-id="5bd54-129">You expand each node by choosing the **+** button on the node.</span></span> <span data-ttu-id="5bd54-130">Чтобы развернуть все узлы, выберите **Раскрыть все** на ленте.</span><span class="sxs-lookup"><span data-stu-id="5bd54-130">To expand all nodes, choose **Expand All** on the ribbon.</span></span>  

### <a name="to-select-or-clear-nodes-in-an-xml-schema"></a><span data-ttu-id="5bd54-131">Выбор или удаление узлов в XML-схеме</span><span class="sxs-lookup"><span data-stu-id="5bd54-131">To select or clear nodes in an XML schema</span></span>  

1. <span data-ttu-id="5bd54-132">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Средство просмотра схем XML**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="5bd54-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **XML Schema Viewer**, and then choose the related link.</span></span>  

2. <span data-ttu-id="5bd54-133">Заполните поля в заголовке, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="5bd54-133">Fill the fields on the header as described in the following table.</span></span>  

    |<span data-ttu-id="5bd54-134">Поле</span><span class="sxs-lookup"><span data-stu-id="5bd54-134">Field</span></span>|<span data-ttu-id="5bd54-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd54-135">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5bd54-136">**Код схемы XML**</span><span class="sxs-lookup"><span data-stu-id="5bd54-136">**XML Schema Code**</span></span>|<span data-ttu-id="5bd54-137">Укажите файл XML-схемы, загруженный на шаге 5 в разделе "Загрузка файла XML-схемы".</span><span class="sxs-lookup"><span data-stu-id="5bd54-137">Specify the XML schema file that you loaded in step 5 in the "To load an XML schema file" section.</span></span>|  
    |<span data-ttu-id="5bd54-138">**Новый номер XMLport**</span><span class="sxs-lookup"><span data-stu-id="5bd54-138">**New XMLport No.**</span></span>|<span data-ttu-id="5bd54-139">Укажите номер XMLport, созданного из схемы XML при выборе действия **Создать XMLport**.</span><span class="sxs-lookup"><span data-stu-id="5bd54-139">Specify the number of the XMLport that is created from this XML schema when you choose the **Generate XMLport** action.</span></span>|  

     <span data-ttu-id="5bd54-140">Строки заполняются узлами, представляющими все элементы в XML-схеме.</span><span class="sxs-lookup"><span data-stu-id="5bd54-140">The lines are now filled with nodes representing all elements in the XML schema.</span></span> <span data-ttu-id="5bd54-141">Узлы для элементов, которые являются обязательными согласно XML-схеме, выбираются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5bd54-141">Nodes for elements that are mandatory according to the XML schema are selected by default.</span></span>  

3. <span data-ttu-id="5bd54-142">В первой строке в столбце **Название узла** разверните узел **Документ** и постепенного разворачивайте дочерние узлы, которые необходимо просмотреть.</span><span class="sxs-lookup"><span data-stu-id="5bd54-142">On the first line, in the **Node Name** column, expand the **Document** node, and then gradually expand underlying nodes that you want to review.</span></span>  

     <span data-ttu-id="5bd54-143">В качестве альтернативы щелкните правой кнопкой мыши и выберите **Развернуть все**.</span><span class="sxs-lookup"><span data-stu-id="5bd54-143">Alternatively, right-click on a node and then choose **Expand All**.</span></span>  

4. <span data-ttu-id="5bd54-144">Выберите одно из следующих действий, чтобы изменить узлы для отображения.</span><span class="sxs-lookup"><span data-stu-id="5bd54-144">Choose either of the following actions to change which nodes are displayed.</span></span>  

    |<span data-ttu-id="5bd54-145">**Действие**</span><span class="sxs-lookup"><span data-stu-id="5bd54-145">**Action**</span></span>|<span data-ttu-id="5bd54-146">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd54-146">Description</span></span>|  
    |----------------|---------------------------------------|  
    |<span data-ttu-id="5bd54-147">**Показать все**</span><span class="sxs-lookup"><span data-stu-id="5bd54-147">**Show All**</span></span>|<span data-ttu-id="5bd54-148">Отображаются все узлы.</span><span class="sxs-lookup"><span data-stu-id="5bd54-148">All nodes are shown.</span></span>|  
    |<span data-ttu-id="5bd54-149">**Скрыть необязательные**</span><span class="sxs-lookup"><span data-stu-id="5bd54-149">**Hide Non-Mandatory**</span></span>|<span data-ttu-id="5bd54-150">Отображаются только узлы, представляющие элементы, необходимые согласно XML-схеме.</span><span class="sxs-lookup"><span data-stu-id="5bd54-150">Only nodes representing elements that are required according to the XML schema are shown.</span></span> <span data-ttu-id="5bd54-151">Обычно эти узлы обозначаются **1** в поле **MinOccurs**.</span><span class="sxs-lookup"><span data-stu-id="5bd54-151">These nodes are typically indicated by a **1** in the **MinOccurs** field.</span></span><br /><br /> <span data-ttu-id="5bd54-152">Щелкните **Показать все** для сторнирования представления.</span><span class="sxs-lookup"><span data-stu-id="5bd54-152">Choose **Show All** to reverse the view.</span></span>|  
    |<span data-ttu-id="5bd54-153">**Скрыть невыбранные**</span><span class="sxs-lookup"><span data-stu-id="5bd54-153">**Hide Non-Selected**</span></span>|<span data-ttu-id="5bd54-154">Отображаются только узлы, в которых установлен флажок **Выбрано**.</span><span class="sxs-lookup"><span data-stu-id="5bd54-154">Only nodes where the **Selected** check box is selected are shown.</span></span><br /><br /> <span data-ttu-id="5bd54-155">Щелкните **Показать все** для сторнирования представления.</span><span class="sxs-lookup"><span data-stu-id="5bd54-155">Choose **Show All** to reverse the view.</span></span>|  

5. <span data-ttu-id="5bd54-156">Выберите действие **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="5bd54-156">Choose the **Edit** action.</span></span>  

6. <span data-ttu-id="5bd54-157">С помощью флажка **Выбрано** можно для каждого узла указать, требуется ли включить поддержку элемента в определении обмена данными для связанного файла банка SEPA.</span><span class="sxs-lookup"><span data-stu-id="5bd54-157">In the **Selected** check box, specify for each node if you want the element to be supported in the data exchange definition for the related SEPA bank file.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="5bd54-158">При выборе обязательного дочернего узла все родительские узлы над ним также выбираются.</span><span class="sxs-lookup"><span data-stu-id="5bd54-158">When you select a mandatory child node, all parent nodes above it are also selected.</span></span>  

7. <span data-ttu-id="5bd54-159">Выберите действие **Выбрать все обязательные элементы**, чтобы снова выбрать все узлы, представляющие элементы, которые являются обязательными согласно XML-схеме.</span><span class="sxs-lookup"><span data-stu-id="5bd54-159">Choose the **Select All Mandatory Elements** action to reselect all nodes that represent elements that are mandatory according to the XML schema.</span></span>  

8. <span data-ttu-id="5bd54-160">Выберите действие **Снять выделение** для отмены выбора всех элементов.</span><span class="sxs-lookup"><span data-stu-id="5bd54-160">Choose the **Deselect All** action to clear all selections.</span></span>  

     <span data-ttu-id="5bd54-161">В поле **Выбор** указано, что у узла имеется два или более дочерних узла, которые функционируют как параметры.</span><span class="sxs-lookup"><span data-stu-id="5bd54-161">The **Choice** field specifies that the node has two or more sibling nodes that function as options.</span></span>  

### <a name="to-generate-a-data-exchange-definition-that-is-based-on-an-xml-schema"></a><span data-ttu-id="5bd54-162">Создание определения обмена данными на базе XML-схемы</span><span class="sxs-lookup"><span data-stu-id="5bd54-162">To generate a data exchange definition that is based on an XML schema</span></span>  

1. <span data-ttu-id="5bd54-163">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Схемы XML**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="5bd54-163">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter  **XML Schemas**, and then choose the related link.</span></span>  

2. <span data-ttu-id="5bd54-164">Выберите соответствующую схему XML, затем выберите действие **Открыть средство просмотра XML-схем**.</span><span class="sxs-lookup"><span data-stu-id="5bd54-164">Select the relevant XML schema, and then choose the **Open XML Schema Viewer** action.</span></span>  

3. <span data-ttu-id="5bd54-165">Убедитесь, что выбраны соответствующие узлы.</span><span class="sxs-lookup"><span data-stu-id="5bd54-165">Make sure the relevant nodes are selected.</span></span> <span data-ttu-id="5bd54-166">Дополнительные сведения см. в разделе "Выбор или отмена выбора узлов на XML-схеме".</span><span class="sxs-lookup"><span data-stu-id="5bd54-166">For more information, see the "To select or clear nodes in an XML schema" section.</span></span>  

4. <span data-ttu-id="5bd54-167">На странице **Средство просмотра схем XML** выберите действие **Создать определение обмена данными**.</span><span class="sxs-lookup"><span data-stu-id="5bd54-167">On the **XML Schema Viewer** page, choose the **Generate Data Exchange Definition** action.</span></span>  

 <span data-ttu-id="5bd54-168">Запись определения обмена данными создается на странице **Определения учета обмена**, которую можно заполнить, указав, какие элементы файла сопоставляются с какими полями в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5bd54-168">A data exchange definition is created on the **Posting Exchange Definition** page, which you can complete by specifying which elements in the file map to which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="5bd54-169">Дополнительные сведения см. в разделе [Настройка определений обмена данными](across-how-to-set-up-data-exchange-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="5bd54-169">For more information, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

> [!NOTE]  
> <span data-ttu-id="5bd54-170">Можно также использовать функцию **Получить структуру файла** со страницы **Определения учета обмена**, использующую функциональные возможности страницы **Средство просмотра схем XML** для предварительного заполнения экспресс-вкладки **Определения столбца**.</span><span class="sxs-lookup"><span data-stu-id="5bd54-170">You can also use the **Get File Structure** function from the **Posting Exchange Definition** page, which uses the functionality of the **XML Schema Viewer** page to prefill the **Column Definitions** TastTab.</span></span>  

> [!NOTE]
> <span data-ttu-id="5bd54-171">В волне 1 выпуска 2019 года и более ранних версиях можно было создать XMLport, который был основан на схеме, затем импортировать его в свое решение.</span><span class="sxs-lookup"><span data-stu-id="5bd54-171">In 2019 release wave 1 and earlier versions, you could generate an XMLport that was based on the schema and then import that into your solution.</span></span> <span data-ttu-id="5bd54-172">Это больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bd54-172">This is no longer supported.</span></span>

## <a name="see-also"></a><span data-ttu-id="5bd54-173">См. также</span><span class="sxs-lookup"><span data-stu-id="5bd54-173">See Also</span></span>

[<span data-ttu-id="5bd54-174">Настройка определений обмена данными</span><span class="sxs-lookup"><span data-stu-id="5bd54-174">Set Up Data Exchange Definitions</span></span>](across-how-to-set-up-data-exchange-definitions.md)  
[<span data-ttu-id="5bd54-175">Экспорт платежей в банковский файл</span><span class="sxs-lookup"><span data-stu-id="5bd54-175">Export Payments to a Bank File</span></span>](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file)  
[<span data-ttu-id="5bd54-176">Сбор платежей с прямым дебетом SEPA</span><span class="sxs-lookup"><span data-stu-id="5bd54-176">Collect Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)  
[<span data-ttu-id="5bd54-177">О структуре обмена данными</span><span class="sxs-lookup"><span data-stu-id="5bd54-177">About the Data Exchange Framework</span></span>](across-about-the-data-exchange-framework.md)  
