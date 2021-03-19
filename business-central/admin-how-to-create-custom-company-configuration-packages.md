---
title: Создание настраиваемых пакетов конфигурации организации | Документация Майкрософт
description: По мере роста бизнеса, вероятно, вам придется полагаться на набор типов организаций, используемых для большинства ваших клиентов. Процесс внедрения можно оптимизировать, превратив эти типы в пакеты настроек организации, которые можно использовать повторно.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: a1b1bfd5dd685eb57e291842d7b6d2e3691482fc
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5378302"
---
# <a name="create-custom-company-configuration-packages"></a><span data-ttu-id="64fbb-104">Создание настраиваемых пакетов конфигурации организации</span><span class="sxs-lookup"><span data-stu-id="64fbb-104">Create Custom Company Configuration Packages</span></span>
<span data-ttu-id="64fbb-105">По мере роста бизнеса, вероятно, вам придется полагаться на набор типов организаций, используемых для большинства ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="64fbb-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span></span> <span data-ttu-id="64fbb-106">Процесс внедрения можно оптимизировать, превратив эти типы в пакеты настроек организации, которые можно использовать повторно.</span><span class="sxs-lookup"><span data-stu-id="64fbb-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span></span>  

<span data-ttu-id="64fbb-107">В целом, создайте пакет конфигурации для функциональной области, например, создайте пакет для производственной функциональности.</span><span class="sxs-lookup"><span data-stu-id="64fbb-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span></span> <span data-ttu-id="64fbb-108">Это позволяет применять и настраивать новые области в организации по мере необходимости</span><span class="sxs-lookup"><span data-stu-id="64fbb-108">That lets you apply and set up new areas in a company as you need them</span></span>  

<span data-ttu-id="64fbb-109">Другой подход заключается в создании пакета, содержащего таблицы, которые определяют настройку, например следующие:</span><span class="sxs-lookup"><span data-stu-id="64fbb-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span></span>  

-   <span data-ttu-id="64fbb-110">Настройка модуля ОС</span><span class="sxs-lookup"><span data-stu-id="64fbb-110">Fixed Asset Setup</span></span>  
-   <span data-ttu-id="64fbb-111">Настройка ГК</span><span class="sxs-lookup"><span data-stu-id="64fbb-111">General Ledger Setup</span></span>  
-   <span data-ttu-id="64fbb-112">Товары Настройка</span><span class="sxs-lookup"><span data-stu-id="64fbb-112">Inventory Setup</span></span>  
-   <span data-ttu-id="64fbb-113">Настройка модуля "Производство"</span><span class="sxs-lookup"><span data-stu-id="64fbb-113">Manufacturing Setup</span></span>  
-   <span data-ttu-id="64fbb-114">Настройка модуля "Покупки и поставщики"</span><span class="sxs-lookup"><span data-stu-id="64fbb-114">Purchases and Payables Setup</span></span>  
-   <span data-ttu-id="64fbb-115">Настройка модуля "Маркетинг"</span><span class="sxs-lookup"><span data-stu-id="64fbb-115">Marketing Setup</span></span>  
-   <span data-ttu-id="64fbb-116">Настройка сервиса</span><span class="sxs-lookup"><span data-stu-id="64fbb-116">Service Setup</span></span>  
-   <span data-ttu-id="64fbb-117">Настройка Продаж и Расчетов с клиентами</span><span class="sxs-lookup"><span data-stu-id="64fbb-117">Sales and Receivables Setup</span></span>  
-   <span data-ttu-id="64fbb-118">Настройка модуля "Управление складом"</span><span class="sxs-lookup"><span data-stu-id="64fbb-118">Warehouse Setup</span></span>  
-   <span data-ttu-id="64fbb-119">Общая настройка учета</span><span class="sxs-lookup"><span data-stu-id="64fbb-119">General Posting Setup</span></span>  
-   <span data-ttu-id="64fbb-120">НДС настройка учета</span><span class="sxs-lookup"><span data-stu-id="64fbb-120">VAT Posting Setup</span></span>  
-   <span data-ttu-id="64fbb-121">Настройка учета запасов</span><span class="sxs-lookup"><span data-stu-id="64fbb-121">Inventory Posting Setup</span></span>  

