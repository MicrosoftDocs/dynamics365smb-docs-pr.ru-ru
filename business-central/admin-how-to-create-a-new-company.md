---
title: Создание новой организации | Документация Майкрософт
description: Для использования служб RapidStart Services создаются таблицы и страницы, но они не содержат никаких данных.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 703b70a608bd6b25b9a3218eb59e8666fcd6a0ab
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5378327"
---
# <a name="create-a-new-company"></a><span data-ttu-id="27a18-103">Создание новой организации</span><span class="sxs-lookup"><span data-stu-id="27a18-103">Create a New Company</span></span>
<span data-ttu-id="27a18-104">Для использования служб RapidStart Services для [!INCLUDE[prod_short](includes/prod_short.md)] необходимо сначала создать новую организацию, для которой необходимо выполнить реализацию клиента.</span><span class="sxs-lookup"><span data-stu-id="27a18-104">To use RapidStart Services for [!INCLUDE[prod_short](includes/prod_short.md)], you first create a new company for which you want to perform a customer implementation.</span></span> <span data-ttu-id="27a18-105">При создании новой организации создаются стандартные таблицы и страницы [!INCLUDE[prod_short](includes/prod_short.md)], но без сведений.</span><span class="sxs-lookup"><span data-stu-id="27a18-105">When you create a new company, the standard [!INCLUDE[prod_short](includes/prod_short.md)] tables and pages are created, but there is no data in them.</span></span>

<span data-ttu-id="27a18-106">Кроме того, можно применить специфические данные настройки организации после ее инициализации.</span><span class="sxs-lookup"><span data-stu-id="27a18-106">In addition, you can apply specific setup data to your company after you initialize it.</span></span> <span data-ttu-id="27a18-107">Информация предоставляется в пакете конфигурации (файл с расширением RAPIDSTAR), который хранит данные в сжатом формате.</span><span class="sxs-lookup"><span data-stu-id="27a18-107">The information is provided in a configuration package, a .rapidstart file, which delivers content in a compressed format.</span></span>  

<span data-ttu-id="27a18-108">Примеры пакетов конфигурации, включая файлы для определенных стран и регионов, поставляются вместе с демонстрационной организацией CRONUS.</span><span class="sxs-lookup"><span data-stu-id="27a18-108">Example configuration packages, including country/region-specific files, are included with the CRONUS demonstration company.</span></span> <span data-ttu-id="27a18-109">Используйте следующую процедуру для использования примера пакета конфигураций в новой компании.</span><span class="sxs-lookup"><span data-stu-id="27a18-109">Use the following procedures to use the example configuration package with a new company.</span></span>  

