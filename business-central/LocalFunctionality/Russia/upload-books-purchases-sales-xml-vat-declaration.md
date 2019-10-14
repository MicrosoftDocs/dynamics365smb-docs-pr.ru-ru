---
title: Загрузка книг покупок и продаж в России
description: Российские усовершенствования включают поддержку загрузки книг покупок и продаж и деклараций НДС в формате XML.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 4de4230e3537a2b5c242ca5c0e22caaf210b6aba
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301117"
---
# <a name="upload-books-of-purchases-and-sales-and-the-vat-declaration-in-xml-format"></a><span data-ttu-id="021de-103">Загрузка книг покупок и продаж и декларации НДС в формате XML</span><span class="sxs-lookup"><span data-stu-id="021de-103">Upload Books of Purchases and Sales and the VAT Declaration in XML Format</span></span>

<span data-ttu-id="021de-104">Чтобы загрузить отчеты по НДС в файлы XML, необходимо настроить папку, в которую будут загружаться файлы.</span><span class="sxs-lookup"><span data-stu-id="021de-104">To upload VAT reports to XML files, you must configure the folder where the files will be uploaded.</span></span>

<span data-ttu-id="021de-105">Выберите **Настройка регламентного отчета** и заполнит поля **Имя папки отчетов Excel** и **Имя папки для электронных файлов**.</span><span class="sxs-lookup"><span data-stu-id="021de-105">Go to **Statutory Report Setup** and fill **Excel Reports Folder Name** and **Electronic Files Folder Name**.</span></span>

## <a name="vat-declaration"></a><span data-ttu-id="021de-106">Декларация по НДС</span><span class="sxs-lookup"><span data-stu-id="021de-106">VAT Declaration</span></span>

<span data-ttu-id="021de-107">Файл декларации по НДС формируется на основе сгенерированных данных по книгам НДС покупок и продаж, дополнительным листам и журналу счетов.</span><span class="sxs-lookup"><span data-stu-id="021de-107">The VAT Declaration file is formed on the basis of the generated data on VAT Purchase Ledgers or VAT Sales Ledgers, additional sheets and the journal of invoices.</span></span>

<span data-ttu-id="021de-108">Для правильного формирования декларации по НДС необходимо:</span><span class="sxs-lookup"><span data-stu-id="021de-108">For the correct formation of the VAT Declaration is necessary:</span></span>

1. <span data-ttu-id="021de-109">Сформировать книги НДС покупок НДС или продаж, дополнительные листы за требуемый период (см. [Практическое руководство. Создание книг НДС](How-to-Create-VAT-Ledgers.md)).</span><span class="sxs-lookup"><span data-stu-id="021de-109">Generate VAT Purchase Ledgers or VAT Sales Ledgers, additional sheets for the required period (see [How to: Create VAT Ledgers](How-to-Create-VAT-Ledgers.md)).</span></span>

2. <span data-ttu-id="021de-110">При необходимости исправить данные в книгах НДС покупок или продаж.</span><span class="sxs-lookup"><span data-stu-id="021de-110">Correct the data of VAT Purchase Ledgers or VAT Sales Ledgers, if necessary.</span></span>

3. <span data-ttu-id="021de-111">Сформировать и проверить журналы счетов.</span><span class="sxs-lookup"><span data-stu-id="021de-111">Generate and check the journal of invoices.</span></span>

4. <span data-ttu-id="021de-112">Загрузить книги покупок и продаж, а также дополнительные листы в формате XML.</span><span class="sxs-lookup"><span data-stu-id="021de-112">Upload purchase and sales books, as well as additional sheets in XML format.</span></span>

5. <span data-ttu-id="021de-113">Загрузить журнал выставленных и полученных счетов (если есть операции за период) в формате XML.</span><span class="sxs-lookup"><span data-stu-id="021de-113">Upload the journal of issued and received invoices (if there are operations for the period) in XML format.</span></span>

