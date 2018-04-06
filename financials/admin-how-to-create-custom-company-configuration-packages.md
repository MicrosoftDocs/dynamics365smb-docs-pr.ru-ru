---
title: "Создание настраиваемых пакетов конфигурации организации | Документы Майкрософт"
description: "По мере роста бизнеса, вероятно, вам придется полагаться на набор типов организаций, используемых для большинства ваших клиентов. Процесс внедрения можно оптимизировать, превратив эти типы в пакеты настроек организации, которые можно использовать повторно."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/05/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 37fe7a482b88626adff1ef16496a785399d19a8d
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="create-custom-company-configuration-packages"></a><span data-ttu-id="c3158-104">Создание настраиваемых пакетов конфигурации организации</span><span class="sxs-lookup"><span data-stu-id="c3158-104">Create Custom Company Configuration Packages</span></span>
<span data-ttu-id="c3158-105">По мере роста бизнеса, вероятно, вам придется полагаться на набор типов организаций, используемых для большинства ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="c3158-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span></span> <span data-ttu-id="c3158-106">Процесс внедрения можно оптимизировать, превратив эти типы в пакеты настроек организации, которые можно использовать повторно.</span><span class="sxs-lookup"><span data-stu-id="c3158-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span></span>  

<span data-ttu-id="c3158-107">В целом, создайте пакет конфигурации для функциональной области, например, создайте пакет для производственной функциональности.</span><span class="sxs-lookup"><span data-stu-id="c3158-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span></span> <span data-ttu-id="c3158-108">Это позволяет применять и настраивать новые области в организации по мере необходимости</span><span class="sxs-lookup"><span data-stu-id="c3158-108">That lets you apply and set up new areas in a company as you need them</span></span>  

<span data-ttu-id="c3158-109">Другой подход заключается в создании пакета, содержащего таблицы, которые определяют настройку, например следующие:</span><span class="sxs-lookup"><span data-stu-id="c3158-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span></span>  

-   <span data-ttu-id="c3158-110">Настройка модуля ОС</span><span class="sxs-lookup"><span data-stu-id="c3158-110">Fixed Asset Setup</span></span>  
-   <span data-ttu-id="c3158-111">Настройка ГК</span><span class="sxs-lookup"><span data-stu-id="c3158-111">General Ledger Setup</span></span>  
-   <span data-ttu-id="c3158-112">Товары Настройка</span><span class="sxs-lookup"><span data-stu-id="c3158-112">Inventory Setup</span></span>  
-   <span data-ttu-id="c3158-113">Настройка модуля "Производство"</span><span class="sxs-lookup"><span data-stu-id="c3158-113">Manufacturing Setup</span></span>  
-   <span data-ttu-id="c3158-114">Настройка модуля "Покупки и поставщики"</span><span class="sxs-lookup"><span data-stu-id="c3158-114">Purchases and Payables Setup</span></span>  
-   <span data-ttu-id="c3158-115">Настройка модуля "Маркетинг"</span><span class="sxs-lookup"><span data-stu-id="c3158-115">Marketing Setup</span></span>  
-   <span data-ttu-id="c3158-116">Настройка сервиса</span><span class="sxs-lookup"><span data-stu-id="c3158-116">Service Setup</span></span>  
-   <span data-ttu-id="c3158-117">Настройка Продаж и Расчетов с клиентами</span><span class="sxs-lookup"><span data-stu-id="c3158-117">Sales and Receivables Setup</span></span>  
-   <span data-ttu-id="c3158-118">Настройка модуля "Управление складом"</span><span class="sxs-lookup"><span data-stu-id="c3158-118">Warehouse Setup</span></span>  
-   <span data-ttu-id="c3158-119">Общая настройка учета</span><span class="sxs-lookup"><span data-stu-id="c3158-119">General Posting Setup</span></span>  
-   <span data-ttu-id="c3158-120">НДС настройка учета</span><span class="sxs-lookup"><span data-stu-id="c3158-120">VAT Posting Setup</span></span>  
-   <span data-ttu-id="c3158-121">Настройка учета запасов</span><span class="sxs-lookup"><span data-stu-id="c3158-121">Inventory Posting Setup</span></span>  

