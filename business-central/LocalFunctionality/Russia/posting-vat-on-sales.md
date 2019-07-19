---
title: Учет НДС в продажах в России
description: Российские улучшения включают НДС в документах продажи.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: c999dd07d66fb13dcdceea43f4b6e11044b97c15
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738210"
---
# <a name="posting-vat-on-sales"></a><span data-ttu-id="6a810-103">Учет НДС в продажах</span><span class="sxs-lookup"><span data-stu-id="6a810-103">Posting VAT on Sales</span></span>

<span data-ttu-id="6a810-104">В окно **Настройка учета НДС** (код 472) были добавлены следующие поля:</span><span class="sxs-lookup"><span data-stu-id="6a810-104">The following fields have been added to the **VAT Posting Setup** window (ID 472):</span></span>

| <span data-ttu-id="6a810-105">Поле</span><span class="sxs-lookup"><span data-stu-id="6a810-105">Field</span></span>                       | <span data-ttu-id="6a810-106">Описание</span><span class="sxs-lookup"><span data-stu-id="6a810-106">Description</span></span>                                                  |
| :-------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="6a810-107">**Тип транз. НДС**</span><span class="sxs-lookup"><span data-stu-id="6a810-107">**Trans. VAT Type**</span></span>         | <span data-ttu-id="6a810-108">Используется для определения правила выделения НДС.</span><span class="sxs-lookup"><span data-stu-id="6a810-108">Used to define the rule for extracting VAT.</span></span>                  |
| <span data-ttu-id="6a810-109">**НДС транз. счет ГК**</span><span class="sxs-lookup"><span data-stu-id="6a810-109">**Trans. VAT Account**</span></span>      | <span data-ttu-id="6a810-110">Используется для указания счета регистрации суммы НДС от реализации и предоплат клиента, которая должна уплачиваться в федеральный бюджет.</span><span class="sxs-lookup"><span data-stu-id="6a810-110">Used to specify an account to register the VAT amount from the gain and from the customer's prepayments to be paid to the federal budget.</span></span> |
| <span data-ttu-id="6a810-111">**Тип суммы для счета-фактуры**</span><span class="sxs-lookup"><span data-stu-id="6a810-111">**Tax Invoice Amount Type**</span></span> | <span data-ttu-id="6a810-112">Используется для выбора значения НДС.</span><span class="sxs-lookup"><span data-stu-id="6a810-112">Used to select the value of VAT.</span></span> <span data-ttu-id="6a810-113">В зависимости от значения в этом поле введенные суммы НДС используются в разных столбцах книг НДС покупок или продаж.</span><span class="sxs-lookup"><span data-stu-id="6a810-113">Depending on the value in this field, VAT entry amounts are used in different columns of the VAT purchase or sales ledgers.</span></span> |

<span data-ttu-id="6a810-114">Указанные действия выполняются для каждой комбинации учетной группы НДС продаж продукта и учетной группы НДС продаж.</span><span class="sxs-lookup"><span data-stu-id="6a810-114">The above actions are taken for each combination of the Sales VAT Product posting group and Sales VAT posting group.</span></span> 

<span data-ttu-id="6a810-115">Для поля **Тип транз. НДС** возможны следующие значения:</span><span class="sxs-lookup"><span data-stu-id="6a810-115">In the **Trans. VAT Type** field, the following options are available:</span></span>

- <span data-ttu-id="6a810-116">**Сумма + налог**</span><span class="sxs-lookup"><span data-stu-id="6a810-116">**Amount + Tax**</span></span>
- <span data-ttu-id="6a810-117">**Сумма и налог**</span><span class="sxs-lookup"><span data-stu-id="6a810-117">**Amount & Tax**</span></span>

<span data-ttu-id="6a810-118">Для учета НДС выберите действие **Сумма + налог**.</span><span class="sxs-lookup"><span data-stu-id="6a810-118">To account for VAT, choose the **Amount + Tax** action.</span></span>

<span data-ttu-id="6a810-119">Ниже приводится процедура создания бухгалтерских проводок.</span><span class="sxs-lookup"><span data-stu-id="6a810-119">The following procedure shows how the accounting entries are created.</span></span>

1. <span data-ttu-id="6a810-120">Введите в поле **Номер счета НДС транз.** значение "Субсчет 90-3, Налог на добавленную стоимость".</span><span class="sxs-lookup"><span data-stu-id="6a810-120">In the **Trans. VAT Account No.** field, enter Subaccount 90-3, Gain VAT.</span></span>
2. <span data-ttu-id="6a810-121">В поле **Счет НДС продаж** введите "Субсчет 68, Расчеты по налогам и сборам".</span><span class="sxs-lookup"><span data-stu-id="6a810-121">In the **Sales VAT Account** field, enter Subaccount 68, VAT to Federal Budget.</span></span>