6. <span data-ttu-id="021de-114">Создать декларацию по НДС в формате XML.</span><span class="sxs-lookup"><span data-stu-id="021de-114">Generate the VAT Declaration in XML format.</span></span>

7. <span data-ttu-id="021de-115">Сгенерированные файлы будут находиться в папке, указанной в разделе **Настройка регламентного отчета, Имя папки для электронных файлов**.</span><span class="sxs-lookup"><span data-stu-id="021de-115">The generated files will be located in the folder specified in the setting **Statutory Report Setup, Electronic Files Folder Name.**</span></span>

## <a name="upload-purchase-and-sales-books-and-additional-sheets-to-xml-files"></a><span data-ttu-id="021de-116">Загрузка книг покупок и продаж, а также дополнительных листов в файлы XML</span><span class="sxs-lookup"><span data-stu-id="021de-116">Upload purchase and sales books, and additional sheets to XML files</span></span>

<span data-ttu-id="021de-117">Чтобы загрузить книги НДС покупок или продаж в XML, вы должны выбрать строку с созданной книгой НДС, выбрать "Печать" и выбрать "Экспорт XML".</span><span class="sxs-lookup"><span data-stu-id="021de-117">To upload VAT Purchase Ledgers or VAT Sales Ledgers to XML, you need to stand on the line with the generated VAT Ledger, click Print, Export XML (to upload the book).</span></span>

<span data-ttu-id="021de-118">Система сгенерирует файл XML в папке, указанной в настройках, и заполнит поле "Имя файла XML" для книги.</span><span class="sxs-lookup"><span data-stu-id="021de-118">The system will generate an XML file in the folder specified in the settings and fill the Name of XML file field for the book.</span></span>

<span data-ttu-id="021de-119">Вы должны загружать дополнительные листы в XML, только если они не пусты.</span><span class="sxs-lookup"><span data-stu-id="021de-119">You should upload additional sheets to XML only if they are not empty.</span></span>

<span data-ttu-id="021de-120">Чтобы выгрузить дополнительные листы книг НДС покупок или продаж в формате XML, необходимо выбрать строку с созданной книгой НДС, выбрать "Печать", выбрать "Экспорт дополнительного листа XML" (для загрузки дополнительного листа в рабочую книгу в формате XML).</span><span class="sxs-lookup"><span data-stu-id="021de-120">For unloading of additional sheets of VAT Purchase Ledgers or VAT Sales Ledgers in the XML you need to stand on the line with the generated  VAT Ledger, click Print, Export additional sheet XML (for upload of additional sheet in the workbook in XML).</span></span>

<span data-ttu-id="021de-121">Система сгенерирует файл XML в папке, указанной в настройках, и заполнит поле "Имя файла XML" для дополнительного листа.</span><span class="sxs-lookup"><span data-stu-id="021de-121">The system will generate an XML file in the folder specified in the settings and fill the Name of XML file field for the additional sheet.</span></span>

## <a name="uploading-vat-declaration-to-xml"></a><span data-ttu-id="021de-122">Загрузка декларации по НДС в XML</span><span class="sxs-lookup"><span data-stu-id="021de-122">Uploading VAT Declaration to XML</span></span>

<span data-ttu-id="021de-123">Чтобы создать файл декларации, выберите **Подразделения -> Декларация по НДС -> Экспорт декларации по НДС в XML**:</span><span class="sxs-lookup"><span data-stu-id="021de-123">To generate a Declaration file, go to **Departments -> VAT Declaration -> Export VAT Declaration to XML**:</span></span>

<span data-ttu-id="021de-124">Чтобы рассчитать и загрузить файл, необходимо указать:</span><span class="sxs-lookup"><span data-stu-id="021de-124">To calculate and upload a file, you must specify:</span></span>

