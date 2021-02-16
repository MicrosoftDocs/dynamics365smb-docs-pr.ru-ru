---
title: Обзор компонентов интеграции и архитектуры Power BI для Business Central | Документация Майкрософт
description: Анализ данных, бизнес-аналитика и КПЭ на основе данных Business Central становятся проще благодаря приложениям Business Central для Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.reviewer: edupont
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: 23a0c72775dbddc89a81105de3b2ed79d1f09432
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4753774"
---
# <a name="power-bi-integration-component-and-architecture-overview-for-prod_short"></a><span data-ttu-id="f32b5-103">Обзор компонентов и архитектуры интеграции Power BI для [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="f32b5-103">Power BI Integration Component and Architecture Overview for [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>

<span data-ttu-id="f32b5-104">В этой статье вы узнаете о различных аспектах интеграции Power BI с [!INCLUDE[prod_short](includes/prod_short.md)], чтобы помочь вам разобраться в его реализации и использовании.</span><span class="sxs-lookup"><span data-stu-id="f32b5-104">In this article, you'll learn about the different aspects of Power BI integration with [!INCLUDE[prod_short](includes/prod_short.md)] to help you understand its implementation and use.</span></span>

## <a name="components"></a><span data-ttu-id="f32b5-105">Компоненты</span><span class="sxs-lookup"><span data-stu-id="f32b5-105">Components</span></span>

<span data-ttu-id="f32b5-106">В следующей таблице описаны основные компоненты, связанные с интеграцией Power BI.</span><span class="sxs-lookup"><span data-stu-id="f32b5-106">The following table describes the major components involved with Power BI integration.</span></span>

|<span data-ttu-id="f32b5-107">Компонент</span><span class="sxs-lookup"><span data-stu-id="f32b5-107">Component</span></span>|<span data-ttu-id="f32b5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f32b5-108">Description</span></span>|
|---------|-----------|
|<span data-ttu-id="f32b5-109">Power BI</span><span class="sxs-lookup"><span data-stu-id="f32b5-109">Power BI</span></span>|<span data-ttu-id="f32b5-110">Облачная служба размещения отчетов и управления ими.</span><span class="sxs-lookup"><span data-stu-id="f32b5-110">A cloud-based report hosting and management service.</span></span>|
|<span data-ttu-id="f32b5-111">Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="f32b5-111">Power BI Desktop</span></span>|<span data-ttu-id="f32b5-112">Инструмент разработки для создания отчетов и панелей мониторинга, позволяющий запускать отчеты.</span><span class="sxs-lookup"><span data-stu-id="f32b5-112">An authoring tool for building reports and dashboards, and allows you to run reports.</span></span> <span data-ttu-id="f32b5-113">Он доступен для бесплатной загрузки в Microsoft Store и устанавливается локально.</span><span class="sxs-lookup"><span data-stu-id="f32b5-113">It's available as a free download on Microsoft Store and is installed locally.</span></span>|
|[!INCLUDE[prod_short](includes/prod_short.md)]|<span data-ttu-id="f32b5-114">Сетевое или локальное решение с соединителями, доступными для Power BI, и возможностью внедрить часть Power BI.</span><span class="sxs-lookup"><span data-stu-id="f32b5-114">Online or on-premises solution with connectors exposed to Power BI and the ability to embed a Power BI part.</span></span>|

## <a name="whats-available-from-the-start"></a><span data-ttu-id="f32b5-115">Что доступно с самого начала</span><span class="sxs-lookup"><span data-stu-id="f32b5-115">What's available from the start</span></span>

<span data-ttu-id="f32b5-116">В следующей таблице описаны доступные функции.</span><span class="sxs-lookup"><span data-stu-id="f32b5-116">The following table describes available features.</span></span>