<span data-ttu-id="6a810-122">Следующие бухгалтерские проводки создают различные настройки.</span><span class="sxs-lookup"><span data-stu-id="6a810-122">The following accounting entries create the different settings.</span></span>

 

| <span data-ttu-id="6a810-123">Бухгалтерские проводки</span><span class="sxs-lookup"><span data-stu-id="6a810-123">Accounting Entries</span></span> | <span data-ttu-id="6a810-124">Параметры</span><span class="sxs-lookup"><span data-stu-id="6a810-124">Settings</span></span>                                                     |
| :----------------- | :----------------------------------------------------------- |
| <span data-ttu-id="6a810-125">**Сумма + налог**</span><span class="sxs-lookup"><span data-stu-id="6a810-125">**Amount + Tax**</span></span>   | <span data-ttu-id="6a810-126">Дебет 62 Поступления и платежи - Кредит 90-1 выручка от продажи   Дебет 90-3 Налог на добавленную стоимость   Кредит 68 Расчеты по налогам и сборам   Сумма НДС продаж</span><span class="sxs-lookup"><span data-stu-id="6a810-126">Debit 62 Payables and Receivables - Credit 90-1 Gain and Sales Amount Including VAT   Debit 90-3 Gain VAT   Credit 68 VAT to Federal Budget   Sales VAT Amount</span></span> |
| <span data-ttu-id="6a810-127">**Сумма и налог**</span><span class="sxs-lookup"><span data-stu-id="6a810-127">**Amount & Tax**</span></span>   | <span data-ttu-id="6a810-128">Дебет 62 Поступления и платежи   Кредит 90-1 Прибыль   Сумма Без НДС   Дебет 62 Поступления и платежи   Кредит 90-3 Налог на добавленную стоимость   Сумма НДС продаж   Дебет 90-3 Налог на добавленную стоимость   Кредит 68 Расчеты по налогам и сборам   Сумма НДС продаж</span><span class="sxs-lookup"><span data-stu-id="6a810-128">Debit 62 Payables and Receivables   Credit 90-1 Gain   Amount Excluding VAT   Debit 62 Payables and Receivables   Credit 90-3 Gain VAT   Sales VAT Amount   Debit 90-3 Gain VAT   Credit 68 VAT to Budget   Sales VAT amount</span></span> |
|                    | <span data-ttu-id="6a810-129">Дебет 62 Поступления и платежи   Кредит 90-1 Прибыль   Сумма Без НДС   Дебет 62 Поступления и платежи   Кредит 68 Расчеты по налогам и сборам   Сумма НДС продаж</span><span class="sxs-lookup"><span data-stu-id="6a810-129">Debit 62 Payables and Receivables   Credit 90-1 Gain   Amount Excluding VAT   Debit 62 Payables and Receivables   Credit 68 VAT to Budget   Sales VAT Amount</span></span> |

## <a name="trans-vat-account-field"></a><span data-ttu-id="6a810-130">Поле "НДС транз. счет ГК"</span><span class="sxs-lookup"><span data-stu-id="6a810-130">Trans. VAT Account Field</span></span>

<span data-ttu-id="6a810-131">В поле **НДС транз. счет ГК** введите субсчет 90-3, "Налог на добавленную стоимость", или субсчет 62 "НДС по предоплате".</span><span class="sxs-lookup"><span data-stu-id="6a810-131">In the **Trans. VAT Account** field, enter Subaccount 90-3 Gain VAT or Subaccount 62 Prepayment VAT.</span></span> <span data-ttu-id="6a810-132">Если это поле пустое, для учета будет использоваться счет из учетных групп клиентов из поля **Счет дебиторской задолженности**.</span><span class="sxs-lookup"><span data-stu-id="6a810-132">If this field is blank, the postings use the account from the Customer posting groups from the **Receivables Account** field.</span></span>

## <a name="see-also"></a><span data-ttu-id="6a810-133">См. также</span><span class="sxs-lookup"><span data-stu-id="6a810-133">See Also</span></span>

[<span data-ttu-id="6a810-134">Книги НДС</span><span class="sxs-lookup"><span data-stu-id="6a810-134">VAT Ledgers</span></span>](VAT-Ledgers.md)  