<span data-ttu-id="64fbb-122">Для просмотра полного списка таблиц настройки выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Ручная настройка**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="64fbb-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manual Setup**, and then choose the related link.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="64fbb-123">Будьте осторожны, если вы выбираете таблицы или поля с одинаковым временным именем, но различаются специальными символами, такими как %, &, <, >, ( и ).</span><span class="sxs-lookup"><span data-stu-id="64fbb-123">Use caution if you choose tables or fields that have the same temporal name but are differentiated by special characters, such as %, &, <, >, (, and ).</span></span> <span data-ttu-id="64fbb-124">Например, таблица "XYZ" может содержать поля "Поле 1" и "Поле 1%".</span><span class="sxs-lookup"><span data-stu-id="64fbb-124">For example, table "XYZ" might contain the "Field 1" and "Field 1%" fields.</span></span>
>
> <span data-ttu-id="64fbb-125">Процессор XML принимает только некоторые специальные символы и удаляет те, которые не принимает.</span><span class="sxs-lookup"><span data-stu-id="64fbb-125">The XML processor accepts only some special characters, and will remove those it does not.</span></span> <span data-ttu-id="64fbb-126">Если удаление специального символа, такого как знак "%" в имени "Поле 1%", приводит к появлению двух или более таблиц или полей с одинаковыми именами, при экспорте или импорте пакета конфигурации произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="64fbb-126">If removing a special character, such as the % sign in "Field 1%," results in two or more tables or fields with the same name an error will occur when you export or import a configuration package.</span></span>

## <a name="to-create-a-custom-company-configuration-package"></a><span data-ttu-id="64fbb-127">Создание настраиваемых пакетов конфигурации организации</span><span class="sxs-lookup"><span data-stu-id="64fbb-127">To create a custom company configuration package</span></span>  
1.  <span data-ttu-id="64fbb-128">Создать новую компанию.</span><span class="sxs-lookup"><span data-stu-id="64fbb-128">Create a new company.</span></span> <span data-ttu-id="64fbb-129">Дополнительную информацию см. в разделе [Создание новой организации в Business Central](about-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="64fbb-129">For more information, see [Creating New Companies in Business Central](about-new-company.md).</span></span>  
3.  <span data-ttu-id="64fbb-130">Настройка новой организации в соответствии с требованиями.</span><span class="sxs-lookup"><span data-stu-id="64fbb-130">Set up the new company in the way you need.</span></span> <span data-ttu-id="64fbb-131">Заполните все необходимые таблицы настройки.</span><span class="sxs-lookup"><span data-stu-id="64fbb-131">Fill in all required setup tables.</span></span>  
4.  <span data-ttu-id="64fbb-132">Откройте новую организацию.</span><span class="sxs-lookup"><span data-stu-id="64fbb-132">Open the new company.</span></span>
5. <span data-ttu-id="64fbb-133">Откройте страницу **Журнал конфигураций**.</span><span class="sxs-lookup"><span data-stu-id="64fbb-133">Open the **Configuration Worksheet** page.</span></span>  
6.  <span data-ttu-id="64fbb-134">Добавьте таблицы, которые необходимо передать в журнал другой организации.</span><span class="sxs-lookup"><span data-stu-id="64fbb-134">Add the tables that you want to transfer to another company to the worksheet.</span></span> <span data-ttu-id="64fbb-135">Назначьте пакету строки журнала.</span><span class="sxs-lookup"><span data-stu-id="64fbb-135">Assign the worksheet lines to the package.</span></span>  
7.  <span data-ttu-id="64fbb-136">Создайте анкету для наиболее часто используемых таблиц настройки.</span><span class="sxs-lookup"><span data-stu-id="64fbb-136">Create a questionnaire for the most frequently used setup tables.</span></span>  
8.  <span data-ttu-id="64fbb-137">Создайте шаблоны конфигураций, чтобы упростить создание основных данных, таких как клиенты или товары.</span><span class="sxs-lookup"><span data-stu-id="64fbb-137">Create configuration templates to make it easier to create master data, such as customers or items.</span></span>  
9.  <span data-ttu-id="64fbb-138">Экспортируйте пакет в виде файла .rapidstart.</span><span class="sxs-lookup"><span data-stu-id="64fbb-138">Export your package as a .rapidstart file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="64fbb-139">См. также</span><span class="sxs-lookup"><span data-stu-id="64fbb-139">See Also</span></span>  
[<span data-ttu-id="64fbb-140">Настройка организации со службами RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="64fbb-140">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="64fbb-141">Администрация</span><span class="sxs-lookup"><span data-stu-id="64fbb-141">Administration</span></span>](admin-setup-and-administration.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]