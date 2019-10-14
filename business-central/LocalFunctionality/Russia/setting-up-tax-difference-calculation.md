---
title: Настройка расчета налоговых разниц в России
description: Российские усовершенствования включают расчет налоговых разниц по основным средствам.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 42852ba7a37bcde47da90e15a30f2db609f434f5
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301124"
---
# <a name="setting-up-tax-difference-calculation"></a><span data-ttu-id="48b0c-103">Настройка расчета налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="48b0c-103">Setting up Tax Difference Calculation</span></span>

<span data-ttu-id="48b0c-104">Расчет налоговых разниц необходимо настроить, если имеется налоговая разница в представлении операций с основными средствами, операций себестоимости товаров или финансовых операций в бухгалтерском и налоговом учете, для которых необходимо зафиксировать расходы, подлежащие списанию.</span><span class="sxs-lookup"><span data-stu-id="48b0c-104">Tax difference calculations must be set up if there is a tax difference for the presentation of fixed asset entries, item cost entries, or finance transactions in bookkeeping and tax accounting for which expenses to write off must be fixed.</span></span> <span data-ttu-id="48b0c-105">Чтобы настроить налоговую разницу, выберите действие **Настройка**, а затем выберите действие **Налоговые разницы**.</span><span class="sxs-lookup"><span data-stu-id="48b0c-105">To set tax difference, choose the **Setup** action, and then choose the **Tax Differences** action.</span></span>

## <a name="setting-up-posting-groups"></a><span data-ttu-id="48b0c-106">Настройка учетных групп</span><span class="sxs-lookup"><span data-stu-id="48b0c-106">Setting Up Posting Groups</span></span>

<span data-ttu-id="48b0c-107">В пункте меню **Учетные группы налоговых разниц** необходимо указать финансовые счета из настроенного плана счетов, на которых будут учитываться финансовые транзакции с налоговыми разницами.</span><span class="sxs-lookup"><span data-stu-id="48b0c-107">In the **Tax Difference Posting Groups** you must determine finance accounts from the set up chart of accounts, where finance transactions with tax differences are accounted for.</span></span>

<span data-ttu-id="48b0c-108">Если имеются строки журнала, которые необходимо нормализовать перед списанием расходов, эти журналы невозможно учесть без запуска периодического задания нормализации.</span><span class="sxs-lookup"><span data-stu-id="48b0c-108">If there are journal lines that must be normalized before writing off expenses, those journals cannot be posted without running a periodic job of normalizing.</span></span>

<span data-ttu-id="48b0c-109">В следующей процедуре показан порядок обработки функции нормализации.</span><span class="sxs-lookup"><span data-stu-id="48b0c-109">The following procedure shows how to process a normalization function.</span></span>

1. <span data-ttu-id="48b0c-110">В окне **Журнал расходов будущих периодов** выберите **Расчет нормируемой амортизации**</span><span class="sxs-lookup"><span data-stu-id="48b0c-110">In the **Future Expenses Journal** window, choose the **Calculate Depreciation by Norm.**</span></span> <span data-ttu-id="48b0c-111">.</span><span class="sxs-lookup"><span data-stu-id="48b0c-111">action</span></span>
2. <span data-ttu-id="48b0c-112">В окне **Расчет аморт. РБП по норм.** на экспресс-вкладке **Налоговая разница** установите фильтр для налоговой разницы.</span><span class="sxs-lookup"><span data-stu-id="48b0c-112">In the **Calculate FE Depr. With Norm** window, on the **Tax Difference** FastTab, enter the filter for the tax difference.</span></span>
3. <span data-ttu-id="48b0c-113">На экспресс-вкладке **Параметры** введите учетный период, для которого выполняется расчет.</span><span class="sxs-lookup"><span data-stu-id="48b0c-113">On the **Options** FastTab, enter the accounting period for which the counting is done.</span></span>
4. <span data-ttu-id="48b0c-114">Для печати отчета выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="48b0c-114">Choose the **Print** action to print the report.</span></span>
5. <span data-ttu-id="48b0c-115">Выполните операцию учета журнала расходов будущих периодов.</span><span class="sxs-lookup"><span data-stu-id="48b0c-115">Post the future expenses journal.</span></span>

## <a name="see-also"></a><span data-ttu-id="48b0c-116">См. также</span><span class="sxs-lookup"><span data-stu-id="48b0c-116">See Also</span></span>

[<span data-ttu-id="48b0c-117">Налоговые регистры</span><span class="sxs-lookup"><span data-stu-id="48b0c-117">Tax Registers</span></span>](Tax-Registers.md)  
[<span data-ttu-id="48b0c-118">Налоговые разницы</span><span class="sxs-lookup"><span data-stu-id="48b0c-118">Tax Differences</span></span>](Tax-Differences.md)  
[<span data-ttu-id="48b0c-119">Регистры налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="48b0c-119">Tax Difference Registers</span></span>](Tax-Difference-Registers.md)  
[<span data-ttu-id="48b0c-120">Практическое руководство. Настройка юрисдикций нормы</span><span class="sxs-lookup"><span data-stu-id="48b0c-120">How to: Set Up Norm Jurisdictions</span></span>](How-to-Set-Up-Norm-Jurisdictions.md)  
[<span data-ttu-id="48b0c-121">Практическое руководство. Учет налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="48b0c-121">How to: Post Tax Differences</span></span>](How-to-Post-Tax-Differences.md)  
