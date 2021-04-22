---
title: Настройка процентных ставок
description: Узнайте, как настроить Business Central, чтобы вы могли информировать клиентов о дополнительных расходах, отправляя напоминания о финансовых расходах.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment due, debt, overdue, fee, charge
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 08a2443f94efbc9920145109b4b7499a3a4e05b3
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5783626"
---
# <a name="set-up-finance-charge-terms"></a><span data-ttu-id="3d2e6-103">Настройка процентных ставок</span><span class="sxs-lookup"><span data-stu-id="3d2e6-103">Set Up Finance Charge Terms</span></span>

<span data-ttu-id="3d2e6-104">Если клиент не внес оплату в срок, указанный для оплаты, проценты могут быть вычислены автоматически и добавлены к просроченным суммам счета клиента.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-104">When a customer does not pay by the due date, you can have finance charges calculated automatically and add them to the overdue amounts on the customer's account.</span></span> <span data-ttu-id="3d2e6-105">Клиентов можно проинформировать о добавленных процентах путем отправки им процент-нот.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-105">You can inform customers of the added charges by sending finance charge memos.</span></span> <span data-ttu-id="3d2e6-106">Но сначала необходимо настроить код, который представляет расчет каждой процентной ставки.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-106">But first, you must set up a code that represents each finance charge calculation.</span></span> <span data-ttu-id="3d2e6-107">Затем можно ввести этот код в поле "Код процентной ставки" в карточках клиента.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-107">Then you can enter this code in the Fin. Charge Terms Code field on customer cards.</span></span>  

## <a name="finance-charge-terms"></a><span data-ttu-id="3d2e6-108">Процентные ставки</span><span class="sxs-lookup"><span data-stu-id="3d2e6-108">Finance charge terms</span></span>

<span data-ttu-id="3d2e6-109">Вы должны настроить процентные ставки для каждого расчета финансовых сборов, а затем назначить условия клиенту в поле **Код процентной ставки** на странице **Клиент**.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-109">You must set up finance charge terms for each finance charge calculation, and then assign the terms to the customer in the **Fin. Charge Terms Code** field on the **Customer** page.</span></span>

<span data-ttu-id="3d2e6-110">Процент-ноты рассчитываются с использованием методов среднего ежедневного баланса или задолженности.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-110">Finance charges can be calculated using either the average daily balance or the balance due methods.</span></span>

* <span data-ttu-id="3d2e6-111">Среднесуточный остаток</span><span class="sxs-lookup"><span data-stu-id="3d2e6-111">Average daily balance</span></span>  
  
  <span data-ttu-id="3d2e6-112">Принимается во внимание количество дней просрочки оплаты:</span><span class="sxs-lookup"><span data-stu-id="3d2e6-112">The number of days the payment is overdue is taken into account:</span></span>  
  <span data-ttu-id="3d2e6-113">*Метод "Среднесуточный остаток"* - *Процент-нота* = *Сумма просроченного платежа* x *(Просроченные дни / Процентный период)* x *(Процентная ставка/100)*</span><span class="sxs-lookup"><span data-stu-id="3d2e6-113">*Average Daily Balance method* - *Finance Charge* = *Overdue Amount* x *(Days Overdue / Interest Period)* x *(Interest Rate/100)*</span></span>

* <span data-ttu-id="3d2e6-114">Сумма задолженности</span><span class="sxs-lookup"><span data-stu-id="3d2e6-114">Balance due</span></span>  
  
  <span data-ttu-id="3d2e6-115">Сумма процентных выплат — это процент по просроченной сумме:</span><span class="sxs-lookup"><span data-stu-id="3d2e6-115">The finance charge is a percentage of the overdue amount:</span></span>  
  <span data-ttu-id="3d2e6-116">*Метод "Сумма задолженности"* - *Процент-нота* = *Сумма просроченного платежа* x *(Процентная ставка / 100)*</span><span class="sxs-lookup"><span data-stu-id="3d2e6-116">*Balance Due method* - *Finance Charge* = *Overdue Amount* x *(Interest Rate / 100)*</span></span>

