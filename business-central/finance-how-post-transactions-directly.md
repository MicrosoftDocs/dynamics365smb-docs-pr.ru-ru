---
title: Запись расходов или доходов непосредственно в ГК | Документация Майкрософт
description: Для бизнес-операций, которые не представлены документами, например небольшими расходами или наличными поступлениями, можно создавать соответствующие транзакции путем учета строк журналов на странице финансового журнала.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct posting, general ledger
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 0908d3fedb9946dafdaa0795edd6d018785bd3e5
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2302264"
---
# <a name="post-transactions-directly-to-the-general-ledger"></a><span data-ttu-id="34367-103">Учет транзакций непосредственно в главной книге</span><span class="sxs-lookup"><span data-stu-id="34367-103">Post Transactions Directly to the General Ledger</span></span>

<span data-ttu-id="34367-104">Финансовые журналы используются для учета финансовых транзакций непосредственно на счетах главной книги и других счетах, таких как банковские счета, счета клиентов, счета поставщиков и счета сотрудников.</span><span class="sxs-lookup"><span data-stu-id="34367-104">You use general journals to post financial transactions directly to general ledger accounts and other accounts, such as bank, customer, vendor, and employee accounts.</span></span>  

<span data-ttu-id="34367-105">Типичное использование финансового журнала — учет расходования собственных средств сотрудниками во время служебной деятельности для последующей компенсации.</span><span class="sxs-lookup"><span data-stu-id="34367-105">A typical use of the general journal is to post employees' expenditure of own money during business activities, for later reimbursement.</span></span> <span data-ttu-id="34367-106">Дополнительные сведения см. в разделе [Регистрация и возмещение расходов сотрудников](finance-how-record-reimburse-employee-expenses.md).</span><span class="sxs-lookup"><span data-stu-id="34367-106">For more information, see [Record and Reimburse Employees' Expenses](finance-how-record-reimburse-employee-expenses.md).</span></span>

<span data-ttu-id="34367-107">Финансовые журналы используются для учета транзакций по счетам главной книги и другим счетам, таким как банковские счета, счета клиентов, счета поставщиков и счета сотрудников.</span><span class="sxs-lookup"><span data-stu-id="34367-107">General journals post financial transactions directly to general ledger accounts and other accounts, such as bank, customer, vendor, and employee accounts.</span></span> <span data-ttu-id="34367-108">В результате учета в финансовом журнале всегда создаются операции по счетам главной книги.</span><span class="sxs-lookup"><span data-stu-id="34367-108">Posting with a general journal always creates entries on general ledger accounts.</span></span> <span data-ttu-id="34367-109">Это верно, даже если, к примеру, строка журнала учитывается в счете клиента, так как операция учитывается в счете дебиторской задолженности главной книги через учетную группу.</span><span class="sxs-lookup"><span data-stu-id="34367-109">This is true even when, for example, you post a journal line to a customer account, because an entry is posted to a general ledger receivables account through a posting group.</span></span> <span data-ttu-id="34367-110">Вы можете персонализировать свою версию финансового журнала, настроив шаблон или раздел журнала.</span><span class="sxs-lookup"><span data-stu-id="34367-110">You can personalize your version of a general journal by setting up a journal batch or template.</span></span> <span data-ttu-id="34367-111">Дополнительные сведения см. в разделе [Работа с финансовыми журналами](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="34367-111">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>

<span data-ttu-id="34367-112">В отличие от операций, которые учитываются с помощью документов, требующих обработки кредит-нот, вы можете корректно сторнировать операции, учтенные из финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="34367-112">Unlike for entries that are posted with documents, which require a credit memo process, you can correctly reverse entries that are posted with the general journal.</span></span> <span data-ttu-id="34367-113">Дополнительные сведения см. в разделе [Сторнирование учета в журнале и отмена приходных/расходных накладных](finance-how-reverse-journal-posting.md).</span><span class="sxs-lookup"><span data-stu-id="34367-113">For more information, see [Reverse Journal Postings and Undo Receipts/Shipments](finance-how-reverse-journal-posting.md).</span></span>

## <a name="to-post-a-transaction-directly-to-a-general-ledger-account"></a><span data-ttu-id="34367-114">Учет транзакции непосредственно на счете главной книге</span><span class="sxs-lookup"><span data-stu-id="34367-114">To post a transaction directly to a general ledger account</span></span>

1. <span data-ttu-id="34367-115">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовые журналы**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="34367-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="34367-116">Откройте соответствующий раздел финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="34367-116">Open the relevant general journal batch.</span></span> <span data-ttu-id="34367-117">Дополнительные сведения см. в разделе [Работа с финансовыми журналами](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="34367-117">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="34367-118">На новой строке журнала заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="34367-118">On a new journal line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]    

    > [!NOTE]
    > [!INCLUDE[journal-showhide-columns-inline-tip](includes/journal-showhide-columns-inline-tip.md)]
4. <span data-ttu-id="34367-119">Повторите шаг 3 для всех отдельных транзакций, которые требуется учесть.</span><span class="sxs-lookup"><span data-stu-id="34367-119">Repeat step 3 for all the separate transactions that you want to post.</span></span>

    > [!TIP]  
    > <span data-ttu-id="34367-120">Если необходимо ввести строки нескольких транзакций над одной строкой балансирующего счета, например, для одного банковского счета, установите флажок **Предлагаемая балансирующая сумма** в строке раздела на странице **Разделы финансового журнала**.</span><span class="sxs-lookup"><span data-stu-id="34367-120">If you want to enter multiple transaction lines above one balance-account line, for example, for one bank account, then select the **Suggest Balancing Amount** check box on the line for your batch on the **General Journal Batches** page.</span></span> <span data-ttu-id="34367-121">Затем в поле **Сумма** строки балансирующего счета автоматически будет подставлено значение, необходимое для балансировки транзакций.</span><span class="sxs-lookup"><span data-stu-id="34367-121">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the transactions.</span></span>
5. <span data-ttu-id="34367-122">Выберите действие **Учет**, чтобы записать транзакции на указанных счетах ГК.</span><span class="sxs-lookup"><span data-stu-id="34367-122">Choose the **Post** action to record the transactions on the specified G/L accounts.</span></span>

## <a name="see-also"></a><span data-ttu-id="34367-123">См. также</span><span class="sxs-lookup"><span data-stu-id="34367-123">See Also</span></span>

[<span data-ttu-id="34367-124">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="34367-124">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="34367-125">Регистрация и возмещение расходов сотрудников</span><span class="sxs-lookup"><span data-stu-id="34367-125">Record and Reimburse Employees' Expenses</span></span>](finance-how-record-reimburse-employee-expenses.md)  
[<span data-ttu-id="34367-126">Сторнирование учета в журнале и отмена приходных/расходных накладных</span><span class="sxs-lookup"><span data-stu-id="34367-126">Reverse Journal Postings and Undo Receipts/Shipments</span></span>](finance-how-reverse-journal-posting.md)  
[<span data-ttu-id="34367-127">Финансы</span><span class="sxs-lookup"><span data-stu-id="34367-127">Finance</span></span>](finance.md)  
<span data-ttu-id="34367-128">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="34367-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
