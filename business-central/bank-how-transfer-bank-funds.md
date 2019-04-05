---
title: Перевод банковских средств | Документы Майкрософт
description: Вы можете переводить суммы между банковскими счетами, в том числе в различных валютах, учитывая транзакции в финансовом журнале.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account transfer, multiple currencies
ms.date: 11/18/2018
ms.author: sgroespe
ms.openlocfilehash: 486196d228d9a19d6fbba1e171e138bd5693ac94
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "804544"
---
# <a name="transfer-bank-funds"></a><span data-ttu-id="f5937-103">Перевод банковских средств</span><span class="sxs-lookup"><span data-stu-id="f5937-103">Transfer Bank Funds</span></span>
<span data-ttu-id="f5937-104">Иногда бывает необходимо перевести сумму с одного банковского счета на другой.</span><span class="sxs-lookup"><span data-stu-id="f5937-104">You may sometimes need to transfer an amount from one bank account to another.</span></span> <span data-ttu-id="f5937-105">Для этого необходимо учесть транзакцию в финансовом журнале.</span><span class="sxs-lookup"><span data-stu-id="f5937-105">To do this, you must post the a transaction in the general journal.</span></span> <span data-ttu-id="f5937-106">Задача зависит от того, используется на банковских счетах одна валюта или различные валюты.</span><span class="sxs-lookup"><span data-stu-id="f5937-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a><span data-ttu-id="f5937-107">Учет перемещения между банковскими счетами с одним кодом валюты</span><span class="sxs-lookup"><span data-stu-id="f5937-107">To post a transfer between bank accounts with the same currency code</span></span>
1. <span data-ttu-id="f5937-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовый журнал**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f5937-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="f5937-109">В строке журнала заполните поля **Дата учета** и **Номер документа**</span><span class="sxs-lookup"><span data-stu-id="f5937-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="f5937-110">В поле **Тип счета** выберите значение **Банковский счет**.</span><span class="sxs-lookup"><span data-stu-id="f5937-110">In the **Account Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="f5937-111">В поле **Номер счета** выберите банк, из которого необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="f5937-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="f5937-112">В поле **Сумма** укажите сумму для перевода.</span><span class="sxs-lookup"><span data-stu-id="f5937-112">In the **Amount** field, enter the amount to be transferred.</span></span>
6. <span data-ttu-id="f5937-113">Выберите действие **Показать больше столбцов** для просмотра всех доступных полей.</span><span class="sxs-lookup"><span data-stu-id="f5937-113">Choose the **Show More Columns** action to view all available fields.</span></span>
7. <span data-ttu-id="f5937-114">В поле **Тип баланс. счета** выберите **Банковский счет.**</span><span class="sxs-lookup"><span data-stu-id="f5937-114">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
8. <span data-ttu-id="f5937-115">В поле **Номер баланс. счета** выберите банковский счет, на который необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="f5937-115">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
9. <span data-ttu-id="f5937-116">Учтите журнал.</span><span class="sxs-lookup"><span data-stu-id="f5937-116">Post the journal.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a><span data-ttu-id="f5937-117">Учет перемещения между банковскими счетами с разными кодами валют</span><span class="sxs-lookup"><span data-stu-id="f5937-117">To post a transfer between bank accounts with different currency codes</span></span>
<span data-ttu-id="f5937-118">Для переноса средств между банковскими счетами, которые используют различные валюты, необходимо учесть две строки финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="f5937-118">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span></span>

