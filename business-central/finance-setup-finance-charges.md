---
title: Настройка процентных ставок
description: Узнайте, как настроить Business Central, чтобы вы могли информировать клиентов о дополнительных расходах, отправляя напоминания о финансовых расходах.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment due, debt, overdue, fee, charge
ms.date: 12/03/2020
ms.author: edupont
ms.openlocfilehash: aba5ca8eb9425c11c7f8a55a08a153ee18821632
ms.sourcegitcommit: 06bfb3aa59de50d983175e68e681b9d206423242
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "4672000"
---
# <a name="set-up-finance-charge-terms"></a><span data-ttu-id="ac754-103">Настройка процентных ставок</span><span class="sxs-lookup"><span data-stu-id="ac754-103">Set Up Finance Charge Terms</span></span>

<span data-ttu-id="ac754-104">Если клиент не внес оплату в срок, указанный для оплаты, проценты могут быть вычислены автоматически и добавлены к просроченным суммам счета клиента.</span><span class="sxs-lookup"><span data-stu-id="ac754-104">When a customer does not pay by the due date, you can have finance charges calculated automatically and add them to the overdue amounts on the customer's account.</span></span> <span data-ttu-id="ac754-105">Клиентов можно проинформировать о добавленных процентах путем отправки им процент-нот.</span><span class="sxs-lookup"><span data-stu-id="ac754-105">You can inform customers of the added charges by sending finance charge memos.</span></span> <span data-ttu-id="ac754-106">Но сначала необходимо настроить код, который представляет расчет каждой процентной ставки.</span><span class="sxs-lookup"><span data-stu-id="ac754-106">But first, you must set up a code that represents each finance charge calculation.</span></span> <span data-ttu-id="ac754-107">Затем можно ввести этот код в поле "Код процентной ставки" в карточках клиента.</span><span class="sxs-lookup"><span data-stu-id="ac754-107">Then you can enter this code in the Fin. Charge Terms Code field on customer cards.</span></span>  

## <a name="finance-charge-terms"></a><span data-ttu-id="ac754-108">Процентные ставки</span><span class="sxs-lookup"><span data-stu-id="ac754-108">Finance charge terms</span></span>

<span data-ttu-id="ac754-109">Вы должны настроить процентные ставки для каждого расчета финансовых сборов, а затем назначить условия клиенту в поле **Код процентной ставки** на странице **Клиент**.</span><span class="sxs-lookup"><span data-stu-id="ac754-109">You must set up finance charge terms for each finance charge calculation, and then assign the terms to the customer in the **Fin. Charge Terms Code** field on the **Customer** page.</span></span>

<span data-ttu-id="ac754-110">Процент-ноты рассчитываются с использованием методов среднего ежедневного баланса или задолженности.</span><span class="sxs-lookup"><span data-stu-id="ac754-110">Finance charges can be calculated using either the average daily balance or the balance due methods.</span></span>

* <span data-ttu-id="ac754-111">Среднесуточный остаток</span><span class="sxs-lookup"><span data-stu-id="ac754-111">Average daily balance</span></span>  
  
  <span data-ttu-id="ac754-112">Принимается во внимание количество дней просрочки оплаты:</span><span class="sxs-lookup"><span data-stu-id="ac754-112">The number of days the payment is overdue is taken into account:</span></span>  
  <span data-ttu-id="ac754-113">*Метод "Среднесуточный остаток"* - *Процент-нота* = *Сумма просроченного платежа* x *(Просроченные дни / Процентный период)* x *(Процентная ставка/100)*</span><span class="sxs-lookup"><span data-stu-id="ac754-113">*Average Daily Balance method* - *Finance Charge* = *Overdue Amount* x *(Days Overdue / Interest Period)* x *(Interest Rate/100)*</span></span>

* <span data-ttu-id="ac754-114">Сумма задолженности</span><span class="sxs-lookup"><span data-stu-id="ac754-114">Balance due</span></span>  
  
  <span data-ttu-id="ac754-115">Сумма процентных выплат — это процент по просроченной сумме:</span><span class="sxs-lookup"><span data-stu-id="ac754-115">The finance charge is a percentage of the overdue amount:</span></span>  
  <span data-ttu-id="ac754-116">*Метод "Сумма задолженности"* - *Процент-нота* = *Сумма просроченного платежа* x *(Процентная ставка / 100)*</span><span class="sxs-lookup"><span data-stu-id="ac754-116">*Balance Due method* - *Finance Charge* = *Overdue Amount* x *(Interest Rate / 100)*</span></span>

