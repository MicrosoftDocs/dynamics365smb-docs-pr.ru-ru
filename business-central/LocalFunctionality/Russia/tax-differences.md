---
title: Налоговые разницы в России
description: Российские усовершенствования включают управление налоговыми разницами.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 0a237ee47e5ee1189e4f6df12f7a450a9b328b51
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5382719"
---
# <a name="tax-differences"></a><span data-ttu-id="d3b62-103">Налоговые разницы</span><span class="sxs-lookup"><span data-stu-id="d3b62-103">Tax Differences</span></span>

<span data-ttu-id="d3b62-104">Налоговые разницы представляют собой расхождения сумм налога, вызванные различиями в правилах признания доходов и расходов в бухгалтерском и налоговом учете.</span><span class="sxs-lookup"><span data-stu-id="d3b62-104">Tax differences are variations in tax amounts caused by the different rules for recognizing income and expenses between entries for book accounting and tax accounting.</span></span> 

<span data-ttu-id="d3b62-105">В [!INCLUDE[prod_short](../../includes/prod_short.md)] можно настроить регистры налоговых разниц и журналы налоговых разниц для отслеживания и управления разницами между суммами бухгалтерского и налогового учета.</span><span class="sxs-lookup"><span data-stu-id="d3b62-105">In [!INCLUDE[prod_short](../../includes/prod_short.md)], you can set up tax difference registers and tax difference journals to track and manage differences between book accounting and tax accounting amounts.</span></span>

## <a name="preparing-the-chart-of-accounts"></a><span data-ttu-id="d3b62-106">Подготовка плана счетов</span><span class="sxs-lookup"><span data-stu-id="d3b62-106">Preparing the Chart of Accounts</span></span>

<span data-ttu-id="d3b62-107">Перед настройкой налоговых разниц необходимо убедиться, что план счетов настроен для корректной обработки налогового учета и налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="d3b62-107">Before you set up tax differences, you will have to make sure that your chart of accounts is set up to correctly handle tax accounting and tax differences.</span></span> <span data-ttu-id="d3b62-108">Как минимум план счетов должен содержать счет налоговых разниц для транзакций доходов и расходов.</span><span class="sxs-lookup"><span data-stu-id="d3b62-108">At a minimum, your chart of accounts must contain tax difference accounts for income and expense transactions.</span></span>

## <a name="getting-started-with-tax-differences"></a><span data-ttu-id="d3b62-109">Начало работы с налоговыми разницами</span><span class="sxs-lookup"><span data-stu-id="d3b62-109">Getting Started with Tax Differences</span></span> 

<span data-ttu-id="d3b62-110">Для настройки и просмотра операций налоговых разниц используются следующие таблицы, поддерживающие окна налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="d3b62-110">To set up and view tax difference entries, you will use the following tables, which support tax differences windows.</span></span>

| <span data-ttu-id="d3b62-111">Окно</span><span class="sxs-lookup"><span data-stu-id="d3b62-111">Window</span></span>                     | <span data-ttu-id="d3b62-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d3b62-112">Description</span></span>                                                  |
| :------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="d3b62-113">Учетная группа</span><span class="sxs-lookup"><span data-stu-id="d3b62-113">Tax Diff.</span></span> <span data-ttu-id="d3b62-114">налоговой разницы</span><span class="sxs-lookup"><span data-stu-id="d3b62-114">Posting Group</span></span>    | <span data-ttu-id="d3b62-115">Определяет учетные группы для транзакций налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="d3b62-115">Specifies posting groups for tax difference transactions.</span></span>    |
| <span data-ttu-id="d3b62-116">Учетная группа</span><span class="sxs-lookup"><span data-stu-id="d3b62-116">Tax Diff.</span></span> <span data-ttu-id="d3b62-117">налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="d3b62-117">Journal Template</span></span> | <span data-ttu-id="d3b62-118">Определяет журналы, используемые для учета операций налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="d3b62-118">Specifies the journals that are used for posting tax difference entries.</span></span> |
| <span data-ttu-id="d3b62-119">Операция корресп. налогового расчета</span><span class="sxs-lookup"><span data-stu-id="d3b62-119">Tax Calc. Corresp. Entry</span></span>   | <span data-ttu-id="d3b62-120">Определяет данные налоговой разницы, необходимые для внешних отчетов и форм.</span><span class="sxs-lookup"><span data-stu-id="d3b62-120">Specifies tax difference information that is needed for external reports and forms.</span></span> |
| <span data-ttu-id="d3b62-121">Учетная группа</span><span class="sxs-lookup"><span data-stu-id="d3b62-121">Tax Diff.</span></span> <span data-ttu-id="d3b62-122">журнала</span><span class="sxs-lookup"><span data-stu-id="d3b62-122">Journal Line</span></span>     | <span data-ttu-id="d3b62-123">Определяет учтенные операции журнала налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="d3b62-123">Specifies posted tax difference journal entries.</span></span>             |

## <a name="see-also"></a><span data-ttu-id="d3b62-124">См. также</span><span class="sxs-lookup"><span data-stu-id="d3b62-124">See Also</span></span>

[<span data-ttu-id="d3b62-125">Настройка расчета налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="d3b62-125">Setting up Tax Difference Calculation</span></span>](Setting-up-Tax-Difference-Calculation.md)  
[<span data-ttu-id="d3b62-126">Регистры налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="d3b62-126">Tax Difference Registers</span></span>](Tax-Difference-Registers.md)  
[<span data-ttu-id="d3b62-127">Налоговый учет</span><span class="sxs-lookup"><span data-stu-id="d3b62-127">Tax Accounting</span></span>](Tax-Accounting.md)  
[<span data-ttu-id="d3b62-128">Налоговые регистры</span><span class="sxs-lookup"><span data-stu-id="d3b62-128">Tax Registers</span></span>](Tax-Registers.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]