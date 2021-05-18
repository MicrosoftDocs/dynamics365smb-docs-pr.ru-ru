---
title: Перевод банковских средств
description: Вы можете переводить суммы между банковскими счетами, в том числе в различных валютах, учитывая транзакции в финансовом журнале.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account transfer, multiple currencies
ms.date: 04/29/2021
ms.author: edupont
ms.openlocfilehash: da9c8711751040cecb267a3b2209bad2534b618b
ms.sourcegitcommit: 08ca5798cf3f04fc3ea38fff40c1860196a70adf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "5985391"
---
# <a name="transfer-bank-funds"></a><span data-ttu-id="f4f5b-103">Перевод банковских средств</span><span class="sxs-lookup"><span data-stu-id="f4f5b-103">Transfer Bank Funds</span></span>

<span data-ttu-id="f4f5b-104">Иногда бывает необходимо перевести сумму с одного банковского счета в [!INCLUDE[prod_short](includes/prod_short.md)] на другой.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-104">You may sometimes need to transfer an amount from one bank account in [!INCLUDE[prod_short](includes/prod_short.md)] to another.</span></span> <span data-ttu-id="f4f5b-105">Для этого необходимо учесть транзакцию на странице **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-105">To do this, you must post the transaction on the **General Journal** page.</span></span> <span data-ttu-id="f4f5b-106">Задача зависит от того, используется на банковских счетах одна валюта или различные валюты.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a><span data-ttu-id="f4f5b-107">Учет перемещения между банковскими счетами с одним кодом валюты</span><span class="sxs-lookup"><span data-stu-id="f4f5b-107">To post a transfer between bank accounts with the same currency code</span></span>

1. <span data-ttu-id="f4f5b-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовый журнал**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="f4f5b-109">В строке журнала заполните поля **Дата учета** и **Номер документа**</span><span class="sxs-lookup"><span data-stu-id="f4f5b-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="f4f5b-110">В поле **Тип счета** выберите значение **Банковский счет**.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-110">In the **Account Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="f4f5b-111">В поле **Номер счета** выберите банк, из которого необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="f4f5b-112">В поле **Сумма** укажите сумму для перевода.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-112">In the **Amount** field, enter the amount to be transferred.</span></span>

    <span data-ttu-id="f4f5b-113">Далее необходимо указать балансирующий счет.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-113">Next, you must specify the balancing account.</span></span> <span data-ttu-id="f4f5b-114">Если вы не видите соответствующие поля, выберите действие **Показать больше столбцов** для просмотра всех доступных полей.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-114">If you can't see the relevant fields, then choose the **Show More Columns** action to view all available fields.</span></span>
6. <span data-ttu-id="f4f5b-115">В поле **Тип баланс. счета** выберите **Банковский счет.**</span><span class="sxs-lookup"><span data-stu-id="f4f5b-115">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="f4f5b-116">В поле **Номер баланс. счета** выберите банковский счет, на который необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-116">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="f4f5b-117">Учтите журнал.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-117">Post the journal.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a><span data-ttu-id="f4f5b-118">Учет перемещения между банковскими счетами с разными кодами валют</span><span class="sxs-lookup"><span data-stu-id="f4f5b-118">To post a transfer between bank accounts with different currency codes</span></span>

<span data-ttu-id="f4f5b-119">Для переноса средств между банковскими счетами, которые используют различные валюты, необходимо учесть две строки финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-119">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span></span>

