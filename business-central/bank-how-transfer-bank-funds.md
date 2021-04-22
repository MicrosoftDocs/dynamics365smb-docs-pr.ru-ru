---
title: Перевод банковских средств | Документация Майкрософт
description: Вы можете переводить суммы между банковскими счетами, в том числе в различных валютах, учитывая транзакции в финансовом журнале.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account transfer, multiple currencies
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: dea39ba380eee574205d57ba198f15213c341ea0
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779736"
---
# <a name="transfer-bank-funds"></a><span data-ttu-id="268fb-103">Перевод банковских средств</span><span class="sxs-lookup"><span data-stu-id="268fb-103">Transfer Bank Funds</span></span>
<span data-ttu-id="268fb-104">Иногда бывает необходимо перевести сумму с одного банковского счета в [!INCLUDE[prod_short](includes/prod_short.md)] на другой.</span><span class="sxs-lookup"><span data-stu-id="268fb-104">You may sometimes need to transfer an amount from one bank account in [!INCLUDE[prod_short](includes/prod_short.md)] to another.</span></span> <span data-ttu-id="268fb-105">Для этого необходимо учесть транзакцию на странице **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="268fb-105">To do this, you must post the a transaction on the **General Journal** page.</span></span> <span data-ttu-id="268fb-106">Задача зависит от того, используется на банковских счетах одна валюта или различные валюты.</span><span class="sxs-lookup"><span data-stu-id="268fb-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a><span data-ttu-id="268fb-107">Учет перемещения между банковскими счетами с одним кодом валюты</span><span class="sxs-lookup"><span data-stu-id="268fb-107">To post a transfer between bank accounts with the same currency code</span></span>
1. <span data-ttu-id="268fb-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовый журнал**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="268fb-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="268fb-109">В строке журнала заполните поля **Дата учета** и **Номер документа**</span><span class="sxs-lookup"><span data-stu-id="268fb-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="268fb-110">В поле **Тип счета** выберите значение **Банковский счет**.</span><span class="sxs-lookup"><span data-stu-id="268fb-110">In the **Account Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="268fb-111">В поле **Номер счета** выберите банк, из которого необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="268fb-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="268fb-112">В поле **Сумма** укажите сумму для перевода.</span><span class="sxs-lookup"><span data-stu-id="268fb-112">In the **Amount** field, enter the amount to be transferred.</span></span>
6. <span data-ttu-id="268fb-113">Выберите действие **Показать больше столбцов** для просмотра всех доступных полей.</span><span class="sxs-lookup"><span data-stu-id="268fb-113">Choose the **Show More Columns** action to view all available fields.</span></span>
7. <span data-ttu-id="268fb-114">В поле **Тип баланс. счета** выберите **Банковский счет.**</span><span class="sxs-lookup"><span data-stu-id="268fb-114">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
8. <span data-ttu-id="268fb-115">В поле **Номер баланс. счета** выберите банковский счет, на который необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="268fb-115">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
9. <span data-ttu-id="268fb-116">Учтите журнал.</span><span class="sxs-lookup"><span data-stu-id="268fb-116">Post the journal.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a><span data-ttu-id="268fb-117">Учет перемещения между банковскими счетами с разными кодами валют</span><span class="sxs-lookup"><span data-stu-id="268fb-117">To post a transfer between bank accounts with different currency codes</span></span>
<span data-ttu-id="268fb-118">Для переноса средств между банковскими счетами, которые используют различные валюты, необходимо учесть две строки финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="268fb-118">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span></span>

