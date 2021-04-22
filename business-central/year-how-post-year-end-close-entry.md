---
title: Учет операции закрытия года
description: Описывается порядок открытия журнала, указанного в пакетном задании "Закрытие отчета о прибылях и убытках", и проверки и учета операции закрытия года.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 5c822685ae5723bc6b13f9fedad45dbddefdb956
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776596"
---
# <a name="post-the-year-end-closing-entry"></a><span data-ttu-id="55f12-103">Учет операции закрытия года</span><span class="sxs-lookup"><span data-stu-id="55f12-103">Post the Year-End Closing Entry</span></span>

<span data-ttu-id="55f12-104">После использования пакетного задания **Закрытие отчета о прибылях и убытках** для создания закрывающей операции (операций) на конец года необходимо открыть журнал, указанный для пакетного задания, и затем просмотреть и учесть записи.</span><span class="sxs-lookup"><span data-stu-id="55f12-104">After you use the **Close Income Statement** batch job to generate the year-end closing entry or entries, you must open the journal you specified in the batch job, and then review and post the entries.</span></span>  

> [!TIP]
> <span data-ttu-id="55f12-105">В зависимости от рабочих процессов вашей организации вы можете закрыть или не закрывать учетные периоды и финансовые годы в [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="55f12-105">Depending on your organizations work processes, you can choose to close or not close accounting periods and fiscal years in [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="55f12-106">В следующей процедуре предполагается, что вы закрыли финансовый год с помощью варианта *Учетные периоды*, создав запись закрытия года с использованием пакетного задания **Закрытие отчета о прибылях и убытках**, и теперь готовы к разноске записи закрытия в конце года вместе с операциями корреспондирующего счета собственных средств.</span><span class="sxs-lookup"><span data-stu-id="55f12-106">The following procedure assumes that you have closed the fiscal year using the *Accounting Periods* option, generated a year-end closing entry using the **Close Income Statement** batch job, and are now ready to post the year-end closing entry along with the offsetting equity account entries.</span></span> <span data-ttu-id="55f12-107">Ваша организация может выбрать другой вариант работы, например, разнести запись закрытия года как часть закрытия финансового года.</span><span class="sxs-lookup"><span data-stu-id="55f12-107">Your organization can choose to work differently, such as post the year-end closing entry as part of closing the fiscal year.</span></span>

## <a name="to-post-the-year-end-closing-entry"></a><span data-ttu-id="55f12-108">Учет операции закрытия года</span><span class="sxs-lookup"><span data-stu-id="55f12-108">To post the year end closing entry</span></span>

1. <span data-ttu-id="55f12-109">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовый журнал**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="55f12-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="55f12-110">На странице **Финансовый журнал** в поле **Код раздела** выберите раздел, который содержит закрывающие операции.</span><span class="sxs-lookup"><span data-stu-id="55f12-110">On the **General Journal** page, in the **Batch Name** field, select the batch that contains the closing entries.</span></span>
3. <span data-ttu-id="55f12-111">Проверьте записи.</span><span class="sxs-lookup"><span data-stu-id="55f12-111">Review the entries.</span></span>
4. <span data-ttu-id="55f12-112">Чтобы учесть журнал, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="55f12-112">To post the journal, choose the **Post** action.</span></span>

> [!NOTE]  
> <span data-ttu-id="55f12-113">При обнаружении ошибки отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="55f12-113">If an error is detected, an error message is displayed.</span></span> <span data-ttu-id="55f12-114">Если учет выполнен успешно, система удалит учтенные записи из журнала.</span><span class="sxs-lookup"><span data-stu-id="55f12-114">If the posting is successful, the posted entries are removed from the journal.</span></span> <span data-ttu-id="55f12-115">После завершения учета запись учитывается во всех счетах прибылей и убытков, при этом ее сальдо становится нулевым, и результат года переносится в балансовый отчет.</span><span class="sxs-lookup"><span data-stu-id="55f12-115">After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.</span></span>

## <a name="see-also"></a><span data-ttu-id="55f12-116">См. также</span><span class="sxs-lookup"><span data-stu-id="55f12-116">See Also</span></span>

[<span data-ttu-id="55f12-117">Закрытие учетных периодов</span><span class="sxs-lookup"><span data-stu-id="55f12-117">Close Accounting Periods</span></span>](year-close-account-periods.md)  
[<span data-ttu-id="55f12-118">Закрытие книг</span><span class="sxs-lookup"><span data-stu-id="55f12-118">Closing Books</span></span>](year-close-books.md)  
[<span data-ttu-id="55f12-119">Закрытие отчета о прибылях и убытках</span><span class="sxs-lookup"><span data-stu-id="55f12-119">Close Income Statement</span></span>](year-close-income-statement.md)  
<span data-ttu-id="55f12-120">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="55f12-120">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]