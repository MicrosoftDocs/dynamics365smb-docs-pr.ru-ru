---
title: Восстановление НДС в России
description: Российские улучшения включают восстановление НДС.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 7be675bc815d6056c50c23b13097363a27c79bc4
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738271"
---
# <a name="vat-reinstatement"></a><span data-ttu-id="2f9dd-103">Восстановление НДС</span><span class="sxs-lookup"><span data-stu-id="2f9dd-103">VAT reinstatement</span></span>

<span data-ttu-id="2f9dd-104">В некоторых случаях плательщики НДС обязаны восстановить НДС.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-104">In certain cases, VAT payers are required to reinstate VAT.</span></span>

<span data-ttu-id="2f9dd-105">Известно, что организации, приобретающие основные средства, товары, работы, услуги (далее — товары), имеют право принять к вычету входящий НДС по ним при выполнении необходимых условий.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-105">It is known that the organizations acquiring fixed assets, goods, works, services (further – goods), have the right to accept to deduction of the input VAT on them at accomplishment of all conditions for deduction.</span></span> <span data-ttu-id="2f9dd-106">Но если впоследствии обстоятельства изменятся и станет ясно, что права на вычет НДС не было, налог нужно будет восстановить.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-106">But if later circumstances change and it becomes clear that there is no right to deduct VAT, the tax will have to be reinstate.</span></span> <span data-ttu-id="2f9dd-107">Иными словами, восстановленный НДС — это ранее вычтенный НДС, который в определенном объеме должен быть возвращен в бюджет.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-107">In other words, the reinstatement VAT is previously deducted VAT, which in a certain amount must be returned back to the budget.</span></span>

## <a name="vat-accounting-group-settings"></a><span data-ttu-id="2f9dd-108">Параметры группы учета НДС</span><span class="sxs-lookup"><span data-stu-id="2f9dd-108">VAT accounting group settings</span></span>  

<span data-ttu-id="2f9dd-109">Восстановление НДС возможно в случае использования транзитного НДС с учетом через журнал НДС вручную.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-109">VAT reinstatement is possible in case of using transit VAT with manual post through the VAT journal.</span></span>  

<span data-ttu-id="2f9dd-110">В разделе **Настройка учета НДС** необходимо настроить следующее:</span><span class="sxs-lookup"><span data-stu-id="2f9dd-110">In **VAT posting setup**, settings must be made:</span></span>  

- <span data-ttu-id="2f9dd-111">Тип расчета НДС - ОБЫЧНЫЙ НДС.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-111">VAT calculation type – NORMAL VAT.</span></span> 
-  <span data-ttu-id="2f9dd-112">Тип нереализованного НДС — НЕ ПУСТО (например, "Проценты").</span><span class="sxs-lookup"><span data-stu-id="2f9dd-112">The unrealized VAT type is NOT EMPTY (for example Percentage).</span></span>  
- <span data-ttu-id="2f9dd-113">НДС транз. счет ГК — поле не должно быть заполнено.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-113">Trans. VAT account – must not be filled.</span></span> 
- <span data-ttu-id="2f9dd-114">Тип транз. НДС — поле не должно быть заполнено.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-114">Transit VAT Type – should not be filled.</span></span>  
- <span data-ttu-id="2f9dd-115">Зачет НДС вручную — установлен.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-115">Manual VAT Settlement checked.</span></span>  
- <span data-ttu-id="2f9dd-116">Указаны шаблон зачета и раздел зачета НДС.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-116">The template and batch VAT settlement is specified.</span></span>  
- <span data-ttu-id="2f9dd-117">Заданы шаблон восстановления НДС и раздел восстановления НДС.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-117">VAT reinstatement template and VAT reinstatement batch – set.</span></span>

## <a name="vat-reinstatement"></a><span data-ttu-id="2f9dd-118">Восстановление НДС</span><span class="sxs-lookup"><span data-stu-id="2f9dd-118">VAT reinstatement</span></span>

<span data-ttu-id="2f9dd-119">Для восстановления ранее принятого к вычету НДС используется **Журнал восстановления НДС**.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-119">To reinstate previously accepted for deduction of VAT used **VAT Reinstatement Worksheet**.</span></span>

1. <span data-ttu-id="2f9dd-120">На странице **Журнал восстановления НДС** вы должны запустить задачу **Предложить документы**.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-120">In the **VAT Reinstatement Worksheet** page, you must run the task **Suggest Documents**.</span></span>  

2. <span data-ttu-id="2f9dd-121">Вы должны установить фильтр по дате (обычно на конец месяца, в котором документы были прочитаны).</span><span class="sxs-lookup"><span data-stu-id="2f9dd-121">You must set a filter by date (usually at the end of the month, as the documents were read).</span></span>  

    <span data-ttu-id="2f9dd-122">Вы можете установить фильтр по НДС бизнес-группе или НДС товарной группе.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-122">And you can specify a filter on VAT Business and VAT product posting groups.</span></span>  

    <span data-ttu-id="2f9dd-123">В результате выполнения задания в журнале должны быть восстановлены строки операций с НДС (список документов покупок, в которых есть операции с НДС, ранее принятые для учета).</span><span class="sxs-lookup"><span data-stu-id="2f9dd-123">As a result of the work of the task in the journal, the VAT lines of operations to be restored (a list of purchase documents in which there are VAT operations previously accepted for post).</span></span> 

    <span data-ttu-id="2f9dd-124">Поле **Сумма реализованного НДС** отражает сумму НДС по документу, который была принята к вычету и которая может быть восстановлена.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-124">The field **Realized VAT Amount** reflects the amount of VAT on the document, which was deducted and which can be reinstate.</span></span>

3. <span data-ttu-id="2f9dd-125">В этом журнале выберите строки, которые вы хотите восстановить, и нажмите кнопку "Копировать строки в журнал".</span><span class="sxs-lookup"><span data-stu-id="2f9dd-125">In this worksheet, select the lines that you want to reinstate and click the "Copy lines to Journal" button.</span></span> <span data-ttu-id="2f9dd-126">Перед этим вам необходимо установить фильтр по дате, щелкнув правой кнопкой мыши по названию любого столбца.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-126">Before that, you need to set a filter by date by right-clicking on the name of any column.</span></span> <span data-ttu-id="2f9dd-127">Добавьте фильтр "Фильтровать итоги по".</span><span class="sxs-lookup"><span data-stu-id="2f9dd-127">Add filter "Filter totals by".</span></span> 
4. <span data-ttu-id="2f9dd-128">Вы можете восстановить всю транзакцию (на всю сумму НДС продаж), вы можете установить коэффициент (например, 0,5), чтобы восстановить часть суммы.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-128">You can reistate the entire transaction (for the entire amount of VAT sold), you can set a factor (for example, 0.5) to reistate part of the amount.</span></span>
5. <span data-ttu-id="2f9dd-129">Выбранная строка будет перенесена в журнал восстановления НДС для учета.</span><span class="sxs-lookup"><span data-stu-id="2f9dd-129">The selected line will be transferred to the VAT Reinstatement journal for posting.</span></span>

## <a name="see-also"></a><span data-ttu-id="2f9dd-130">См. также</span><span class="sxs-lookup"><span data-stu-id="2f9dd-130">See Also</span></span>

[<span data-ttu-id="2f9dd-131">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="2f9dd-131">Russia Local Functionality</span></span>](russia-local-functionality.md)  