1. <span data-ttu-id="268fb-119">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовый журнал**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="268fb-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="268fb-120">Создайте две строки журнала и заполните поля **Дата учета** и **Номер документа**.</span><span class="sxs-lookup"><span data-stu-id="268fb-120">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="268fb-121">В первой строке журнала в поле **Тип** выберите **Банковский счет**.</span><span class="sxs-lookup"><span data-stu-id="268fb-121">On the first journal line, in the **Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="268fb-122">В поле **Номер счета** выберите банковский счет, с которого необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="268fb-122">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="268fb-123">В поле **Сумма** введите сумму в валюте банковского счета.</span><span class="sxs-lookup"><span data-stu-id="268fb-123">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="268fb-124">Введите суммы кредита со знаком "минус".</span><span class="sxs-lookup"><span data-stu-id="268fb-124">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="268fb-125">Введите суммы дебета без знака "минус".</span><span class="sxs-lookup"><span data-stu-id="268fb-125">Enter debit amounts without a minus sign.</span></span>
6. <span data-ttu-id="268fb-126">В поле **Тип баланс. счета** выберите **Банковский счет.**</span><span class="sxs-lookup"><span data-stu-id="268fb-126">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="268fb-127">В поле **Номер баланс. счета** выберите банковский счет, на который необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="268fb-127">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="268fb-128">Во второй строке журнала в поле **Тип** выберите **Банковский счет**.</span><span class="sxs-lookup"><span data-stu-id="268fb-128">On the second journal line, in the **Type** field, select **Bank Account**.</span></span>
9. <span data-ttu-id="268fb-129">В поле **Номер счета** выберите банковский счет, на который необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="268fb-129">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
10. <span data-ttu-id="268fb-130">В поле **Сумма** введите сумму в валюте банковского счета.</span><span class="sxs-lookup"><span data-stu-id="268fb-130">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="268fb-131">Введите суммы кредита со знаком "минус".</span><span class="sxs-lookup"><span data-stu-id="268fb-131">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="268fb-132">Введите суммы дебета без знака "минус".</span><span class="sxs-lookup"><span data-stu-id="268fb-132">Enter debit amounts without a minus sign.</span></span>
11. <span data-ttu-id="268fb-133">В поле **Тип баланс. счета** выберите **Банковский счет.**</span><span class="sxs-lookup"><span data-stu-id="268fb-133">In the **Bal. Account Type** field, select **Bank Account**.</span></span>  
12. <span data-ttu-id="268fb-134">В поле **Номер баланс. счета** выберите банковский счет, с которого необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="268fb-134">In the **Bal. Account No.** field, select the bank account from which you want to transfer the funds.</span></span>

    > [!NOTE]  
    > <span data-ttu-id="268fb-135">Если валютные курсы, используемые в журнале, отличаются от валютных курсов на странице **Валютные курсы**, введите в третью строку положительную или отрицательную курсовую разницу.</span><span class="sxs-lookup"><span data-stu-id="268fb-135">If the exchange rates used in the journal are different than the exchange rates on the **Currency Exchange Rates** page, enter a third line for the exchange rate gain or loss.</span></span> <span data-ttu-id="268fb-136">Введите **Счет ГК** в поле **Тип счета**.</span><span class="sxs-lookup"><span data-stu-id="268fb-136">Enter **G/L Account** in the **Account Type** field.</span></span> <span data-ttu-id="268fb-137">Введите номер счета ГК для прибыли или убытка по курсовой разнице в поле **Номер счета**.</span><span class="sxs-lookup"><span data-stu-id="268fb-137">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span></span> <span data-ttu-id="268fb-138">Введите прибыль или убыток по курсовой разнице в поле **Сумма** со знаком минус или без него для сумм кредита и дебета соответственно.</span><span class="sxs-lookup"><span data-stu-id="268fb-138">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign for credits and debits respectively.</span></span>
13. <span data-ttu-id="268fb-139">Учтите журнал.</span><span class="sxs-lookup"><span data-stu-id="268fb-139">Post the journal.</span></span>

## <a name="see-also"></a><span data-ttu-id="268fb-140">См. также</span><span class="sxs-lookup"><span data-stu-id="268fb-140">See Also</span></span>
[<span data-ttu-id="268fb-141">Выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="268fb-141">Reconciling Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="268fb-142">Настройка банковских операций</span><span class="sxs-lookup"><span data-stu-id="268fb-142">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="268fb-143">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="268fb-143">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="268fb-144">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="268fb-144">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]