---
title: Акт инвентаризации расчетов с клиентами и поставщиками ИНВ-17 в России
description: Улучшения в России включают поддержку акта ИНВ-17 и приложения к акту ИНВ-17.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: bef0d9a07793bc73a191c4832423777362dfaf10
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5786663"
---
# <a name="inventory-act-of-receivables-and-payables-inv-17"></a><span data-ttu-id="e495c-103">Акт инвентаризации расчетов с клиентами и поставщиками ИНВ-17</span><span class="sxs-lookup"><span data-stu-id="e495c-103">Inventory Act of Receivables And Payables INV-17</span></span>

<span data-ttu-id="e495c-104">Функция "Акт инвентаризации расчетов с клиентами и поставщиками" позволяет выполнить инвентаризацию долгов и обязательств и напечатать отчеты в следующих форматах:</span><span class="sxs-lookup"><span data-stu-id="e495c-104">The inventory act of receivables and payables feature enables you to prepare an inventory of debts and liabilities, and print reports in the following formats:</span></span> 

- <span data-ttu-id="e495c-105">ИНВ-17</span><span class="sxs-lookup"><span data-stu-id="e495c-105">INV-17</span></span>
- <span data-ttu-id="e495c-106">Приложение к ИНВ-17</span><span class="sxs-lookup"><span data-stu-id="e495c-106">Supplement to INV-17</span></span>

## <a name="setting-up-a-number-series-for-inventory-acts"></a><span data-ttu-id="e495c-107">Настройка серии номеров для актов инвентаризации</span><span class="sxs-lookup"><span data-stu-id="e495c-107">Setting Up a Number Series for Inventory Acts</span></span>

<span data-ttu-id="e495c-108">Ниже приводится процедура настройки серии номеров для актов инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="e495c-108">The following procedure shows how to set up a number series for inventory acts.</span></span> 

1. <span data-ttu-id="e495c-109">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка ГК**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e495c-109">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="e495c-110">В окне **Настройка ГК** заполните поле **Серия ном. актов инв. расч. с контрагентами**.</span><span class="sxs-lookup"><span data-stu-id="e495c-110">In the **General Ledger Setup** window, fill in the **Contractor Invent. Act Nos.** field.</span></span>

## <a name="inventory-act-processing"></a><span data-ttu-id="e495c-111">Обработка актов инвентаризации</span><span class="sxs-lookup"><span data-stu-id="e495c-111">Inventory Act Processing</span></span>

<span data-ttu-id="e495c-112">Вы можете создавать и обрабатывать акты инвентаризации с контрагентами.</span><span class="sxs-lookup"><span data-stu-id="e495c-112">You can create and process inventory acts of contractors' accounts.</span></span> <span data-ttu-id="e495c-113">Также эти акты можно напечатать.</span><span class="sxs-lookup"><span data-stu-id="e495c-113">You can print inventory acts.</span></span>

### <a name="creating-an-inventory-act-card"></a><span data-ttu-id="e495c-114">Создание карточки акта инвентаризации</span><span class="sxs-lookup"><span data-stu-id="e495c-114">Creating an Inventory Act Card</span></span>

<span data-ttu-id="e495c-115">Ниже приводится процедура создания карточки акта инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="e495c-115">The following procedure shows how to create an inventory act card.</span></span> 

1. <span data-ttu-id="e495c-116">Выберите действие **Главная книга**, выберите действие **Анализ и отчетность**, затем выберите действие **Акты инв. расч. с контрагентами**.</span><span class="sxs-lookup"><span data-stu-id="e495c-116">Choose the **General Ledger** action, choose the **Analysis & Reporting** action, and then choose the **Contractor Invent. Act.** action.</span></span>