<span data-ttu-id="c3158-122">Для просмотра полного списка таблиц настройки выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Настройка**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="c3158-122">To see a complete list of setup tables, Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Setup**, and then choose the related link.</span></span>  

## <a name="to-create-a-custom-company-configuration-package"></a><span data-ttu-id="c3158-123">Создание настраиваемых пакетов конфигурации организации</span><span class="sxs-lookup"><span data-stu-id="c3158-123">To create a custom company configuration package</span></span>  
1.  <span data-ttu-id="c3158-124">Откройте новый [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="c3158-124">Create a new [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="c3158-125">***НЕВОЗМОЖНО Ссылка на справку для "Создание нового арендатора"***.</span><span class="sxs-lookup"><span data-stu-id="c3158-125">***NOT POSSIBLE Link to help for "Creating a New Tenant"***.</span></span>   
2.  <span data-ttu-id="c3158-126">Создайте новую организацию для шаблона отрасли или решения.</span><span class="sxs-lookup"><span data-stu-id="c3158-126">Create a new company for the industry or solution template.</span></span> <span data-ttu-id="c3158-127">Дополнительные сведения см. в разделе [Создание организации](admin-how-to-create-a-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="c3158-127">For more information, see [Create a New Company](admin-how-to-create-a-new-company.md).</span></span>  
3.  <span data-ttu-id="c3158-128">Настройка новой организации в соответствии с требованиями.</span><span class="sxs-lookup"><span data-stu-id="c3158-128">Setup the new company in the way you need.</span></span> <span data-ttu-id="c3158-129">Заполните все необходимые таблицы настройки.</span><span class="sxs-lookup"><span data-stu-id="c3158-129">Fill in all required setup tables.</span></span>  
4.  <span data-ttu-id="c3158-130">Откройте новую организацию.</span><span class="sxs-lookup"><span data-stu-id="c3158-130">Open the new company.</span></span>
5. <span data-ttu-id="c3158-131">Откройте окно **Журнал конфигураций**.</span><span class="sxs-lookup"><span data-stu-id="c3158-131">Open the **Configuration Worksheet** window.</span></span>  
6.  <span data-ttu-id="c3158-132">Добавьте таблицы, которые необходимо передать в журнал другой организации.</span><span class="sxs-lookup"><span data-stu-id="c3158-132">Add the tables that you want to transfer to another company to the worksheet.</span></span> <span data-ttu-id="c3158-133">Назначьте пакету строки журнала.</span><span class="sxs-lookup"><span data-stu-id="c3158-133">Assign the worksheet lines to the package.</span></span>  
7.  <span data-ttu-id="c3158-134">Создайте анкету для наиболее часто используемых таблиц настройки.</span><span class="sxs-lookup"><span data-stu-id="c3158-134">Create a questionnaire for the most frequently used setup tables.</span></span>  
8.  <span data-ttu-id="c3158-135">Создайте шаблоны конфигураций, чтобы упростить создание основных данных, таких как клиенты или товары.</span><span class="sxs-lookup"><span data-stu-id="c3158-135">Create configuration templates to make it easier to create master data, such as customers or items.</span></span>  
9.  <span data-ttu-id="c3158-136">Экспортируйте пакет в виде файла .rapidstart.</span><span class="sxs-lookup"><span data-stu-id="c3158-136">Export your package as a .rapidstart file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c3158-137">См. также</span><span class="sxs-lookup"><span data-stu-id="c3158-137">See Also</span></span>  
[<span data-ttu-id="c3158-138">Настройка компании с помощью служб RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="c3158-138">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="c3158-139">Администрация</span><span class="sxs-lookup"><span data-stu-id="c3158-139">Administration</span></span>](admin-setup-and-administration.md)