<span data-ttu-id="ac754-117">Кроме этого, каждое условие в таблице "Процентные ставки" связано с подтаблицей таблицы "Процент-нота - текст".</span><span class="sxs-lookup"><span data-stu-id="ac754-117">Additionally, each term in the Finance Charge Terms table is linked to a subtable, the Finance Charge Text table.</span></span> <span data-ttu-id="ac754-118">При каждой настройке процентных ставок можно определять начало и/или конец текста, включаемого в процент-ноту.</span><span class="sxs-lookup"><span data-stu-id="ac754-118">For each set of finance charge terms, you can define a beginning and/or an ending text to include on the finance charge memo.</span></span>

### <a name="to-set-up-finance-charge-terms"></a><span data-ttu-id="ac754-119">Настройка процентных ставок</span><span class="sxs-lookup"><span data-stu-id="ac754-119">To set up finance charge terms</span></span>

1. <span data-ttu-id="ac754-120">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Процентные ставки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="ac754-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Finance Charge Terms**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ac754-121">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="ac754-121">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="ac754-122">Чтобы использовать более одного сочетания процентных ставок, настройте код для каждой из них.</span><span class="sxs-lookup"><span data-stu-id="ac754-122">To use more than one combination of finance charge terms, set up a code for each one.</span></span>

    <span data-ttu-id="ac754-123">Для каждой процентной ставки можно указать отдельные условия, которые могут включать дополнительную оплату как в рублях, так и в иностранной валюте.</span><span class="sxs-lookup"><span data-stu-id="ac754-123">For each finance charge term, you can specify individual conditions that can include additional fees in both LCY and in foreign currency.</span></span> <span data-ttu-id="ac754-124">Для каждого условия на странице **Процентные ставки** можно определить дополнительные сборы в иностранной валюте.</span><span class="sxs-lookup"><span data-stu-id="ac754-124">You can define additional fees in foreign currencies for each term on the **Finance Charge Terms** page.</span></span>
4. <span data-ttu-id="ac754-125">Выберите действие **Валюты**.</span><span class="sxs-lookup"><span data-stu-id="ac754-125">Choose the **Currencies** action.</span></span>
5. <span data-ttu-id="ac754-126">На странице **Валюты для процент. ставок** укажите для каждого условия код валюты и дополнительный сбор.</span><span class="sxs-lookup"><span data-stu-id="ac754-126">On the **Currencies for Fin. Chrg. Terms** page, define for each term a currency code and an additional fee.</span></span>

    > [!NOTE]  
    > <span data-ttu-id="ac754-127">При создании процент-нот в иностранной валюте программой будут использоваться настроенные условия по иностранной валюте.</span><span class="sxs-lookup"><span data-stu-id="ac754-127">When you create finance charges in a foreign currency, the foreign currency conditions that you set up here will be used to create finance charge memos.</span></span> <span data-ttu-id="ac754-128">Если никаких процентных ставок в иностранной валюте не установлено, будут использоваться процентные ставки в рублях, указанные на странице **Процентные ставки**, и затем конвертироваться в соответствующую валюту.</span><span class="sxs-lookup"><span data-stu-id="ac754-128">If there are no foreign currency finance charge conditions set up, the LCY finance charge conditions specified on the **Finance Charge Terms** page will be used and then converted to the relevant currency.</span></span>

    <span data-ttu-id="ac754-129">Для каждого условия процентных ставок можно указать текст, который будет распечатан до (**Начальный текст**) или после (**Заключительный текст**) операций процент-ноты.</span><span class="sxs-lookup"><span data-stu-id="ac754-129">For each finance charge term, you can specify text that will be printed before (**Beginning Text**) or after (**Ending Text**) on the entries on the finance charge memo.</span></span>  