<span data-ttu-id="3d2e6-117">Кроме этого, каждое условие в таблице "Процентные ставки" связано с подтаблицей таблицы "Процент-нота - текст".</span><span class="sxs-lookup"><span data-stu-id="3d2e6-117">Additionally, each term in the Finance Charge Terms table is linked to a subtable, the Finance Charge Text table.</span></span> <span data-ttu-id="3d2e6-118">При каждой настройке процентных ставок можно определять начало и/или конец текста, включаемого в процент-ноту.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-118">For each set of finance charge terms, you can define a beginning and/or an ending text to include on the finance charge memo.</span></span>

### <a name="to-set-up-finance-charge-terms"></a><span data-ttu-id="3d2e6-119">Настройка процентных ставок</span><span class="sxs-lookup"><span data-stu-id="3d2e6-119">To set up finance charge terms</span></span>

1. <span data-ttu-id="3d2e6-120">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Процентные ставки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Finance Charge Terms**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3d2e6-121">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-121">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="3d2e6-122">Чтобы использовать более одного сочетания процентных ставок, настройте код для каждой из них.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-122">To use more than one combination of finance charge terms, set up a code for each one.</span></span>

    <span data-ttu-id="3d2e6-123">Для каждой процентной ставки можно указать отдельные условия, которые могут включать дополнительную оплату как в рублях, так и в иностранной валюте.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-123">For each finance charge term, you can specify individual conditions that can include additional fees in both LCY and in foreign currency.</span></span> <span data-ttu-id="3d2e6-124">Для каждого условия на странице **Процентные ставки** можно определить дополнительные сборы в иностранной валюте.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-124">You can define additional fees in foreign currencies for each term on the **Finance Charge Terms** page.</span></span>
4. <span data-ttu-id="3d2e6-125">Выберите действие **Валюты**.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-125">Choose the **Currencies** action.</span></span>
5. <span data-ttu-id="3d2e6-126">На странице **Валюты для процент. ставок** укажите для каждого условия код валюты и дополнительный сбор.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-126">On the **Currencies for Fin. Chrg. Terms** page, define for each term a currency code and an additional fee.</span></span>

    > [!NOTE]  
    > <span data-ttu-id="3d2e6-127">При создании процент-нот в иностранной валюте программой будут использоваться настроенные условия по иностранной валюте.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-127">When you create finance charges in a foreign currency, the foreign currency conditions that you set up here will be used to create finance charge memos.</span></span> <span data-ttu-id="3d2e6-128">Если никаких процентных ставок в иностранной валюте не установлено, будут использоваться процентные ставки в рублях, указанные на странице **Процентные ставки**, и затем конвертироваться в соответствующую валюту.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-128">If there are no foreign currency finance charge conditions set up, the LCY finance charge conditions specified on the **Finance Charge Terms** page will be used and then converted to the relevant currency.</span></span>

    <span data-ttu-id="3d2e6-129">Для каждого условия процентных ставок можно указать текст, который будет распечатан до (**Начальный текст**) или после (**Заключительный текст**) операций процент-ноты.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-129">For each finance charge term, you can specify text that will be printed before (**Beginning Text**) or after (**Ending Text**) on the entries on the finance charge memo.</span></span>  
6. <span data-ttu-id="3d2e6-130">Выберите действие **Начальный текст** или **Заключительный текст** соответственно, а затем заполните страницу **Текст процент-ноты**.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-130">Choose the **Beginning Text** or **Ending Text** actions respectively, and fill on the **Finance Charge Text** page.</span></span>
7. <span data-ttu-id="3d2e6-131">Для автоматической вставки связанных значений в полученный текст процент-ноты введите следующие заполнители в поле **Текст**.</span><span class="sxs-lookup"><span data-stu-id="3d2e6-131">To automatically insert related values in the resulting finance charge text, enter the following placeholders in the **Text** field.</span></span>