2. <span data-ttu-id="e495c-117">В окне **Карточка Товары Фин. Счет** введите сведения в следующие поля:</span><span class="sxs-lookup"><span data-stu-id="e495c-117">In the **Inventory Account Card** window, enter information in the following fields:</span></span>

   | <span data-ttu-id="e495c-118">Поле</span><span class="sxs-lookup"><span data-stu-id="e495c-118">Field</span></span>                    | <span data-ttu-id="e495c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e495c-119">Description</span></span>                                                  |
   | :----------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="e495c-120">**Номер**</span><span class="sxs-lookup"><span data-stu-id="e495c-120">**No.**</span></span>                  | <span data-ttu-id="e495c-121">В этом поле отображается номер акта, и оно заполняется автоматически из серии номеров.</span><span class="sxs-lookup"><span data-stu-id="e495c-121">This field displays the number of the act, and is filled in automatically from the number series.</span></span> |
   | <span data-ttu-id="e495c-122">**Дата акта**</span><span class="sxs-lookup"><span data-stu-id="e495c-122">**Act Date**</span></span>             | <span data-ttu-id="e495c-123">В этом поле отображается дата акта, и оно заполняется рабочей датой.</span><span class="sxs-lookup"><span data-stu-id="e495c-123">This field displays the act date, and is filled in with the work date.</span></span> |
   | <span data-ttu-id="e495c-124">**Дата инвентаризации**</span><span class="sxs-lookup"><span data-stu-id="e495c-124">**Inventory Date**</span></span>       | <span data-ttu-id="e495c-125">В этом поле отображается дата инвентаризации, и оно заполняется рабочей датой.</span><span class="sxs-lookup"><span data-stu-id="e495c-125">This field displays the date of inventory, and is filled with the work date.</span></span> <span data-ttu-id="e495c-126">Долги и обязательства будут рассчитываться на эту дату.</span><span class="sxs-lookup"><span data-stu-id="e495c-126">Debts and liabilities will be calculated on this date.</span></span> |
   | <span data-ttu-id="e495c-127">**Тип документа-основания**</span><span class="sxs-lookup"><span data-stu-id="e495c-127">**Reason Document Type**</span></span> | <span data-ttu-id="e495c-128">Выберите тип документа-основания из следующих:   -   **Приказ** -   **Постановление** -   **Распоряжение**.</span><span class="sxs-lookup"><span data-stu-id="e495c-128">Select the type of reason document from the following:   -   **Order** -   **Resolution** -   **Regulation**</span></span> |

3. <span data-ttu-id="e495c-129">Выберите действие **Добавить строки**.</span><span class="sxs-lookup"><span data-stu-id="e495c-129">Choose the **Add Lines** action.</span></span>

   > [!NOTE]
   > <span data-ttu-id="e495c-130">Нельзя задавать фильтры.</span><span class="sxs-lookup"><span data-stu-id="e495c-130">You must not set filters.</span></span>

   <span data-ttu-id="e495c-131">Создаются долги и обязательства для поставщиков и клиентов, а также строки.</span><span class="sxs-lookup"><span data-stu-id="e495c-131">Debts and liabilities for vendors and customers are calculated, and lines are created.</span></span> <span data-ttu-id="e495c-132">Для каждого клиента и поставщика рассчитываются и отображаются в отдельной строке общая сумма долгов и обязательств на дату инвентаризации (учитывая группы учета).</span><span class="sxs-lookup"><span data-stu-id="e495c-132">For each customer and vendor, the total debt and the total liability amount (taking posting groups into account) on the inventory date are calculated, and shown in a separate line.</span></span> <span data-ttu-id="e495c-133">Поля строк описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e495c-133">The line fields are listed in the following table.</span></span>

