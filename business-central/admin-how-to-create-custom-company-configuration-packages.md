---
title: "Создание настраиваемых пакетов конфигурации организации | Документы Майкрософт"
description: "По мере роста бизнеса, вероятно, вам придется полагаться на набор типов организаций, используемых для большинства ваших клиентов. Процесс внедрения можно оптимизировать, превратив эти типы в пакеты настроек организации, которые можно использовать повторно."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: e26174fcf723e13ef5a9ed0b386006c0439e1c7a
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="create-custom-company-configuration-packages"></a><span data-ttu-id="17fc7-104">Создание настраиваемых пакетов конфигурации организации</span><span class="sxs-lookup"><span data-stu-id="17fc7-104">Create Custom Company Configuration Packages</span></span>
<span data-ttu-id="17fc7-105">По мере роста бизнеса, вероятно, вам придется полагаться на набор типов организаций, используемых для большинства ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="17fc7-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span></span> <span data-ttu-id="17fc7-106">Процесс внедрения можно оптимизировать, превратив эти типы в пакеты настроек организации, которые можно использовать повторно.</span><span class="sxs-lookup"><span data-stu-id="17fc7-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span></span>  

<span data-ttu-id="17fc7-107">В целом, создайте пакет конфигурации для функциональной области, например, создайте пакет для производственной функциональности.</span><span class="sxs-lookup"><span data-stu-id="17fc7-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span></span> <span data-ttu-id="17fc7-108">Это позволяет применять и настраивать новые области в организации по мере необходимости</span><span class="sxs-lookup"><span data-stu-id="17fc7-108">That lets you apply and set up new areas in a company as you need them</span></span>  

<span data-ttu-id="17fc7-109">Другой подход заключается в создании пакета, содержащего таблицы, которые определяют настройку, например следующие:</span><span class="sxs-lookup"><span data-stu-id="17fc7-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span></span>  

-   <span data-ttu-id="17fc7-110">Настройка модуля ОС</span><span class="sxs-lookup"><span data-stu-id="17fc7-110">Fixed Asset Setup</span></span>  
-   <span data-ttu-id="17fc7-111">Настройка ГК</span><span class="sxs-lookup"><span data-stu-id="17fc7-111">General Ledger Setup</span></span>  
-   <span data-ttu-id="17fc7-112">Товары Настройка</span><span class="sxs-lookup"><span data-stu-id="17fc7-112">Inventory Setup</span></span>  
-   <span data-ttu-id="17fc7-113">Настройка модуля "Производство"</span><span class="sxs-lookup"><span data-stu-id="17fc7-113">Manufacturing Setup</span></span>  
-   <span data-ttu-id="17fc7-114">Настройка модуля "Покупки и поставщики"</span><span class="sxs-lookup"><span data-stu-id="17fc7-114">Purchases and Payables Setup</span></span>  
-   <span data-ttu-id="17fc7-115">Настройка модуля "Маркетинг"</span><span class="sxs-lookup"><span data-stu-id="17fc7-115">Marketing Setup</span></span>  
-   <span data-ttu-id="17fc7-116">Настройка сервиса</span><span class="sxs-lookup"><span data-stu-id="17fc7-116">Service Setup</span></span>  
-   <span data-ttu-id="17fc7-117">Настройка Продаж и Расчетов с клиентами</span><span class="sxs-lookup"><span data-stu-id="17fc7-117">Sales and Receivables Setup</span></span>  
-   <span data-ttu-id="17fc7-118">Настройка модуля "Управление складом"</span><span class="sxs-lookup"><span data-stu-id="17fc7-118">Warehouse Setup</span></span>  
-   <span data-ttu-id="17fc7-119">Общая настройка учета</span><span class="sxs-lookup"><span data-stu-id="17fc7-119">General Posting Setup</span></span>  
-   <span data-ttu-id="17fc7-120">НДС настройка учета</span><span class="sxs-lookup"><span data-stu-id="17fc7-120">VAT Posting Setup</span></span>  
-   <span data-ttu-id="17fc7-121">Настройка учета запасов</span><span class="sxs-lookup"><span data-stu-id="17fc7-121">Inventory Posting Setup</span></span>  