6. <span data-ttu-id="ac754-130">Выберите действие **Начальный текст** или **Заключительный текст** соответственно, а затем заполните страницу **Текст процент-ноты**.</span><span class="sxs-lookup"><span data-stu-id="ac754-130">Choose the **Beginning Text** or **Ending Text** actions respectively, and fill on the **Finance Charge Text** page.</span></span>
7. <span data-ttu-id="ac754-131">Для автоматической вставки связанных значений в полученный текст процент-ноты введите следующие заполнители в поле **Текст**.</span><span class="sxs-lookup"><span data-stu-id="ac754-131">To automatically insert related values in the resulting finance charge text, enter the following placeholders in the **Text** field.</span></span>

|<span data-ttu-id="ac754-132">Заполнитель</span><span class="sxs-lookup"><span data-stu-id="ac754-132">Placeholder</span></span>|<span data-ttu-id="ac754-133">Значение</span><span class="sxs-lookup"><span data-stu-id="ac754-133">Value</span></span>|  
|-----------------|-----------|  
|<span data-ttu-id="ac754-134">%1</span><span class="sxs-lookup"><span data-stu-id="ac754-134">%1</span></span>|<span data-ttu-id="ac754-135">Содержимое поля **Дата документа** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="ac754-135">Content of the **Document Date** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="ac754-136">%2</span><span class="sxs-lookup"><span data-stu-id="ac754-136">%2</span></span>|<span data-ttu-id="ac754-137">Содержимое поля **Срок оплаты** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="ac754-137">Content of the **Due Date** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="ac754-138">%3</span><span class="sxs-lookup"><span data-stu-id="ac754-138">%3</span></span>|<span data-ttu-id="ac754-139">Содержимое поля **Процентная ставка** в связанных процентных ставках</span><span class="sxs-lookup"><span data-stu-id="ac754-139">Content of the **Interest Rate** field on the related finance charge terms</span></span>|  
|<span data-ttu-id="ac754-140">%4</span><span class="sxs-lookup"><span data-stu-id="ac754-140">%4</span></span>|<span data-ttu-id="ac754-141">Содержимое поля **Сумма остатка** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="ac754-141">Content of the **Remaining Amount** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="ac754-142">%5</span><span class="sxs-lookup"><span data-stu-id="ac754-142">%5</span></span>|<span data-ttu-id="ac754-143">Содержимое поля **Сумма процентов** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="ac754-143">Content of the **Interest Amount** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="ac754-144">%6</span><span class="sxs-lookup"><span data-stu-id="ac754-144">%6</span></span>|<span data-ttu-id="ac754-145">Содержимое поля **Дополнительный сбор** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="ac754-145">Content of the **Additional Fee** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="ac754-146">%7</span><span class="sxs-lookup"><span data-stu-id="ac754-146">%7</span></span>|<span data-ttu-id="ac754-147">Итоговая сумма напоминания</span><span class="sxs-lookup"><span data-stu-id="ac754-147">The total amount of the reminder</span></span>|  
|<span data-ttu-id="ac754-148">%8</span><span class="sxs-lookup"><span data-stu-id="ac754-148">%8</span></span>|<span data-ttu-id="ac754-149">Содержимое поля **Код валюты** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="ac754-149">Content of the **Currency Code** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="ac754-150">%9</span><span class="sxs-lookup"><span data-stu-id="ac754-150">%9</span></span>|<span data-ttu-id="ac754-151">Содержимое поля **Дата учета** в заголовке процент-ноты</span><span class="sxs-lookup"><span data-stu-id="ac754-151">Content of the **Posting Date** field on the finance charge memo header</span></span>|  

## <a name="see-also"></a><span data-ttu-id="ac754-152">См. также</span><span class="sxs-lookup"><span data-stu-id="ac754-152">See also</span></span>

[<span data-ttu-id="ac754-153">Сбор непогашенных остатков задолженности</span><span class="sxs-lookup"><span data-stu-id="ac754-153">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="ac754-154">Настройка условий и уровней напоминаний</span><span class="sxs-lookup"><span data-stu-id="ac754-154">Set Up Reminder Terms and Levels</span></span>](finance-setup-reminders.md)  
[<span data-ttu-id="ac754-155">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="ac754-155">Setting Up Finance</span></span>](finance-setup-finance.md)  
