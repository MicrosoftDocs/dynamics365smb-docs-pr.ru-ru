---
title: Использование Business Central в Power BI | Документация Майкрософт
description: Можно сделать данные доступными в качестве источника данных в Power BI и создать мощные отчеты о состоянии вашего бизнеса.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 4f140303f037ea4a914cba1ded44fd453bcdfabb
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3187896"
---
# <a name="using-prodlong-as-power-bi-data-source-for-building-reports"></a><span data-ttu-id="dce95-103">Использование [!INCLUDE [prodlong](includes/prodlong.md)] как источника данных Power BI для создания отчетов</span><span class="sxs-lookup"><span data-stu-id="dce95-103">Using [!INCLUDE [prodlong](includes/prodlong.md)] as Power BI Data Source for Building Reports</span></span>

<span data-ttu-id="dce95-104">Можно сделать данные [!INCLUDE[prodlong](includes/prodlong.md)] доступными в качестве источника данных в Power BI и создать мощные отчеты о состоянии вашего бизнеса.</span><span class="sxs-lookup"><span data-stu-id="dce95-104">You can make your [!INCLUDE[prodlong](includes/prodlong.md)] data available as a data source in Power BI and build powerful reports of the state of your business.</span></span>  

<span data-ttu-id="dce95-105">Вы должны иметь допустимую учетную запись в [!INCLUDE[prodshort](includes/prodshort.md)] и в Power BI.</span><span class="sxs-lookup"><span data-stu-id="dce95-105">You must have a valid account with [!INCLUDE[prodshort](includes/prodshort.md)] and with Power BI.</span></span> <span data-ttu-id="dce95-106">Также необходимо скачать [Power BI Desktop](https://powerbi.microsoft.com/desktop/).</span><span class="sxs-lookup"><span data-stu-id="dce95-106">You must also download [Power BI Desktop](https://powerbi.microsoft.com/desktop/).</span></span> <span data-ttu-id="dce95-107">Для получения дополнительной информации см. раздел [Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data),</span><span class="sxs-lookup"><span data-stu-id="dce95-107">For more information, see [Quickstart: Connect to data in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data).</span></span>  

## <a name="to-add-prodshort-as-a-data-source-in-power-bi-desktop"></a><span data-ttu-id="dce95-108">Добавление [!INCLUDE[prodshort](includes/prodshort.md)] как источника данных в Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="dce95-108">To add [!INCLUDE[prodshort](includes/prodshort.md)] as a data source in Power BI Desktop</span></span>

1. <span data-ttu-id="dce95-109">В Power BI Desktop в левой области навигации выберите **Получить данные**.</span><span class="sxs-lookup"><span data-stu-id="dce95-109">In Power BI Desktop, in the left navigation pane, choose **Get Data**.</span></span>
2. <span data-ttu-id="dce95-110">На странице **Получить данные** выберите **Веб-службы**, выберите **Microsoft Dynamics 365 Business Central**, затем нажмите кнопку **Подключиться**.</span><span class="sxs-lookup"><span data-stu-id="dce95-110">On the **Get Data** page, choose **Online Services**, choose **Microsoft Dynamics 365 Business Central**, and then choose the **Connect** button.</span></span>
3. <span data-ttu-id="dce95-111">Power BI отобразит мастер с руководством по процессу подключения, включая вход в [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="dce95-111">Power BI displays a wizard that will guide you through the connection process, including signing into [!INCLUDE [prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="dce95-112">Выберите **Войти**, затем выберите соответствующий учетную запись.</span><span class="sxs-lookup"><span data-stu-id="dce95-112">Choose **Sign in**, and then choose the relevant account.</span></span> <span data-ttu-id="dce95-113">Используйте ту же учетную запись, которая использовалась для входа в [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="dce95-113">Use the same account that you sign into [!INCLUDE [prodshort](includes/prodshort.md)] with.</span></span>
4. <span data-ttu-id="dce95-114">Нажмите кнопку **Подключиться**, чтобы продолжить.</span><span class="sxs-lookup"><span data-stu-id="dce95-114">Choose the **Connect** button to continue.</span></span> <span data-ttu-id="dce95-115">Мастер Power BI отобразит список сред, компаний и источников данных Microsoft [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="dce95-115">The Power BI wizard shows a list of Microsoft [!INCLUDE[d365fin](includes/d365fin_md.md)] environments, companies, and data sources.</span></span> <span data-ttu-id="dce95-116">Эти источники данных представляют все веб-службы, которые вы опубликовали из [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="dce95-116">These data sources represent all the web services that you have published from [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>

    <span data-ttu-id="dce95-117">Вместо этого можно также создать новый URL-адрес веб-службы в [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="dce95-117">You can also create a new web service URL in [!INCLUDE [prodshort](includes/prodshort.md)] instead.</span></span> <span data-ttu-id="dce95-118">Выберите одно из следующих методов:</span><span class="sxs-lookup"><span data-stu-id="dce95-118">Choose one of the following methods:</span></span>

      - <span data-ttu-id="dce95-119">Используйте действие **Создать набор данных** на странице **Веб-службы**</span><span class="sxs-lookup"><span data-stu-id="dce95-119">Use the **Create Data Set** action on the **Web Services** page</span></span>
      - <span data-ttu-id="dce95-120">Используйте мастер настройки **Настройка отчетности**</span><span class="sxs-lookup"><span data-stu-id="dce95-120">Use the **Set Up Reporting** Assisted Setup guide</span></span>
      - <span data-ttu-id="dce95-121">Выберите **Изменить в Excel** в любых списках</span><span class="sxs-lookup"><span data-stu-id="dce95-121">Choose the **Edit in Excel** action in any lists</span></span>

5. <span data-ttu-id="dce95-122">Укажите данные, которые требуется добавить в модель данных, а затем нажмите кнопку **Загрузить**.</span><span class="sxs-lookup"><span data-stu-id="dce95-122">Specify the data you want to add to your data model, and then choose the **Load** button.</span></span>
6. <span data-ttu-id="dce95-123">Повторите предыдущие шаги для добавления дополнительных данных [!INCLUDE [prodshort](includes/prodshort.md)] или других данных в модель данных Power BI.</span><span class="sxs-lookup"><span data-stu-id="dce95-123">Repeat the previous steps to add additional [!INCLUDE [prodshort](includes/prodshort.md)], or other data, to your Power BI data model.</span></span>

> [!NOTE]  
> <span data-ttu-id="dce95-124">После успешного подключения к [!INCLUDE [prodshort](includes/prodshort.md)] выполнять повторный вход не требуется.</span><span class="sxs-lookup"><span data-stu-id="dce95-124">Once you have successfully connected to [!INCLUDE [prodshort](includes/prodshort.md)], you will not be prompted again to sign in.</span></span>

<span data-ttu-id="dce95-125">После загрузки данных они отображаются в правой области навигации на странице.</span><span class="sxs-lookup"><span data-stu-id="dce95-125">Once the data is loaded, you can see it in the right navigation on the page.</span></span> <span data-ttu-id="dce95-126">Вы успешно подключились к данным [!INCLUDE [prodshort](includes/prodshort.md)] и можете начать создание отчета Power BI.</span><span class="sxs-lookup"><span data-stu-id="dce95-126">You have successfully connected to your [!INCLUDE [prodshort](includes/prodshort.md)] data, and you can begin building your Power BI report.</span></span>  

<span data-ttu-id="dce95-127">Перед построением отчета рекомендуется импортировать файлы темы [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="dce95-127">Before building your report, we recommend that you import the [!INCLUDE [prodshort](includes/prodshort.md)] theme file.</span></span>  <span data-ttu-id="dce95-128">Файл темы создаст цветовую палитру, чтобы можно было создавать отчеты с таким же цветовым стилем, что и приложения [!INCLUDE [prodshort](includes/prodshort.md)] без необходимости определения настраиваемых цветов для каждого визуального элемента.</span><span class="sxs-lookup"><span data-stu-id="dce95-128">The theme file will create a color palette so that you can build reports with the same color styling as the [!INCLUDE [prodshort](includes/prodshort.md)] apps without requiring you to define custom colors for each visual.</span></span>

<span data-ttu-id="dce95-129">Дополнительные сведения см. в разделе [Документация по Power BI](/power-bi/consumer/).</span><span class="sxs-lookup"><span data-stu-id="dce95-129">For more information, see the [Power BI documentation](/power-bi/consumer/).</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="dce95-130">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="dce95-130">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="dce95-131">См. также</span><span class="sxs-lookup"><span data-stu-id="dce95-131">See Also</span></span>

[<span data-ttu-id="dce95-132">Включение бизнес-данных для Power BI</span><span class="sxs-lookup"><span data-stu-id="dce95-132">Enabling Your Business Data for Power BI</span></span>](admin-powerbi.md)  
[<span data-ttu-id="dce95-133">Бизнес-аналитика</span><span class="sxs-lookup"><span data-stu-id="dce95-133">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="dce95-134">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="dce95-134">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="dce95-135">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="dce95-135">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="dce95-136">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="dce95-136">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="dce95-137">Финансы</span><span class="sxs-lookup"><span data-stu-id="dce95-137">Finance</span></span>](finance.md)  
[<span data-ttu-id="dce95-138">Быстрый старт: подключение к данным в Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="dce95-138">Quickstart: Connect to data in Power BI Desktop</span></span>](/power-bi/desktop-quickstart-connect-to-data)  
