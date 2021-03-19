---
title: Просмотр и редактирование в Excel из Business Central
description: Узнайте, как открывать страницы в Microsoft Excel из Business Central для более тщательного анализа данных.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 11/06/2020
ms.author: jswymer
ms.openlocfilehash: 5e585d4bc7d9f7ce159671c10298f734fd5a09d5
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5378827"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a><span data-ttu-id="2218b-103">Просмотр и редактирование в Excel из Business Central</span><span class="sxs-lookup"><span data-stu-id="2218b-103">Viewing and Editing in Excel From Business Central</span></span>

<span data-ttu-id="2218b-104">В случае страниц, на которых отображается список записей в строках и столбцах, например список клиентов, заказов на продажи или счетов, можно также просмотреть записи с помощью Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="2218b-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span></span> <span data-ttu-id="2218b-105">Для этого существует два варианта.</span><span class="sxs-lookup"><span data-stu-id="2218b-105">To do this, you have two options.</span></span> <span data-ttu-id="2218b-106">Можно выбрать действие **Открыть в Excel** или действие **Изменить в Excel** на странице.</span><span class="sxs-lookup"><span data-stu-id="2218b-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span></span> <span data-ttu-id="2218b-107">Различия между двумя действиями состоят в следующем:</span><span class="sxs-lookup"><span data-stu-id="2218b-107">The differences between the two actions are as follows:</span></span>  

## <a name="open-in-excel"></a><span data-ttu-id="2218b-108">Открыть в Excel</span><span class="sxs-lookup"><span data-stu-id="2218b-108">Open in Excel</span></span>

- <span data-ttu-id="2218b-109">С помощью этого действия Excel учитывает все фильтры на странице, которые ограничивают отображаемые записи.</span><span class="sxs-lookup"><span data-stu-id="2218b-109">With this action, Excel respects any filters on the page that limit the records shown.</span></span> <span data-ttu-id="2218b-110">Книга Excel будет содержать те же строки и столбцы, которые отображаются на странице в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="2218b-110">The Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

- <span data-ttu-id="2218b-111">Можно внести изменения в записи в Excel, но невозможно опубликовать изменения обратно в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="2218b-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="2218b-112">Можно только сохранить изменения в файл Microsoft Excel на компьютере.</span><span class="sxs-lookup"><span data-stu-id="2218b-112">You can only save the changes to Excel file on your computer.</span></span>

- <span data-ttu-id="2218b-113">Это действие работает как в Windows, так и в macOS.</span><span class="sxs-lookup"><span data-stu-id="2218b-113">This action works on both on Windows and macOS.</span></span>

> [!NOTE]
> <span data-ttu-id="2218b-114">Для [!INCLUDE[prod_short](includes/prod_short.md)] On-premises действие **Открыть в Excel** доступно по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2218b-114">For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Open in Excel** action is available by default.</span></span> <span data-ttu-id="2218b-115">Тем не менее, если вы настроили [!INCLUDE[prod_short](includes/prod_short.md)] On-premises для редактирования данных в Excel, то действие **Открыть в Excel** заменяется действием **Изменить в Excel**.</span><span class="sxs-lookup"><span data-stu-id="2218b-115">However, if you set up [!INCLUDE[prod_short](includes/prod_short.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span></span>

## <a name="edit-in-excel"></a><span data-ttu-id="2218b-116">Изменить в Excel</span><span class="sxs-lookup"><span data-stu-id="2218b-116">Edit in Excel</span></span>

- <span data-ttu-id="2218b-117">Благодаря этому действию Excel учитывает большинство фильтров на странице, которые ограничивают отображаемые записи, поэтому книга Excel будет содержать почти те же записи и столбцы.</span><span class="sxs-lookup"><span data-stu-id="2218b-117">With this action, Excel respects most filters on the page that limit the records shown, so the Excel workbook will contain almost the same records and columns.</span></span>

- <span data-ttu-id="2218b-118">Преимущество действия **Изменить в Excel** заключается в том, что оно позволяет внести изменения в записи в Excel, затем опубликовать эти изменения обратно в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="2218b-118">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

- <span data-ttu-id="2218b-119">Оно работает только в Windows, но не в macOS.</span><span class="sxs-lookup"><span data-stu-id="2218b-119">It only works on Windows; not macOS.</span></span>

