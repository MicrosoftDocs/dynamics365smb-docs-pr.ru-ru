---
title: "Настройка основных средств | Документы Майкрософт"
description: "Узнайте оп последовательности задач, которые следует выполнить для настройки основных средств, например машин или оборудования."
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: machinery, buildings
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 9dea8be0f5b0200f97082dc25dbaa2483ad6c735
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="setting-up-fixed-assets"></a><span data-ttu-id="3baba-103">Настройка основных средств</span><span class="sxs-lookup"><span data-stu-id="3baba-103">Setting Up Fixed Assets</span></span>
<span data-ttu-id="3baba-104">До начала работы с основными средствами необходимо определить несколько вещей.</span><span class="sxs-lookup"><span data-stu-id="3baba-104">Before you can work with Fixed Assets, you need to define a few things:</span></span>  

* <span data-ttu-id="3baba-105">Способ страхования, ведения и амортизации основных средств.</span><span class="sxs-lookup"><span data-stu-id="3baba-105">How you insure, maintain, and depreciate fixed assets.</span></span>  
* <span data-ttu-id="3baba-106">Способ регистрации записей и других значений в главной книге.</span><span class="sxs-lookup"><span data-stu-id="3baba-106">How you record costs and other values in the general ledger.</span></span>  

<span data-ttu-id="3baba-107">Таблица ниже содержит ссылки на дополнительную информацию.</span><span class="sxs-lookup"><span data-stu-id="3baba-107">The table below has links to more information.</span></span> <span data-ttu-id="3baba-108">После настройки этих вещей можно приступить к различным действиям.</span><span class="sxs-lookup"><span data-stu-id="3baba-108">After you set those things up, you can start various activities.</span></span> <span data-ttu-id="3baba-109">Дополнительные сведения см. в разделе [Основные средства](fa-manage.md).</span><span class="sxs-lookup"><span data-stu-id="3baba-109">For more information, see [Fixed Assets](fa-manage.md).</span></span>  

> [!NOTE]  
>   <span data-ttu-id="3baba-110">Вы можете записывать транзакции по основным средствам в окне **Журнал ГК учета основных средств** или в окне **Журнал ОС** в зависимости от назначения транзакций: для финансовой отчетности или для внутреннего управления.</span><span class="sxs-lookup"><span data-stu-id="3baba-110">You can record fixed asset transactions in the **Fixed Asset G/L Journal** or **Fixed Asset Journal** windows, depending on whether the transactions are for financial reporting or for internal management.</span></span> <span data-ttu-id="3baba-111">В справке для основных средств описывается только использование окна **Журнал ГК учета основных средств**.</span><span class="sxs-lookup"><span data-stu-id="3baba-111">Help for Fixed Assets only describes how to use the **Fixed Asset G/L Journal** window.</span></span>  

<span data-ttu-id="3baba-112">Если вы включаете действие основного средства в разделе **Интеграция С ГК** в окне **Карточка книги амортизации**, окно **Журнал ГК учета основных средств** будет использоваться для учета транзакций для соответствующего действия.</span><span class="sxs-lookup"><span data-stu-id="3baba-112">When you enable a fixed asset activity in the **G/L Integration** section in the **Depreciation Book Card** window, the **Fixed Asset G/L Journal** window is used to post transactions for the activity.</span></span>

