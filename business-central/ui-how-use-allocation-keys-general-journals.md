---
title: Использование ключей распределения в финансовых журналах | Документация Майкрософт
description: Узнайте, как можно использовать ключи распределения в журналах.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost accounting
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: 9c540b04b7dcda7cd3b656a86679228af08261c9
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2310928"
---
# <a name="use-allocation-keys-in-general-journals"></a><span data-ttu-id="eb475-103">Использование ключей распределения в финансовых журналах</span><span class="sxs-lookup"><span data-stu-id="eb475-103">Use Allocation Keys in General Journals</span></span>
<span data-ttu-id="eb475-104">При учете журнала операцию финансового журнала можно распределить по нескольким разным счетам.</span><span class="sxs-lookup"><span data-stu-id="eb475-104">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="eb475-105">Распределение может выполняться по количеству, по процентному отношению или сумме.</span><span class="sxs-lookup"><span data-stu-id="eb475-105">The allocation can be made by quantity, percentage, or amount.</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="eb475-106">Настройка ключей распределения</span><span class="sxs-lookup"><span data-stu-id="eb475-106">To set up allocation keys</span></span>
1. <span data-ttu-id="eb475-107">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Типовой финансовый журнал**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="eb475-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="eb475-108">Выберите поле **Код раздела**, чтобы открыть страницу **Разделы финансового журнала**.</span><span class="sxs-lookup"><span data-stu-id="eb475-108">Choose the **Batch Name** field to open the **General Journal Batches** page.</span></span>
3. <span data-ttu-id="eb475-109">Вы можете изменить распределения в существующем разделе в списке или создать новый раздел с распределениями.</span><span class="sxs-lookup"><span data-stu-id="eb475-109">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
   * <span data-ttu-id="eb475-110">Для создания нового раздела выберите действие **Создать** и перейдите к следующему шагу.</span><span class="sxs-lookup"><span data-stu-id="eb475-110">To create a new batch, choose the **New** action, and go to the next step.</span></span>
   * <span data-ttu-id="eb475-111">Для изменения распределений в существующем журнале выберите журнал и перейдите к шагу 7.</span><span class="sxs-lookup"><span data-stu-id="eb475-111">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="eb475-112">В поле **Название** укажите название раздела, например CLEANING.</span><span class="sxs-lookup"><span data-stu-id="eb475-112">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="eb475-113">В поле **Описание** введите описание, например "Журнал для расходов по уборке".</span><span class="sxs-lookup"><span data-stu-id="eb475-113">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="eb475-114">По завершении закройте страницу.</span><span class="sxs-lookup"><span data-stu-id="eb475-114">When you are done, close the page.</span></span> <span data-ttu-id="eb475-115">Откроется новый пустой типовой журнал.</span><span class="sxs-lookup"><span data-stu-id="eb475-115">A new, empty recurring journal opens.</span></span>
6. <span data-ttu-id="eb475-116">Заполните поля строки.</span><span class="sxs-lookup"><span data-stu-id="eb475-116">Fill in the fields on the line.</span></span>
7. <span data-ttu-id="eb475-117">Выберите действие **Распределения**.</span><span class="sxs-lookup"><span data-stu-id="eb475-117">Choose the **Allocations** action.</span></span>
8. <span data-ttu-id="eb475-118">Добавьте строку для каждого распределения.</span><span class="sxs-lookup"><span data-stu-id="eb475-118">Add a line for each allocation.</span></span> <span data-ttu-id="eb475-119">Следует по выбору заполнить поля **Распределение (%)**, **Распред. кол-во** или **Сумма**.</span><span class="sxs-lookup"><span data-stu-id="eb475-119">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="eb475-120">Следует также заполнить поле **Номер счета** и, если производится распределение транзакции по глобальным измерениям, поля глобального измерения.</span><span class="sxs-lookup"><span data-stu-id="eb475-120">You must also fill in the **Account No.** field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="eb475-121">Если в строке указан процент, сумма в поле **Сумма** будет рассчитана автоматически.</span><span class="sxs-lookup"><span data-stu-id="eb475-121">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="eb475-122">Эти суммы по знаку противоположны итоговой сумме из поля **Сумма** типового журнала.</span><span class="sxs-lookup"><span data-stu-id="eb475-122">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="eb475-123">После ввода строк распределения выберите **OK**, чтобы вернуться на страницу **Типовой финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="eb475-123">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** page.</span></span> <span data-ttu-id="eb475-124">Поле **Распред. сумма (руб.)** будет заполнено и его значение будет соответствовать полю **Сумма**.</span><span class="sxs-lookup"><span data-stu-id="eb475-124">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="eb475-125">Выполните учет журнала.</span><span class="sxs-lookup"><span data-stu-id="eb475-125">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="eb475-126">Изменение уже настроенного ключа распределения</span><span class="sxs-lookup"><span data-stu-id="eb475-126">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="eb475-127">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Типовой финансовый журнал**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="eb475-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="eb475-128">На странице **Типовой финансовый журнал** выберите журнал с распределением.</span><span class="sxs-lookup"><span data-stu-id="eb475-128">On the **Recurring General Journal** page, select the journal with the allocation.</span></span>
3. <span data-ttu-id="eb475-129">Выберите строку с распределением, а затем выберите действие **Распределения**.</span><span class="sxs-lookup"><span data-stu-id="eb475-129">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="eb475-130">Измените соответствующие поля и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="eb475-130">Change the relevant fields, and then choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="eb475-131">См. также</span><span class="sxs-lookup"><span data-stu-id="eb475-131">See Also</span></span>
[<span data-ttu-id="eb475-132">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="eb475-132">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="eb475-133">Учет документов и журналов</span><span class="sxs-lookup"><span data-stu-id="eb475-133">Posting Documents and Journals</span></span>](ui-post-documents-journals.md)  
<span data-ttu-id="eb475-134">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="eb475-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
