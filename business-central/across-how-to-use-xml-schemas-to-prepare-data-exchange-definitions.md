---
title: Создание XMLports на основе XML-схем | Документация Майкрософт
description: Используйте XML-схемы для настройки платформы обмена документами.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 65392cc5f47353b9266d5198b739835fd329c204
ms.sourcegitcommit: d0dc5e5c46b932899e2a9c7183959d0ff37738d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "3076687"
---
# <a name="use-xml-schemas-to-prepare-data-exchange-definitions"></a><span data-ttu-id="06359-103">Использование XML-схем для определения обмена данными</span><span class="sxs-lookup"><span data-stu-id="06359-103">Use XML Schemas to Prepare Data Exchange Definitions</span></span>
<span data-ttu-id="06359-104">Чтобы разрешить импорт или экспорт данных в файл в формате XML с использованием платформы обмена данными в [!INCLUDE[d365fin](includes/d365fin_md.md)], можно воспользоваться XML-схемами для определения элементов данных, которыми можно обмениваться с [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="06359-104">To enable import/export of data in XML files through the data exchange framework in [!INCLUDE[d365fin](includes/d365fin_md.md)], you can use XML schemas to define which data elements you want to exchange with [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="06359-105">Эта работа выполняется на странице **Средство просмотра схем XML** путем загрузки файла XML-схемы. Для этого нужно выбрать соответствующие элементы данных и инициализировать определение обмена данными или XMLport.</span><span class="sxs-lookup"><span data-stu-id="06359-105">You perform this work on the **XML Schema Viewer** page by loading the XML schema file, selecting the relevant data elements, and then initializing either a data exchange definition or an XMLport.</span></span>  

 <span data-ttu-id="06359-106">Определив, какие элементы данных необходимо включить с учетом XML-схемы, можно воспользоваться действием **Создать XMLport** для создания объекта XMLport.</span><span class="sxs-lookup"><span data-stu-id="06359-106">When you have defined which data elements to include based on the XML schema, you can use the **Generate XMLport** action to create the XMLport object.</span></span>  

 <span data-ttu-id="06359-107">Кроме того, можно использовать действие **Создать определение обмена данными**, чтобы инициализировать определение обмена данными на основании выбранных элементов данных, которую затем можно закончить в структуре обмена данными.</span><span class="sxs-lookup"><span data-stu-id="06359-107">Alternatively, you can use the **Generate Data Exchange Definition** action to initialize a data exchange definition based on the selected data elements, which you then complete in the Data Exchange Framework.</span></span> <span data-ttu-id="06359-108">В результате создается запись на странице **Определения учета обмена**, где затем определяется, какие элементы в файле сопоставляются полям в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="06359-108">This creates a record on the **Posting Exchange Definition** page where you continue by defining which elements in the file map to which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="06359-109">Дополнительные сведения см. в разделе [Настройка определений обмена данными](across-how-to-set-up-data-exchange-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="06359-109">For more information, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

 <span data-ttu-id="06359-110">Этот раздел содержит следующие процедуры:</span><span class="sxs-lookup"><span data-stu-id="06359-110">This topic contains the following procedures:</span></span>  

-   <span data-ttu-id="06359-111">загрузка файла XML-схемы</span><span class="sxs-lookup"><span data-stu-id="06359-111">To load an XML schema file</span></span>  

-   <span data-ttu-id="06359-112">Выбор или удаление узлов в XML-схеме</span><span class="sxs-lookup"><span data-stu-id="06359-112">To select or clear nodes in an XML schema</span></span>  

-   <span data-ttu-id="06359-113">Создание определения обмена данными на базе XML-схемы</span><span class="sxs-lookup"><span data-stu-id="06359-113">To generate a data exchange definition that is based on an XML schema</span></span>  

-   <span data-ttu-id="06359-114">Создание XMLport для файла на основе XML-схемы</span><span class="sxs-lookup"><span data-stu-id="06359-114">To generate an XMLport for the file that is based on an XML schema</span></span>  

-   <span data-ttu-id="06359-115">Импорт XMLport в конструктор объектов</span><span class="sxs-lookup"><span data-stu-id="06359-115">To import an XMLport into the Object Designer</span></span>  

### <a name="to-load-an-xml-schema-file"></a><span data-ttu-id="06359-116">загрузка файла XML-схемы</span><span class="sxs-lookup"><span data-stu-id="06359-116">To load an XML schema file</span></span>  

1.  <span data-ttu-id="06359-117">Убедитесь, что доступен соответствующий файл XML-схемы.</span><span class="sxs-lookup"><span data-stu-id="06359-117">Make sure that the relevant XML schema file is available.</span></span> <span data-ttu-id="06359-118">Расширение файла – XSD.</span><span class="sxs-lookup"><span data-stu-id="06359-118">The file extension is .xsd.</span></span>  

2.  <span data-ttu-id="06359-119">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Схемы XML**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="06359-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **XML Schemas**, and then choose the related link.</span></span>  

3.  <span data-ttu-id="06359-120">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="06359-120">Choose the **New** action.</span></span>  

4.  <span data-ttu-id="06359-121">Заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="06359-121">Fill the fields as described in the following table.</span></span>  

    |<span data-ttu-id="06359-122">Поле</span><span class="sxs-lookup"><span data-stu-id="06359-122">Field</span></span>|<span data-ttu-id="06359-123">Описание</span><span class="sxs-lookup"><span data-stu-id="06359-123">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="06359-124">**Код**</span><span class="sxs-lookup"><span data-stu-id="06359-124">**Code**</span></span>|<span data-ttu-id="06359-125">Указание кода для определения XML-схемы.</span><span class="sxs-lookup"><span data-stu-id="06359-125">Specify a code to identify the XML schema.</span></span>|  
    |<span data-ttu-id="06359-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="06359-126">**Description**</span></span>|<span data-ttu-id="06359-127">Указание описания XML-схемы.</span><span class="sxs-lookup"><span data-stu-id="06359-127">Specify a description of the XML schema.</span></span>|  

     <span data-ttu-id="06359-128">В поле **Целевое пространство имен** задается любое пространство имен из файла XML-схемы, загруженного для соответствующей строки.</span><span class="sxs-lookup"><span data-stu-id="06359-128">The **Target Namespace** field specifies any namespace in the XML schema file that has been loaded for the line.</span></span>  

5.  <span data-ttu-id="06359-129">Выберите действие **Схема загрузки**, затем выберите файл схемы XML.</span><span class="sxs-lookup"><span data-stu-id="06359-129">Choose the **Load Schema** action, and then select the XML schema file.</span></span>  

     <span data-ttu-id="06359-130">Если файл загружен, остальные поля в строке заполняются сведениями из этого файла, а также устанавливается флажок **Схема загружена**.</span><span class="sxs-lookup"><span data-stu-id="06359-130">When the file is loaded, the rest of the fields on the line are filled with information from the file, and the **Schema is Loaded** check box is selected.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="06359-131">Дерево загруженной XML-схемы по умолчанию свернуто.</span><span class="sxs-lookup"><span data-stu-id="06359-131">The tree of the loaded XML schema is collapsed by default.</span></span> <span data-ttu-id="06359-132">Можно развернуть каждый узел нажатием кнопки **+** на нем.</span><span class="sxs-lookup"><span data-stu-id="06359-132">You expand each node by choosing the **+** button on the node.</span></span> <span data-ttu-id="06359-133">Чтобы развернуть все узлы, выберите **Раскрыть все** на ленте.</span><span class="sxs-lookup"><span data-stu-id="06359-133">To expand all nodes, choose **Expand All** on the ribbon.</span></span>  

### <a name="to-select-or-clear-nodes-in-an-xml-schema"></a><span data-ttu-id="06359-134">Выбор или удаление узлов в XML-схеме</span><span class="sxs-lookup"><span data-stu-id="06359-134">To select or clear nodes in an XML schema</span></span>  

1.  <span data-ttu-id="06359-135">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Средство просмотра схем XML**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="06359-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **XML Schema Viewer**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="06359-136">Заполните поля в заголовке, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="06359-136">Fill the fields on the header as described in the following table.</span></span>  

    |<span data-ttu-id="06359-137">Поле</span><span class="sxs-lookup"><span data-stu-id="06359-137">Field</span></span>|<span data-ttu-id="06359-138">Описание</span><span class="sxs-lookup"><span data-stu-id="06359-138">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="06359-139">**Код схемы XML**</span><span class="sxs-lookup"><span data-stu-id="06359-139">**XML Schema Code**</span></span>|<span data-ttu-id="06359-140">Укажите файл XML-схемы, загруженный на шаге 5 в разделе "Загрузка файла XML-схемы".</span><span class="sxs-lookup"><span data-stu-id="06359-140">Specify the XML schema file that you loaded in step 5 in the “To load an XML schema file” section.</span></span>|  
    |<span data-ttu-id="06359-141">**Новый номер XMLport**</span><span class="sxs-lookup"><span data-stu-id="06359-141">**New XMLport No.**</span></span>|<span data-ttu-id="06359-142">Укажите номер XMLport, созданного из схемы XML при выборе действия **Создать XMLport**.</span><span class="sxs-lookup"><span data-stu-id="06359-142">Specify the number of the XMLport that is created from this XML schema when you choose the **Generate XMLport** action.</span></span>|  

     <span data-ttu-id="06359-143">Строки заполняются узлами, представляющими все элементы в XML-схеме.</span><span class="sxs-lookup"><span data-stu-id="06359-143">The lines are now filled with nodes representing all elements in the XML schema.</span></span> <span data-ttu-id="06359-144">Узлы для элементов, которые являются обязательными согласно XML-схеме, выбираются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="06359-144">Nodes for elements that are mandatory according to the XML schema are selected by default.</span></span>  

3.  <span data-ttu-id="06359-145">В первой строке в столбце **Название узла** разверните узел **Документ** и постепенного разворачивайте дочерние узлы, которые необходимо просмотреть.</span><span class="sxs-lookup"><span data-stu-id="06359-145">On the first line, in the **Node Name** column, expand the **Document** node, and then gradually expand underlying nodes that you want to review.</span></span>  

     <span data-ttu-id="06359-146">В качестве альтернативы щелкните правой кнопкой мыши и выберите **Развернуть все**.</span><span class="sxs-lookup"><span data-stu-id="06359-146">Alternatively, right-click on a node and then choose **Expand All**.</span></span>  

4.  <span data-ttu-id="06359-147">Выберите одно из следующих действий, чтобы изменить узлы для отображения.</span><span class="sxs-lookup"><span data-stu-id="06359-147">Choose either of the following actions to change which nodes are displayed.</span></span>  

    |<span data-ttu-id="06359-148">**Действие**</span><span class="sxs-lookup"><span data-stu-id="06359-148">**Action**</span></span>|<span data-ttu-id="06359-149">Описание</span><span class="sxs-lookup"><span data-stu-id="06359-149">Description</span></span>|  
    |----------------|---------------------------------------|  
    |<span data-ttu-id="06359-150">**Показать все**</span><span class="sxs-lookup"><span data-stu-id="06359-150">**Show All**</span></span>|<span data-ttu-id="06359-151">Отображаются все узлы.</span><span class="sxs-lookup"><span data-stu-id="06359-151">All nodes are shown.</span></span>|  
    |<span data-ttu-id="06359-152">**Скрыть необязательные**</span><span class="sxs-lookup"><span data-stu-id="06359-152">**Hide Non-Mandatory**</span></span>|<span data-ttu-id="06359-153">Отображаются только узлы, представляющие элементы, необходимые согласно XML-схеме.</span><span class="sxs-lookup"><span data-stu-id="06359-153">Only nodes representing elements that are required according to the XML schema are shown.</span></span> <span data-ttu-id="06359-154">Обычно эти узлы обозначаются **1** в поле **MinOccurs**.</span><span class="sxs-lookup"><span data-stu-id="06359-154">These nodes are typically indicated by a **1** in the **MinOccurs** field.</span></span><br /><br /> <span data-ttu-id="06359-155">Щелкните **Показать все** для сторнирования представления.</span><span class="sxs-lookup"><span data-stu-id="06359-155">Choose **Show All** to reverse the view.</span></span>|  
    |<span data-ttu-id="06359-156">**Скрыть невыбранные**</span><span class="sxs-lookup"><span data-stu-id="06359-156">**Hide Non-Selected**</span></span>|<span data-ttu-id="06359-157">Отображаются только узлы, в которых установлен флажок **Выбрано**.</span><span class="sxs-lookup"><span data-stu-id="06359-157">Only nodes where the **Selected** check box is selected are shown.</span></span><br /><br /> <span data-ttu-id="06359-158">Щелкните **Показать все** для сторнирования представления.</span><span class="sxs-lookup"><span data-stu-id="06359-158">Choose **Show All** to reverse the view.</span></span>|  

5.  <span data-ttu-id="06359-159">Выберите действие **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="06359-159">Choose the **Edit** action.</span></span>  

6.  <span data-ttu-id="06359-160">С помощью флажка **Выбрано** можно для каждого узла указать, требуется ли включить поддержку элемента в определении обмена данными для связанного файла банка SEPA.</span><span class="sxs-lookup"><span data-stu-id="06359-160">In the **Selected** check box, specify for each node if you want the element to be supported in the data exchange definition for the related SEPA bank file.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="06359-161">При выборе обязательного дочернего узла все родительские узлы над ним также выбираются.</span><span class="sxs-lookup"><span data-stu-id="06359-161">When you select a mandatory child node, all parent nodes above it are also selected.</span></span>  

7.  <span data-ttu-id="06359-162">Выберите действие **Выбрать все обязательные элементы**, чтобы снова выбрать все узлы, представляющие элементы, которые являются обязательными согласно XML-схеме.</span><span class="sxs-lookup"><span data-stu-id="06359-162">Choose the **Select All Mandatory Elements** action to reselect all nodes that represent elements that are mandatory according to the XML schema.</span></span>  

8.  <span data-ttu-id="06359-163">Выберите действие **Снять выделение** для отмены выбора всех элементов.</span><span class="sxs-lookup"><span data-stu-id="06359-163">Choose the **Deselect All** action to clear all selections.</span></span>  

     <span data-ttu-id="06359-164">В поле **Выбор** указано, что у узла имеется два или более дочерних узла, которые функционируют как параметры.</span><span class="sxs-lookup"><span data-stu-id="06359-164">The **Choice** field specifies that the node has two or more sibling nodes that function as options.</span></span>  

### <a name="to-generate-a-data-exchange-definition-that-is-based-on-an-xml-schema"></a><span data-ttu-id="06359-165">Создание определения обмена данными на базе XML-схемы</span><span class="sxs-lookup"><span data-stu-id="06359-165">To generate a data exchange definition that is based on an XML schema</span></span>  

1.  <span data-ttu-id="06359-166">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Схемы XML**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="06359-166">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter  **XML Schemas**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="06359-167">Выберите соответствующую схему XML, затем выберите действие **Открыть средство просмотра XML-схем**.</span><span class="sxs-lookup"><span data-stu-id="06359-167">Select the relevant XML schema, and then choose the **Open XML Schema Viewer** action.</span></span>  

3.  <span data-ttu-id="06359-168">Убедитесь, что выбраны соответствующие узлы.</span><span class="sxs-lookup"><span data-stu-id="06359-168">Make sure the relevant nodes are selected.</span></span> <span data-ttu-id="06359-169">Дополнительные сведения см. в разделе "Выбор или отмена выбора узлов на XML-схеме".</span><span class="sxs-lookup"><span data-stu-id="06359-169">For more information, see the “To select or clear nodes in an XML schema” section.</span></span>  

4.  <span data-ttu-id="06359-170">На странице **Средство просмотра схем XML** выберите действие **Создать определение обмена данными**.</span><span class="sxs-lookup"><span data-stu-id="06359-170">On the **XML Schema Viewer** page, choose the **Generate Data Exchange Definition** action.</span></span>  

 <span data-ttu-id="06359-171">Запись определения обмена данными создается на странице **Определения учета обмена**, которую можно заполнить, указав, какие элементы файла сопоставляются с какими полями в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="06359-171">A data exchange definition is created on the **Posting Exchange Definition** page, which you can complete by specifying which elements in the file map to which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="06359-172">Дополнительные сведения см. в разделе [Настройка определений обмена данными](across-how-to-set-up-data-exchange-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="06359-172">For more information, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="06359-173">Можно также использовать функцию **Получить структуру файла** со страницы **Определения учета обмена**, использующую функциональные возможности страницы **Средство просмотра схем XML** для предварительного заполнения экспресс-вкладки **Определения столбца**.</span><span class="sxs-lookup"><span data-stu-id="06359-173">You can also use the **Get File Structure** function from the **Posting Exchange Definition** page, which uses the functionality of the **XML Schema Viewer** page to prefill the **Column Definitions** TastTab.</span></span>  

### <a name="to-generate-an-xmlport-that-is-based-on-an-xml-schema"></a><span data-ttu-id="06359-174">Создание XMLport на базе XML-схемы</span><span class="sxs-lookup"><span data-stu-id="06359-174">To generate an XMLport that is based on an XML schema</span></span>  

1.  <span data-ttu-id="06359-175">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Схемы XML**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="06359-175">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter  **XML Schemas**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="06359-176">Выберите соответствующую схему XML, затем выберите действие **Открыть средство просмотра XML-схем**.</span><span class="sxs-lookup"><span data-stu-id="06359-176">Select the relevant XML schema, and then choose the **Open XML Schema Viewer** action.</span></span>  

3.  <span data-ttu-id="06359-177">В поле **Новый номер XMLport**</span><span class="sxs-lookup"><span data-stu-id="06359-177">In the **New XMLport No.**</span></span> <span data-ttu-id="06359-178">укажите номер, который будет присвоен новому объекту XMLport при его создании.</span><span class="sxs-lookup"><span data-stu-id="06359-178">field, specify the number that the new XMLport object will be given when it is generated.</span></span>  

4.  <span data-ttu-id="06359-179">Убедитесь, что выбраны соответствующие узлы.</span><span class="sxs-lookup"><span data-stu-id="06359-179">Make sure the relevant nodes are selected.</span></span> <span data-ttu-id="06359-180">Дополнительные сведения см. в разделе "Выбор или отмена выбора узлов на XML-схеме".</span><span class="sxs-lookup"><span data-stu-id="06359-180">For more information, see the “To select or clear nodes in an XML schema” section.</span></span>  

5.  <span data-ttu-id="06359-181">Выберите действие **Создать XMLport** и сохраните объект как TXT-файл в соответствующем местоположении.</span><span class="sxs-lookup"><span data-stu-id="06359-181">Choose the **Generate XMLport** action, and then save the object as a .txt file in an appropriate location.</span></span>  

6. <span data-ttu-id="06359-182">Импортируйте новый XMLport в среду разработки [!INCLUDE[d365fin](includes/d365fin_md.md)] и скомпилируйте его.</span><span class="sxs-lookup"><span data-stu-id="06359-182">Import the new XMLport into the [!INCLUDE[d365fin](includes/d365fin_md.md)] development environment and compile it.</span></span>

## <a name="see-also"></a><span data-ttu-id="06359-183">См. также</span><span class="sxs-lookup"><span data-stu-id="06359-183">See Also</span></span>  
<span data-ttu-id="06359-184">[Настройка определений обмена данными](across-how-to-set-up-data-exchange-definitions.md) </span><span class="sxs-lookup"><span data-stu-id="06359-184">[Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md) </span></span>  
<span data-ttu-id="06359-185">[Экспорт платежей в банковский файл](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file) </span><span class="sxs-lookup"><span data-stu-id="06359-185">[Export Payments to a Bank File](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file) </span></span>  
<span data-ttu-id="06359-186">[Сбор платежей с прямым дебетом SEPA](finance-collect-payments-with-sepa-direct-debit.md) </span><span class="sxs-lookup"><span data-stu-id="06359-186">[Collect Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span></span>  
[<span data-ttu-id="06359-187">О структуре обмена данными</span><span class="sxs-lookup"><span data-stu-id="06359-187">About the Data Exchange Framework</span></span>](across-about-the-data-exchange-framework.md)