|<span data-ttu-id="f32b5-117">Функция</span><span class="sxs-lookup"><span data-stu-id="f32b5-117">Feature</span></span>|<span data-ttu-id="f32b5-118">Поддержка [!INCLUDE[prod_short](includes/prod_short.md)] Online или On-Premises</span><span class="sxs-lookup"><span data-stu-id="f32b5-118">[!INCLUDE[prod_short](includes/prod_short.md)] online or on-premises support</span></span>|
|-------|---------------------|
|<span data-ttu-id="f32b5-119">Соединители Power BI</span><span class="sxs-lookup"><span data-stu-id="f32b5-119">Power BI connectors</span></span>|<span data-ttu-id="f32b5-120">Оба.</span><span class="sxs-lookup"><span data-stu-id="f32b5-120">Both.</span></span> <span data-ttu-id="f32b5-121">Различные соединители для версий Online и On-Premises.</span><span class="sxs-lookup"><span data-stu-id="f32b5-121">Different connectors for online and on-premises.</span></span> <span data-ttu-id="f32b5-122">Один и тот же разъем используется для Power BI Desktop и службы Power BI</span><span class="sxs-lookup"><span data-stu-id="f32b5-122">Same connector used for Power BI Desktop and Power BI Service</span></span> |
|<span data-ttu-id="f32b5-123">Встроенный интерфейс для просмотра заданного отчета внутри информационной панели в [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="f32b5-123">Embedded experience for viewing a given report inside a FactBox in [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>|<span data-ttu-id="f32b5-124">Оба.</span><span class="sxs-lookup"><span data-stu-id="f32b5-124">Both.</span></span> <span data-ttu-id="f32b5-125">Требуется конфигурация для отображения отчетов в локальной среде.</span><span class="sxs-lookup"><span data-stu-id="f32b5-125">Requires configuration to display reports for on-premises.</span></span>|
|<span data-ttu-id="f32b5-126">Управление отчетами Power BI из [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="f32b5-126">Power BI report management from [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>|<span data-ttu-id="f32b5-127">Online</span><span class="sxs-lookup"><span data-stu-id="f32b5-127">Online</span></span>|
|<span data-ttu-id="f32b5-128">Отчеты Power BI по умолчанию в ролевых центрах, развернутых в Power BI</span><span class="sxs-lookup"><span data-stu-id="f32b5-128">Default Power BI reports on role centers deployed to Power BI</span></span>|<span data-ttu-id="f32b5-129">Online</span><span class="sxs-lookup"><span data-stu-id="f32b5-129">Online</span></span>|
|<span data-ttu-id="f32b5-130">Приложения Power BI в Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="f32b5-130">Power BI Apps on Microsoft AppSource</span></span>|<span data-ttu-id="f32b5-131">Online.</span><span class="sxs-lookup"><span data-stu-id="f32b5-131">Online.</span></span>|

## <a name="architecture"></a><span data-ttu-id="f32b5-132">Архитектура</span><span class="sxs-lookup"><span data-stu-id="f32b5-132">Architecture</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="f32b5-133">интегрируется с Power BI через соединитель с использованием OData.</span><span class="sxs-lookup"><span data-stu-id="f32b5-133">integrates with Power BI through a connector using OData.</span></span> <span data-ttu-id="f32b5-134">Источник данных для отчетов Power BI представляется как веб-служба OData.</span><span class="sxs-lookup"><span data-stu-id="f32b5-134">The data source for Power BI reports is exposed as OData web services.</span></span>

![Архитектура Power BI для интеграции с Business Central](./media/power-bi-architecture.png)

## <a name="general-flow"></a><span data-ttu-id="f32b5-136">Общий поток</span><span class="sxs-lookup"><span data-stu-id="f32b5-136">General Flow</span></span>

<span data-ttu-id="f32b5-137">На следующей диаграмме показан основной рабочий процесс для пользователей при подключении [!INCLUDE[prod_short](includes/prod_short.md)] к Power BI.</span><span class="sxs-lookup"><span data-stu-id="f32b5-137">The following diagram illustrates the basic workflow for users when connecting [!INCLUDE[prod_short](includes/prod_short.md)] to Power BI.</span></span>

![Рабочий поток Power BI для интеграции с Business Central](./media/power-bi-flow.png)

1. <span data-ttu-id="f32b5-139">Пользователь регистрируется на учетную запись Power BI.</span><span class="sxs-lookup"><span data-stu-id="f32b5-139">User signs up for a Power BI account.</span></span>
2. <span data-ttu-id="f32b5-140">Пользователь подключается к Power BI из [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="f32b5-140">User connects to Power BI from [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>
3. [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="f32b5-141">проверяет лицензию.</span><span class="sxs-lookup"><span data-stu-id="f32b5-141">verifies the license.</span></span>
4. [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="f32b5-142">развертывает отчеты по умолчанию в службе Power BI.</span><span class="sxs-lookup"><span data-stu-id="f32b5-142">deploys default reports to the Power BI service.</span></span> <span data-ttu-id="f32b5-143">Этот шаг выполняется только для [!INCLUDE[prod_short](includes/prod_short.md)] Online.</span><span class="sxs-lookup"><span data-stu-id="f32b5-143">This step only happens for [!INCLUDE[prod_short](includes/prod_short.md)] online.</span></span>
5. [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="f32b5-144">делает отчеты в Power BI доступными для выбора в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="f32b5-144">makes reports in Power BI available for selection in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="f32b5-145">Отчеты по умолчанию автоматически отображаются в частях Power BI.</span><span class="sxs-lookup"><span data-stu-id="f32b5-145">Default reports are automatically displayed in Power BI parts.</span></span>
6. <span data-ttu-id="f32b5-146">Пользователь создает отчет в Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="f32b5-146">User creates a report in Power BI Desktop.</span></span>
7. <span data-ttu-id="f32b5-147">Пользователь публикует отчет в службе Power BI.</span><span class="sxs-lookup"><span data-stu-id="f32b5-147">User publishes the report to the Power BI service.</span></span> <span data-ttu-id="f32b5-148">Отчеты затем становятся доступными для выбора в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="f32b5-148">The reports are then available for selection in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="f32b5-149">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="f32b5-149">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="f32b5-150">См. также</span><span class="sxs-lookup"><span data-stu-id="f32b5-150">See Also</span></span>

[<span data-ttu-id="f32b5-151">Business Central и Power BI</span><span class="sxs-lookup"><span data-stu-id="f32b5-151">Business Central and Power BI</span></span>](admin-powerbi.md)  
[<span data-ttu-id="f32b5-152">Power BI для потребителей</span><span class="sxs-lookup"><span data-stu-id="f32b5-152">Power BI for consumers</span></span>](/power-bi/consumer/end-user-consumer)  
[<span data-ttu-id="f32b5-153">"Новый внешний вид" службы Power BI</span><span class="sxs-lookup"><span data-stu-id="f32b5-153">The 'new look' of the Power BI service</span></span>](/power-bi/service-new-look)  
[<span data-ttu-id="f32b5-154">Быстрый старт: подключение к данным в Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="f32b5-154">Quickstart: Connect to data in Power BI Desktop</span></span>](/power-bi/desktop-quickstart-connect-to-data)  
[<span data-ttu-id="f32b5-155">Документация Power BI</span><span class="sxs-lookup"><span data-stu-id="f32b5-155">Power BI documentation</span></span>](/power-bi/)  
[<span data-ttu-id="f32b5-156">Бизнес-аналитика</span><span class="sxs-lookup"><span data-stu-id="f32b5-156">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="f32b5-157">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="f32b5-157">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="f32b5-158">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="f32b5-158">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="f32b5-159">[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="f32b5-159">[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span></span>  
<span data-ttu-id="f32b5-160">[Использование [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="f32b5-160">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span></span>  
<span data-ttu-id="f32b5-161">[Использование [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных Power Apps](across-how-use-financials-data-source-powerapps.md)</span><span class="sxs-lookup"><span data-stu-id="f32b5-161">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)</span></span>  
<span data-ttu-id="f32b5-162">[Использование [!INCLUDE[prod_short](includes/prod_short.md)] в Power Automate](across-how-use-financials-data-source-flow.md)</span><span class="sxs-lookup"><span data-stu-id="f32b5-162">[Using [!INCLUDE[prod_short](includes/prod_short.md)] in Power Automate](across-how-use-financials-data-source-flow.md)</span></span>  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  
