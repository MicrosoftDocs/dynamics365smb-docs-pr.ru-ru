---
title: "Связывание данных с Flow | Документы Майкрософт"
description: "Данные Financials можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания автоматического бизнес-процесса."
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 01/25/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: b4e2e7bc1c2622d329c73ae5bf47b4accff10aa8
ms.openlocfilehash: dde99e50c6984a7ec162b4047e8640e6affb3f25
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="using-included365finincludesd365finmdmd-in-an-automated-workflow"></a><span data-ttu-id="e638d-103">Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в автоматическом бизнес-процессе</span><span class="sxs-lookup"><span data-stu-id="e638d-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow</span></span>
<span data-ttu-id="e638d-104">Можно использовать данные [!INCLUDE[d365fin](includes/d365fin_md.md)] как часть рабочего процесса в Microsoft Flow.</span><span class="sxs-lookup"><span data-stu-id="e638d-104">You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="e638d-105">Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в Flow.</span><span class="sxs-lookup"><span data-stu-id="e638d-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.</span></span>  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-flow"></a><span data-ttu-id="e638d-106">Добавление [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных в Flow</span><span class="sxs-lookup"><span data-stu-id="e638d-106">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Flow</span></span>
1. <span data-ttu-id="e638d-107">В браузере перейдите к [flow.microsoft.com](https://flow.microsoft.com/en-us/) и выполните вход.</span><span class="sxs-lookup"><span data-stu-id="e638d-107">In your browser, navigate to [flow.microsoft.com](https://flow.microsoft.com/en-us/), and then sign in.</span></span>
2. <span data-ttu-id="e638d-108">Выберите **Мои Flow** в ленте вверху страницы.</span><span class="sxs-lookup"><span data-stu-id="e638d-108">Choose **My Flows** from the ribbon at the top of the page.</span></span>
3. <span data-ttu-id="e638d-109">В окне **Мои Flow** выберите параметр **Создать новый**.</span><span class="sxs-lookup"><span data-stu-id="e638d-109">In the **My Flows** window, choose the **Create from blank** option.</span></span>
4. <span data-ttu-id="e638d-110">Из списка доступных триггеров выберите один из доступных триггеров [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="e638d-110">From the list of available triggers, select one of the [!INCLUDE[d365fin](includes/d365fin_md.md)] triggers available:</span></span>  
    <span data-ttu-id="e638d-111">*Если запрашивается утверждение клиента*</span><span class="sxs-lookup"><span data-stu-id="e638d-111">*When a customer approval is requested*,</span></span>  
    <span data-ttu-id="e638d-112">*Если запрашивается утверждение раздела финансового журнала*</span><span class="sxs-lookup"><span data-stu-id="e638d-112">*When a general journal batch approval is requested*,</span></span>  
    <span data-ttu-id="e638d-113">*Если запрашивается утверждение строки финансового журнала*</span><span class="sxs-lookup"><span data-stu-id="e638d-113">*When a general journal line approval is requested*,</span></span>  
    <span data-ttu-id="e638d-114">*Если запрашивается утверждение товара*</span><span class="sxs-lookup"><span data-stu-id="e638d-114">*When an item approval is requested*,</span></span>  
    <span data-ttu-id="e638d-115">*Если запрашивается утверждение документа покупки*</span><span class="sxs-lookup"><span data-stu-id="e638d-115">*When a purchase document approval is requested*,</span></span>  
    <span data-ttu-id="e638d-116">*Если запрашивается утверждение документа продажи*, или</span><span class="sxs-lookup"><span data-stu-id="e638d-116">*When a sales document approval is requested*, or</span></span>  
    <span data-ttu-id="e638d-117">*Если запрашивается утверждение поставщика*</span><span class="sxs-lookup"><span data-stu-id="e638d-117">*When a vendor aproval is requested*.</span></span>
5. <span data-ttu-id="e638d-118">Поток предложит вам выбрать организацию с вашем арендаторе [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e638d-118">Flow will prompt you to select a company within your [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant.</span></span> <span data-ttu-id="e638d-119">Поскольку каждый этап во Flow не зависит от следующего, может потребоваться определить организацию несколько раз при использовании шаблона [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e638d-119">Because each step in the Flow is independent of the next, you may be required to define the company multiple times when using a [!INCLUDE[d365fin](includes/d365fin_md.md)] template.</span></span>

<span data-ttu-id="e638d-120">На этом шаге вы успешно подключились с данным Finance and Operations, Business edition и готовы начать создание потока.</span><span class="sxs-lookup"><span data-stu-id="e638d-120">At this point, you have successfully connected to your Finance and Operations, Business edition data and are ready to begin building your flow.</span></span> <span data-ttu-id="e638d-121">Дополнительные сведения см. в разделе [Документация Flow](https://flow.microsoft.com/documentation/getting-started/).</span><span class="sxs-lookup"><span data-stu-id="e638d-121">For more information, see the [Flow documentation](https://flow.microsoft.com/documentation/getting-started/).</span></span>

<span data-ttu-id="e638d-122">При устранении неполадок с Microsoft Flow см. раздел [Устранение неполадок при интеграции с Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="e638d-122">For troubleshooting your Microsoft Flow, see [Troubleshooting Integration with Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="e638d-123">См. также</span><span class="sxs-lookup"><span data-stu-id="e638d-123">See Also</span></span>
<span data-ttu-id="e638d-124">[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="e638d-124">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="e638d-125">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="e638d-125">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="e638d-126">[Управление пользователями и разрешениями](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="e638d-126">[Manage Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="e638d-127">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="e638d-127">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="e638d-128">Финансы</span><span class="sxs-lookup"><span data-stu-id="e638d-128">Finance</span></span>](finance.md)  

