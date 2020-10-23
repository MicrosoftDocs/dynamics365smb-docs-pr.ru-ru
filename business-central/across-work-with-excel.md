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
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: b25413c8f0479aaccfc67ae96f2870690f993dfa
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3927276"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a><span data-ttu-id="47004-103">Просмотр и редактирование в Excel из Business Central</span><span class="sxs-lookup"><span data-stu-id="47004-103">Viewing and Editing in Excel From Business Central</span></span>

<span data-ttu-id="47004-104">В случае страниц, на которых отображается список записей в строках и столбцах, например список клиентов, заказов на продажи или счетов, можно также просмотреть записи с помощью Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="47004-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span></span> <span data-ttu-id="47004-105">Для этого существует два варианта.</span><span class="sxs-lookup"><span data-stu-id="47004-105">To do this, you have two options.</span></span> <span data-ttu-id="47004-106">Можно выбрать действие **Открыть в Excel** или действие **Изменить в Excel** на странице.</span><span class="sxs-lookup"><span data-stu-id="47004-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span></span> <span data-ttu-id="47004-107">Различия между двумя действиями состоят в следующем:</span><span class="sxs-lookup"><span data-stu-id="47004-107">The differences between the two actions is as follows:</span></span>  

## <a name="open-in-excel"></a><span data-ttu-id="47004-108">Открыть в Excel</span><span class="sxs-lookup"><span data-stu-id="47004-108">Open in Excel</span></span>

- <span data-ttu-id="47004-109">С помощью этого действия Excel учитывает все фильтры на странице, которые ограничивают отображаемые записи.</span><span class="sxs-lookup"><span data-stu-id="47004-109">With this action, Excel respects any filters on the page that limit the records shown.</span></span> <span data-ttu-id="47004-110">Это означает, что книга Excel будет содержать те же строки и столбцы, которые отображаются на странице в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="47004-110">This means that the Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

- <span data-ttu-id="47004-111">Можно внести изменения в записи в Excel, но невозможно опубликовать изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="47004-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="47004-112">Можно только сохранить изменения в файл Microsoft Excel на компьютере.</span><span class="sxs-lookup"><span data-stu-id="47004-112">You can only save the changes to Excel file on your computer.</span></span>

- <span data-ttu-id="47004-113">Это действие работает как в Windows, так и в macOS.</span><span class="sxs-lookup"><span data-stu-id="47004-113">This action works on both on Windows and macOS.</span></span>

