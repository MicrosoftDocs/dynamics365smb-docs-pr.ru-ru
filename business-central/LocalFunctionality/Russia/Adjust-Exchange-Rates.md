---
title: Корректировка валютных курсов в России
description: Российские усовершенствования включают корректировку валютных курсов.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 83038da9c11dc0e1668527e49ceb7484c8759805
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301203"
---
# <a name="adjust-exchange-rates"></a><span data-ttu-id="4827d-103">Корректировка валютных курсов</span><span class="sxs-lookup"><span data-stu-id="4827d-103">Adjust Exchange Rates</span></span>

<span data-ttu-id="4827d-104">Разница для между российской и международной функцией — российский отчет создает корректировочную операцию для каждой операции Поставщика и Клиента и использует учетную группу из операции не из карточки Продавца и Клиента.</span><span class="sxs-lookup"><span data-stu-id="4827d-104">The difference for Russian task and worldwide task - Russian report create adjustment entry for every Vendor and Customer entry and uses posting group from entry not from Vendor and Customer card.</span></span>

1. <span data-ttu-id="4827d-105">Выберите **Коррекция Курс. Разниц**.</span><span class="sxs-lookup"><span data-stu-id="4827d-105">Go to **Adjust Exchange Rates**.</span></span>

2.  <span data-ttu-id="4827d-106">Заполните поля:</span><span class="sxs-lookup"><span data-stu-id="4827d-106">Fill the fields:</span></span>

   | <span data-ttu-id="4827d-107">Поле</span><span class="sxs-lookup"><span data-stu-id="4827d-107">Field</span></span>                                           | <span data-ttu-id="4827d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4827d-108">Description</span></span>                                                  |
   | ----------------------------------------------- | ------------------------------------------------------------ |
   | <span data-ttu-id="4827d-109">Дата начала</span><span class="sxs-lookup"><span data-stu-id="4827d-109">Starting Date</span></span>                                   | <span data-ttu-id="4827d-110">Определяет начало периода, операции за который должны быть скорректированы. Как правило, поле оставляется пустым, но вы можете указать дату.</span><span class="sxs-lookup"><span data-stu-id="4827d-110">Specifies the beginning of the period for which entries are adjusted.This field is usually left blank, but you can enter a date.</span></span> |
   | <span data-ttu-id="4827d-111">Дата окончания</span><span class="sxs-lookup"><span data-stu-id="4827d-111">Ending Date</span></span>                                     | <span data-ttu-id="4827d-112">Определяет дату, до которой информация будет обрабатываться отчетом или пакетным заданием.</span><span class="sxs-lookup"><span data-stu-id="4827d-112">Specifies the date to which the report or batch job processes information.</span></span> |
   | <span data-ttu-id="4827d-113">Описание учета</span><span class="sxs-lookup"><span data-stu-id="4827d-113">Posting Description</span></span>                             | <span data-ttu-id="4827d-114">Определяет текст для операций главной книги, создаваемых с помощью пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="4827d-114">Specifies text for the general ledger entries that are created by the batch job.</span></span> <span data-ttu-id="4827d-115">Текст по умолчанию — Коррекция валютного курса для %1 %2, где %1 заменяется кодом валюты, а %2 — корректируемой валютной суммой.</span><span class="sxs-lookup"><span data-stu-id="4827d-115">The default text is Exchange Rate Adjmt. of %1 %2, in which %1 is replaced by the currency code and %2 is replaced by the currency amount that is adjusted.</span></span> <span data-ttu-id="4827d-116">Например, Коррекция валютного курса для DEM 38000.</span><span class="sxs-lookup"><span data-stu-id="4827d-116">For example, Exchange Rate Adjmt. of DEM 38,000.</span></span> |
   | <span data-ttu-id="4827d-117">Дата учета</span><span class="sxs-lookup"><span data-stu-id="4827d-117">Posting Date</span></span>                                    | <span data-ttu-id="4827d-118">Определяет дату учета операций, которые следует включить в отчет или пакетное задание.</span><span class="sxs-lookup"><span data-stu-id="4827d-118">Specifies the posting date of the entries that you want to include in the report or batch job.</span></span> |
   | <span data-ttu-id="4827d-119">Номер документа</span><span class="sxs-lookup"><span data-stu-id="4827d-119">Document No.</span></span>                                    | <span data-ttu-id="4827d-120">Определяет номер документа, который будет отображаться в операциях главной книги, создаваемых пакетным заданием.</span><span class="sxs-lookup"><span data-stu-id="4827d-120">Specifies the document number that will appear on the general ledger entries that are created by the batch job.</span></span> |
   | <span data-ttu-id="4827d-121">Коррекция счетов ГК по доп. отчетной валюте</span><span class="sxs-lookup"><span data-stu-id="4827d-121">Adjust G/L Accounts for Add.-Reporting Currency</span></span> | <span data-ttu-id="4827d-122">Указывает, нужно ли выполнять учет в дополнительной отчетной валюте и корректировать счета главной книги в связи с колебаниями курса местной валюты относительно дополнительной отчетной валюты.</span><span class="sxs-lookup"><span data-stu-id="4827d-122">Specifies if you want to post in an additional reporting currency and adjust general ledger accounts for currency fluctuations between LCY and the additional reporting currency.</span></span> |
   | <span data-ttu-id="4827d-123">Коррекция банк. счетов</span><span class="sxs-lookup"><span data-stu-id="4827d-123">Adjust Bank Accounts</span></span>                            | <span data-ttu-id="4827d-124">Указывает, требуется ли применять корректировку</span><span class="sxs-lookup"><span data-stu-id="4827d-124">Specifies if you want to adjust</span></span>                              |
   | <span data-ttu-id="4827d-125">Коррекция клиентов</span><span class="sxs-lookup"><span data-stu-id="4827d-125">Adjust Customer</span></span>                                 | <span data-ttu-id="4827d-126">Указывает, требуется ли применять корректировку к операциям клиентов</span><span class="sxs-lookup"><span data-stu-id="4827d-126">Specifies if you want to adjust customer entries</span></span>             |
   | <span data-ttu-id="4827d-127">Коррекция поставщиков</span><span class="sxs-lookup"><span data-stu-id="4827d-127">Adjust Vendor</span></span>                                   | <span data-ttu-id="4827d-128">Указывает, требуется ли применять корректировку к операциям поставщиков</span><span class="sxs-lookup"><span data-stu-id="4827d-128">Specifies if you want to adjust vendor entries</span></span>               |

   3. <span data-ttu-id="4827d-129">Щелкните ОК.</span><span class="sxs-lookup"><span data-stu-id="4827d-129">Click "Ok".</span></span>
   
   ## <a name="see-also"></a><span data-ttu-id="4827d-130">См. также</span><span class="sxs-lookup"><span data-stu-id="4827d-130">See Also</span></span> 

[<span data-ttu-id="4827d-131">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="4827d-131">Russia Local Functionality</span></span>](russia-local-functionality.md)
