---
title: Корректировка валютных курсов в России
description: Российские усовершенствования включают корректировку валютных курсов.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: b1445c2e69e4c72f8ac8638885614fc7e273e844
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738284"
---
# <a name="adjust-exchange-rates"></a><span data-ttu-id="0af63-103">Корректировка валютных курсов</span><span class="sxs-lookup"><span data-stu-id="0af63-103">Adjust Exchange Rates</span></span>

<span data-ttu-id="0af63-104">Разница для между российской и международной функцией — российский отчет создает корректировочную операцию для каждой операции Поставщика и Клиента и использует учетную группу из операции не из карточки Продавца и Клиента.</span><span class="sxs-lookup"><span data-stu-id="0af63-104">The difference for Russian task and worldwide task - Russian report create adjustment entry for every Vendor and Customer entry and uses posting group from entry not from Vendor and Customer card.</span></span>

1. <span data-ttu-id="0af63-105">Выберите **Коррекция Курс. Разниц**.</span><span class="sxs-lookup"><span data-stu-id="0af63-105">Go to **Adjust Exchange Rates**.</span></span>

2.  <span data-ttu-id="0af63-106">Заполните поля:</span><span class="sxs-lookup"><span data-stu-id="0af63-106">Fill the fields:</span></span>

   | <span data-ttu-id="0af63-107">Поле</span><span class="sxs-lookup"><span data-stu-id="0af63-107">Field</span></span>                                           | <span data-ttu-id="0af63-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0af63-108">Description</span></span>                                                  |
   | ----------------------------------------------- | ------------------------------------------------------------ |
   | <span data-ttu-id="0af63-109">Дата начала</span><span class="sxs-lookup"><span data-stu-id="0af63-109">Starting Date</span></span>                                   | <span data-ttu-id="0af63-110">Определяет начало периода, операции за который должны быть скорректированы. Как правило, поле оставляется пустым, но вы можете указать дату.</span><span class="sxs-lookup"><span data-stu-id="0af63-110">Specifies the beginning of the period for which entries are adjusted.This field is usually left blank, but you can enter a date.</span></span> |
   | <span data-ttu-id="0af63-111">Дата окончания</span><span class="sxs-lookup"><span data-stu-id="0af63-111">Ending Date</span></span>                                     | <span data-ttu-id="0af63-112">Определяет дату, до которой информация будет обрабатываться отчетом или пакетным заданием.</span><span class="sxs-lookup"><span data-stu-id="0af63-112">Specifies the date to which the report or batch job processes information.</span></span> |
   | <span data-ttu-id="0af63-113">Описание учета</span><span class="sxs-lookup"><span data-stu-id="0af63-113">Posting Description</span></span>                             | <span data-ttu-id="0af63-114">Определяет текст для операций главной книги, создаваемых с помощью пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="0af63-114">Specifies text for the general ledger entries that are created by the batch job.</span></span> <span data-ttu-id="0af63-115">Текст по умолчанию — Коррекция валютного курса для %1 %2, где %1 заменяется кодом валюты, а %2 — корректируемой валютной суммой.</span><span class="sxs-lookup"><span data-stu-id="0af63-115">The default text is Exchange Rate Adjmt. of %1 %2, in which %1 is replaced by the currency code and %2 is replaced by the currency amount that is adjusted.</span></span> <span data-ttu-id="0af63-116">Например, Коррекция валютного курса для DEM 38000.</span><span class="sxs-lookup"><span data-stu-id="0af63-116">For example, Exchange Rate Adjmt. of DEM 38,000.</span></span> |
   | <span data-ttu-id="0af63-117">Дата учета</span><span class="sxs-lookup"><span data-stu-id="0af63-117">Posting Date</span></span>                                    | <span data-ttu-id="0af63-118">Определяет дату учета операций, которые следует включить в отчет или пакетное задание.</span><span class="sxs-lookup"><span data-stu-id="0af63-118">Specifies the posting date of the entries that you want to include in the report or batch job.</span></span> |
   | <span data-ttu-id="0af63-119">Номер документа</span><span class="sxs-lookup"><span data-stu-id="0af63-119">Document No.</span></span>                                    | <span data-ttu-id="0af63-120">Определяет номер документа, который будет отображаться в операциях главной книги, создаваемых пакетным заданием.</span><span class="sxs-lookup"><span data-stu-id="0af63-120">Specifies the document number that will appear on the general ledger entries that are created by the batch job.</span></span> |
   | <span data-ttu-id="0af63-121">Коррекция счетов ГК по доп. отчетной валюте</span><span class="sxs-lookup"><span data-stu-id="0af63-121">Adjust G/L Accounts for Add.-Reporting Currency</span></span> | <span data-ttu-id="0af63-122">Указывает, нужно ли выполнять учет в дополнительной отчетной валюте и корректировать счета главной книги в связи с колебаниями курса местной валюты относительно дополнительной отчетной валюты.</span><span class="sxs-lookup"><span data-stu-id="0af63-122">Specifies if you want to post in an additional reporting currency and adjust general ledger accounts for currency fluctuations between LCY and the additional reporting currency.</span></span> |
   | <span data-ttu-id="0af63-123">Коррекция банк. счетов</span><span class="sxs-lookup"><span data-stu-id="0af63-123">Adjust Bank Accounts</span></span>                            | <span data-ttu-id="0af63-124">Указывает, требуется ли применять корректировку</span><span class="sxs-lookup"><span data-stu-id="0af63-124">Specifies if you want to adjust</span></span>                              |
   | <span data-ttu-id="0af63-125">Коррекция клиентов</span><span class="sxs-lookup"><span data-stu-id="0af63-125">Adjust Customer</span></span>                                 | <span data-ttu-id="0af63-126">Указывает, требуется ли применять корректировку к операциям клиентов</span><span class="sxs-lookup"><span data-stu-id="0af63-126">Specifies if you want to adjust customer entries</span></span>             |
   | <span data-ttu-id="0af63-127">Коррекция поставщиков</span><span class="sxs-lookup"><span data-stu-id="0af63-127">Adjust Vendor</span></span>                                   | <span data-ttu-id="0af63-128">Указывает, требуется ли применять корректировку к операциям поставщиков</span><span class="sxs-lookup"><span data-stu-id="0af63-128">Specifies if you want to adjust vendor entries</span></span>               |

   3. <span data-ttu-id="0af63-129">Щелкните ОК.</span><span class="sxs-lookup"><span data-stu-id="0af63-129">Click "Ok".</span></span>
   
   ## <a name="see-also"></a><span data-ttu-id="0af63-130">См. также</span><span class="sxs-lookup"><span data-stu-id="0af63-130">See Also</span></span> 

[<span data-ttu-id="0af63-131">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="0af63-131">Russia Local Functionality</span></span>](russia-local-functionality.md)