- <span data-ttu-id="021de-125">**Год**</span><span class="sxs-lookup"><span data-stu-id="021de-125">**Year**</span></span> 
- <span data-ttu-id="021de-126">**Тип периода** — Квартал, если декларация подается ежеквартально</span><span class="sxs-lookup"><span data-stu-id="021de-126">**Period type** – Quarter if the Declaration is submitted quarterly</span></span>
- <span data-ttu-id="021de-127">**Номер периода**</span><span class="sxs-lookup"><span data-stu-id="021de-127">**Period number**</span></span>

<span data-ttu-id="021de-128">В полях **НДС - книги покупок** и **НДС - книги продаж** вы должны выбрать сгенерированные книги покупок и продаж.</span><span class="sxs-lookup"><span data-stu-id="021de-128">In the **VAT purchase ledgers** and **VAT sales ledgers** fields, you must select the generated purchase and sales books.</span></span>

<span data-ttu-id="021de-129">Если книги не отображаются за выбранный период, вы можете очистить фильтр, и все книги будут доступны для выбора.</span><span class="sxs-lookup"><span data-stu-id="021de-129">If the books do not appear in the selected period, you can remove the filter and all the books will be available for selection.</span></span>

<span data-ttu-id="021de-130">Система автоматически заполняет данные об именах файлов XML для книг НДС покупок и продаж, а также для дополнительных листов, на основе ранее выгруженных файлов:</span><span class="sxs-lookup"><span data-stu-id="021de-130">The system automatically completes the data on the names of XML files for VAT Purchase Ledgers, VAT Sales Ledgers and additional sheets on the basis of previously unloaded files:</span></span>

- <span data-ttu-id="021de-131">Имя "НДС - книги покупок"</span><span class="sxs-lookup"><span data-stu-id="021de-131">XML Purchase Ledgers name</span></span>
- <span data-ttu-id="021de-132">Имя "НДС - книги продаж"</span><span class="sxs-lookup"><span data-stu-id="021de-132">XML Sales Ledgers name</span></span>
- <span data-ttu-id="021de-133">Имя дополнительного листа "НДС - книги продаж"</span><span class="sxs-lookup"><span data-stu-id="021de-133">XML Sales Ledgers additional sheet name</span></span>
- <span data-ttu-id="021de-134">Имя дополнительного листа "НДС - книги покупок"</span><span class="sxs-lookup"><span data-stu-id="021de-134">XML Purchase Ledgers additional sheet name</span></span>

<span data-ttu-id="021de-135">**Код места** — необходимо указать код местонахождения организации.</span><span class="sxs-lookup"><span data-stu-id="021de-135">**Place Code** – you must specify the location code of the organization.</span></span>

<span data-ttu-id="021de-136">**Код подписывающего лица** — выберите код сотрудника.</span><span class="sxs-lookup"><span data-stu-id="021de-136">**SignatoryNo** – choose the code of the employee.</span></span>

<span data-ttu-id="021de-137">**Код налогового органа** — укажите код налогового органа, куда подается декларация.</span><span class="sxs-lookup"><span data-stu-id="021de-137">**Tax Auth No** – specify the code of the tax authority where the Declaration is submitted.</span></span>

<span data-ttu-id="021de-138">Чтобы загрузить декларацию, нажмите кнопку ОК в правом нижнем углу формы.</span><span class="sxs-lookup"><span data-stu-id="021de-138">To upload the Declaration, click OK in the lower right corner of the form.</span></span>

<span data-ttu-id="021de-139">Сгенерированный файл будут находиться в папке, указанной в разделе **Настройка регламентного отчета, Имя папки для электронных файлов**.</span><span class="sxs-lookup"><span data-stu-id="021de-139">The generated file will be located in the folder specified in the configuration **Statutory Report Setup, Electronic Files Folder Name**.</span></span>

## <a name="see-also"></a><span data-ttu-id="021de-140">См. также</span><span class="sxs-lookup"><span data-stu-id="021de-140">See Also</span></span>

[<span data-ttu-id="021de-141">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="021de-141">Russia Local Functionality</span></span>](russia-local-functionality.md)  