|<span data-ttu-id="3d2e6-132">Заполнитель</span><span class="sxs-lookup"><span data-stu-id="3d2e6-132">Placeholder</span></span>|<span data-ttu-id="3d2e6-133">Значение</span><span class="sxs-lookup"><span data-stu-id="3d2e6-133">Value</span></span>|  
|-----------------|-----------|  
|<span data-ttu-id="3d2e6-134">%1</span><span class="sxs-lookup"><span data-stu-id="3d2e6-134">%1</span></span>|<span data-ttu-id="3d2e6-135">Содержимое поля **Дата документа** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="3d2e6-135">Content of the **Document Date** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="3d2e6-136">%2</span><span class="sxs-lookup"><span data-stu-id="3d2e6-136">%2</span></span>|<span data-ttu-id="3d2e6-137">Содержимое поля **Срок оплаты** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="3d2e6-137">Content of the **Due Date** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="3d2e6-138">%3</span><span class="sxs-lookup"><span data-stu-id="3d2e6-138">%3</span></span>|<span data-ttu-id="3d2e6-139">Содержимое поля **Процентная ставка** в связанных процентных ставках</span><span class="sxs-lookup"><span data-stu-id="3d2e6-139">Content of the **Interest Rate** field on the related finance charge terms</span></span>|  
|<span data-ttu-id="3d2e6-140">%4</span><span class="sxs-lookup"><span data-stu-id="3d2e6-140">%4</span></span>|<span data-ttu-id="3d2e6-141">Содержимое поля **Сумма остатка** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="3d2e6-141">Content of the **Remaining Amount** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="3d2e6-142">%5</span><span class="sxs-lookup"><span data-stu-id="3d2e6-142">%5</span></span>|<span data-ttu-id="3d2e6-143">Содержимое поля **Сумма процентов** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="3d2e6-143">Content of the **Interest Amount** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="3d2e6-144">%6</span><span class="sxs-lookup"><span data-stu-id="3d2e6-144">%6</span></span>|<span data-ttu-id="3d2e6-145">Содержимое поля **Дополнительный сбор** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="3d2e6-145">Content of the **Additional Fee** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="3d2e6-146">%7</span><span class="sxs-lookup"><span data-stu-id="3d2e6-146">%7</span></span>|<span data-ttu-id="3d2e6-147">Итоговая сумма напоминания</span><span class="sxs-lookup"><span data-stu-id="3d2e6-147">The total amount of the reminder</span></span>|  
|<span data-ttu-id="3d2e6-148">%8</span><span class="sxs-lookup"><span data-stu-id="3d2e6-148">%8</span></span>|<span data-ttu-id="3d2e6-149">Содержимое поля **Код валюты** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="3d2e6-149">Content of the **Currency Code** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="3d2e6-150">%9</span><span class="sxs-lookup"><span data-stu-id="3d2e6-150">%9</span></span>|<span data-ttu-id="3d2e6-151">Содержимое поля **Дата учета** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="3d2e6-151">Content of the **Posting Date** field on the finance charge memo header</span></span>|  

## <a name="see-also"></a><span data-ttu-id="3d2e6-152">См. также</span><span class="sxs-lookup"><span data-stu-id="3d2e6-152">See also</span></span>

[<span data-ttu-id="3d2e6-153">Сбор непогашенных остатков задолженности</span><span class="sxs-lookup"><span data-stu-id="3d2e6-153">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="3d2e6-154">Настройка условий и уровней напоминаний</span><span class="sxs-lookup"><span data-stu-id="3d2e6-154">Set Up Reminder Terms and Levels</span></span>](finance-setup-reminders.md)  
[<span data-ttu-id="3d2e6-155">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="3d2e6-155">Setting Up Finance</span></span>](finance-setup-finance.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]