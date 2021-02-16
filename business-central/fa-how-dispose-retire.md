---
title: Списание или выбытие ОС | Документация Майкрософт
description: Вы должны учитывать стоимость выбытия при продаже, списании или отбраковке основных средств.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: scrap
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 16d052c67a2d9b5513e9dac901dfeddce0527512
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4749422"
---
# <a name="dispose-of-or-retire-fixed-assets"></a><span data-ttu-id="5a005-103">Списание или выбытие основных средств</span><span class="sxs-lookup"><span data-stu-id="5a005-103">Dispose of or Retire Fixed Assets</span></span>

<span data-ttu-id="5a005-104">При продаже основного средства или его списании по другим причинам необходимо учесть сумму выбытия для расчета и регистрации прибыли или убытков.</span><span class="sxs-lookup"><span data-stu-id="5a005-104">When you sell or otherwise dispose of a fixed asset, the disposal value must be posted to calculate and record the gain or loss.</span></span> <span data-ttu-id="5a005-105">Операция выбытия должна быть последней операцией, учтенной для основного средства.</span><span class="sxs-lookup"><span data-stu-id="5a005-105">A disposal entry must be the last entry posted for a fixed asset.</span></span> <span data-ttu-id="5a005-106">Для частично списанного основного средства можно учесть более одной операции выбытия.</span><span class="sxs-lookup"><span data-stu-id="5a005-106">For partially disposed fixed assets, you can post more than one disposal entry.</span></span> <span data-ttu-id="5a005-107">Общая сумма всех учтенных сумм выбытия должна быть суммой по кредиту.</span><span class="sxs-lookup"><span data-stu-id="5a005-107">The total of all posted disposal amounts must be a credit amount.</span></span>  

