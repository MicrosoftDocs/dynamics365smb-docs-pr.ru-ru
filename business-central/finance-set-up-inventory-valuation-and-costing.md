---
title: "Настройка оценки стоимости запасов и учета себестоимости | Microsoft Docs"
description: "В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: af4c256b59739abce9ec22bce254fe8e2dff4e29
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="setting-up-inventory-valuation-and-costing"></a><span data-ttu-id="bbece-103">Настройка оценки стоимости запасов и учета себестоимости</span><span class="sxs-lookup"><span data-stu-id="bbece-103">Setting Up Inventory Valuation and Costing</span></span>
<span data-ttu-id="bbece-104">Чтобы обеспечить правильную запись валютных курсов, необходимо настроить различные поля и окна, прежде чем приступать к выполнению товарных транзакций.</span><span class="sxs-lookup"><span data-stu-id="bbece-104">To make sure that inventory costs are recorded correctly, you must set up various fields and windows before you begin to make item transactions.</span></span>

<span data-ttu-id="bbece-105">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="bbece-105">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="bbece-106">**Задача**</span><span class="sxs-lookup"><span data-stu-id="bbece-106">**To**</span></span>|<span data-ttu-id="bbece-107">**Ссылка**</span><span class="sxs-lookup"><span data-stu-id="bbece-107">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="bbece-108">Настройка метода учета себестоимости для каждого товара для управления использованием входящей себестоимости с целью доступа к стоимости запасов и проданных товаров.</span><span class="sxs-lookup"><span data-stu-id="bbece-108">Set a costing method for each item to govern how its incoming cost is used to assess inventory value and the cost of goods sold.</span></span>|[<span data-ttu-id="bbece-109">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="bbece-109">Register New Items</span></span>](inventory-how-register-new-items.md)|  
|<span data-ttu-id="bbece-110">Обеспечение автоматического учета стоимости в главной книге при учете транзакции запасов.</span><span class="sxs-lookup"><span data-stu-id="bbece-110">Ensure that the cost is automatically posted to the general ledger whenever an inventory transaction is posted.</span></span>|<span data-ttu-id="bbece-111">Поле **Автомат. учет себест.** на странице **Настройка модуля "Запасы"**</span><span class="sxs-lookup"><span data-stu-id="bbece-111">**Automatic Cost Posting** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="bbece-112">Обеспечение учета ожидаемой себестоимости в главной книге для определения по промежуточным счетам главной книги подлежащих оплате сумм и стоимости проданных товаров до фактического выставления за них счетов.</span><span class="sxs-lookup"><span data-stu-id="bbece-112">Ensure that expected costs are posted to the general ledger to see from the interim G/L accounts an estimate of the amounts due and the cost of the traded items before they are actually invoiced.</span></span>|<span data-ttu-id="bbece-113">Поле **Учет ожидаемой себест. в ГК** на странице **Настройка модуля "Запасы"**</span><span class="sxs-lookup"><span data-stu-id="bbece-113">**Expected Cost Posting to G/L** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="bbece-114">Настройка системы для автоматической коррекции при любых изменениях себестоимости при каждом учете транзакции запасов.</span><span class="sxs-lookup"><span data-stu-id="bbece-114">Set the system up to adjust for any cost changes automatically every time you post inventory transactions.</span></span>|[<span data-ttu-id="bbece-115">Корректировка себестоимости товаров</span><span class="sxs-lookup"><span data-stu-id="bbece-115">Adjust Item Costs</span></span>](inventory-how-adjust-item-costs.md)|  
|<span data-ttu-id="bbece-116">Указание способа вычисления средней себестоимости: только для каждого товара или для каждого товара каждой единицы учета запасов и для каждой разновидности товаров.</span><span class="sxs-lookup"><span data-stu-id="bbece-116">Define if the average cost is to be calculated per item only or per item for each stockkeping unit and for each variant of the item.</span></span>|<span data-ttu-id="bbece-117">Поле **Тип расчета средней себестоимости** на странице **Настройка модуля "Запасы"**</span><span class="sxs-lookup"><span data-stu-id="bbece-117">**Average Cost Calc. Type** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="bbece-118">Выбор периода времени, который должен использоваться для вычисления средневзвешенной себестоимости товаров, для которых используются метод средней себестоимости.</span><span class="sxs-lookup"><span data-stu-id="bbece-118">Select the period of time you would like the program to use for calculating the weighted average cost of items that use the average costing method.</span></span>|<span data-ttu-id="bbece-119">Поле **Период расчета средней себестоимости** на странице **Настройка модуля "Запасы"**</span><span class="sxs-lookup"><span data-stu-id="bbece-119">**Average Cost Period** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="bbece-120">Определение периодов учета запасов для управления стоимостью запасов во времени путем запрета учета транзакций в закрытых периодах учета запасов.</span><span class="sxs-lookup"><span data-stu-id="bbece-120">Define inventory periods to control inventory value over time by disallowing transaction posting in closed inventory periods.</span></span>|[<span data-ttu-id="bbece-121">Работа с учетными периодами</span><span class="sxs-lookup"><span data-stu-id="bbece-121">Work with Inventory Periods</span></span>](finance-how-to-work-with-inventory-periods.md)|  
|<span data-ttu-id="bbece-122">Обеспечение применения возврата продажи к исходной исходящей транзакции для сохранения стоимости запасов.</span><span class="sxs-lookup"><span data-stu-id="bbece-122">Ensure that sales returns are applied to the original outbound transaction to preserve inventory value.</span></span>|<span data-ttu-id="bbece-123">Поле **Точный возврат себест. обязат.** на странице **Продажи и расчеты с дебиторами**</span><span class="sxs-lookup"><span data-stu-id="bbece-123">**Exact Cost Reversing Mandatory** field in the **Sales & Receivables** page</span></span>|  
|<span data-ttu-id="bbece-124">Обеспечение применения возврата покупок к исходной входящей транзакции для сохранения стоимости запасов.</span><span class="sxs-lookup"><span data-stu-id="bbece-124">Ensure that purchase returns are applied to the original inbound transaction to preserve inventory value.</span></span>|<span data-ttu-id="bbece-125">Поле **Точный возврат себест. обязат.** на странице **Покупки и расчеты с кредиторами**</span><span class="sxs-lookup"><span data-stu-id="bbece-125">**Exact Cost Reversing Mandatory** field in the **´Purchases & Payables** page</span></span>|
|<span data-ttu-id="bbece-126">Настройка правил округления для применения при коррекции или предложении цен товаров и при корректировке или предложении стандартной себестоимости.</span><span class="sxs-lookup"><span data-stu-id="bbece-126">Set up the rounding rules to apply when adjusting or suggesting item prices and when adjusting or suggesting standard costs.</span></span>|<span data-ttu-id="bbece-127">Страница **Метод округления**</span><span class="sxs-lookup"><span data-stu-id="bbece-127">**Rounding Method** page</span></span>|  

## <a name="see-also"></a><span data-ttu-id="bbece-128">См. также</span><span class="sxs-lookup"><span data-stu-id="bbece-128">See Also</span></span>  
[<span data-ttu-id="bbece-129">Управление себестоимостью товаров</span><span class="sxs-lookup"><span data-stu-id="bbece-129">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="bbece-130">Работа с Business Central</span><span class="sxs-lookup"><span data-stu-id="bbece-130">Working with Business Central</span></span>](ui-work-product.md)  
[<span data-ttu-id="bbece-131">Финансы</span><span class="sxs-lookup"><span data-stu-id="bbece-131">Finance</span></span>](finance.md)  

