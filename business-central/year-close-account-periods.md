---
title: "Закрытие учетных периодов для финансового года | Документы Майкрософт"
description: "Описывается порядок закрытия учетных периодов, составляющих финансовый год."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: f0bdc88cb2d52ed8e1558fb140f904f792e539ff
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="close-accounting-periods"></a><span data-ttu-id="a5952-103">Закрытие учетных периодов</span><span class="sxs-lookup"><span data-stu-id="a5952-103">Close Accounting Periods</span></span>
<span data-ttu-id="a5952-104">При завершении финансового года следует завершить периоды, которые его образуют.</span><span class="sxs-lookup"><span data-stu-id="a5952-104">When a fiscal year is over, you must close the periods that comprise it.</span></span>

## <a name="to-close-accounting-periods"></a><span data-ttu-id="a5952-105">Практическое руководство. Закрытие учетных периодов</span><span class="sxs-lookup"><span data-stu-id="a5952-105">To close accounting periods</span></span>
1. <span data-ttu-id="a5952-106">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учетные периоды**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="a5952-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Accounting Periods**, and then choose the related link.</span></span>
2. <span data-ttu-id="a5952-107">В окне **Учетные периоды** выберите действие **Закрыть год**.</span><span class="sxs-lookup"><span data-stu-id="a5952-107">In the **Accounting Periods** window, choose the **Close Year** action.</span></span>

    <span data-ttu-id="a5952-108">Если открыто несколько финансовых лет, автоматически считается, что должен быть закрыт более ранний год.</span><span class="sxs-lookup"><span data-stu-id="a5952-108">If more than one fiscal year is open, the earliest one is automatically selected to be closed.</span></span> <span data-ttu-id="a5952-109">Отображается сообщение, указывающее подлежащий закрытию год и сообщающее о последствиях закрытия года.</span><span class="sxs-lookup"><span data-stu-id="a5952-109">A message displays identifying the year that will close and the consequences of closing the year.</span></span>
3. <span data-ttu-id="a5952-110">Для закрытия года нажмите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="a5952-110">To close the year, choose the **Yes** button.</span></span>

<span data-ttu-id="a5952-111">Финансовый год закрыт, и выбираются поля **Закрыто** и **Дата закрыта** для всех периодов в таком году.</span><span class="sxs-lookup"><span data-stu-id="a5952-111">The fiscal year is closed, and the **Closed** and **Date Locked** fields for all the periods in the year are selected.</span></span> <span data-ttu-id="a5952-112">Финансовый год не может быть открыт снова, и флажок из полей **Закрыто** или **Дата закрыта** удалить нельзя.</span><span class="sxs-lookup"><span data-stu-id="a5952-112">The fiscal year cannot be opened again and you cannot remove the check mark from the **Closed** or **Date Locked** fields.</span></span>

> [!NOTE]  
>   <span data-ttu-id="a5952-113">Нельзя закрыть финансовый год, если прежде не будет открыт новый финансовый год.</span><span class="sxs-lookup"><span data-stu-id="a5952-113">You cannot close a fiscal year before you create a new one.</span></span> <span data-ttu-id="a5952-114">Следует отметить, что после закрытия финансового года уже невозможно изменить дату начала следующего финансового года.</span><span class="sxs-lookup"><span data-stu-id="a5952-114">Notice that when a fiscal year has been closed, you cannot change the starting date of the following fiscal year.</span></span>

<span data-ttu-id="a5952-115">Несмотря на то, что финансовый год закрыт, можно по-прежнему производить учет ГК операций по нему.</span><span class="sxs-lookup"><span data-stu-id="a5952-115">Even though a fiscal year has been closed, you can still post general ledger entries to it.</span></span> <span data-ttu-id="a5952-116">При этом операции будут помечаться как учтенные по закрытому финансовому году, и будет выбрано поле **Операция прошлого года**.</span><span class="sxs-lookup"><span data-stu-id="a5952-116">When you do this, the entries will be marked as posted to a closed fiscal year and the **Prior-Year Entry** field will be selected.</span></span>

<span data-ttu-id="a5952-117">После закрытия финансового года счета прибылей и убытков следует закрыть, а результаты года должны быть перемещены на счет в балансовом отчете.</span><span class="sxs-lookup"><span data-stu-id="a5952-117">After a fiscal year is closed, you must close the income statement accounts and transfer the year's results to an account in the balance sheet.</span></span> <span data-ttu-id="a5952-118">Эти действия можно повторять при каждом учете закрытого финансового года.</span><span class="sxs-lookup"><span data-stu-id="a5952-118">You can repeat this every time that you post to the closed fiscal year.</span></span>

## <a name="see-also"></a><span data-ttu-id="a5952-119">См. также</span><span class="sxs-lookup"><span data-stu-id="a5952-119">See Also</span></span>
[<span data-ttu-id="a5952-120">Закрытие книг</span><span class="sxs-lookup"><span data-stu-id="a5952-120">Closing Books</span></span>](year-close-books.md)  
[<span data-ttu-id="a5952-121">Учет операции закрытия года</span><span class="sxs-lookup"><span data-stu-id="a5952-121">Post the Year-End Closing Entry</span></span>](year-how-post-year-end-close-entry.md)  
[<span data-ttu-id="a5952-122">Открытие нового финансового года</span><span class="sxs-lookup"><span data-stu-id="a5952-122">Open a New Fiscal Year</span></span>](finance-how-open-new-fiscal-year.md)  
<span data-ttu-id="a5952-123">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a5952-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