<span data-ttu-id="17fc7-122">Для просмотра полного списка таблиц настройки выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="17fc7-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Setup**, and then choose the related link.</span></span>  

## <a name="to-create-a-custom-company-configuration-package"></a><span data-ttu-id="17fc7-123">Создание настраиваемых пакетов конфигурации организации</span><span class="sxs-lookup"><span data-stu-id="17fc7-123">To create a custom company configuration package</span></span>  
1.  <span data-ttu-id="17fc7-124">Откройте новый [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="17fc7-124">Create a new [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="17fc7-125">***НЕВОЗМОЖНО Ссылка на справку для "Создание нового арендатора"***.</span><span class="sxs-lookup"><span data-stu-id="17fc7-125">***NOT POSSIBLE Link to help for "Creating a New Tenant"***.</span></span>   
2.  <span data-ttu-id="17fc7-126">Создайте новую организацию для шаблона отрасли или решения.</span><span class="sxs-lookup"><span data-stu-id="17fc7-126">Create a new company for the industry or solution template.</span></span> <span data-ttu-id="17fc7-127">Дополнительные сведения см. в разделе [Создание организации](admin-how-to-create-a-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="17fc7-127">For more information, see [Create a New Company](admin-how-to-create-a-new-company.md).</span></span>  
3.  <span data-ttu-id="17fc7-128">Настройка новой организации в соответствии с требованиями.</span><span class="sxs-lookup"><span data-stu-id="17fc7-128">Setup the new company in the way you need.</span></span> <span data-ttu-id="17fc7-129">Заполните все необходимые таблицы настройки.</span><span class="sxs-lookup"><span data-stu-id="17fc7-129">Fill in all required setup tables.</span></span>  
4.  <span data-ttu-id="17fc7-130">Откройте новую организацию.</span><span class="sxs-lookup"><span data-stu-id="17fc7-130">Open the new company.</span></span>
5. <span data-ttu-id="17fc7-131">Откройте окно **Журнал конфигураций**.</span><span class="sxs-lookup"><span data-stu-id="17fc7-131">Open the **Configuration Worksheet** window.</span></span>  
6.  <span data-ttu-id="17fc7-132">Добавьте таблицы, которые необходимо передать в журнал другой организации.</span><span class="sxs-lookup"><span data-stu-id="17fc7-132">Add the tables that you want to transfer to another company to the worksheet.</span></span> <span data-ttu-id="17fc7-133">Назначьте пакету строки журнала.</span><span class="sxs-lookup"><span data-stu-id="17fc7-133">Assign the worksheet lines to the package.</span></span>  
7.  <span data-ttu-id="17fc7-134">Создайте анкету для наиболее часто используемых таблиц настройки.</span><span class="sxs-lookup"><span data-stu-id="17fc7-134">Create a questionnaire for the most frequently used setup tables.</span></span>  
8.  <span data-ttu-id="17fc7-135">Создайте шаблоны конфигураций, чтобы упростить создание основных данных, таких как клиенты или товары.</span><span class="sxs-lookup"><span data-stu-id="17fc7-135">Create configuration templates to make it easier to create master data, such as customers or items.</span></span>  
9.  <span data-ttu-id="17fc7-136">Экспортируйте пакет в виде файла .rapidstart.</span><span class="sxs-lookup"><span data-stu-id="17fc7-136">Export your package as a .rapidstart file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="17fc7-137">См. также</span><span class="sxs-lookup"><span data-stu-id="17fc7-137">See Also</span></span>  
[<span data-ttu-id="17fc7-138">Настройка компании с помощью служб RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="17fc7-138">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="17fc7-139">Администрация</span><span class="sxs-lookup"><span data-stu-id="17fc7-139">Administration</span></span>](admin-setup-and-administration.md)

