---
title: Налоговые разницы в России
description: Российские усовершенствования включают управление налоговыми разницами.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: e66193c2ceabcc4ab6737208e4a450cc5c48d9db
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738234"
---
# <a name="tax-differences"></a><span data-ttu-id="f0535-103">Налоговые разницы</span><span class="sxs-lookup"><span data-stu-id="f0535-103">Tax Differences</span></span>

<span data-ttu-id="f0535-104">Налоговые разницы представляют собой расхождения сумм налога, вызванные различиями в правилах признания доходов и расходов в бухгалтерском и налоговом учете.</span><span class="sxs-lookup"><span data-stu-id="f0535-104">Tax differences are variations in tax amounts caused by the different rules for recognizing income and expenses between entries for book accounting and tax accounting.</span></span> 

<span data-ttu-id="f0535-105">В [!INCLUDE[prodshort](../../includes/prodshort.md)] можно настроить регистры налоговых разниц и журналы налоговых разниц для отслеживания и управления разницами между суммами бухгалтерского и налогового учета.</span><span class="sxs-lookup"><span data-stu-id="f0535-105">In [!INCLUDE[prodshort](../../includes/prodshort.md)], you can set up tax difference registers and tax difference journals to track and manage differences between book accounting and tax accounting amounts.</span></span>

## <a name="preparing-the-chart-of-accounts"></a><span data-ttu-id="f0535-106">Подготовка плана счетов</span><span class="sxs-lookup"><span data-stu-id="f0535-106">Preparing the Chart of Accounts</span></span>

<span data-ttu-id="f0535-107">Перед настройкой налоговых разниц необходимо убедиться, что план счетов настроен для корректной обработки налогового учета и налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="f0535-107">Before you set up tax differences, you will have to make sure that your chart of accounts is set up to correctly handle tax accounting and tax differences.</span></span> <span data-ttu-id="f0535-108">Как минимум план счетов должен содержать счет налоговых разниц для транзакций доходов и расходов.</span><span class="sxs-lookup"><span data-stu-id="f0535-108">At a minimum, your chart of accounts must contain tax difference accounts for income and expense transactions.</span></span>

## <a name="getting-started-with-tax-differences"></a><span data-ttu-id="f0535-109">Начало работы с налоговыми разницами</span><span class="sxs-lookup"><span data-stu-id="f0535-109">Getting Started with Tax Differences</span></span> 

<span data-ttu-id="f0535-110">Для настройки и просмотра операций налоговых разниц используются следующие таблицы, поддерживающие окна налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="f0535-110">To set up and view tax difference entries, you will use the following tables, which support tax differences windows.</span></span>

| <span data-ttu-id="f0535-111">Окно</span><span class="sxs-lookup"><span data-stu-id="f0535-111">Window</span></span>                     | <span data-ttu-id="f0535-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f0535-112">Description</span></span>                                                  |
| :------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="f0535-113">Учетная группа налоговой разницы</span><span class="sxs-lookup"><span data-stu-id="f0535-113">Tax Diff. Posting Group</span></span>    | <span data-ttu-id="f0535-114">Определяет учетные группы для транзакций налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="f0535-114">Specifies posting groups for tax difference transactions.</span></span>    |
| <span data-ttu-id="f0535-115">Шаблон налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="f0535-115">Tax Diff. Journal Template</span></span> | <span data-ttu-id="f0535-116">Определяет журналы, используемые для учета операций налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="f0535-116">Specifies the journals that are used for posting tax difference entries.</span></span> |
| <span data-ttu-id="f0535-117">Операция корресп. налогового расчета</span><span class="sxs-lookup"><span data-stu-id="f0535-117">Tax Calc. Corresp. Entry</span></span>   | <span data-ttu-id="f0535-118">Определяет данные налоговой разницы, необходимые для внешних отчетов и форм.</span><span class="sxs-lookup"><span data-stu-id="f0535-118">Specifies tax difference information that is needed for external reports and forms.</span></span> |
| <span data-ttu-id="f0535-119">Строка налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="f0535-119">Tax Diff. Journal Line</span></span>     | <span data-ttu-id="f0535-120">Определяет учтенные операции журнала налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="f0535-120">Specifies posted tax difference journal entries.</span></span>             |

## <a name="see-also"></a><span data-ttu-id="f0535-121">См. также</span><span class="sxs-lookup"><span data-stu-id="f0535-121">See Also</span></span>

[<span data-ttu-id="f0535-122">Настройка расчета налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="f0535-122">Setting up Tax Difference Calculation</span></span>](Setting-up-Tax-Difference-Calculation.md)  
[<span data-ttu-id="f0535-123">Регистры налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="f0535-123">Tax Difference Registers</span></span>](Tax-Difference-Registers.md)  
[<span data-ttu-id="f0535-124">Налоговый учет</span><span class="sxs-lookup"><span data-stu-id="f0535-124">Tax Accounting</span></span>](Tax-Accounting.md)  
[<span data-ttu-id="f0535-125">Налоговые регистры</span><span class="sxs-lookup"><span data-stu-id="f0535-125">Tax Registers</span></span>](Tax-Registers.md)  
