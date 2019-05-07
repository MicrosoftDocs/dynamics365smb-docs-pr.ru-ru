---
title: Проверка и учет операции закрытия года | Документы Майкрософт
description: Описывается порядок открытия журнала, указанного в пакетном задании "Закрытие отчета о прибылях и убытках", и проверки и учета операции закрытия года.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: 878079fd02a2d54ae6b878fa54c7006dee779c15
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "914908"
---
# <a name="post-the-year-end-closing-entry"></a><span data-ttu-id="a9c06-103">Учет операции закрытия года</span><span class="sxs-lookup"><span data-stu-id="a9c06-103">Post the Year-End Closing Entry</span></span>
<span data-ttu-id="a9c06-104">После использования пакетного задания **Закрытие отчета о прибылях и убытках** для создания закрывающей операции (операций) на конец года необходимо открыть журнал, указанный для пакетного задания, и затем просмотреть и учесть записи.</span><span class="sxs-lookup"><span data-stu-id="a9c06-104">After you use the **Close Income Statement** batch job to generate the year-end closing entry or entries, you must open the journal you specified in the batch job, and then review and post the entries.</span></span>

## <a name="to-post-the-year-end-closing-entry"></a><span data-ttu-id="a9c06-105">Учет операции закрытия года</span><span class="sxs-lookup"><span data-stu-id="a9c06-105">To post the year end closing entry</span></span>
1. <span data-ttu-id="a9c06-106">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовый журнал**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="a9c06-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="a9c06-107">На странице **Финансовый журнал** в поле **Код раздела** выберите раздел, который содержит закрывающие операции.</span><span class="sxs-lookup"><span data-stu-id="a9c06-107">On the **General Journal** page, in the **Batch Name** field, select the batch that contains the closing entries.</span></span>
3. <span data-ttu-id="a9c06-108">Проверьте записи.</span><span class="sxs-lookup"><span data-stu-id="a9c06-108">Review the entries.</span></span>
4. <span data-ttu-id="a9c06-109">Чтобы учесть журнал, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="a9c06-109">To post the journal, choose the **Post** action.</span></span>

> [!NOTE]  
>   <span data-ttu-id="a9c06-110">При обнаружении ошибки отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="a9c06-110">If an error is detected, an error message is displayed.</span></span> <span data-ttu-id="a9c06-111">Если учет выполнен успешно, система удалит учтенные записи из журнала.</span><span class="sxs-lookup"><span data-stu-id="a9c06-111">If the posting is successful, the posted entries are removed from the journal.</span></span> <span data-ttu-id="a9c06-112">После завершения учета запись учитывается во всех счетах прибылей и убытков, при этом ее сальдо становится нулевым, и результат года переносится в балансовый отчет.</span><span class="sxs-lookup"><span data-stu-id="a9c06-112">After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.</span></span>

## <a name="see-also"></a><span data-ttu-id="a9c06-113">См. также</span><span class="sxs-lookup"><span data-stu-id="a9c06-113">See Also</span></span>
[<span data-ttu-id="a9c06-114">Закрытие учетных периодов</span><span class="sxs-lookup"><span data-stu-id="a9c06-114">Close Accounting Periods</span></span>](year-close-account-periods.md)  
[<span data-ttu-id="a9c06-115">Закрытие книг</span><span class="sxs-lookup"><span data-stu-id="a9c06-115">Closing Books</span></span>](year-close-books.md)  
[<span data-ttu-id="a9c06-116">Закрытие отчета о прибылях и убытках</span><span class="sxs-lookup"><span data-stu-id="a9c06-116">Close Income Statement</span></span>](year-close-income-statement.md)  
<span data-ttu-id="a9c06-117">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a9c06-117">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
