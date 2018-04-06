---
title: "Выдача, печать, отмена и аннулирование платежных документов | Microsoft Docs"
description: "Далее описывается процедура выдачи платежных документов с помощью журнала платежей, печать платежных документов и их аннулирование или просмотр операций книги платежей в Business Central."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment journal, print check, vendor payment, creditor, debt, balance due, AP
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 0c1b37616b4aafc9535f2d3fbf60b915c490dd0b
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="work-with-checks"></a><span data-ttu-id="ea309-103">Работа с платежными документами</span><span class="sxs-lookup"><span data-stu-id="ea309-103">Work With Checks</span></span>
<span data-ttu-id="ea309-104">Можно выпустить электронные платежные документы или создать их вручную в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="ea309-104">You can issue electronic and manual checks in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="ea309-105">Оба метода используют журнал платежей для выпуска платежных документов для поставщиков.</span><span class="sxs-lookup"><span data-stu-id="ea309-105">Both methods use the payment journal to issue checks to vendors.</span></span> <span data-ttu-id="ea309-106">Также можно аннулировать платежные документы и просмотреть операции с платежными документами.</span><span class="sxs-lookup"><span data-stu-id="ea309-106">You can also void checks and view check ledger entries.</span></span>

<span data-ttu-id="ea309-107">В результате процесса выпуска платежных документов предлагаются платежи, создаются операции главной книги и печатаются электронные платежные документы.</span><span class="sxs-lookup"><span data-stu-id="ea309-107">The process of issuing checks suggests payments, creates ledger entries, and prints the computer checks.</span></span>

> [!NOTE]  
>   <span data-ttu-id="ea309-108">Чтобы банк выполнил клиринг только проверенных платежных документов и сумм, ему можно отправить файл, содержащий сведения о поставщике, платежном документе и платеже.</span><span class="sxs-lookup"><span data-stu-id="ea309-108">To make sure that your bank only clears validated checks and amounts, you can send them a file that contains vendor, check, and payment information.</span></span> <span data-ttu-id="ea309-109">Дополнительные сведения см. в разделе [Экспорт файла Positive Pay](finance-how-positive-pay.md).</span><span class="sxs-lookup"><span data-stu-id="ea309-109">For more information, see [Export a Positive Pay file](finance-how-positive-pay.md).</span></span>

<span data-ttu-id="ea309-110">Ваши принтер должен быть соответствующим образом настроен для использования форм платежных документов, и вы должны определить макеты чеков для использования.</span><span class="sxs-lookup"><span data-stu-id="ea309-110">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span></span> <span data-ttu-id="ea309-111">Дополнительные сведения см. в разделе [Определение макетов платежных документов](finance-how-define-check-layouts.md)</span><span class="sxs-lookup"><span data-stu-id="ea309-111">For more information, see [Define Check Layouts](finance-how-define-check-layouts.md)</span></span>