> [!NOTE]
> <span data-ttu-id="47004-114">Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Открыть в Excel** доступно по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="47004-114">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Open in Excel** action is available by default.</span></span> <span data-ttu-id="47004-115">Тем не менее, если вы настроили [!INCLUDE[prodshort](includes/prodshort.md)] On-premises для редактирования данных в Excel, то действие **Открыть в Excel** заменяется действием **Изменить в Excel**.</span><span class="sxs-lookup"><span data-stu-id="47004-115">However, if you set up [!INCLUDE[prodshort](includes/prodshort.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span></span>

## <a name="edit-in-excel"></a><span data-ttu-id="47004-116">Изменить в Excel</span><span class="sxs-lookup"><span data-stu-id="47004-116">Edit in Excel</span></span>

- <span data-ttu-id="47004-117">С помощью этого действия Excel учитывает большинство фильтров на странице, которые ограничивают отображаемые записи.</span><span class="sxs-lookup"><span data-stu-id="47004-117">With this action, Excel respects most filters on the page that limit the records shown.</span></span> <span data-ttu-id="47004-118">Это означает, что книга Excel будет содержать почти те же записи и столбцы.</span><span class="sxs-lookup"><span data-stu-id="47004-118">This means that the Excel workbook will contain almost the same records and columns.</span></span>

- <span data-ttu-id="47004-119">Преимущество действия **Изменить в Excel** заключается в том, что оно позволяет внести изменения в записи в Excel, затем опубликовать эти изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="47004-119">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

- <span data-ttu-id="47004-120">Оно работает только в Windows, но не в macOS.</span><span class="sxs-lookup"><span data-stu-id="47004-120">It only works on Windows; not macOS.</span></span>

- <span data-ttu-id="47004-121">Вы можете сменить компанию, с которой вы работаете.</span><span class="sxs-lookup"><span data-stu-id="47004-121">You can switch the company that your are working with.</span></span> <span data-ttu-id="47004-122">Для этого выберите значок **Параметры** ![Параметры надстроек Excel](media/cogwheel.png "Параметры надстроек Excel") на панели надстроек Excel, затем выберите компанию в поле **Компания**.</span><span class="sxs-lookup"><span data-stu-id="47004-122">To do this, select the **Options** icon ![Excel add-in options](media/cogwheel.png "Excel add-in options") in the Excel Add-in pane, then select the company from the **Company** field.</span></span>  

    > [!IMPORTANT]
    > <span data-ttu-id="47004-123">При смене компании убедитесь, что поле **Среда** не пустое.</span><span class="sxs-lookup"><span data-stu-id="47004-123">When changing the company, make sure that the **Environment** field is not empty.</span></span> <span data-ttu-id="47004-124">Если оно пустое, установите для него один из доступных параметров; в противном случае надстройка не будет работать правильно.</span><span class="sxs-lookup"><span data-stu-id="47004-124">If it is, then set it to one of the available options; otherwise, the add-in will not work correctly.</span></span>  

<span data-ttu-id="47004-125">Если вы вносите изменения в надстройку, вы должны перезагрузить ее, чтобы обновить подключение.</span><span class="sxs-lookup"><span data-stu-id="47004-125">If you make changes to the add-in, you must reload it in order to update the connection.</span></span> <span data-ttu-id="47004-126">Чтобы перезагрузить, используйте меню ![Меню надстроек Excel](media/excel-addin-menu.png "Меню надстроек Excel") в правом верхнем углу надстройки.</span><span class="sxs-lookup"><span data-stu-id="47004-126">To reload, use the ![Excel add-in menu](media/excel-addin-menu.png "Excel add-in menu") menu in the top-right corner of the add-in.</span></span>

> [!NOTE]
> <span data-ttu-id="47004-127">Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Изменить в Excel** доступно только в том случае, если ваш администратор настроил надстройку Excel, и доступна только для веб-клиента.</span><span class="sxs-lookup"><span data-stu-id="47004-127">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator, and only available for the Web client.</span></span> <span data-ttu-id="47004-128">Для администраторов порядок установки надстройки Excel приведен в разделе [Настройка надстройки Excel для редактирования данных Business Central](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="47004-128">For administrators, if you want to learn how to install the excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

### <a name="see-the-differences-between-the-options"></a><span data-ttu-id="47004-129">См. разницу между параметрами</span><span class="sxs-lookup"><span data-stu-id="47004-129">See the differences between the options</span></span>
<br><br>  

> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="47004-130">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="47004-130">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="47004-131">См. также</span><span class="sxs-lookup"><span data-stu-id="47004-131">See Also</span></span>

[<span data-ttu-id="47004-132">Анализ финансовых отчетов в Microsoft Excel</span><span class="sxs-lookup"><span data-stu-id="47004-132">Analyzing Financial Statements in Microsoft Excel</span></span>](finance-analyze-excel.md)  
[<span data-ttu-id="47004-133">Работа с Business Central</span><span class="sxs-lookup"><span data-stu-id="47004-133">Working with Business Central</span></span>](ui-work-product.md)  
[<span data-ttu-id="47004-134">Улучшения интеграции с Excel в волне 2 выпуска 2019 года</span><span class="sxs-lookup"><span data-stu-id="47004-134">Enhancements to Excel integration in 2019 release wave 2</span></span>](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration)  
