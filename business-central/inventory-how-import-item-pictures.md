---
title: Импорт нескольких изображений товаров из ZIP-файла | Документация Майкрософт
description: Можно импортировать несколько изображений товаров за один раз. Просто присвойте файлам изображений имена, соответствующие номера ваших товаров, упакуйте из в ZIP-файл, затем с помощью страницы "Импорт изображений товаров" управляйте тем, какие изображения товаров следует импортировать.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: product, image
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 4d4221ca3af412cc2548634cc6920f58171233ce
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5785927"
---
# <a name="import-multiple-item-pictures"></a><span data-ttu-id="acf14-104">Импорт нескольких изображений товаров</span><span class="sxs-lookup"><span data-stu-id="acf14-104">Import Multiple Item Pictures</span></span>
<span data-ttu-id="acf14-105">Можно импортировать несколько изображений товаров за один раз.</span><span class="sxs-lookup"><span data-stu-id="acf14-105">You can import multiple item pictures in one go.</span></span> <span data-ttu-id="acf14-106">Просто присвойте файлам изображений имена, соответствующие номера ваших товаров, упакуйте из в ZIP-файл, затем с помощью страницы **Импорт изображений товаров** управляйте тем, какие изображения товаров следует импортировать.</span><span class="sxs-lookup"><span data-stu-id="acf14-106">Simply name your picture files with names corresponding to your item numbers, compress them to a ZIP file, and then use the **Import Item Pictures** page to manage which item pictures to import.</span></span>

<span data-ttu-id="acf14-107">Поддерживаются все распространенные форматы файлов.</span><span class="sxs-lookup"><span data-stu-id="acf14-107">All common file formats are supported.</span></span>

## <a name="to-name-picture-files-by-the-item-names-and-prepare-the-zip-file"></a><span data-ttu-id="acf14-108">Присвоение файлам изображений названий товаров и подготовка ZIP-файла</span><span class="sxs-lookup"><span data-stu-id="acf14-108">To name picture files by the item names and prepare the ZIP file</span></span>
1. <span data-ttu-id="acf14-109">В месте, в котором хранятся изображения товаров, назовите каждый файл в соответствии с номером связанного товара.</span><span class="sxs-lookup"><span data-stu-id="acf14-109">At the location where your item pictures are stored, name each files according to the number of the related item.</span></span> <span data-ttu-id="acf14-110">Например:</span><span class="sxs-lookup"><span data-stu-id="acf14-110">For example:</span></span>

    |<span data-ttu-id="acf14-111">Код товара</span><span class="sxs-lookup"><span data-stu-id="acf14-111">Item No.</span></span>|<span data-ttu-id="acf14-112">Имя файла</span><span class="sxs-lookup"><span data-stu-id="acf14-112">File Name</span></span>|
    |-|-|
    |<span data-ttu-id="acf14-113">1000</span><span class="sxs-lookup"><span data-stu-id="acf14-113">1000</span></span>|<span data-ttu-id="acf14-114">1000.bmp</span><span class="sxs-lookup"><span data-stu-id="acf14-114">1000.bmp</span></span>|
    |<span data-ttu-id="acf14-115">1001</span><span class="sxs-lookup"><span data-stu-id="acf14-115">1001</span></span>|<span data-ttu-id="acf14-116">1001.bmp</span><span class="sxs-lookup"><span data-stu-id="acf14-116">1001.bmp</span></span>|
    |<span data-ttu-id="acf14-117">1002</span><span class="sxs-lookup"><span data-stu-id="acf14-117">1002</span></span>|<span data-ttu-id="acf14-118">1002.bmp</span><span class="sxs-lookup"><span data-stu-id="acf14-118">1002.bmp</span></span>|

2. <span data-ttu-id="acf14-119">Соберите все файлы в ZIP-файл.</span><span class="sxs-lookup"><span data-stu-id="acf14-119">Collect all the files in a ZIP file.</span></span> <span data-ttu-id="acf14-120">Например, в Проводнике Windows выберите файлы, затем выберите **Отправить**, **Сжатая папка**.</span><span class="sxs-lookup"><span data-stu-id="acf14-120">For example, in Windows Explorer, select the files, and then choose **Send to**, **Compressed (zipped) folder**.</span></span>     

## <a name="to-import-item-pictures"></a><span data-ttu-id="acf14-121">Импорт изображений товаров</span><span class="sxs-lookup"><span data-stu-id="acf14-121">To import item pictures</span></span>
1. <span data-ttu-id="acf14-122">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Запасы"**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="acf14-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="acf14-123">Выберите действие **Импорт изображений товаров**.</span><span class="sxs-lookup"><span data-stu-id="acf14-123">Choose the **Import Item Pictures** action.</span></span>
3. <span data-ttu-id="acf14-124">В поле **Выбор ZIP-файла** выберите соответствующую ZIP-папку, затем нажмите кнопку **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="acf14-124">In the **Select a ZIP file** field, select the relevant ZIP folder, and then choose the **Open** button.</span></span>

    <span data-ttu-id="acf14-125">Строка для каждого товара и изображения создается на странице **Импорт изображений товаров**.</span><span class="sxs-lookup"><span data-stu-id="acf14-125">A line for each item and picture is created on the **Import Item Pictures** page.</span></span>

    > [!NOTE]
    > <span data-ttu-id="acf14-126">Для карточек товаров, на которых уже есть изображение, установлен флажок **Изображение уже существует**.</span><span class="sxs-lookup"><span data-stu-id="acf14-126">For item cards that already have a picture, the **Picture Already Exists** check box is selected.</span></span> <span data-ttu-id="acf14-127">Если вы не хотите заменять никакие существующие изображения, снимите флажок **Заменять изображения**.</span><span class="sxs-lookup"><span data-stu-id="acf14-127">If you do not want any existing pictures to be replaced, deselect the **Replace Pictures** check box.</span></span> <span data-ttu-id="acf14-128">Если не требуется заменять отдельные существующие изображения, удалите соответствующие строки.</span><span class="sxs-lookup"><span data-stu-id="acf14-128">If you do not want individual existing pictures to be replaced, delete the lines in question.</span></span>

3. <span data-ttu-id="acf14-129">Выберите действие **Импорт изображений**.</span><span class="sxs-lookup"><span data-stu-id="acf14-129">Choose the **Import Pictures** action.</span></span>

<span data-ttu-id="acf14-130">Поле **Статус импорта** обновляется для отображения того, был ли импорт изображения пропущен или завершен.</span><span class="sxs-lookup"><span data-stu-id="acf14-130">The **Import Status** field is updated to show if the picture import was skipped or completed.</span></span>       

## <a name="see-also"></a><span data-ttu-id="acf14-131">См. также</span><span class="sxs-lookup"><span data-stu-id="acf14-131">See Also</span></span>
[<span data-ttu-id="acf14-132">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="acf14-132">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="acf14-133">Создание серий номеров</span><span class="sxs-lookup"><span data-stu-id="acf14-133">Create Number Series</span></span>](ui-create-number-series.md)  
[<span data-ttu-id="acf14-134">Запасы</span><span class="sxs-lookup"><span data-stu-id="acf14-134">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="acf14-135">Покупки</span><span class="sxs-lookup"><span data-stu-id="acf14-135">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="acf14-136">Продажи</span><span class="sxs-lookup"><span data-stu-id="acf14-136">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="acf14-137">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="acf14-137">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]