## <a name="to-issue-checks"></a><span data-ttu-id="ea309-112">Выпуск платежных документов</span><span class="sxs-lookup"><span data-stu-id="ea309-112">To issue checks</span></span>
1. <span data-ttu-id="ea309-113">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы платежей**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="ea309-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="ea309-114">Заполните журнал соответствующими платежами, например с помощью функции "Предлож. оплаты поставщикам".</span><span class="sxs-lookup"><span data-stu-id="ea309-114">Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function.</span></span> <span data-ttu-id="ea309-115">Дополнительные сведения см. в разделе [Предложение оплаты поставщикам](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="ea309-115">For more information, see [Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>
3. <span data-ttu-id="ea309-116">В **Вид платежа** в строках для платежа, которые вы ходите осуществить с помощь платежного документа, выберите один из следующих вариантов:</span><span class="sxs-lookup"><span data-stu-id="ea309-116">In the **Bank Payment Type** field on journal lines for payment that you want to make with checks, select one of the following options:</span></span>

   * <span data-ttu-id="ea309-117">**Компьютерный**. Выберите эту опцию, если хотите, чтобы программа распечатала платежный документ на сумму из этой строки журнала платежей.</span><span class="sxs-lookup"><span data-stu-id="ea309-117">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span></span> <span data-ttu-id="ea309-118">Платежные документы нужно печатать до учета строк журнала.</span><span class="sxs-lookup"><span data-stu-id="ea309-118">You must print the checks before you can post the journal lines.</span></span> <span data-ttu-id="ea309-119">Параметр **Компьютерный** можно выбрать, только если параметр **Тип баланс. счета** или **Тип счета** имеет значение **Банковский счет**.</span><span class="sxs-lookup"><span data-stu-id="ea309-119">You can only select **Computer Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>
   * <span data-ttu-id="ea309-120">**Ручной**. Выберите эту опцию, если платежный документ создан вручную и нужно создать соответствующую операцию книги платежных документов на эту сумму.</span><span class="sxs-lookup"><span data-stu-id="ea309-120">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span></span> <span data-ttu-id="ea309-121">При использовании этого параметра невозможно распечатывать платежные документы из [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="ea309-121">By using this option, you cannot print checks from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="ea309-122">Параметр **Ручной** можно выбрать, только если параметр **Тип баланс. счета** или **Тип счета** имеет значение **Банковский счет**.</span><span class="sxs-lookup"><span data-stu-id="ea309-122">You can only select **Manual Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

     > [!NOTE]  
     >   <span data-ttu-id="ea309-123">Компьютерные платежные документы нужно печатать до учета соответствующих строк журнала.</span><span class="sxs-lookup"><span data-stu-id="ea309-123">You must print computer checks before you post the related journal lines.</span></span>
4. <span data-ttu-id="ea309-124">В случае компьютерных платежных документов выберите **Печать платежного документа**.</span><span class="sxs-lookup"><span data-stu-id="ea309-124">In case of computer checks, choose **Print Check**.</span></span>
5. <span data-ttu-id="ea309-125">В окне **Платежный документ** заполните поля по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="ea309-125">In the **Check** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
6. <span data-ttu-id="ea309-126">Нажмите кнопку **Печать**.</span><span class="sxs-lookup"><span data-stu-id="ea309-126">Choose the **Print** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="ea309-127">Если необходимо напечатать платежные документы в нескольких валютах с различных банковских счетов, следует выполнить пакетное задание **Печать платежного документа** отдельно по каждой валюте и указать соответствующий банковский счет.</span><span class="sxs-lookup"><span data-stu-id="ea309-127">If you want to print checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span></span>

## <a name="to-cancel-printed-checks-that-are-not-posted"></a><span data-ttu-id="ea309-128">Отмена напечатанных платежных документов. которые не учтены</span><span class="sxs-lookup"><span data-stu-id="ea309-128">To cancel printed checks that are not posted</span></span>
<span data-ttu-id="ea309-129">Вы можете отменить неучтенные платежные документы после их печати с помощью действия **Аннулировать платеж. документ** в окне **Журнал платежей**.</span><span class="sxs-lookup"><span data-stu-id="ea309-129">You can cancel non-posted checks after they have been printed by using the **Void Check** action in the **Payment Journal** window.</span></span>

1. <span data-ttu-id="ea309-130">В окне **Журнал платежей** выберите **Аннулировать платеж. документ**, а затем выберите платежные документы для отмены.</span><span class="sxs-lookup"><span data-stu-id="ea309-130">In the **Payment Journal** window, choose the **Void Check**, and then choose which checks to cancel.</span></span>

## <a name="to-void-checks"></a><span data-ttu-id="ea309-131">Аннулирование платежных документов</span><span class="sxs-lookup"><span data-stu-id="ea309-131">To void checks</span></span>
<span data-ttu-id="ea309-132">Если платеж с помощью платежного документа учтен, аннулировать (отменять) платежные документы можно только в итоговых операциях книги банка.</span><span class="sxs-lookup"><span data-stu-id="ea309-132">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span></span>

1. <span data-ttu-id="ea309-133">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Банковские счета**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="ea309-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="ea309-134">Выберите соответствующий банковский счет, выберите действие **Изменить**, а затем выберите действие **Книга платежных документов**.</span><span class="sxs-lookup"><span data-stu-id="ea309-134">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span></span>
3. <span data-ttu-id="ea309-135">В окне **Книга платежных документов** выберите действие **Аннулировать платеж. документ**.</span><span class="sxs-lookup"><span data-stu-id="ea309-135">In the **Check Ledger Entries** window, choose the **Void Check** action.</span></span>
4. <span data-ttu-id="ea309-136">Установите флажок **Аннулировать только платеж. документ**.</span><span class="sxs-lookup"><span data-stu-id="ea309-136">Select the **Void Check Only** check box.</span></span>
5. <span data-ttu-id="ea309-137">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="ea309-137">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="ea309-138">См. также</span><span class="sxs-lookup"><span data-stu-id="ea309-138">See Also</span></span>
[<span data-ttu-id="ea309-139">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="ea309-139">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="ea309-140">Настройка банковских операций</span><span class="sxs-lookup"><span data-stu-id="ea309-140">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="ea309-141">Экспорт файла Positive Pay</span><span class="sxs-lookup"><span data-stu-id="ea309-141">Export a Positive Pay file</span></span>](finance-how-positive-pay.md)  
<span data-ttu-id="ea309-142">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ea309-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

