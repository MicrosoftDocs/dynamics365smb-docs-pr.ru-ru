---
title: Импорт и экспорт макета отчета и документа | Документация Майкрософт
description: Можно импортировать и экспортировать существующий пользовательский макет отчета в виде файла в расположении на компьютере или в сети.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 01/13/2020
ms.author: sgroespe
ms.openlocfilehash: 8ec498030368aa2e6378068c88910b787c3632f8
ms.sourcegitcommit: ead69ebe5b29927876a4fb23afb6c066f8854591
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2020
ms.locfileid: "2954053"
---
# <a name="import-and-export-custom-report-layouts"></a><span data-ttu-id="1765b-103">Импорт и экспорт пользовательских макетов отчетов</span><span class="sxs-lookup"><span data-stu-id="1765b-103">Import and Export Custom Report Layouts</span></span>
<span data-ttu-id="1765b-104">Можно импортировать и экспортировать существующий пользовательский макет отчета в виде файла в расположении на компьютере или в сети.</span><span class="sxs-lookup"><span data-stu-id="1765b-104">You can import and export an existing custom report layout as a file to and from a location on your computer and network.</span></span> <span data-ttu-id="1765b-105">Например, можно экспортировать макет отчета, а затем отправить файл другому лицу для изменения.</span><span class="sxs-lookup"><span data-stu-id="1765b-105">For example, you can export a report layout, and then send the file to another person to modify.</span></span> <span data-ttu-id="1765b-106">Это лицо может затем внести изменения в макет и вернуть файл, чтобы вы могли импортировать его обратно.</span><span class="sxs-lookup"><span data-stu-id="1765b-106">That person can then make the modifications to layout and return the file to you so that you can import it back.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="1765b-107">Невозможно импортировать экспортировать встроенные макеты отчетов.</span><span class="sxs-lookup"><span data-stu-id="1765b-107">You cannot import or export built-in report layouts.</span></span>  

### <a name="to-export-a-report-layout-to-a-file"></a><span data-ttu-id="1765b-108">Экспорт макета отчета в файл</span><span class="sxs-lookup"><span data-stu-id="1765b-108">To export a report layout to a file</span></span>  

1.  <span data-ttu-id="1765b-109">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Выбор макета отчета**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1765b-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Layout Selection**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="1765b-110">Выберите строку отчета, которая содержит пользовательский макет отчета, который требуется экспортировать, затем выберите действие **Пользовательские макеты**.</span><span class="sxs-lookup"><span data-stu-id="1765b-110">Select the row for the report that contains the custom report layout that you want to export, and then choose the **Custom Layouts** action.</span></span>  

3.  <span data-ttu-id="1765b-111">На странице **Макеты отчета** выберите макет отчета, который требуется экспортировать в файл, затем выберите действие **Экспортировать макет**.</span><span class="sxs-lookup"><span data-stu-id="1765b-111">On the **Report Layouts** page, select the report layout that you want to export to a file, and then choose the **Export Layout** action.</span></span>  

4.  <span data-ttu-id="1765b-112">В диалоговом окне **Экспорт файла** выберите кнопку **Сохранить** и сохраните файл в расположение на компьютере или в сети.</span><span class="sxs-lookup"><span data-stu-id="1765b-112">In the **Export File** dialog box, choose the **Save** button, and then save the file to a location on your computer or network.</span></span>  

### <a name="to-import-a-report-layout-file"></a><span data-ttu-id="1765b-113">Импорт файла макета отчета</span><span class="sxs-lookup"><span data-stu-id="1765b-113">To import a report layout file</span></span>  

1.  <span data-ttu-id="1765b-114">Убедитесь, что соответствующий файл, определяющий макет отчета, доступен на компьютере или в сети.</span><span class="sxs-lookup"><span data-stu-id="1765b-114">Make sure that the relevant file that defines the report layout is available on your computer or network.</span></span>  

     <span data-ttu-id="1765b-115">Для макетов отчета Word файл должен иметь расширение DOCX.</span><span class="sxs-lookup"><span data-stu-id="1765b-115">A Word report layout file must have the .docx file type extension.</span></span> <span data-ttu-id="1765b-116">Для макетов отчета RDLC файл должен иметь расширение RDLC или RDL.</span><span class="sxs-lookup"><span data-stu-id="1765b-116">An RDLC report layout file must have the .rdlc or .rdl file type extension.</span></span>  

2.  <span data-ttu-id="1765b-117">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Выбор макета отчета**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1765b-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Layout Selection**, and then choose the related link.</span></span>  

3.  <span data-ttu-id="1765b-118">Выберите строку отчета, для которого требуется импортировать макет отчета, затем выберите действие **Пользовательские макеты**.</span><span class="sxs-lookup"><span data-stu-id="1765b-118">Select the row for the report to which you want to import the report layout, and then choose the **Custom Layouts** action.</span></span>  

4.  <span data-ttu-id="1765b-119">На странице **Макеты отчета** выберите макет отчета, в который требуется импортировать файл, затем выберите действие **Импортировать макет**.</span><span class="sxs-lookup"><span data-stu-id="1765b-119">On the **Report Layouts** page, select the report layout to which you want to import the file, and then choose the **Import Layout** action.</span></span>  

5.  <span data-ttu-id="1765b-120">В диалоговом окне **Импорт** выберите документ, определяющий макет отчета, и выберите кнопку **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="1765b-120">In the **Import** dialog box, select the document that defines the report layout, and then choose the **Open** button.</span></span>  

 <span data-ttu-id="1765b-121">Исходный пользовательский макет отчета заменяется на импортированный макет отчета.</span><span class="sxs-lookup"><span data-stu-id="1765b-121">The original custom report layout is replaced with the imported report layout.</span></span>  

## <a name="see-related-training-at-microsoft-learnlearnmoduleschange-documents-dynamics-365-business-centralindex"></a><span data-ttu-id="1765b-122">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/change-documents-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="1765b-122">See Related Training at [Microsoft Learn](/learn/modules/change-documents-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="1765b-123">См. также</span><span class="sxs-lookup"><span data-stu-id="1765b-123">See Also</span></span>  
 <span data-ttu-id="1765b-124">[Создание и изменение пользовательского макета отчета](ui-how-create-custom-report-layout.md) </span><span class="sxs-lookup"><span data-stu-id="1765b-124">[Create and Modify a Custom Report Layout](ui-how-create-custom-report-layout.md) </span></span>  
 [<span data-ttu-id="1765b-125">Управление макетами отчетов и документов</span><span class="sxs-lookup"><span data-stu-id="1765b-125">Managing Report and Document Layouts</span></span>](ui-manage-report-layouts.md)  
 [<span data-ttu-id="1765b-126">Работа с отчетами, пакетными заданиями и XMLport</span><span class="sxs-lookup"><span data-stu-id="1765b-126">Working with Reports, Batch Jobs, and XMLports</span></span>](ui-work-report.md)    
