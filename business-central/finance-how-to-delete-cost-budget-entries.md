---
title: "Практическое руководство. Удаление записей бюджета расходов | Документы Майкрософт"
description: "Используйте пакетное задание **Удалить записи бюджета затрат** для отмены операций бюджета затрат из регистра бюджета затрат."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: f578247ef835b3c7803adb123e18eec62b0864b9
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="delete-cost-budget-entries"></a><span data-ttu-id="2e971-103">Удалить записи затрат бюджета</span><span class="sxs-lookup"><span data-stu-id="2e971-103">Delete Cost Budget Entries</span></span>
<span data-ttu-id="2e971-104">Используйте пакетное задание **Удалить записи бюджета затрат** для отмены операций бюджета затрат из регистра бюджета затрат.</span><span class="sxs-lookup"><span data-stu-id="2e971-104">You use the **Delete Cost Budget Entries** batch job to cancel cost budget entries from the cost budget register.</span></span>  

<span data-ttu-id="2e971-105">Чтобы исключить все пропуски по операциям бюджета затрат и операциям регистра затрат, нельзя удалить единственную операцию или раздел операций в середине списка операций регистра.</span><span class="sxs-lookup"><span data-stu-id="2e971-105">To prevent any gaps in the cost budget entries and cost register entries, you cannot delete a single entry or a batch of entries in the middle of the list of register entries.</span></span>  

### <a name="to-delete-a-cost-budget-entry"></a><span data-ttu-id="2e971-106">Удаление записи бюджета затрат</span><span class="sxs-lookup"><span data-stu-id="2e971-106">To delete a cost budget entry</span></span>  

1.  <span data-ttu-id="2e971-107">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Удалить записи затрат бюджета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2e971-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Cost Budget Entries**, and then choose the related link.</span></span>  

    <span data-ttu-id="2e971-108">В поле **В журнал №**</span><span class="sxs-lookup"><span data-stu-id="2e971-108">The **To Register No.**</span></span> <span data-ttu-id="2e971-109">содержится номер последней операции регистра, и поле не может быть изменено.</span><span class="sxs-lookup"><span data-stu-id="2e971-109">field contains the last register entry number and cannot be changed.</span></span>  

    <span data-ttu-id="2e971-110">Можно использовать поле **Из журнала №**</span><span class="sxs-lookup"><span data-stu-id="2e971-110">You can use the **From Register No.**</span></span> <span data-ttu-id="2e971-111">для выбора номера операции регистра, с которого должно начаться удаление.</span><span class="sxs-lookup"><span data-stu-id="2e971-111">field to select a register entry number from which the deletion should begin.</span></span>  
2.  <span data-ttu-id="2e971-112">Нажмите кнопку **ОК**, чтобы удалить выбранные операции бюджета затрат.</span><span class="sxs-lookup"><span data-stu-id="2e971-112">Choose the **OK** button to delete the selected cost budget entries.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2e971-113">Чтобы избежать случайного удаления бюджетных операций, можно закрыть операции регистра, пометив эти строки как **Закрыто** в поле **Закрыто** на странице **Журналы бюджета расходов**.</span><span class="sxs-lookup"><span data-stu-id="2e971-113">To avoid an accidental deletion of cost budget entries, you can close register entries by marking the lines as **Closed** in the **Closed** field on the **Cost Budget Registers** page.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2e971-114">См. также</span><span class="sxs-lookup"><span data-stu-id="2e971-114">See Also</span></span>  
<span data-ttu-id="2e971-115">[Учет по затратам](finance-manage-cost-accounting.md)
[Создание бюджетов затрат](finance-create-cost-budgets.md)</span><span class="sxs-lookup"><span data-stu-id="2e971-115">[Accounting for Costs](finance-manage-cost-accounting.md)
[Creating Cost Budgets](finance-create-cost-budgets.md)</span></span>  
<span data-ttu-id="2e971-116">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2e971-116">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

