---
title: Создание настраиваемых пакетов конфигурации организации | Документация Майкрософт
description: По мере роста бизнеса, вероятно, вам придется полагаться на набор типов организаций, используемых для большинства ваших клиентов. Процесс внедрения можно оптимизировать, превратив эти типы в пакеты настроек организации, которые можно использовать повторно.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 99fad48961dc201a25af061cf982a1c65d9446bd
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2878869"
---
# <a name="create-custom-company-configuration-packages"></a><span data-ttu-id="a7bf3-104">Создание настраиваемых пакетов конфигурации организации</span><span class="sxs-lookup"><span data-stu-id="a7bf3-104">Create Custom Company Configuration Packages</span></span>
<span data-ttu-id="a7bf3-105">По мере роста бизнеса, вероятно, вам придется полагаться на набор типов организаций, используемых для большинства ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span></span> <span data-ttu-id="a7bf3-106">Процесс внедрения можно оптимизировать, превратив эти типы в пакеты настроек организации, которые можно использовать повторно.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span></span>  

<span data-ttu-id="a7bf3-107">В целом, создайте пакет конфигурации для функциональной области, например, создайте пакет для производственной функциональности.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span></span> <span data-ttu-id="a7bf3-108">Это позволяет применять и настраивать новые области в организации по мере необходимости</span><span class="sxs-lookup"><span data-stu-id="a7bf3-108">That lets you apply and set up new areas in a company as you need them</span></span>  

<span data-ttu-id="a7bf3-109">Другой подход заключается в создании пакета, содержащего таблицы, которые определяют настройку, например следующие:</span><span class="sxs-lookup"><span data-stu-id="a7bf3-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span></span>  

-   <span data-ttu-id="a7bf3-110">Настройка модуля ОС</span><span class="sxs-lookup"><span data-stu-id="a7bf3-110">Fixed Asset Setup</span></span>  
-   <span data-ttu-id="a7bf3-111">Настройка ГК</span><span class="sxs-lookup"><span data-stu-id="a7bf3-111">General Ledger Setup</span></span>  
-   <span data-ttu-id="a7bf3-112">Товары Настройка</span><span class="sxs-lookup"><span data-stu-id="a7bf3-112">Inventory Setup</span></span>  
-   <span data-ttu-id="a7bf3-113">Настройка модуля "Производство"</span><span class="sxs-lookup"><span data-stu-id="a7bf3-113">Manufacturing Setup</span></span>  
-   <span data-ttu-id="a7bf3-114">Настройка модуля "Покупки и поставщики"</span><span class="sxs-lookup"><span data-stu-id="a7bf3-114">Purchases and Payables Setup</span></span>  
-   <span data-ttu-id="a7bf3-115">Настройка модуля "Маркетинг"</span><span class="sxs-lookup"><span data-stu-id="a7bf3-115">Marketing Setup</span></span>  
-   <span data-ttu-id="a7bf3-116">Настройка сервиса</span><span class="sxs-lookup"><span data-stu-id="a7bf3-116">Service Setup</span></span>  
-   <span data-ttu-id="a7bf3-117">Настройка Продаж и Расчетов с клиентами</span><span class="sxs-lookup"><span data-stu-id="a7bf3-117">Sales and Receivables Setup</span></span>  
-   <span data-ttu-id="a7bf3-118">Настройка модуля "Управление складом"</span><span class="sxs-lookup"><span data-stu-id="a7bf3-118">Warehouse Setup</span></span>  
-   <span data-ttu-id="a7bf3-119">Общая настройка учета</span><span class="sxs-lookup"><span data-stu-id="a7bf3-119">General Posting Setup</span></span>  
-   <span data-ttu-id="a7bf3-120">НДС настройка учета</span><span class="sxs-lookup"><span data-stu-id="a7bf3-120">VAT Posting Setup</span></span>  
-   <span data-ttu-id="a7bf3-121">Настройка учета запасов</span><span class="sxs-lookup"><span data-stu-id="a7bf3-121">Inventory Posting Setup</span></span>  

<span data-ttu-id="a7bf3-122">Для просмотра полного списка таблиц настройки выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Ручная настройка**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manual Setup**, and then choose the related link.</span></span>  

## <a name="to-create-a-custom-company-configuration-package"></a><span data-ttu-id="a7bf3-123">Создание настраиваемых пакетов конфигурации организации</span><span class="sxs-lookup"><span data-stu-id="a7bf3-123">To create a custom company configuration package</span></span>  
1.  <span data-ttu-id="a7bf3-124">Создать новую компанию.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-124">Create a new company.</span></span> <span data-ttu-id="a7bf3-125">Дополнительную информацию см. в разделе [Создание новой организации в Business Central](about-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="a7bf3-125">For more information, see [Creating New Companies in Business Central](about-new-company.md).</span></span>  
3.  <span data-ttu-id="a7bf3-126">Настройка новой организации в соответствии с требованиями.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-126">Set up the new company in the way you need.</span></span> <span data-ttu-id="a7bf3-127">Заполните все необходимые таблицы настройки.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-127">Fill in all required setup tables.</span></span>  
4.  <span data-ttu-id="a7bf3-128">Откройте новую организацию.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-128">Open the new company.</span></span>
5. <span data-ttu-id="a7bf3-129">Откройте страницу **Журнал конфигураций**.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-129">Open the **Configuration Worksheet** page.</span></span>  
6.  <span data-ttu-id="a7bf3-130">Добавьте таблицы, которые необходимо передать в журнал другой организации.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-130">Add the tables that you want to transfer to another company to the worksheet.</span></span> <span data-ttu-id="a7bf3-131">Назначьте пакету строки журнала.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-131">Assign the worksheet lines to the package.</span></span>  
7.  <span data-ttu-id="a7bf3-132">Создайте анкету для наиболее часто используемых таблиц настройки.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-132">Create a questionnaire for the most frequently used setup tables.</span></span>  
8.  <span data-ttu-id="a7bf3-133">Создайте шаблоны конфигураций, чтобы упростить создание основных данных, таких как клиенты или товары.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-133">Create configuration templates to make it easier to create master data, such as customers or items.</span></span>  
9.  <span data-ttu-id="a7bf3-134">Экспортируйте пакет в виде файла .rapidstart.</span><span class="sxs-lookup"><span data-stu-id="a7bf3-134">Export your package as a .rapidstart file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a7bf3-135">См. также</span><span class="sxs-lookup"><span data-stu-id="a7bf3-135">See Also</span></span>  
[<span data-ttu-id="a7bf3-136">Настройка организации со службами RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="a7bf3-136">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="a7bf3-137">Администрация</span><span class="sxs-lookup"><span data-stu-id="a7bf3-137">Administration</span></span>](admin-setup-and-administration.md)