1. <span data-ttu-id="f4f5b-120">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовый журнал**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="f4f5b-121">Создайте две строки журнала и заполните поля **Дата учета** и **Номер документа**.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-121">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="f4f5b-122">В первой строке журнала в поле **Тип** выберите **Банковский счет**.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-122">On the first journal line, in the **Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="f4f5b-123">В поле **Номер счета** выберите банковский счет, с которого необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-123">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="f4f5b-124">В поле **Количество** введите сумму в валюте банковского счета со знаком минус или без него.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-124">In the **Amount** field, enter the amount in the currency of the bank account with or without a minus sign.</span></span>

    > [!TIP]
    > <span data-ttu-id="f4f5b-125">Сумма без знака минус — дебет, а сумма со знаком минус — кредит.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-125">An amount without a sign is a debit, and an amount with a minus sign is a credit.</span></span>

    > [!NOTE]
    > <span data-ttu-id="f4f5b-126">Некоторые компании предпочитают переводить между счетами по отдельным строкам журнала.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-126">Some companies prefer to transfer between accounts on separate journal lines.</span></span> <span data-ttu-id="f4f5b-127">Другие компании предпочитают размещать все в одной строке журнала, используя балансирующий счет.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-127">Other companies prefer to post everything on one journal line by using a balancing account.</span></span> <span data-ttu-id="f4f5b-128">Если вы не знаете, что делать, посоветуйтесь со своим местным экспертом.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-128">Check with your local expert if you're not sure what to do.</span></span>
    >
    > <span data-ttu-id="f4f5b-129">Если ваша компания предпочитает использовать балансирующий счет, установите поле **Тип баланс. счета** как **Банковский счет**, и установите **Номер баланс. счета** как банковский счет, на который вы хотите перевести средства.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-129">If your company prefers to use a balancing account, then set the **Bal. Account Type** field to **Bank Account**, and set the **Bal. Account No.** field to the bank account to which you want to transfer the funds.</span></span> <span data-ttu-id="f4f5b-130">Затем переходите к шагу 9 или 10.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-130">Then proceed to step 9 or 10.</span></span>
    >
    > <span data-ttu-id="f4f5b-131">Если ваша компания предпочитает использовать отдельную строку журнала, переходите к следующему шагу.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-131">If your company prefers to use a separate journal line, then move on to the next step.</span></span>
6. <span data-ttu-id="f4f5b-132">Во второй строке журнала в поле **Тип** выберите **Банковский счет**.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-132">On the second journal line, in the **Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="f4f5b-133">В поле **Номер счета** выберите банковский счет, на который необходимо перевести средства.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-133">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="f4f5b-134">В поле **Количество** введите сумму в валюте банковского счета со знаком минус или без него.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-134">In the **Amount** field, enter the amount in the currency of the bank account with or without a minus sign.</span></span>

    > [!TIP]
    > <span data-ttu-id="f4f5b-135">Сумма без знака минус — дебет, а сумма со знаком минус — кредит.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-135">An amount without a sign is a debit, and an amount with a minus sign is a credit.</span></span>
9. <span data-ttu-id="f4f5b-136">Если валютные курсы, используемые в журнале, отличаются от валютных курсов на странице **Валютные курсы**, введите новую строку журнала для прибыли или убытка по курсовым разницам.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-136">If the exchange rates used in the journal are different than the exchange rates on the **Currency Exchange Rates** page, enter a new journal line for the exchange rate gain or loss.</span></span>  

    1. <span data-ttu-id="f4f5b-137">Введите **Счет ГК** в поле **Тип счета**.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-137">Enter **G/L Account** in the **Account Type** field.</span></span>  

    2. <span data-ttu-id="f4f5b-138">Введите номер счета ГК для прибыли или убытка по курсовой разнице в поле **Номер счета**.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-138">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span></span>  

    3. <span data-ttu-id="f4f5b-139">Введите прибыли или убытки по курсовым разницам в поле **Количество** со знаком минус или без него.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-139">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign.</span></span>

    > [!TIP]
    > <span data-ttu-id="f4f5b-140">Сумма без знака минус — дебет, а сумма со знаком минус — кредит.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-140">An amount without a sign is a debit, and an amount with a minus sign is a credit.</span></span>
10. <span data-ttu-id="f4f5b-141">Учтите журнал.</span><span class="sxs-lookup"><span data-stu-id="f4f5b-141">Post the journal.</span></span>

## <a name="see-also"></a><span data-ttu-id="f4f5b-142">См. также</span><span class="sxs-lookup"><span data-stu-id="f4f5b-142">See Also</span></span>

[<span data-ttu-id="f4f5b-143">Выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="f4f5b-143">Reconciling Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="f4f5b-144">Настройка банковских операций</span><span class="sxs-lookup"><span data-stu-id="f4f5b-144">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="f4f5b-145">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="f4f5b-145">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="f4f5b-146">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f4f5b-146">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]