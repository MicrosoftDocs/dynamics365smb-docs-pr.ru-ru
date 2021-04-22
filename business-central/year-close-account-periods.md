---
title: Закрытие учетных периодов для финансового года | Документация Майкрософт
description: Описывается порядок закрытия учетных периодов, составляющих финансовый год.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: a26baaf947fdac133e3bfcd50489d680231d9971
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5786686"
---
# <a name="close-accounting-periods"></a><span data-ttu-id="9c14d-103">Закрытие учетных периодов</span><span class="sxs-lookup"><span data-stu-id="9c14d-103">Close Accounting Periods</span></span>
<span data-ttu-id="9c14d-104">При завершении финансового года следует завершить периоды, которые его образуют.</span><span class="sxs-lookup"><span data-stu-id="9c14d-104">When a fiscal year is over, you must close the periods that comprise it.</span></span>

## <a name="to-close-accounting-periods"></a><span data-ttu-id="9c14d-105">Практическое руководство. Закрытие учетных периодов</span><span class="sxs-lookup"><span data-stu-id="9c14d-105">To close accounting periods</span></span>
1. <span data-ttu-id="9c14d-106">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учетные периоды**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="9c14d-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Accounting Periods**, and then choose the related link.</span></span>
2. <span data-ttu-id="9c14d-107">На странице **Учетные периоды** выберите действие **Закрыть год**.</span><span class="sxs-lookup"><span data-stu-id="9c14d-107">On the **Accounting Periods** page, choose the **Close Year** action.</span></span>

    <span data-ttu-id="9c14d-108">Если открыто несколько финансовых лет, автоматически считается, что должен быть закрыт более ранний год.</span><span class="sxs-lookup"><span data-stu-id="9c14d-108">If more than one fiscal year is open, the earliest one is automatically selected to be closed.</span></span> <span data-ttu-id="9c14d-109">Отображается сообщение, указывающее подлежащий закрытию год и сообщающее о последствиях закрытия года.</span><span class="sxs-lookup"><span data-stu-id="9c14d-109">A message displays identifying the year that will close and the consequences of closing the year.</span></span>
3. <span data-ttu-id="9c14d-110">Для закрытия года нажмите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="9c14d-110">To close the year, choose the **Yes** button.</span></span>

<span data-ttu-id="9c14d-111">Финансовый год закрыт, и выбираются поля **Закрыто** и **Дата закрыта** для всех периодов в таком году.</span><span class="sxs-lookup"><span data-stu-id="9c14d-111">The fiscal year is closed, and the **Closed** and **Date Locked** fields for all the periods in the year are selected.</span></span> <span data-ttu-id="9c14d-112">Финансовый год не может быть открыт снова, и флажок из полей **Закрыто** или **Дата закрыта** удалить нельзя.</span><span class="sxs-lookup"><span data-stu-id="9c14d-112">The fiscal year cannot be opened again and you cannot remove the check mark from the **Closed** or **Date Locked** fields.</span></span>

> [!NOTE]  
>   <span data-ttu-id="9c14d-113">Нельзя закрыть финансовый год, если прежде не будет открыт новый финансовый год.</span><span class="sxs-lookup"><span data-stu-id="9c14d-113">You cannot close a fiscal year before you create a new one.</span></span> <span data-ttu-id="9c14d-114">Следует отметить, что после закрытия финансового года уже невозможно изменить дату начала следующего финансового года.</span><span class="sxs-lookup"><span data-stu-id="9c14d-114">Notice that when a fiscal year has been closed, you cannot change the starting date of the following fiscal year.</span></span>

<span data-ttu-id="9c14d-115">Несмотря на то, что финансовый год закрыт, можно по-прежнему производить учет ГК операций по нему.</span><span class="sxs-lookup"><span data-stu-id="9c14d-115">Even though a fiscal year has been closed, you can still post general ledger entries to it.</span></span> <span data-ttu-id="9c14d-116">При этом операции будут помечаться как учтенные по закрытому финансовому году, и будет выбрано поле **Операция прошлого года**.</span><span class="sxs-lookup"><span data-stu-id="9c14d-116">When you do this, the entries will be marked as posted to a closed fiscal year and the **Prior-Year Entry** field will be selected.</span></span>

<span data-ttu-id="9c14d-117">После закрытия финансового года счета прибылей и убытков следует закрыть, а результаты года должны быть перемещены на счет в балансовом отчете.</span><span class="sxs-lookup"><span data-stu-id="9c14d-117">After a fiscal year is closed, you must close the income statement accounts and transfer the year's results to an account in the balance sheet.</span></span> <span data-ttu-id="9c14d-118">Эти действия можно повторять при каждом учете закрытого финансового года.</span><span class="sxs-lookup"><span data-stu-id="9c14d-118">You can repeat this every time that you post to the closed fiscal year.</span></span>

## <a name="see-also"></a><span data-ttu-id="9c14d-119">См. также</span><span class="sxs-lookup"><span data-stu-id="9c14d-119">See Also</span></span>

[<span data-ttu-id="9c14d-120">Закрытие книг</span><span class="sxs-lookup"><span data-stu-id="9c14d-120">Closing Books</span></span>](year-close-books.md)  
[<span data-ttu-id="9c14d-121">Учет операции закрытия года</span><span class="sxs-lookup"><span data-stu-id="9c14d-121">Post the Year-End Closing Entry</span></span>](year-how-post-year-end-close-entry.md)  
[<span data-ttu-id="9c14d-122">Работа с учетными периодами и финансовыми годами</span><span class="sxs-lookup"><span data-stu-id="9c14d-122">Work with Accounting Periods and Fiscal Years</span></span>](finance-accounting-periods-and-fiscal-years.md)  
<span data-ttu-id="9c14d-123">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9c14d-123">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]