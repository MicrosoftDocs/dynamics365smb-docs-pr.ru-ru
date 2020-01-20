---
title: Просмотр и редактирование в Excel из Business Central | Документация Майкрософт
description: Узнайте, как открывать страницы в Microsoft Excel из Business Central для более тщательного анализа данных.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 01/13/2020
ms.author: jswymer
ms.openlocfilehash: 9fd5c6c242932d75addcfa5c1811bdd1aff99a94
ms.sourcegitcommit: ead69ebe5b29927876a4fb23afb6c066f8854591
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2020
ms.locfileid: "2953055"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a><span data-ttu-id="4f151-103">Просмотр и редактирование в Excel из Business Central</span><span class="sxs-lookup"><span data-stu-id="4f151-103">Viewing and Editing in Excel From Business Central</span></span>

<span data-ttu-id="4f151-104">В случае страниц, на которых отображается список записей в строках и столбцах, например список клиентов, заказов на продажи или счетов, можно также просмотреть записи с помощью Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="4f151-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span></span> <span data-ttu-id="4f151-105">Для этого существует два варианта.</span><span class="sxs-lookup"><span data-stu-id="4f151-105">To do this, you have two options.</span></span> <span data-ttu-id="4f151-106">Можно выбрать действие **Открыть в Excel** или действие **Изменить в Excel** на странице.</span><span class="sxs-lookup"><span data-stu-id="4f151-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span></span> <span data-ttu-id="4f151-107">Различия между двумя действиями состоят в следующем:</span><span class="sxs-lookup"><span data-stu-id="4f151-107">The differences between the two actions is as follows:</span></span>  

## <a name="open-in-excel"></a><span data-ttu-id="4f151-108">Открыть в Excel</span><span class="sxs-lookup"><span data-stu-id="4f151-108">Open in Excel</span></span>

- <span data-ttu-id="4f151-109">С помощью этого действия Excel учитывает все фильтры на странице, которые ограничивают отображаемые записи.</span><span class="sxs-lookup"><span data-stu-id="4f151-109">With this action, Excel respects any filters on the page that limit the records shown.</span></span> <span data-ttu-id="4f151-110">Это означает, что книга Excel будет содержать те же строки и столбцы, которые отображаются на странице в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="4f151-110">This means that the Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

- <span data-ttu-id="4f151-111">Можно внести изменения в записи в Excel, но невозможно опубликовать изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="4f151-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="4f151-112">Можно только сохранить изменения в файл Microsoft Excel на компьютере.</span><span class="sxs-lookup"><span data-stu-id="4f151-112">You can only save the changes to Excel file on your computer.</span></span>

- <span data-ttu-id="4f151-113">Это действие работает как в Windows, так и в macOS.</span><span class="sxs-lookup"><span data-stu-id="4f151-113">This action works on both on Windows and macOS.</span></span>

> [!NOTE]
> <span data-ttu-id="4f151-114">Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Открыть в Excel** доступно по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4f151-114">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Open in Excel** action is available by default.</span></span> <span data-ttu-id="4f151-115">Тем не менее, если вы настроили [!INCLUDE [prodshort](includes/prodshort.md)] On-premises для редактирования данных в Excel, то действие **Открыть в Excel** заменяется действием **Изменить в Excel**.</span><span class="sxs-lookup"><span data-stu-id="4f151-115">However, if you set up [!INCLUDE [prodshort](includes/prodshort.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span></span>

## <a name="edit-in-excel"></a><span data-ttu-id="4f151-116">Изменить в Excel</span><span class="sxs-lookup"><span data-stu-id="4f151-116">Edit in Excel</span></span>

- <span data-ttu-id="4f151-117">С помощью этого действия Excel учитывает большинство фильтров на странице, которые ограничивают отображаемые записи.</span><span class="sxs-lookup"><span data-stu-id="4f151-117">With this action, Excel respects most filters on the page that limit the records shown.</span></span> <span data-ttu-id="4f151-118">Это означает, что книга Excel будет содержать почти те же записи и столбцы.</span><span class="sxs-lookup"><span data-stu-id="4f151-118">This means that the Excel workbook will contain almost the same records and columns.</span></span>

- <span data-ttu-id="4f151-119">Преимущество действия **Изменить в Excel** заключается в том, что оно позволяет внести изменения в записи в Excel, затем опубликовать эти изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="4f151-119">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

- <span data-ttu-id="4f151-120">Оно работает только в Windows, но не в macOS.</span><span class="sxs-lookup"><span data-stu-id="4f151-120">It only works on Windows; not macOS.</span></span>

<span data-ttu-id="4f151-121">Это было улучшено в выпуске 2019 года, волна 2.</span><span class="sxs-lookup"><span data-stu-id="4f151-121">This was enhanced in 2019 release wave 2.</span></span> <span data-ttu-id="4f151-122">Для получения дополнительной информации см. раздел [Улучшения интеграции с Excel](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration).</span><span class="sxs-lookup"><span data-stu-id="4f151-122">For more information, see [Enhancements to Excel integration](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration).</span></span>

> [!NOTE]
> <span data-ttu-id="4f151-123">Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Изменить в Excel** доступно только в том случае, если ваш администратор настроил надстройку Excel.</span><span class="sxs-lookup"><span data-stu-id="4f151-123">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator.</span></span> <span data-ttu-id="4f151-124">Для администраторов порядок установки надстройки Excel приведен в разделе [Настройка надстройки Excel для редактирования данных Business Central](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="4f151-124">For administrators, if you want to learn how to install the excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

> [!NOTE]
> <span data-ttu-id="4f151-125">Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises эта функция доступна только для веб-клиента.</span><span class="sxs-lookup"><span data-stu-id="4f151-125">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, this feature is only available for the Web client.</span></span>

### <a name="see-the-differences-between-the-options"></a><span data-ttu-id="4f151-126">См. разницу между параметрами</span><span class="sxs-lookup"><span data-stu-id="4f151-126">See the differences between the options</span></span>
<br><br>  

> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-related-training-at-microsoft-learnlearnmodulesconfigure-powerbi-excel-dynamics-365-business-centralindex"></a><span data-ttu-id="4f151-127">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="4f151-127">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="4f151-128">См. также</span><span class="sxs-lookup"><span data-stu-id="4f151-128">See Also</span></span>
[<span data-ttu-id="4f151-129">Работа с Business Central</span><span class="sxs-lookup"><span data-stu-id="4f151-129">Working with Business Central</span></span>](ui-work-product.md)  