| <span data-ttu-id="e495c-134">Поле</span><span class="sxs-lookup"><span data-stu-id="e495c-134">Field</span></span>                              | <span data-ttu-id="e495c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="e495c-135">Description</span></span>          |
| ---------------------------------- | -------------------- |
| <span data-ttu-id="e495c-136">**Тип контрагента**</span><span class="sxs-lookup"><span data-stu-id="e495c-136">**Contractor Type**</span></span>                | <span data-ttu-id="e495c-137">В этом поле отображается тип контрагента (клиент, поставщик).</span><span class="sxs-lookup"><span data-stu-id="e495c-137">This field displays the contractor type (Customer, Vendor).</span></span>  |
| <span data-ttu-id="e495c-138">**Код контрагента**</span><span class="sxs-lookup"><span data-stu-id="e495c-138">**Contractor No.**</span></span>                 | <span data-ttu-id="e495c-139">В этом поле отображается номер, соответствующий контрагенту.</span><span class="sxs-lookup"><span data-stu-id="e495c-139">This field displays the number corresponding to the contractor.</span></span> |
| <span data-ttu-id="e495c-140">**Название контрагента**</span><span class="sxs-lookup"><span data-stu-id="e495c-140">**Contractor Name**</span></span>                | <span data-ttu-id="e495c-141">В этом поле показано имя контрагента.</span><span class="sxs-lookup"><span data-stu-id="e495c-141">This field displays the name of the contractor.</span></span>    |
| <span data-ttu-id="e495c-142">**Учетная Группа, Фин. Счет Но.**</span><span class="sxs-lookup"><span data-stu-id="e495c-142">**Posting Group, G/L Account No.**</span></span> | <span data-ttu-id="e495c-143">В данном поле отображается группа учета и счет расчетов с клиентами или поставщиками, для которого рассчитывается сумма долгов или обязательств.</span><span class="sxs-lookup"><span data-stu-id="e495c-143">This field displays the posting group and the receivables or payables account for which the debt or liability amount is calculated.</span></span> |
| <span data-ttu-id="e495c-144">**Категория**</span><span class="sxs-lookup"><span data-stu-id="e495c-144">**Category**</span></span>                       | <span data-ttu-id="e495c-145">В этом поле отображается категория суммы (долги, обязательства).</span><span class="sxs-lookup"><span data-stu-id="e495c-145">This field displays the amount category (Debts, Liabilities).</span></span> |
| <span data-ttu-id="e495c-146">**Общая сумма**</span><span class="sxs-lookup"><span data-stu-id="e495c-146">**Total Amount**</span></span>                   | <span data-ttu-id="e495c-147">В этом поле отображается общая сумма долгов и обязательств.</span><span class="sxs-lookup"><span data-stu-id="e495c-147">This field displays the total amount of debts or liabilities.</span></span> |
| <span data-ttu-id="e495c-148">**Подтвержденная сумма**</span><span class="sxs-lookup"><span data-stu-id="e495c-148">**Confirmed Amount**</span></span>               | <span data-ttu-id="e495c-149">В этом поле отображается общая сумма долгов и обязательств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e495c-149">This field displays the total amount of debts or liabilities by default.</span></span> |

### <a name="changing-separate-lines-in-an-inventory-act"></a><span data-ttu-id="e495c-150">Изменение отдельных строк акта инвентаризации</span><span class="sxs-lookup"><span data-stu-id="e495c-150">Changing Separate Lines in an Inventory Act</span></span>

<span data-ttu-id="e495c-151">Ниже приводится процедура изменения отдельных строк акта инвентаризации в окне **Карточка Товары Фин. Счет**.</span><span class="sxs-lookup"><span data-stu-id="e495c-151">The following procedure shows how to change individual lines in an inventory act in the **Inventory Account Card** window.</span></span> 

1. <span data-ttu-id="e495c-152">Укажите, один из следующих вариантов для суммы (или части суммы):</span><span class="sxs-lookup"><span data-stu-id="e495c-152">Specify whether the amount (or part of the amount) is one of the following:</span></span>

    - <span data-ttu-id="e495c-153">Подтверждена контрагентом</span><span class="sxs-lookup"><span data-stu-id="e495c-153">Confirmed by contractor</span></span>
    - <span data-ttu-id="e495c-154">Не подтверждена</span><span class="sxs-lookup"><span data-stu-id="e495c-154">Not confirmed</span></span>
    - <span data-ttu-id="e495c-155">Просрочено</span><span class="sxs-lookup"><span data-stu-id="e495c-155">Overdue</span></span>

2. <span data-ttu-id="e495c-156">Если сумма не подтверждена, введите неподтвержденную сумму в поле **Неподтвержденная сумма**.</span><span class="sxs-lookup"><span data-stu-id="e495c-156">If the amount is not confirmed, enter the amount that is not confirmed in the **Not Confirmed Amount** field.</span></span>

3. <span data-ttu-id="e495c-157">Если сумма просрочена, введите сумму в поле **С истекшим сроком исковой давности**.</span><span class="sxs-lookup"><span data-stu-id="e495c-157">If the amount is overdue, enter the overdue amount in the **Overdue Amount** field.</span></span>

4. <span data-ttu-id="e495c-158">Чтобы исправить строку с неправильной суммой (например, если некоторые документы не учтены или не применены), выберите действие **Добавить строки**.</span><span class="sxs-lookup"><span data-stu-id="e495c-158">To correct a line that has an incorrect amount (for instance, if some documents are not posted, or not applied), choose the **Add Lines** action.</span></span>

