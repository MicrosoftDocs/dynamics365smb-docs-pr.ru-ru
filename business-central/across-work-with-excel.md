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
ms.date: 10/24/2019
ms.author: jswymer
ms.openlocfilehash: 99fe339426b755b70983d8ec9345858357043347
ms.sourcegitcommit: 893e13fa75b2d04dedd4a29abda216e3e54b24ae
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "2808749"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a><span data-ttu-id="b710d-103">Просмотр и редактирование в Excel из Business Central</span><span class="sxs-lookup"><span data-stu-id="b710d-103">Viewing and Editing in Excel From Business Central</span></span>

<span data-ttu-id="b710d-104">В случае страниц, на которых отображается список записей в строках и столбцах, например список клиентов, заказов на продажи или счетов, можно также просмотреть записи с помощью Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="b710d-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span></span> <span data-ttu-id="b710d-105">Для этого существует два варианта.</span><span class="sxs-lookup"><span data-stu-id="b710d-105">To do this, you have two options.</span></span> <span data-ttu-id="b710d-106">Можно выбрать действие **Открыть в Excel** или действие **Изменить в Excel** на странице.</span><span class="sxs-lookup"><span data-stu-id="b710d-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span></span> <span data-ttu-id="b710d-107">Различия между двумя действиями состоят в следующем:</span><span class="sxs-lookup"><span data-stu-id="b710d-107">The differences between the two actions is as follows:</span></span>  

## <a name="open-in-excel"></a><span data-ttu-id="b710d-108">Открыть в Excel</span><span class="sxs-lookup"><span data-stu-id="b710d-108">Open in Excel</span></span>

- <span data-ttu-id="b710d-109">С помощью этого действия Excel учитывает все фильтры на странице, которые ограничивают отображаемые записи.</span><span class="sxs-lookup"><span data-stu-id="b710d-109">With this action, Excel respects any filters on the page that limit the records shown.</span></span> <span data-ttu-id="b710d-110">Это означает, что книга Excel будет содержать те же строки и столбцы, которые отображаются на странице в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="b710d-110">This means that the Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

- <span data-ttu-id="b710d-111">Можно внести изменения в записи в Excel, но невозможно опубликовать изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="b710d-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="b710d-112">Можно только сохранить изменения в файл Microsoft Excel на компьютере.</span><span class="sxs-lookup"><span data-stu-id="b710d-112">You can only save the changes to Excel file on your computer.</span></span> 

- <span data-ttu-id="b710d-113">Это действие работает как в Windows, так и в macOS.</span><span class="sxs-lookup"><span data-stu-id="b710d-113">This action works on both on Windows and macOS.</span></span> 

> [!NOTE]
> <span data-ttu-id="b710d-114">Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Открыть в Excel** доступно по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b710d-114">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Open in Excel** action is available by default.</span></span> <span data-ttu-id="b710d-115">Тем не менее, если вы настроили [!INCLUDE [prodshort](includes/prodshort.md)] On-premises для редактирования данных в Excel, то действие **Открыть в Excel** заменяется действием **Изменить в Excel**.</span><span class="sxs-lookup"><span data-stu-id="b710d-115">However, if you set up [!INCLUDE [prodshort](includes/prodshort.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span></span>

## <a name="edit-in-excel"></a><span data-ttu-id="b710d-116">Изменить в Excel</span><span class="sxs-lookup"><span data-stu-id="b710d-116">Edit in Excel</span></span>

- <span data-ttu-id="b710d-117">С помощью этого действия Excel учитывает большинство фильтров на странице, которые ограничивают отображаемые записи.</span><span class="sxs-lookup"><span data-stu-id="b710d-117">With this action, Excel respects most filters on the page that limit the records shown.</span></span> <span data-ttu-id="b710d-118">Это означает, что книга Excel будет содержать почти те же записи и столбцы.</span><span class="sxs-lookup"><span data-stu-id="b710d-118">This means that the Excel workbook will contain almost the same records and columns.</span></span>

- <span data-ttu-id="b710d-119">Преимущество действия **Изменить в Excel** заключается в том, что оно позволяет внести изменения в записи в Excel, затем опубликовать эти изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="b710d-119">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

- <span data-ttu-id="b710d-120">Оно работает только в Windows, но не в macOS.</span><span class="sxs-lookup"><span data-stu-id="b710d-120">It only works on Windows; not macOS.</span></span>

<span data-ttu-id="b710d-121">Это было улучшено в выпуске 2019 года, волна 2.</span><span class="sxs-lookup"><span data-stu-id="b710d-121">This was enhanced in 2019 release wave 2.</span></span> <span data-ttu-id="b710d-122">Для получения дополнительной информации см. раздел [Улучшения интеграции с Excel](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration).</span><span class="sxs-lookup"><span data-stu-id="b710d-122">For more information, see [Enhancements to Excel integration](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration).</span></span>

> [!NOTE]
> <span data-ttu-id="b710d-123">Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Изменить в Excel** доступно только в том случае, если ваш администратор настроил надстройку Excel.</span><span class="sxs-lookup"><span data-stu-id="b710d-123">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator.</span></span> <span data-ttu-id="b710d-124">Для администраторов порядок установки надстройки Excel приведен в разделе [Настройка надстройки Excel для редактирования данных Business Central](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="b710d-124">For administrators, if you want to learn how to install the excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

> [!NOTE]
> <span data-ttu-id="b710d-125">Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises эта функция доступна только для веб-клиента.</span><span class="sxs-lookup"><span data-stu-id="b710d-125">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, this feature is only available for the Web client.</span></span>

### <a name="see-the-differences-between-the-options"></a><span data-ttu-id="b710d-126">См. разницу между параметрами</span><span class="sxs-lookup"><span data-stu-id="b710d-126">See the differences between the options</span></span> 
<br><br>  

> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-also"></a><span data-ttu-id="b710d-127">См. также</span><span class="sxs-lookup"><span data-stu-id="b710d-127">See Also</span></span>
[<span data-ttu-id="b710d-128">Работа с Business Central</span><span class="sxs-lookup"><span data-stu-id="b710d-128">Working with Business Central</span></span>](ui-work-product.md)  