> [!NOTE]  
> <span data-ttu-id="5a005-108">При бартере основных средств необходимо записать продажу старого актива (выбытие) и покупку нового актива (приобретение).</span><span class="sxs-lookup"><span data-stu-id="5a005-108">If you trade-in a fixed asset for another one, you must record both the sale of the old asset (disposal) and the purchase of the new one (acquisition).</span></span> <span data-ttu-id="5a005-109">Дополнительные сведения см. в разделе [Приобретение основных средств](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="5a005-109">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span></span>  

<span data-ttu-id="5a005-110">Следующие шаги предполагают, что вы уже настроили соответствующие учетные группы на странице **Учетные группы ОС**.</span><span class="sxs-lookup"><span data-stu-id="5a005-110">The following steps assume that you have already set up the relevant posting groups in the **FA Posting Groups** page.</span></span> <span data-ttu-id="5a005-111">Дополнительные сведения см. в разделе [Настройка учетных групп основных средств](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span><span class="sxs-lookup"><span data-stu-id="5a005-111">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span></span>  

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a><span data-ttu-id="5a005-112">Учет выбытия с использованием журнала ГК учета основных средств</span><span class="sxs-lookup"><span data-stu-id="5a005-112">To post a disposal from the fixed asset G/L journal</span></span>

1. <span data-ttu-id="5a005-113">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы ГК учета основных средств**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="5a005-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Asset G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="5a005-114">Создайте начальную строку журнала и заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="5a005-114">Create an initial journal line and fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="5a005-115">В поле **Тип учета ОС** выберите **Реализация**.</span><span class="sxs-lookup"><span data-stu-id="5a005-115">In the **FA Posting Type** field, select **Disposal**.</span></span>  
4. <span data-ttu-id="5a005-116">Выберите действие **Вставить баланс. счет ОС**.</span><span class="sxs-lookup"><span data-stu-id="5a005-116">Choose the **Insert FA Bal. Account** action.</span></span> <span data-ttu-id="5a005-117">Вторая строка журнала создается для балансирующего счета, который настроен для учета выбытия.</span><span class="sxs-lookup"><span data-stu-id="5a005-117">A second journal line is created for the balancing account that is set up for disposal posting.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="5a005-118">Шаг 4 работает только в том случае, если выполнены следующие настройки: на странице **Карточка учетной группы ОС** для учетной группы основного средства поле **Счет ГК реализации** содержит дебетовый счет главной книги, а поле **Баланс. счет реализации** содержит счет главной книги, на котором требуется учитывать балансовые операции для повышения стоимости.</span><span class="sxs-lookup"><span data-stu-id="5a005-118">Step 4 only works if you have set up the following: On the **FA Posting Group Card** page for the posting group of the fixed asset, the **Disposal Account** field contains the general ledger debit account and the **Disposal Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span></span> <span data-ttu-id="5a005-119">Дополнительные сведения см. в разделе [Настройка учетных групп основных средств](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span><span class="sxs-lookup"><span data-stu-id="5a005-119">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span></span>  
5. <span data-ttu-id="5a005-120">Выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="5a005-120">Choose the **Post** action.</span></span>  

<span data-ttu-id="5a005-121">В случае продажи или другого выбытия части основного средства, следует разделить средство до регистрации транзакции реализации.</span><span class="sxs-lookup"><span data-stu-id="5a005-121">If you sell or dispose of part of a fixed asset, you must split up the asset before you can record the disposal transaction.</span></span> <span data-ttu-id="5a005-122">Дополнительные сведения см. в разделе [Перемещение, разделение или объединение основных средств](fa-how-trans-split-combine.md).</span><span class="sxs-lookup"><span data-stu-id="5a005-122">For more information, see [Transfer, Split, or Combine Fixed Assets](fa-how-trans-split-combine.md).</span></span>  

## <a name="to-view-disposal-ledger-entries"></a><span data-ttu-id="5a005-123">Просмотр операций книги выбытия</span><span class="sxs-lookup"><span data-stu-id="5a005-123">To view disposal ledger entries</span></span>
<span data-ttu-id="5a005-124">При продаже или списании основного средства сумма списания учитывается в главной книге, в которой можно просмотреть результат.</span><span class="sxs-lookup"><span data-stu-id="5a005-124">When you sell or dispose of a fixed asset, the disposal value is posted to the general ledger where you can view the result.</span></span>  

1. <span data-ttu-id="5a005-125">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Основные средства**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="5a005-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="5a005-126">Выберите основное средство, для которого требуется просмотреть операции, затем выберите действие **Книги амортизации**.</span><span class="sxs-lookup"><span data-stu-id="5a005-126">Select the fixed asset that you want to view entries for, and then choose the **Depreciation Books** action.</span></span>  
3. <span data-ttu-id="5a005-127">Выберите книгу амортизации, для которой требуется просмотреть операции, затем выберите действие **Книга операций**.</span><span class="sxs-lookup"><span data-stu-id="5a005-127">Select the depreciation book that you want to view entries for, and then choose the **Ledger Entries** action.</span></span>  
4. <span data-ttu-id="5a005-128">Выберите строку со значением **Реализация** в поле **Категория учета ОС**, затем выберите действие **Найти записи**.</span><span class="sxs-lookup"><span data-stu-id="5a005-128">Select a line with **Disposal** in the **FA Posting Category** field, and then choose the **Find Entries** action.</span></span>  
5. <span data-ttu-id="5a005-129">На странице **Найти записи** выберите строку операции ГК, затем выберите действие **Показать связанные записи**.</span><span class="sxs-lookup"><span data-stu-id="5a005-129">On the **Find Entries** page, select the general ledger entry line, and then choose the **Show Related Entries** action.</span></span>  

<span data-ttu-id="5a005-130">Открывается страница **Операции главной книги**, на которой можно просмотреть операции, созданные в результате учета реализации.</span><span class="sxs-lookup"><span data-stu-id="5a005-130">The **General Ledger Entries** page opens where you can see the entries that the disposal posting resulted in.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5a005-131">См. также</span><span class="sxs-lookup"><span data-stu-id="5a005-131">See Also</span></span>

[<span data-ttu-id="5a005-132">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="5a005-132">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="5a005-133">Настройка основных средств</span><span class="sxs-lookup"><span data-stu-id="5a005-133">Setting Up Fixed Assets</span></span>](fa-setup.md)  
<span data-ttu-id="5a005-134">[Настройка учетных групп основных средств](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span><span class="sxs-lookup"><span data-stu-id="5a005-134">[To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span></span>  
[<span data-ttu-id="5a005-135">Финансы</span><span class="sxs-lookup"><span data-stu-id="5a005-135">Finance</span></span>](finance.md)  
[<span data-ttu-id="5a005-136">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="5a005-136">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="5a005-137">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5a005-137">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="5a005-138">Найти записи</span><span class="sxs-lookup"><span data-stu-id="5a005-138">Find Entries</span></span>](ui-find-entries.md)  