- <span data-ttu-id="2218b-120">Вы можете сменить компанию, с которой вы работаете.</span><span class="sxs-lookup"><span data-stu-id="2218b-120">You can switch the company that you are working with.</span></span> <span data-ttu-id="2218b-121">Для переключения компании выберите значок **Параметры** ![Параметры надстроек Excel](media/cogwheel.png "Параметры надстроек Excel") на панели надстроек Excel, затем выберите компанию в поле **Компания**.</span><span class="sxs-lookup"><span data-stu-id="2218b-121">To switch company, select the **Options** icon ![Excel add-in options](media/cogwheel.png "Excel add-in options") in the Excel Add-in pane, then select the company from the **Company** field.</span></span>  

    > [!IMPORTANT]
    > <span data-ttu-id="2218b-122">При смене компании убедитесь, что поле **Среда** не пустое.</span><span class="sxs-lookup"><span data-stu-id="2218b-122">When changing the company, make sure that the **Environment** field is not empty.</span></span> <span data-ttu-id="2218b-123">Если оно пустое, установите для него один из доступных параметров; в противном случае надстройка не будет работать правильно.</span><span class="sxs-lookup"><span data-stu-id="2218b-123">If it is, then set it to one of the available options; otherwise, the add-in will not work correctly.</span></span>  

<span data-ttu-id="2218b-124">Если вы вносите изменения в надстройку, вы должны перезагрузить ее, чтобы обновить подключение.</span><span class="sxs-lookup"><span data-stu-id="2218b-124">If you make changes to the add-in, you must reload it to update the connection.</span></span> <span data-ttu-id="2218b-125">Чтобы перезагрузить, используйте меню ![Меню надстроек Excel](media/excel-addin-menu.png "Меню надстроек Excel") в правом верхнем углу надстройки.</span><span class="sxs-lookup"><span data-stu-id="2218b-125">To reload, use the ![Excel add-in menu](media/excel-addin-menu.png "Excel add-in menu") menu in the top-right corner of the add-in.</span></span> <span data-ttu-id="2218b-126">Если вы не можете загрузить надстройку, обратитесь к администратору.</span><span class="sxs-lookup"><span data-stu-id="2218b-126">If you cannot load the add-in, talk to your administrator.</span></span> <span data-ttu-id="2218b-127">Если вы администратор, см. раздел [Настройка надстройки Excel для редактирования данных Business Central](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="2218b-127">If you are the administrator, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

> [!NOTE]
> <span data-ttu-id="2218b-128">Для [!INCLUDE[prod_short](includes/prod_short.md)] On-premises действие **Изменить в Excel** доступно только в том случае, если ваш администратор настроил надстройку Excel, и доступна только для веб-клиента.</span><span class="sxs-lookup"><span data-stu-id="2218b-128">For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator, and only available for the Web client.</span></span> <span data-ttu-id="2218b-129">Для администраторов порядок установки надстройки Excel приведен в разделе [Настройка надстройки Excel для редактирования данных Business Central](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="2218b-129">For administrators, if you want to learn how to install the Excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

### <a name="see-the-differences-between-the-options"></a><span data-ttu-id="2218b-130">См. разницу между параметрами</span><span class="sxs-lookup"><span data-stu-id="2218b-130">See the differences between the options</span></span>
<br><br>  

> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="2218b-131">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="2218b-131">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="2218b-132">См. также</span><span class="sxs-lookup"><span data-stu-id="2218b-132">See Also</span></span>

[<span data-ttu-id="2218b-133">Анализ финансовых отчетов в Microsoft Excel</span><span class="sxs-lookup"><span data-stu-id="2218b-133">Analyzing Financial Statements in Microsoft Excel</span></span>](finance-analyze-excel.md)  
[<span data-ttu-id="2218b-134">Работа с Business Central</span><span class="sxs-lookup"><span data-stu-id="2218b-134">Working with Business Central</span></span>](ui-work-product.md)  
[<span data-ttu-id="2218b-135">Улучшения интеграции с Excel в волне 2 выпуска 2019 года</span><span class="sxs-lookup"><span data-stu-id="2218b-135">Enhancements to Excel integration in 2019 release wave 2</span></span>](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration)  


[!INCLUDE[footer-include](includes/footer-banner.md)]