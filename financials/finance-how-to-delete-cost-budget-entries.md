---
title: "Практическое руководство. Удаление записей бюджета расходов | Документы Майкрософт"
description: "Используйте пакетное задание **Удалить записи бюджета затрат** для отмены операций бюджета затрат из регистра бюджета затрат."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 79c9a58c7cb91ce922b81eec1d2ccad375943203
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-delete-cost-budget-entries"></a><span data-ttu-id="2ada6-103">Практическое руководство. Удаление записей бюджета расходов</span><span class="sxs-lookup"><span data-stu-id="2ada6-103">How to: Delete Cost Budget Entries</span></span>
<span data-ttu-id="2ada6-104">Используйте пакетное задание **Удалить записи бюджета затрат** для отмены операций бюджета затрат из регистра бюджета затрат.</span><span class="sxs-lookup"><span data-stu-id="2ada6-104">You use the **Delete Cost Budget Entries** batch job to cancel cost budget entries from the cost budget register.</span></span>  

<span data-ttu-id="2ada6-105">Чтобы исключить все пропуски по операциям бюджета затрат и операциям регистра затрат, нельзя удалить единственную операцию или раздел операций в середине списка операций регистра.</span><span class="sxs-lookup"><span data-stu-id="2ada6-105">To prevent any gaps in the cost budget entries and cost register entries, you cannot delete a single entry or a batch of entries in the middle of the list of register entries.</span></span>  

### <a name="to-delete-a-cost-budget-entry"></a><span data-ttu-id="2ada6-106">Удаление записи бюджета затрат</span><span class="sxs-lookup"><span data-stu-id="2ada6-106">To delete a cost budget entry</span></span>  

1.  <span data-ttu-id="2ada6-107">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Удалить записи затрат бюджета**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2ada6-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Cost Budget Entries**, and then choose the related link.</span></span>  

    <span data-ttu-id="2ada6-108">В поле **В журнал №**</span><span class="sxs-lookup"><span data-stu-id="2ada6-108">The **To Register No.**</span></span> <span data-ttu-id="2ada6-109">содержится номер последней операции регистра, и поле не может быть изменено.</span><span class="sxs-lookup"><span data-stu-id="2ada6-109">field contains the last register entry number and cannot be changed.</span></span>  

    <span data-ttu-id="2ada6-110">Можно использовать поле **Из журнала №**</span><span class="sxs-lookup"><span data-stu-id="2ada6-110">You can use the **From Register No.**</span></span> <span data-ttu-id="2ada6-111">для выбора номера операции регистра, с которого должно начаться удаление.</span><span class="sxs-lookup"><span data-stu-id="2ada6-111">field to select a register entry number from which the deletion should begin.</span></span>  
2.  <span data-ttu-id="2ada6-112">Нажмите кнопку **OK**, чтобы удалить выбранные операции бюджета затрат.</span><span class="sxs-lookup"><span data-stu-id="2ada6-112">Choose the **OK** button to delete the selected cost budget entries.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2ada6-113">Чтобы избежать случайного удаления бюджетных операций, можно закрыть операции регистра, пометив эти строки как **Закрыто** в поле **Закрыто** в окне **Журналы бюджета расходов**.</span><span class="sxs-lookup"><span data-stu-id="2ada6-113">To avoid an accidental deletion of cost budget entries, you can close register entries by marking the lines as **Closed** in the **Closed** field in the **Cost Budget Registers** window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2ada6-114">См. также</span><span class="sxs-lookup"><span data-stu-id="2ada6-114">See Also</span></span>  
<span data-ttu-id="2ada6-115">[Учет по затратам](finance-manage-cost-accounting.md)
[Создание бюджетов затрат](finance-create-cost-budgets.md)</span><span class="sxs-lookup"><span data-stu-id="2ada6-115">[Accounting for Costs](finance-manage-cost-accounting.md)
[Creating Cost Budgets](finance-create-cost-budgets.md)</span></span>  
<span data-ttu-id="2ada6-116">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2ada6-116">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