> [!NOTE]  
>  <span data-ttu-id="3baba-113">Эта функция требует, чтобы было задано значение **Suite**.</span><span class="sxs-lookup"><span data-stu-id="3baba-113">This functionality requires that the experience is set to **Suite**.</span></span> <span data-ttu-id="3baba-114">Дополнительные сведения см. в разделе [Настройка взаимодействия Financials](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="3baba-114">For more information, see [Customizing Your Financials Experience](ui-experiences.md).</span></span>  

<span data-ttu-id="3baba-115">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="3baba-115">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

| <span data-ttu-id="3baba-116">Действие</span><span class="sxs-lookup"><span data-stu-id="3baba-116">To</span></span> | <span data-ttu-id="3baba-117">Ссылка</span><span class="sxs-lookup"><span data-stu-id="3baba-117">See</span></span> |
| --- | --- |
| <span data-ttu-id="3baba-118">Настройте счета ГК по умолчанию, ключи распределения, шаблоны и разделы журналов для учета основных средств, а также настройте классы и подклассы основных средств, такие как материальные и нематериальные основные средства.</span><span class="sxs-lookup"><span data-stu-id="3baba-118">Set up default G/L accounts, allocation keys, journal templates and batches for fixed asset posting, and set up fixed asset classes and subclasses, such as Tangible and Intangible.</span></span> |[<span data-ttu-id="3baba-119">Практическое руководство. Настройка общих данных основных средств</span><span class="sxs-lookup"><span data-stu-id="3baba-119">How to: Set Up General Fixed Assets Information</span></span>](fa-how-setup-general.md) |
| <span data-ttu-id="3baba-120">Создайте книги амортизации, определите различные методы амортизации, выполните интеграцию с главной книгой и включите дублирование операций в нескольких книгах амортизации.</span><span class="sxs-lookup"><span data-stu-id="3baba-120">Create depreciation books, define various depreciation methods, integrate with the general ledger, and enable duplication of entries in several depreciation books.</span></span> |[<span data-ttu-id="3baba-121">Практическое руководство. Настройка амортизации основных средств</span><span class="sxs-lookup"><span data-stu-id="3baba-121">How to: Set Up Fixed Asset Depreciation</span></span>](fa-how-setup-depreciation.md) |
| <span data-ttu-id="3baba-122">Включите страхование основных средств, настройте общие сведения о страховании, страховую карточку для каждого полиса, а также подготовьте журналы для учета затрат на страхование.</span><span class="sxs-lookup"><span data-stu-id="3baba-122">Enable insurance of fixed assets, set up general insurance information, an insurance card per policy, and prepare journals to post insurance costs.</span></span> |[<span data-ttu-id="3baba-123">Практическое руководство. Настройка страхования основных средств</span><span class="sxs-lookup"><span data-stu-id="3baba-123">How to: Set Up Fixed Asset Insurance</span></span>](fa-how-setup-insurance.md) |
| <span data-ttu-id="3baba-124">Включите обслуживание основных средств, настройте общие сведения об обслуживании, настройте счета учета обслуживания и определите типы работ по техническому обслуживанию.</span><span class="sxs-lookup"><span data-stu-id="3baba-124">Enable maintenance of fixed assets, set up general maintenance information, set up maintenance posting accounts, and define types of maintenance work.</span></span> |[<span data-ttu-id="3baba-125">Практическое руководство. Настройка обслуживания основных средств</span><span class="sxs-lookup"><span data-stu-id="3baba-125">How to: Set Up Fixed Asset Maintenance</span></span>](fa-how-setup-maintenance.md) |
| <span data-ttu-id="3baba-126">Изучите различные методы расчета амортизации основных средств.</span><span class="sxs-lookup"><span data-stu-id="3baba-126">Learn about different fixed asset depreciation methods.</span></span> |[<span data-ttu-id="3baba-127">Методы амортизации</span><span class="sxs-lookup"><span data-stu-id="3baba-127">Depreciation Methods</span></span>](fa-depreciation-methods.md) |

## <a name="see-also"></a><span data-ttu-id="3baba-128">См. также</span><span class="sxs-lookup"><span data-stu-id="3baba-128">See Also</span></span>
[<span data-ttu-id="3baba-129">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="3baba-129">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="3baba-130">Финансы</span><span class="sxs-lookup"><span data-stu-id="3baba-130">Finance</span></span>](finance.md)  
<span data-ttu-id="3baba-131">[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="3baba-131">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
<span data-ttu-id="3baba-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3baba-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

