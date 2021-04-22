---
title: Информация о валюте в России
description: Российские улучшения включают информацию о валюте для импорта курсов валют.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 1e0a6470242658849c79660c0bdd03716e129851
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771367"
---
# <a name="currency-information-import-currency-rates"></a><span data-ttu-id="ccce6-103">Информация о валюте, импорт курсов валют</span><span class="sxs-lookup"><span data-stu-id="ccce6-103">Currency information, Import currency rates</span></span>

<span data-ttu-id="ccce6-104">Информация о местной валюте для печатных форм указана в **Настройка ГК**.</span><span class="sxs-lookup"><span data-stu-id="ccce6-104">Local currency information for printing forms is specified in **General Ledger Setup**.</span></span>

<span data-ttu-id="ccce6-105">Используемые поля на вкладке **Общее**:</span><span class="sxs-lookup"><span data-stu-id="ccce6-105">Used fields on the **General tab**:</span></span>

- <span data-ttu-id="ccce6-106">Код местной валюты</span><span class="sxs-lookup"><span data-stu-id="ccce6-106">LCY Code</span></span>
- <span data-ttu-id="ccce6-107">Описание местной валюты</span><span class="sxs-lookup"><span data-stu-id="ccce6-107">Local currency description</span></span>

### <a name="import-currencies"></a><span data-ttu-id="ccce6-108">Импорт валют</span><span class="sxs-lookup"><span data-stu-id="ccce6-108">Import currencies</span></span>

<span data-ttu-id="ccce6-109">Выберите **Информация об организации**.</span><span class="sxs-lookup"><span data-stu-id="ccce6-109">Go to **Company information**.</span></span> <span data-ttu-id="ccce6-110">Заполните поля:</span><span class="sxs-lookup"><span data-stu-id="ccce6-110">Fill fields:</span></span>

| <span data-ttu-id="ccce6-111">Поле</span><span class="sxs-lookup"><span data-stu-id="ccce6-111">Field</span></span>                          | <span data-ttu-id="ccce6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ccce6-112">Description</span></span>                                                  |
| ------------------------------ | ------------------------------------------------------------ |
| <span data-ttu-id="ccce6-113">**Импорт валютных курсов**</span><span class="sxs-lookup"><span data-stu-id="ccce6-113">**Import Curr. Exch. Rates**</span></span>   | <span data-ttu-id="ccce6-114">Определяет, имеется ли возможность выполнить пакетное задание "Импорт курсов валют".</span><span class="sxs-lookup"><span data-stu-id="ccce6-114">Specifies if it is possible to run the Import Currency Exch. Rate batch job.</span></span> |
| <span data-ttu-id="ccce6-115">**Разрешение конфликтов при импорте**</span><span class="sxs-lookup"><span data-stu-id="ccce6-115">**Import Conflict Resolution**</span></span> | <span data-ttu-id="ccce6-116">Определяет, что произойдет, если пользователь выполнит пакетное задание "Импорт курсов валют" и будут обнаружены конфликтующие курсы валют.</span><span class="sxs-lookup"><span data-stu-id="ccce6-116">Specifies what will happen if a user runs the Import Currency Exch. rate batch job and there are conflicting exchange rates.</span></span> |

<span data-ttu-id="ccce6-117">Выберите **Валюта**.</span><span class="sxs-lookup"><span data-stu-id="ccce6-117">Go to **Currency**.</span></span> <span data-ttu-id="ccce6-118">На вкладке **Общие** заполните поля для каждой валюты:</span><span class="sxs-lookup"><span data-stu-id="ccce6-118">Оn the **General tab** fill fields for each currency:</span></span>

| <span data-ttu-id="ccce6-119">Поле</span><span class="sxs-lookup"><span data-stu-id="ccce6-119">Field</span></span>                    | <span data-ttu-id="ccce6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ccce6-120">Description</span></span>                                                  |
| ------------------------ | ------------------------------------------------------------ |
| <span data-ttu-id="ccce6-121">**Импорт**</span><span class="sxs-lookup"><span data-stu-id="ccce6-121">**Import**</span></span>               | <span data-ttu-id="ccce6-122">Определяет, содержит ли валюта импортированный курс валют.</span><span class="sxs-lookup"><span data-stu-id="ccce6-122">Specifies if the currency has an imported exchange rate.</span></span>     |
| <span data-ttu-id="ccce6-123">**Код банка (Россия)**</span><span class="sxs-lookup"><span data-stu-id="ccce6-123">**Ru Bank Code**</span></span>         | <span data-ttu-id="ccce6-124">Определяет код российского банка, который связан с валютой.</span><span class="sxs-lookup"><span data-stu-id="ccce6-124">Specifies the Russian bank code associated with the currency.</span></span> |
| <span data-ttu-id="ccce6-125">**Цифровой код банка (Россия)**</span><span class="sxs-lookup"><span data-stu-id="ccce6-125">**Ru Bank Digital Code**</span></span> | <span data-ttu-id="ccce6-126">Определяет цифровой код российского банка, который связан с валютой.</span><span class="sxs-lookup"><span data-stu-id="ccce6-126">Specifies the Russian bank digital code associated with the currency.</span></span> |

##### <a name="import-currency-rates"></a><span data-ttu-id="ccce6-127">Импорт курсов валют:</span><span class="sxs-lookup"><span data-stu-id="ccce6-127">Import currency rates:</span></span>

1. <span data-ttu-id="ccce6-128">Выберите Подразделения -> Финансовый менеджмент -> Периодические операции -> Валюта -> Импорт курсов валют.</span><span class="sxs-lookup"><span data-stu-id="ccce6-128">Go to Departments -> Financial management -> Periodic activities -> Currency -> Import currency rates.</span></span>

2. <span data-ttu-id="ccce6-129">Введите даты начала и окончания периода, для которого вы хотите скорректировать обменные курсы.</span><span class="sxs-lookup"><span data-stu-id="ccce6-129">Enter the start and end dates of the period for which you want to adjust the exchange rates.</span></span>

## <a name="see-also"></a><span data-ttu-id="ccce6-130">См. также</span><span class="sxs-lookup"><span data-stu-id="ccce6-130">See Also</span></span>

[<span data-ttu-id="ccce6-131">Коррекция Курс. Разниц</span><span class="sxs-lookup"><span data-stu-id="ccce6-131">Adjust Exchange Rates</span></span>](Adjust-Exchange-Rates.md)  
[<span data-ttu-id="ccce6-132">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="ccce6-132">Russia Local Functionality</span></span>](russia-local-functionality.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]