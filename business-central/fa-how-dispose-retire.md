---
title: "Списание или выбытие ОС | Документы Майкрософт"
description: "Вы должны учитывать стоимость выбытия при продаже, списании или отбраковке основных средств."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: scrap
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 10e7939378d222e2e2f915c89f820e000615ac1e
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="dispose-of-or-retire-fixed-assets"></a><span data-ttu-id="7c47c-103">Списание или выбытие основных средств</span><span class="sxs-lookup"><span data-stu-id="7c47c-103">Dispose of or Retire Fixed Assets</span></span>
<span data-ttu-id="7c47c-104">При продаже основного средства или его списании по другим причинам необходимо учесть сумму выбытия для расчета и регистрации прибыли или убытков.</span><span class="sxs-lookup"><span data-stu-id="7c47c-104">When you sell or otherwise dispose of a fixed asset, the disposal value must be posted to calculate and record the gain or loss.</span></span> <span data-ttu-id="7c47c-105">Операция выбытия должна быть последней операцией, учтенной для основного средства.</span><span class="sxs-lookup"><span data-stu-id="7c47c-105">A disposal entry must be the last entry posted for a fixed asset.</span></span> <span data-ttu-id="7c47c-106">Для частично списанного основного средства можно учесть более одной операции выбытия.</span><span class="sxs-lookup"><span data-stu-id="7c47c-106">For partially disposed fixed assets, you can post more than one disposal entry.</span></span> <span data-ttu-id="7c47c-107">Общая сумма всех учтенных сумм выбытия должна быть суммой по кредиту.</span><span class="sxs-lookup"><span data-stu-id="7c47c-107">The total of all posted disposal amounts must be a credit amount.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="7c47c-108">При бартере основных средств необходимо записать продажу старого актива (выбытие) и покупку нового актива (приобретение).</span><span class="sxs-lookup"><span data-stu-id="7c47c-108">If you trade-in a fixed asset for another one, you must record both the sale of the old asset (disposal) and the purchase of the new one (acquisition).</span></span> <span data-ttu-id="7c47c-109">Дополнительные сведения см. в разделе [Приобретение основных средств](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="7c47c-109">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span></span>  

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a><span data-ttu-id="7c47c-110">Учет выбытия с использованием журнала ГК учета основных средств</span><span class="sxs-lookup"><span data-stu-id="7c47c-110">To post a disposal from the fixed asset G/L journal</span></span>
1. <span data-ttu-id="7c47c-111">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы ГК для ОС**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="7c47c-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="7c47c-112">Создайте начальную строку журнала и заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="7c47c-112">Create an initial journal line and fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="7c47c-113">В поле **Тип учета ОС** выберите **Реализация**.</span><span class="sxs-lookup"><span data-stu-id="7c47c-113">In the **FA Posting Type** field, select **Disposal**.</span></span>  
4. <span data-ttu-id="7c47c-114">Выберите действие **Вставить баланс. счет ОС**.</span><span class="sxs-lookup"><span data-stu-id="7c47c-114">Choose the **Insert FA Bal. Account** action.</span></span> <span data-ttu-id="7c47c-115">Вторая строка журнала создается для балансирующего счета, который настроен для учета выбытия.</span><span class="sxs-lookup"><span data-stu-id="7c47c-115">A second journal line is created for the balancing account that is set up for disposal posting.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="7c47c-116">Шаг 4 работает только в том случае, если выполнены следующие настройки: на странице **Карточка учетной группы ОС** для учетной группы основного средства поле **Счет ГК реализации** содержит дебетовый счет главной книги, а поле **Баланс. счет реализации** содержит счет главной книги, на котором требуется учитывать балансовые операции для повышения стоимости.</span><span class="sxs-lookup"><span data-stu-id="7c47c-116">Step 4 only works if you have set up the following: On the **FA Posting Group Card** page for the posting group of the fixed asset, the **Disposal Account** field contains the general ledger debit account and the **Disposal Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span></span> <span data-ttu-id="7c47c-117">Дополнительные сведения см. в пункте "Настройка учетных групп основных средств" в разделе [Настройка общих данных основных средств](fa-how-setup-general.md).</span><span class="sxs-lookup"><span data-stu-id="7c47c-117">For more information, see the "To set up fixed asset posting groups" section in [Set Up General Fixed Asset Information](fa-how-setup-general.md).</span></span>  
5. <span data-ttu-id="7c47c-118">Выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="7c47c-118">Choose the **Post** action.</span></span>  

<span data-ttu-id="7c47c-119">В случае продажи или другого выбытия части основного средства, следует разделить средство до регистрации транзакции реализации.</span><span class="sxs-lookup"><span data-stu-id="7c47c-119">If you sell or dispose of part of a fixed asset, you must split up the asset before you can record the disposal transaction.</span></span> <span data-ttu-id="7c47c-120">Дополнительные сведения см. в разделе [Перемещение, разделение или объединение основных средств](fa-how-trans-split-combine.md).</span><span class="sxs-lookup"><span data-stu-id="7c47c-120">For more information, see [Transfer, Split, or Combine Fixed Assets](fa-how-trans-split-combine.md).</span></span>  

## <a name="to-view-disposal-ledger-entries"></a><span data-ttu-id="7c47c-121">Просмотр операций книги выбытия</span><span class="sxs-lookup"><span data-stu-id="7c47c-121">To view disposal ledger entries</span></span>
<span data-ttu-id="7c47c-122">При продаже или списании основного средства сумма списания учитывается в главной книге, в которой можно просмотреть результат.</span><span class="sxs-lookup"><span data-stu-id="7c47c-122">When you sell or dispose of a fixed asset, the disposal value is posted to the general ledger where you can view the result.</span></span>  

1. <span data-ttu-id="7c47c-123">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Основные средства**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="7c47c-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="7c47c-124">Выберите основное средство, для которого требуется просмотреть операции, затем выберите действие **Книги амортизации**.</span><span class="sxs-lookup"><span data-stu-id="7c47c-124">Select the fixed asset that you want to view entries for, and then choose the **Depreciation Books** action.</span></span>  
3. <span data-ttu-id="7c47c-125">Выберите книгу амортизации, для которой требуется просмотреть операции, затем выберите действие **Книга операций**.</span><span class="sxs-lookup"><span data-stu-id="7c47c-125">Select the depreciation book that you want to view entries for, and then choose the **Ledger Entries** action.</span></span>  
4. <span data-ttu-id="7c47c-126">Выберите строку со значением **Реализация** в поле **Категория учета ОС**, затем выберите действие **Перейти**.</span><span class="sxs-lookup"><span data-stu-id="7c47c-126">Select a line with **Disposal** in the **FA Posting Category** field, and then choose the **Navigate** action.</span></span>  
5. <span data-ttu-id="7c47c-127">На странице **Перейти** выберите строку операции ГК, затем выберите действие **Показать**.</span><span class="sxs-lookup"><span data-stu-id="7c47c-127">On the **Navigate** page, select the general ledger entry line, and then choose the **Show** action.</span></span>  

<span data-ttu-id="7c47c-128">Открывается страница **Операции главной книги**, на которой можно просмотреть операции, созданные в результате учета реализации.</span><span class="sxs-lookup"><span data-stu-id="7c47c-128">The **General Ledger Entries** page opens where you can see the entries that the disposal posting resulted in.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7c47c-129">См. также</span><span class="sxs-lookup"><span data-stu-id="7c47c-129">See Also</span></span>
[<span data-ttu-id="7c47c-130">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="7c47c-130">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="7c47c-131">Настройка основных средств</span><span class="sxs-lookup"><span data-stu-id="7c47c-131">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="7c47c-132">Финансы</span><span class="sxs-lookup"><span data-stu-id="7c47c-132">Finance</span></span>](finance.md)  
[<span data-ttu-id="7c47c-133">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="7c47c-133">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="7c47c-134">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7c47c-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

