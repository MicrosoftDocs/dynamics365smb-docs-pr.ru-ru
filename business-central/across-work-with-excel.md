---
title: Просмотр и редактирование в Excel из Business Central | Документы Microsoft
description: Узнайте, как открывать страницы в Microsoft Excel из Business Central для более тщательного анализа данных.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 12/07/2018
ms.author: jswymer
ms.openlocfilehash: 27c137ea6309d40cddc94bc676ec7ea27d5c01fa
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "804458"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a><span data-ttu-id="00b5e-103">Просмотр и редактирование в Excel из Business Central</span><span class="sxs-lookup"><span data-stu-id="00b5e-103">Viewing and Editing in Excel From Business Central</span></span> 

<span data-ttu-id="00b5e-104">В случае страниц, на которых отображается список записей в строках и столбцах, например список клиентов, заказов на продажи или счетов, можно также просмотреть записи с помощью Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="00b5e-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span></span> <span data-ttu-id="00b5e-105">Для этого существует два варианта.</span><span class="sxs-lookup"><span data-stu-id="00b5e-105">To do this, you have two options.</span></span> <span data-ttu-id="00b5e-106">Можно выбрать действие **Открыть в Excel** или действие **Изменить в Excel** на странице.</span><span class="sxs-lookup"><span data-stu-id="00b5e-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span></span> <span data-ttu-id="00b5e-107">Различия между двумя действиями состоят в следующем:</span><span class="sxs-lookup"><span data-stu-id="00b5e-107">The differences between the two actions is as follows:</span></span>  

## <a name="open-in-excel"></a><span data-ttu-id="00b5e-108">Открыть в Excel</span><span class="sxs-lookup"><span data-stu-id="00b5e-108">Open in Excel</span></span>

-    <span data-ttu-id="00b5e-109">С помощью этого действия Excel учитывает все фильтры на странице для ограничения отображаемых записей.</span><span class="sxs-lookup"><span data-stu-id="00b5e-109">With this action, Excel respects any filters on the page the limit the records shown.</span></span> <span data-ttu-id="00b5e-110">Это означает, что книга Excel будет содержать те же строки и столбцы, которые отображаются на странице в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="00b5e-110">This means that the Excel workbook will contain the same rows and columns that appear on the the page in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

-    <span data-ttu-id="00b5e-111">Можно внести изменения в записи в Excel, но невозможно опубликовать изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="00b5e-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="00b5e-112">Можно только сохранить изменения в файл Microsoft Excel на компьютере.</span><span class="sxs-lookup"><span data-stu-id="00b5e-112">You can only save the changes to Excel file on your computer.</span></span> 

-    <span data-ttu-id="00b5e-113">Это действие работает как в Windows, так и в macOS.</span><span class="sxs-lookup"><span data-stu-id="00b5e-113">This action works on both on Windows and macOS.</span></span> 

>[!NOTE]
><span data-ttu-id="00b5e-114">Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Открыть в Excel** недоступно, если имеется действие **Изменить в Excel**.</span><span class="sxs-lookup"><span data-stu-id="00b5e-114">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Open in Excel** action is not available if the **Edit in Excel** action is.</span></span>

## <a name="edit-in-excel"></a><span data-ttu-id="00b5e-115">Изменить в Excel</span><span class="sxs-lookup"><span data-stu-id="00b5e-115">Edit in Excel</span></span>

-    <span data-ttu-id="00b5e-116">С помощью этого действия книга Excel не будет учитывать фильтры на странице для ограничения отображаемых записей.</span><span class="sxs-lookup"><span data-stu-id="00b5e-116">With this action, the Excel workbook does not respect filters on the page the limit the records shown.</span></span> <span data-ttu-id="00b5e-117">Это означает, что книга Excel будет содержать все доступные учетные записи и столбцы, независимо от того, что отображается на странице.</span><span class="sxs-lookup"><span data-stu-id="00b5e-117">This means that the Excel workbook will contain all the available records and columns, regardless of what is shown on the page.</span></span> 

-    <span data-ttu-id="00b5e-118">Преимущество действия **Изменить в Excel** заключается в том, что оно позволяет внести изменения в записи в Excel, затем опубликовать эти изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="00b5e-118">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

-    <span data-ttu-id="00b5e-119">Оно работает только в Windows, но не в macOS.</span><span class="sxs-lookup"><span data-stu-id="00b5e-119">It only works on Windows; not macOS.</span></span>

>[!NOTE]
><span data-ttu-id="00b5e-120">Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Изменить в Excel** доступно только в том случае, если ваш администратор установил надстройку Excel.</span><span class="sxs-lookup"><span data-stu-id="00b5e-120">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been installed by your administrator.</span></span> <span data-ttu-id="00b5e-121">Для администраторов порядок установки надстройки Excel приведен в разделе [Настройка надстройки Excel](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="00b5e-121">For administrators, if you want to learn how to install the excel add-in, see [Setting up the Excel Add-In](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

## <a name="see-also"></a><span data-ttu-id="00b5e-122">См. также</span><span class="sxs-lookup"><span data-stu-id="00b5e-122">See Also</span></span>

[<span data-ttu-id="00b5e-123">Работа с Business Central</span><span class="sxs-lookup"><span data-stu-id="00b5e-123">Working with Business Central</span></span>](ui-work-product.md)  