1. <span data-ttu-id="f5937-119">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовый журнал**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f5937-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="f5937-120">Создайте две строки журнала и заполните поля **Дата учета** и **Номер документа**.</span><span class="sxs-lookup"><span data-stu-id="f5937-120">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="f5937-121">В первой строке журнала в поле **Тип** выберите **Банковский счет**.</span><span class="sxs-lookup"><span data-stu-id="f5937-121">On the first journal line, in the **Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="f5937-122">В поле **Номер счета** выберите банковский счет, с которого необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="f5937-122">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="f5937-123">В поле **Сумма** введите сумму в валюте банковского счета.</span><span class="sxs-lookup"><span data-stu-id="f5937-123">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="f5937-124">Введите суммы кредита со знаком "минус".</span><span class="sxs-lookup"><span data-stu-id="f5937-124">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="f5937-125">Введите суммы дебета без знака "минус".</span><span class="sxs-lookup"><span data-stu-id="f5937-125">Enter debit amounts without a minus sign.</span></span>
6. <span data-ttu-id="f5937-126">В поле **Тип баланс. счета** выберите **Банковский счет.**</span><span class="sxs-lookup"><span data-stu-id="f5937-126">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="f5937-127">В поле **Номер баланс. счета** выберите банковский счет, на который необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="f5937-127">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="f5937-128">Во второй строке журнала в поле **Тип** выберите **Банковский счет**.</span><span class="sxs-lookup"><span data-stu-id="f5937-128">On the second journal line, in the **Type** field, select **Bank Account**.</span></span>
9. <span data-ttu-id="f5937-129">В поле **Номер счета** выберите банковский счет, на который необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="f5937-129">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
10. <span data-ttu-id="f5937-130">В поле **Сумма** введите сумму в валюте банковского счета.</span><span class="sxs-lookup"><span data-stu-id="f5937-130">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="f5937-131">Введите суммы кредита со знаком "минус".</span><span class="sxs-lookup"><span data-stu-id="f5937-131">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="f5937-132">Введите суммы дебета без знака "минус".</span><span class="sxs-lookup"><span data-stu-id="f5937-132">Enter debit amounts without a minus sign.</span></span>
11. <span data-ttu-id="f5937-133">В поле **Тип баланс. счета** выберите **Банковский счет.**</span><span class="sxs-lookup"><span data-stu-id="f5937-133">In the **Bal. Account Type** field, select **Bank Account**.</span></span>  
12. <span data-ttu-id="f5937-134">В поле **Номер баланс. счета** выберите банковский счет, с которого необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="f5937-134">In the **Bal. Account No.** field, select the bank account from which you want to transfer the funds.</span></span>

    > [!NOTE]  
    > <span data-ttu-id="f5937-135">Если валютные курсы, используемые в журнале, отличаются от валютных курсов на странице **Валютные курсы**, введите в третью строку положительную или отрицательную курсовую разницу.</span><span class="sxs-lookup"><span data-stu-id="f5937-135">If the exchange rates used in the journal are different than the exchange rates on the **Currency Exchange Rates** page, enter a third line for the exchange rate gain or loss.</span></span> <span data-ttu-id="f5937-136">Введите **Счет ГК** в поле **Тип счета**.</span><span class="sxs-lookup"><span data-stu-id="f5937-136">Enter **G/L Account** in the **Account Type** field.</span></span> <span data-ttu-id="f5937-137">Введите номер счета ГК для прибыли или убытка по курсовой разнице в поле **Номер счета**.</span><span class="sxs-lookup"><span data-stu-id="f5937-137">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span></span> <span data-ttu-id="f5937-138">Введите прибыль или убыток по курсовой разнице в поле **Сумма** со знаком минус или без него для сумм кредита и дебета соответственно.</span><span class="sxs-lookup"><span data-stu-id="f5937-138">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign for credits and debits respectively.</span></span>
13. <span data-ttu-id="f5937-139">Выполните учет журнала.</span><span class="sxs-lookup"><span data-stu-id="f5937-139">Post the journal.</span></span>

## <a name="see-also"></a><span data-ttu-id="f5937-140">См. также</span><span class="sxs-lookup"><span data-stu-id="f5937-140">See Also</span></span>
[<span data-ttu-id="f5937-141">Управление банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="f5937-141">Managing Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="f5937-142">Настройка банковских операций</span><span class="sxs-lookup"><span data-stu-id="f5937-142">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="f5937-143">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="f5937-143">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="f5937-144">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f5937-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
