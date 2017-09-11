---
title: "Запись расходов или доходов непосредственно в ГК | Документы Майкрософт"
description: "Для бизнес-операций, которые не представлены документами, например небольшими расходами или наличными поступлениями, можно создавать соответствующие транзакции путем учета строк журналов в окне финансового журнала."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct posting, general ledger
ms.date: 06/15/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 7fa0d6b604a60e000208287546d831690a914931
ms.contentlocale: ru-ru
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-post-transactions-directly-to-the-general-ledger"></a><span data-ttu-id="8b6a3-103">Практическое руководство. Учет транзакций непосредственно в главной книге.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-103">How to: Post Transactions Directly to the General Ledger</span></span>
<span data-ttu-id="8b6a3-104">Большинство финансовых транзакций учитываются в главной книге с помощью отдельных бизнес-документов, например счетов покупки и заказов на продажу.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-104">Most financial transactions are posted to the general ledger through dedicated business documents, such as purchase invoices and sales orders.</span></span> <span data-ttu-id="8b6a3-105">Для бизнес-операций, которые не представлены документами в [!INCLUDE[d365fin](includes/d365fin_md.md)], например небольших расходов или наличных поступлений, можно создавать соответствующие транзакции путем учета строк журналов в окне **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-105">For business activities that are not represented by a document in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as smaller expenses or cash receipts, you can create the related transactions by posting journal lines in the **General Journal** window.</span></span>

<span data-ttu-id="8b6a3-106">Финансовые журналы используются для учета транзакций по счетам главной книги и другим счетам, таким как банковские счета, счета клиентов или поставщиков.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-106">General journals post financial transactions directly to general ledger accounts and other accounts, such as bank, customer, and vendor accounts.</span></span> <span data-ttu-id="8b6a3-107">В результате учета в финансовом журнале всегда создаются операции по счетам главной книги.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-107">Posting with a general journal always creates entries on general ledger accounts.</span></span> <span data-ttu-id="8b6a3-108">Это верно, даже если, к примеру, строка журнала учитывается в счете клиента, так как операция учитывается в счете дебиторской задолженности главной книги через учетную группу.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-108">This is true even when, for example, you post a journal line to a customer account, because an entry is posted to a general ledger receivables account through a posting group.</span></span> <span data-ttu-id="8b6a3-109">Вы можете персонализировать свою версию финансового журнала, настроив шаблон или раздел журнала.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-109">You can personalize your version of a general journal by setting up a journal batch or template.</span></span> <span data-ttu-id="8b6a3-110">Дополнительные сведения см. в разделе [Работа с финансовыми журналами](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="8b6a3-110">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>

<span data-ttu-id="8b6a3-111">В отличие от операций, которые учитываются с помощью документов, требующих обработки кредит-нот, вы можете корректно сторнировать операции, учтенные из финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-111">Unlike for entries that are posted with documents, which require a credit memo process, you can correctly reverse entries that are posted with the general journal.</span></span> <span data-ttu-id="8b6a3-112">Дополнительные сведения см. в разделе [Практическое руководство. Сторнирование учета в журнале](finance-how-reverse-journal-posting.md).</span><span class="sxs-lookup"><span data-stu-id="8b6a3-112">For more information, see [How to: Reverse Journal Posting](finance-how-reverse-journal-posting.md).</span></span>

## <a name="to-post-a-transaction-directly-to-a-general-ledger-account"></a><span data-ttu-id="8b6a3-113">Учет транзакции непосредственно на счете главной книге</span><span class="sxs-lookup"><span data-stu-id="8b6a3-113">To post a transaction directly to a general ledger account</span></span>
1. <span data-ttu-id="8b6a3-114">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Финансовые журналы**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="8b6a3-115">Откройте соответствующий раздел финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-115">Open the relevant general journal batch.</span></span> <span data-ttu-id="8b6a3-116">Дополнительные сведения см. в разделе [Работа с финансовыми журналами](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="8b6a3-116">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="8b6a3-117">На новой строке журнала заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-117">On a new journal line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]    
4. <span data-ttu-id="8b6a3-118">Повторите шаг 3 для всех отдельных транзакций, которые требуется учесть.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-118">Repeat step 3 for all the separate transactions that you want to post.</span></span>

    > [!TIP]  
    > <span data-ttu-id="8b6a3-119">Если необходимо ввести строки нескольких транзакций над одной строкой балансирующего счета, например, для одного банковского счета, установите флажок **Предлагаемая балансирующая сумма** в строке раздела в окне **Разделы финансового журнала**.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-119">If you want to enter multiple transaction lines above one balance-account line, for example, for one bank account, then select the **Suggest Balancing Amount** check box on the line for your batch in the **General Journal Batches** window.</span></span> <span data-ttu-id="8b6a3-120">Затем в поле **Сумма** строки балансирующего счета автоматически будет подставлено значение, необходимое для балансировки транзакций.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-120">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the transactions.</span></span>
5. <span data-ttu-id="8b6a3-121">Выберите действие **Учет**, чтобы записать транзакции на указанных счетах ГК.</span><span class="sxs-lookup"><span data-stu-id="8b6a3-121">Choose the **Post** action to record the transactions on the specified G/L accounts.</span></span>

## <a name="see-also"></a><span data-ttu-id="8b6a3-122">См. также</span><span class="sxs-lookup"><span data-stu-id="8b6a3-122">See Also</span></span>
[<span data-ttu-id="8b6a3-123">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="8b6a3-123">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="8b6a3-124">Практическое руководство. Сторнирование учета в журнале</span><span class="sxs-lookup"><span data-stu-id="8b6a3-124">How to: Reverse Journal Posting</span></span>](finance-how-reverse-journal-posting.md)  
[<span data-ttu-id="8b6a3-125">Финансы</span><span class="sxs-lookup"><span data-stu-id="8b6a3-125">Finance</span></span>](finance.md)  
<span data-ttu-id="8b6a3-126">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8b6a3-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

