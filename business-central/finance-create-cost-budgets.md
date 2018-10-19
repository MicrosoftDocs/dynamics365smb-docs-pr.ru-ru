---
title: "Создание бюджетов затрат | Документы Майкрософт"
description: "В этом разделе приводится обзор того, где можно создавать и анализировать бюджеты затрат."
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
ms.openlocfilehash: a107203cf81b149b920944db1fabace6e434221a
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="creating-cost-budgets"></a><span data-ttu-id="dd385-103">Создание бюджетов затрат</span><span class="sxs-lookup"><span data-stu-id="dd385-103">Creating Cost Budgets</span></span>
<span data-ttu-id="dd385-104">Бюджетирование при учете затрат напоминает бюджетирование в Главной книге.</span><span class="sxs-lookup"><span data-stu-id="dd385-104">Budgeting in cost accounting resembles budgeting in the general ledger.</span></span> <span data-ttu-id="dd385-105">Бюджет расходов создается на основе типов затрат, подобно тому как бюджет Главной книги — на основе счетов Главной книги.</span><span class="sxs-lookup"><span data-stu-id="dd385-105">A cost budget is created based on cost types just as a budget for the general ledger is created based on general ledger accounts.</span></span>  

<span data-ttu-id="dd385-106">Бюджет расходов создается на определенный период времени, например финансовый год.</span><span class="sxs-lookup"><span data-stu-id="dd385-106">A cost budget is created for a certain period of time, for example, a fiscal year.</span></span> <span data-ttu-id="dd385-107">Можно создать любое необходимое число бюджетов затрат.</span><span class="sxs-lookup"><span data-stu-id="dd385-107">You can create as many cost budgets as needed.</span></span> <span data-ttu-id="dd385-108">Можно создать новый бюджет затрат вручную, путем импорта бюджета затрат либо путем копирования существующего бюджета затрат как базового.</span><span class="sxs-lookup"><span data-stu-id="dd385-108">You can create a new cost budget manually, or by importing a cost budget, or by copying an existing cost budget as the budget base.</span></span> <span data-ttu-id="dd385-109">Дополнительные сведения см. в разделе [Создание бюджетов ГК](finance-how-create-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="dd385-109">For more information, see [Create G/L Budgets](finance-how-create-budgets.md).</span></span>

<span data-ttu-id="dd385-110">Можно использовать следующие окна для создания и анализа бюджетов затрат.</span><span class="sxs-lookup"><span data-stu-id="dd385-110">You use the following windows to create and analyze cost budgets.</span></span> <span data-ttu-id="dd385-111">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), чтобы найти окно, и прочитайте подсказку для каждого.</span><span class="sxs-lookup"><span data-stu-id="dd385-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon to find a window, and then read the tooltip for each.</span></span>

|<span data-ttu-id="dd385-112">По</span><span class="sxs-lookup"><span data-stu-id="dd385-112">To</span></span>|<span data-ttu-id="dd385-113">Ссылка</span><span class="sxs-lookup"><span data-stu-id="dd385-113">See</span></span>|  
|--------|---------|  
|<span data-ttu-id="dd385-114">Перенос бюджетов из главной книги.</span><span class="sxs-lookup"><span data-stu-id="dd385-114">Transfer budgets from the general ledger.</span></span>|<span data-ttu-id="dd385-115">Пакетное задание **Копировать бюджет ГК в учет затрат**</span><span class="sxs-lookup"><span data-stu-id="dd385-115">**Copy G-L Budget to Cost Acctg.** batch job</span></span>|  
|<span data-ttu-id="dd385-116">Скопируйте бюджеты затрат.</span><span class="sxs-lookup"><span data-stu-id="dd385-116">Copy cost budgets.</span></span>|<span data-ttu-id="dd385-117">Пакетное задание **Копировать бюджет расходов**</span><span class="sxs-lookup"><span data-stu-id="dd385-117">**Copy Cost Budget** batch job</span></span>|  
|<span data-ttu-id="dd385-118">Распределить бюджеты.</span><span class="sxs-lookup"><span data-stu-id="dd385-118">Allocate budgets.</span></span>|<span data-ttu-id="dd385-119">Окно **Распределение затрат**</span><span class="sxs-lookup"><span data-stu-id="dd385-119">**Cost Allocation** window</span></span>|  
|<span data-ttu-id="dd385-120">См. регистры бюджета затрат и записи бюджета затрат.</span><span class="sxs-lookup"><span data-stu-id="dd385-120">See cost budget registers and cost budget entries.</span></span>|<span data-ttu-id="dd385-121">Окно **Журналы бюджета расходов**</span><span class="sxs-lookup"><span data-stu-id="dd385-121">**Cost Budget Registers** window</span></span>|  
|<span data-ttu-id="dd385-122">Печать сравнений бюджета затрат с использованием различных отчетов.</span><span class="sxs-lookup"><span data-stu-id="dd385-122">Print cost budget comparisons using various reports.</span></span>|<span data-ttu-id="dd385-123">Отчет **Баланс/Бюджет затрат**</span><span class="sxs-lookup"><span data-stu-id="dd385-123">**Cost Acctg. Balance-Budget** report</span></span><br /><br /> <span data-ttu-id="dd385-124">Отчет **Ведомость учета затрат/Бюджет**</span><span class="sxs-lookup"><span data-stu-id="dd385-124">**Cost Acctg. Statement-Budget** report</span></span><br /><br /> <span data-ttu-id="dd385-125">отчет **Бюджет затрат по центрам затрат**</span><span class="sxs-lookup"><span data-stu-id="dd385-125">**Cost Budget by Cost Center** report</span></span><br /><br /> <span data-ttu-id="dd385-126">Отчет **Бюджет затрат по объектам затрат**</span><span class="sxs-lookup"><span data-stu-id="dd385-126">**Cost Budget by Cost Object** report</span></span>|  

## <a name="see-also"></a><span data-ttu-id="dd385-127">См. также</span><span class="sxs-lookup"><span data-stu-id="dd385-127">See Also</span></span>  
[<span data-ttu-id="dd385-128">Учет по затратам</span><span class="sxs-lookup"><span data-stu-id="dd385-128">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
[<span data-ttu-id="dd385-129">Создание бюджетов ГК</span><span class="sxs-lookup"><span data-stu-id="dd385-129">Create G/L Budgets</span></span>](finance-how-create-budgets.md)  
<span data-ttu-id="dd385-130">[Терминология в учете затрат](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="dd385-130">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="dd385-131">Определение и распределение затрат</span><span class="sxs-lookup"><span data-stu-id="dd385-131">Defining and Allocating Costs</span></span>](finance-define-and-allocate-costs.md)  
<span data-ttu-id="dd385-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="dd385-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