5. <span data-ttu-id="e495c-159">Выберите код поставщика или клиента, а затем выберите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="e495c-159">Select the vendor or customer code, and then choose the **OK** button.</span></span> 

<span data-ttu-id="e495c-160">Сумма долгов и обязательств для выбранного поставщика или клиента пересчитывается, и строки вставляются в документ.</span><span class="sxs-lookup"><span data-stu-id="e495c-160">The debts and liabilities amount for the selected vendor or customer is recalculated and the lines are inserted in the document.</span></span>

## <a name="printing-the-inv-17-form-and-the-supplement-to-inv-17-form"></a><span data-ttu-id="e495c-161">Печать формы ИНВ-17 и формы Приложение к ИНВ-17</span><span class="sxs-lookup"><span data-stu-id="e495c-161">Printing the INV-17 form and the Supplement to INV-17 form</span></span>

<span data-ttu-id="e495c-162">Ниже приводится процедура печати формы ИНВ-17 и формы Приложение к ИНВ-17.</span><span class="sxs-lookup"><span data-stu-id="e495c-162">The following procedure shows how to print the INV-17 form and the Supplement to INV-17 form.</span></span>

1. <span data-ttu-id="e495c-163">В окне **Карточка Товары Фин. Счет** выберите действие **Выпустить**.</span><span class="sxs-lookup"><span data-stu-id="e495c-163">In the **Inventory Account Card** window, choose the **Release** action.</span></span>
2. <span data-ttu-id="e495c-164">Выберите действие **Акт**, затем выберите действие **Подписи**.</span><span class="sxs-lookup"><span data-stu-id="e495c-164">Choose the **Act** action, and then choose the **Signatures** action.</span></span>
3. <span data-ttu-id="e495c-165">Выберите следующие поля:</span><span class="sxs-lookup"><span data-stu-id="e495c-165">Select the following fields:</span></span>

    - <span data-ttu-id="e495c-166">**Председатель**</span><span class="sxs-lookup"><span data-stu-id="e495c-166">**Chairman**</span></span>
    - <span data-ttu-id="e495c-167">**Член комиссии 1**</span><span class="sxs-lookup"><span data-stu-id="e495c-167">**Member1**</span></span>
    - <span data-ttu-id="e495c-168">**Член комиссии 2**</span><span class="sxs-lookup"><span data-stu-id="e495c-168">**Member2**</span></span>
    - <span data-ttu-id="e495c-169">**Член комиссии 3**</span><span class="sxs-lookup"><span data-stu-id="e495c-169">**Member3**</span></span>
    - <span data-ttu-id="e495c-170">**Бухгалтер**</span><span class="sxs-lookup"><span data-stu-id="e495c-170">**Accountant**</span></span>

    > [!NOTE]
    > <span data-ttu-id="e495c-171">Все выбранные подписи будут отображены в соответствующих полях.</span><span class="sxs-lookup"><span data-stu-id="e495c-171">All selected signatures will be reflected in the appropriate fields.</span></span>

4. <span data-ttu-id="e495c-172">Выберите действие **Печать**, затем выберите действие **Акт инвентаризации ИНВ-17** для печати акта инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="e495c-172">Choose the **Print** action, and then choose the **Invent. Act INV-17** action to print the inventory act.</span></span>
5. <span data-ttu-id="e495c-173">Выберите действие **Печать**, затем выберите действие **Приложение к Акту инвентаризации ИНВ-17** для печати приложения к акту инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="e495c-173">Choose the **Print** action, and then choose the **Supplement to Invent. Act INV-17** action to print the supplement to the inventory act.</span></span>

## <a name="see-also"></a><span data-ttu-id="e495c-174">См. также</span><span class="sxs-lookup"><span data-stu-id="e495c-174">See Also</span></span>

[<span data-ttu-id="e495c-175">Отчеты о платежах (Россия)</span><span class="sxs-lookup"><span data-stu-id="e495c-175">Russian Payables Reports</span></span>](Russian-Payables-Reports.md)  
[<span data-ttu-id="e495c-176">Отчеты по расчетам с клиентами (Россия)</span><span class="sxs-lookup"><span data-stu-id="e495c-176">Russian Receivables Reports</span></span>](Russian-Receivables-Reports.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]