## <a name="to-use-the-sample-basicconfig-configuration-package"></a><span data-ttu-id="27a18-110">Использование образца пакета конфигурации BASICCONFIG</span><span class="sxs-lookup"><span data-stu-id="27a18-110">To use the sample BASICCONFIG configuration package</span></span>  
1. <span data-ttu-id="27a18-111">Откройте демонстрационную организацию «CRONUS Россия ЗАО».</span><span class="sxs-lookup"><span data-stu-id="27a18-111">Open the CRONUS International Ltd. company.</span></span> <span data-ttu-id="27a18-112">Дополнительные сведения см. в разделе [Изменение базовых настроек](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="27a18-112">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span></span>
2. <span data-ttu-id="27a18-113">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Пакеты конфигураций**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="27a18-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Packages**, and then choose the related link.</span></span>  
3. <span data-ttu-id="27a18-114">Выберите пакет BASICCONFIG из списка и выберите действие **Экспортировать пакет**.</span><span class="sxs-lookup"><span data-stu-id="27a18-114">Choose the BASICCONFIG package from the list, and then choose the **Export Package** action.</span></span>  

<span data-ttu-id="27a18-115">Используйте следующую процедуру для создания новой организации и в процессе используйте пакет BASICCONFIG.</span><span class="sxs-lookup"><span data-stu-id="27a18-115">Use the following procedure to create a new company, and use the BASICCONFIG package as part of the process.</span></span>  

## <a name="to-create-a-new-company"></a><span data-ttu-id="27a18-116">Создание организации</span><span class="sxs-lookup"><span data-stu-id="27a18-116">To create a new company</span></span>  
1. <span data-ttu-id="27a18-117">Создать новую компанию.</span><span class="sxs-lookup"><span data-stu-id="27a18-117">Create a new company.</span></span> <span data-ttu-id="27a18-118">Дополнительную информацию см. в разделе [Создание новой организации в [!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="27a18-118">For more information, see [Creating New Companies in [!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md).</span></span>
2. <span data-ttu-id="27a18-119">Из ролевого центра «Внедряющий мастер служб RapidStart Services» теперь можно импортировать пакет конфигурации, который вы экспортировали из организации «CRONUS Россия ЗАО».</span><span class="sxs-lookup"><span data-stu-id="27a18-119">From the RapidStart Services Implementer Role Center, you can now import the configuration package that you exported from the CRONUS International Ltd. company.</span></span>

<span data-ttu-id="27a18-120">После создания новой организации некоторые таблицы заполняются автоматически, даже если не применен ни один шаблон организации.</span><span class="sxs-lookup"><span data-stu-id="27a18-120">After you create a new company, some tables are automatically filled in, even if no company template is applied.</span></span> <span data-ttu-id="27a18-121">Например, можно просмотреть стандартные коды для транзакций учета и пакетных транзакций на странице **Код источника**.</span><span class="sxs-lookup"><span data-stu-id="27a18-121">For example, you can review the standard codes for posting and batch transactions on the **Source Code** page.</span></span> <span data-ttu-id="27a18-122">Если нужно предоставить локальную версию [!INCLUDE[prod_short](includes/prod_short.md)], следует просмотреть эту таблицу и изучить вопросы, связанные с языками.</span><span class="sxs-lookup"><span data-stu-id="27a18-122">If you provide a local version of [!INCLUDE[prod_short](includes/prod_short.md)], you should review this table and consider any local language issues.</span></span>

## <a name="about-data-tables"></a><span data-ttu-id="27a18-123">О таблицах данных</span><span class="sxs-lookup"><span data-stu-id="27a18-123">About Data Tables</span></span>
<span data-ttu-id="27a18-124">Таблицы данных [!INCLUDE[prod_short](includes/prod_short.md)] доступны в двух основных видах: основная таблица и таблица настройки.</span><span class="sxs-lookup"><span data-stu-id="27a18-124">[!INCLUDE[prod_short](includes/prod_short.md)], data tables come in two basic types: Master and Setup.</span></span> <span data-ttu-id="27a18-125">При настойке конфигурации компании можно использовать эти типы, чтобы ориентироваться на стратегию конфигурации.</span><span class="sxs-lookup"><span data-stu-id="27a18-125">When you are setting up a company configuration, you can use these types to focus your configuration strategy.</span></span>  

### <a name="master-data-tables"></a><span data-ttu-id="27a18-126">Таблицы основных данных</span><span class="sxs-lookup"><span data-stu-id="27a18-126">Master Data Tables</span></span>  
<span data-ttu-id="27a18-127">В следующей таблице приведены некоторые из таблиц основных данных.</span><span class="sxs-lookup"><span data-stu-id="27a18-127">The following table lists some of the master data tables.</span></span> <span data-ttu-id="27a18-128">При инициализации новой организации эти таблицы будут пустыми.</span><span class="sxs-lookup"><span data-stu-id="27a18-128">When you initialize a new company, these tables are empty.</span></span>  

|<span data-ttu-id="27a18-129">Номер таблицы</span><span class="sxs-lookup"><span data-stu-id="27a18-129">Table No.</span></span>|<span data-ttu-id="27a18-130">Имя таблицы</span><span class="sxs-lookup"><span data-stu-id="27a18-130">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="27a18-131">15</span><span class="sxs-lookup"><span data-stu-id="27a18-131">15</span></span>|<span data-ttu-id="27a18-132">Счет ГК</span><span class="sxs-lookup"><span data-stu-id="27a18-132">G/L Account</span></span>|  
|<span data-ttu-id="27a18-133">18</span><span class="sxs-lookup"><span data-stu-id="27a18-133">18</span></span>|<span data-ttu-id="27a18-134">Клиент</span><span class="sxs-lookup"><span data-stu-id="27a18-134">Customer</span></span>|  
|<span data-ttu-id="27a18-135">23</span><span class="sxs-lookup"><span data-stu-id="27a18-135">23</span></span>|<span data-ttu-id="27a18-136">Поставщик</span><span class="sxs-lookup"><span data-stu-id="27a18-136">Vendor</span></span>|  
|<span data-ttu-id="27a18-137">27</span><span class="sxs-lookup"><span data-stu-id="27a18-137">27</span></span>|<span data-ttu-id="27a18-138">Пункт меню</span><span class="sxs-lookup"><span data-stu-id="27a18-138">Item</span></span>|  
|<span data-ttu-id="27a18-139">5050</span><span class="sxs-lookup"><span data-stu-id="27a18-139">5050</span></span>|<span data-ttu-id="27a18-140">Контакт</span><span class="sxs-lookup"><span data-stu-id="27a18-140">Contact</span></span>|  

### <a name="setup-data-tables"></a><span data-ttu-id="27a18-141">Настройка таблиц данных</span><span class="sxs-lookup"><span data-stu-id="27a18-141">Setup Data Tables</span></span>  
<span data-ttu-id="27a18-142">В следующей таблице перечислены некоторые из таблиц данных настройки, в которых фиксируются сведения о настройке в анкете конфигурации.</span><span class="sxs-lookup"><span data-stu-id="27a18-142">The following table lists some of the setup data tables, in which you capture setup information in the configuration questionnaire.</span></span> <span data-ttu-id="27a18-143">Эти таблицы содержат базовые данные, когда организация создается.</span><span class="sxs-lookup"><span data-stu-id="27a18-143">These tables contain baseline information when the company is created.</span></span>  

|<span data-ttu-id="27a18-144">Номер таблицы</span><span class="sxs-lookup"><span data-stu-id="27a18-144">Table No.</span></span>|<span data-ttu-id="27a18-145">Имя таблицы</span><span class="sxs-lookup"><span data-stu-id="27a18-145">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="27a18-146">98</span><span class="sxs-lookup"><span data-stu-id="27a18-146">98</span></span>|<span data-ttu-id="27a18-147">Настройка ГК</span><span class="sxs-lookup"><span data-stu-id="27a18-147">General Ledger Setup</span></span>|  
|<span data-ttu-id="27a18-148">311</span><span class="sxs-lookup"><span data-stu-id="27a18-148">311</span></span>|<span data-ttu-id="27a18-149">Настройка модуля "Продажи и дебитор. задолж."</span><span class="sxs-lookup"><span data-stu-id="27a18-149">Sales & Receivables Setup</span></span>|  
|<span data-ttu-id="27a18-150">312</span><span class="sxs-lookup"><span data-stu-id="27a18-150">312</span></span>|<span data-ttu-id="27a18-151">Настройка модуля "Покупки и кредиторская задолженность"</span><span class="sxs-lookup"><span data-stu-id="27a18-151">Purchases & Payables Setup</span></span>|  
|<span data-ttu-id="27a18-152">313</span><span class="sxs-lookup"><span data-stu-id="27a18-152">313</span></span>|<span data-ttu-id="27a18-153">Настройка модуля "Запасы"</span><span class="sxs-lookup"><span data-stu-id="27a18-153">Inventory Setup</span></span>|  

<span data-ttu-id="27a18-154">В дополнение к таблицам данных настроек [!INCLUDE[prod_short](includes/prod_short.md)] также имеет таблицы данных типа настройки, в которых указаны основные сведения об организации и ее бизнес-процессах.</span><span class="sxs-lookup"><span data-stu-id="27a18-154">In addition to setup data tables, [!INCLUDE[prod_short](includes/prod_short.md)] also has setup-type data tables that specify core information about the company and its business processes.</span></span> <span data-ttu-id="27a18-155">В следующей таблице перечислены некоторые из них.</span><span class="sxs-lookup"><span data-stu-id="27a18-155">The following table lists some of them.</span></span>  

|<span data-ttu-id="27a18-156">Номер таблицы</span><span class="sxs-lookup"><span data-stu-id="27a18-156">Table No.</span></span>|<span data-ttu-id="27a18-157">Имя таблицы</span><span class="sxs-lookup"><span data-stu-id="27a18-157">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="27a18-158">3</span><span class="sxs-lookup"><span data-stu-id="27a18-158">3</span></span>|<span data-ttu-id="27a18-159">Условия оплаты</span><span class="sxs-lookup"><span data-stu-id="27a18-159">Payment Terms</span></span>|  
|<span data-ttu-id="27a18-160">4</span><span class="sxs-lookup"><span data-stu-id="27a18-160">4</span></span>|<span data-ttu-id="27a18-161">Валюта</span><span class="sxs-lookup"><span data-stu-id="27a18-161">Currency</span></span>|  
|<span data-ttu-id="27a18-162">6</span><span class="sxs-lookup"><span data-stu-id="27a18-162">6</span></span>|<span data-ttu-id="27a18-163">Ценовые группы клиентов</span><span class="sxs-lookup"><span data-stu-id="27a18-163">Customer Price Groups</span></span>|  
|<span data-ttu-id="27a18-164">5700</span><span class="sxs-lookup"><span data-stu-id="27a18-164">5700</span></span>|<span data-ttu-id="27a18-165">Единица хранения</span><span class="sxs-lookup"><span data-stu-id="27a18-165">Stockkeeping Unit</span></span>|

  

## <a name="see-also"></a><span data-ttu-id="27a18-166">См. также</span><span class="sxs-lookup"><span data-stu-id="27a18-166">See Also</span></span>  
[<span data-ttu-id="27a18-167">Применение конфигураций к новым организациям</span><span class="sxs-lookup"><span data-stu-id="27a18-167">Apply Configurations to New Companies</span></span>](admin-apply-configuration-to-new-companies.md)  
[<span data-ttu-id="27a18-168">Настройка организации со службами RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="27a18-168">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="27a18-169">Администрация</span><span class="sxs-lookup"><span data-stu-id="27a18-169">Administration</span></span>](admin-setup-and-administration.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]