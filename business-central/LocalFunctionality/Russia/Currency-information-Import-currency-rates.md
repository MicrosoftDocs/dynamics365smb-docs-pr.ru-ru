---
title: Информация о валюте в России
description: Российские улучшения включают информацию о валюте для импорта курсов валют.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 2c3b8151598865eac1a3405322e688a1e4df3ab8
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3921314"
---
# <a name="currency-information-import-currency-rates"></a><span data-ttu-id="71b57-103">Информация о валюте, импорт курсов валют</span><span class="sxs-lookup"><span data-stu-id="71b57-103">Currency information, Import currency rates</span></span>

<span data-ttu-id="71b57-104">Информация о местной валюте для печатных форм указана в **Настройка ГК**.</span><span class="sxs-lookup"><span data-stu-id="71b57-104">Local currency information for printing forms is specified in **General Ledger Setup**.</span></span>

<span data-ttu-id="71b57-105">Используемые поля на вкладке **Общее**:</span><span class="sxs-lookup"><span data-stu-id="71b57-105">Used fields on the **General tab**:</span></span>

- <span data-ttu-id="71b57-106">Код местной валюты</span><span class="sxs-lookup"><span data-stu-id="71b57-106">LCY Code</span></span>
- <span data-ttu-id="71b57-107">Описание местной валюты</span><span class="sxs-lookup"><span data-stu-id="71b57-107">Local currency description</span></span>

### <a name="import-currencies"></a><span data-ttu-id="71b57-108">Импорт валют</span><span class="sxs-lookup"><span data-stu-id="71b57-108">Import currencies</span></span>

<span data-ttu-id="71b57-109">Выберите **Информация об организации**.</span><span class="sxs-lookup"><span data-stu-id="71b57-109">Go to **Company information**.</span></span> <span data-ttu-id="71b57-110">Заполните поля:</span><span class="sxs-lookup"><span data-stu-id="71b57-110">Fill fields:</span></span>

| <span data-ttu-id="71b57-111">Поле</span><span class="sxs-lookup"><span data-stu-id="71b57-111">Field</span></span>                          | <span data-ttu-id="71b57-112">Описание</span><span class="sxs-lookup"><span data-stu-id="71b57-112">Description</span></span>                                                  |
| ------------------------------ | ------------------------------------------------------------ |
| <span data-ttu-id="71b57-113">**Импорт валютных курсов**</span><span class="sxs-lookup"><span data-stu-id="71b57-113">**Import Curr. Exch. Rates**</span></span>   | <span data-ttu-id="71b57-114">Определяет, имеется ли возможность выполнить пакетное задание "Импорт курсов валют".</span><span class="sxs-lookup"><span data-stu-id="71b57-114">Specifies if it is possible to run the Import Currency Exch. Rate batch job.</span></span> |
| <span data-ttu-id="71b57-115">**Разрешение конфликтов при импорте**</span><span class="sxs-lookup"><span data-stu-id="71b57-115">**Import Conflict Resolution**</span></span> | <span data-ttu-id="71b57-116">Определяет, что произойдет, если пользователь выполнит пакетное задание "Импорт курсов валют" и будут обнаружены конфликтующие курсы валют.</span><span class="sxs-lookup"><span data-stu-id="71b57-116">Specifies what will happen if a user runs the Import Currency Exch. rate batch job and there are conflicting exchange rates.</span></span> |

<span data-ttu-id="71b57-117">Выберите **Валюта**.</span><span class="sxs-lookup"><span data-stu-id="71b57-117">Go to **Currency**.</span></span> <span data-ttu-id="71b57-118">На вкладке **Общие** заполните поля для каждой валюты:</span><span class="sxs-lookup"><span data-stu-id="71b57-118">Оn the **General tab** fill fields for each currency:</span></span>

| <span data-ttu-id="71b57-119">Поле</span><span class="sxs-lookup"><span data-stu-id="71b57-119">Field</span></span>                    | <span data-ttu-id="71b57-120">Описание</span><span class="sxs-lookup"><span data-stu-id="71b57-120">Description</span></span>                                                  |
| ------------------------ | ------------------------------------------------------------ |
| <span data-ttu-id="71b57-121">**Импорт**</span><span class="sxs-lookup"><span data-stu-id="71b57-121">**Import**</span></span>               | <span data-ttu-id="71b57-122">Определяет, содержит ли валюта импортированный курс валют.</span><span class="sxs-lookup"><span data-stu-id="71b57-122">Specifies if the currency has an imported exchange rate.</span></span>     |
| <span data-ttu-id="71b57-123">**Код банка (Россия)**</span><span class="sxs-lookup"><span data-stu-id="71b57-123">**Ru Bank Code**</span></span>         | <span data-ttu-id="71b57-124">Определяет код российского банка, который связан с валютой.</span><span class="sxs-lookup"><span data-stu-id="71b57-124">Specifies the Russian bank code associated with the currency.</span></span> |
| <span data-ttu-id="71b57-125">**Цифровой код банка (Россия)**</span><span class="sxs-lookup"><span data-stu-id="71b57-125">**Ru Bank Digital Code**</span></span> | <span data-ttu-id="71b57-126">Определяет цифровой код российского банка, который связан с валютой.</span><span class="sxs-lookup"><span data-stu-id="71b57-126">Specifies the Russian bank digital code associated with the currency.</span></span> |

##### <a name="import-currency-rates"></a><span data-ttu-id="71b57-127">Импорт курсов валют:</span><span class="sxs-lookup"><span data-stu-id="71b57-127">Import currency rates:</span></span>

1. <span data-ttu-id="71b57-128">Выберите Подразделения -> Финансовый менеджмент -> Периодические операции -> Валюта -> Импорт курсов валют.</span><span class="sxs-lookup"><span data-stu-id="71b57-128">Go to Departments -> Financial management -> Periodic activities -> Currency -> Import currency rates.</span></span>

2. <span data-ttu-id="71b57-129">Введите даты начала и окончания периода, для которого вы хотите скорректировать обменные курсы.</span><span class="sxs-lookup"><span data-stu-id="71b57-129">Enter the start and end dates of the period for which you want to adjust the exchange rates.</span></span>

## <a name="see-also"></a><span data-ttu-id="71b57-130">См. также</span><span class="sxs-lookup"><span data-stu-id="71b57-130">See Also</span></span>

[<span data-ttu-id="71b57-131">Коррекция Курс. Разниц</span><span class="sxs-lookup"><span data-stu-id="71b57-131">Adjust Exchange Rates</span></span>](Adjust-Exchange-Rates.md)  
[<span data-ttu-id="71b57-132">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="71b57-132">Russia Local Functionality</span></span>](russia-local-functionality.md)  
