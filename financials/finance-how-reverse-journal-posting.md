---
title: "Отмена учета журнала путем учета сторнирующей операции | Документы Майкрософт"
description: "Если выполнен ошибочный учет в финансовом журнале, можно воспользоваться функцией сторнирования транзакции, чтобы отменить учет, сохранив корректный след аудита."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 06/15/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 8126a53d59e72276eb1558fd65fe3c0cd53600cc
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-reverse-journal-posting"></a><span data-ttu-id="ab784-103">Практическое руководство. Сторнирование учета в журнале</span><span class="sxs-lookup"><span data-stu-id="ab784-103">How to: Reverse Journal Posting</span></span>
<span data-ttu-id="ab784-104">Что отменить ошибочную проводку в журнале, выберите операцию и создайте сторнирующую операцию (операции, идентичные исходным, но с противоположным знаком в поле суммы) с таким же номером документа и датой учета, что и у исходной операции.</span><span class="sxs-lookup"><span data-stu-id="ab784-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span></span> <span data-ttu-id="ab784-105">После сторнирования операции необходимо создать корректирующую запись.</span><span class="sxs-lookup"><span data-stu-id="ab784-105">After reversing an entry, you must make the correct entry.</span></span>

<span data-ttu-id="ab784-106">Можно сторнировать только те операции, которые были учтены из строки финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="ab784-106">You can only reverse entries that are posted from a general journal line.</span></span> <span data-ttu-id="ab784-107">Операцию можно сторнировать только один раз.</span><span class="sxs-lookup"><span data-stu-id="ab784-107">An entry can only be reversed once.</span></span>

<span data-ttu-id="ab784-108">Дополнительные сведения об учете из финансового журнала, см. в разделе [Практическое руководство. Учет транзакций непосредственно в главной книге](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="ab784-108">For more information about posting from a general journal, see [How to: Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span></span>

<span data-ttu-id="ab784-109">Операции можно сторнировать из всех окон **Книга операций**.</span><span class="sxs-lookup"><span data-stu-id="ab784-109">You can reverse entries from all **Ledger Entries** windows.</span></span> <span data-ttu-id="ab784-110">Следующая процедура основана на окне **Операции главной книги**.</span><span class="sxs-lookup"><span data-stu-id="ab784-110">The following procedure is based on the **General Ledger Entries** window.</span></span>

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a><span data-ttu-id="ab784-111">Сторнирование учета в журнале для операции главной книги</span><span class="sxs-lookup"><span data-stu-id="ab784-111">To reverse the journal posting of a general ledger entry</span></span>
1. <span data-ttu-id="ab784-112">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Операции главной книги**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="ab784-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Entries**, and then choose the related link.</span></span>
2. <span data-ttu-id="ab784-113">Выберите операцию, которую требуется сторнировать, а затем выберите **Сторнировать транзакцию**.</span><span class="sxs-lookup"><span data-stu-id="ab784-113">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span></span> <span data-ttu-id="ab784-114">Следует отметить, что операцию нужно выполнять из учтенной операции в журнале.</span><span class="sxs-lookup"><span data-stu-id="ab784-114">Note that is must originate from a journal posting.</span></span>
3. <span data-ttu-id="ab784-115">В окне **Сторнировать операции транзакции** выберите соответствующую операцию, а затем выберите действие **Сторнировать**.</span><span class="sxs-lookup"><span data-stu-id="ab784-115">In the **Reverse Transaction Entries** window, select the relevant entry, and then choose the **Reverse** action.</span></span>
4. <span data-ttu-id="ab784-116">Нажмите кнопку **Да** в сообщении подтверждения.</span><span class="sxs-lookup"><span data-stu-id="ab784-116">Choose the **Yes** button on the confirmation message.</span></span>

## <a name="see-also"></a><span data-ttu-id="ab784-117">См. также</span><span class="sxs-lookup"><span data-stu-id="ab784-117">See Also</span></span>
<span data-ttu-id="ab784-118">[Практическое руководство. Учет транзакций непосредственно в главной книге](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="ab784-118">[How to: Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md)</span></span>  
[<span data-ttu-id="ab784-119">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="ab784-119">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="ab784-120">Финансы</span><span class="sxs-lookup"><span data-stu-id="ab784-120">Finance</span></span>](finance.md)  
<span data-ttu-id="ab784-121">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ab784-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

