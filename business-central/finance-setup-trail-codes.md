---
title: Настройка кодов для журналов аудита | Документация Майкрософт
description: Узнайте, что нужно сделать для настройки кодов источников и кодов причин, которые можно использовать при отслеживании журналов аудита.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accounting, auditing, bookkeeping
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: fc491b060d6a4b1039376b0051ef58da104ff1d1
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4750359"
---
# <a name="setting-up-source-codes-and-reason-codes-for-audit-trails"></a><span data-ttu-id="41759-103">Настройка кодов источников и кодов причин для журналов аудита</span><span class="sxs-lookup"><span data-stu-id="41759-103">Setting Up Source Codes and Reason Codes for Audit Trails</span></span>

<span data-ttu-id="41759-104">Всем учтенным операциям автоматически присваиваются коды источника, чтобы можно было выполнить трассировку транзакции до ее источника.</span><span class="sxs-lookup"><span data-stu-id="41759-104">All posted entries are automatically assigned a source code so that transactions can be traced to their origin.</span></span> <span data-ttu-id="41759-105">Если операциям необходимо назначить дополнительный код источника, можно использовать коды причин.</span><span class="sxs-lookup"><span data-stu-id="41759-105">If you want to give entries a supplementary source code, you can use reason codes.</span></span> <span data-ttu-id="41759-106">Коды причин используются для указания причины создания операции.</span><span class="sxs-lookup"><span data-stu-id="41759-106">Reason codes are used to indicate why an entry was created.</span></span> <span data-ttu-id="41759-107">Настроив коды причин, вы сможете присваивать их целым шаблонам журналов и разделам журналов, а также отдельным документам и строкам журналов.</span><span class="sxs-lookup"><span data-stu-id="41759-107">When you set up reason codes, you can assign them to entire journal templates and journal batches, and you can assign them to individual journal lines and documents.</span></span>  

<span data-ttu-id="41759-108">В качестве кодов источников и кодов причин рекомендуется использовать информативные, легкозапоминаемые коды.</span><span class="sxs-lookup"><span data-stu-id="41759-108">For both source codes and reason codes, use codes that are easy to remember and descriptive.</span></span> <span data-ttu-id="41759-109">Код должен быть уникальным, и вы можете создать любое количество кодов.</span><span class="sxs-lookup"><span data-stu-id="41759-109">The code must be unique, and you can set up as many codes as you like.</span></span>

## <a name="define-source-codes"></a><span data-ttu-id="41759-110">Определение кодов источника</span><span class="sxs-lookup"><span data-stu-id="41759-110">Define source codes</span></span>

<span data-ttu-id="41759-111">Иногда необходимо узнать, откуда возникла та или иная операция, например был ли причиной ее возникновения учет финансового журнала или учет счета покупки.</span><span class="sxs-lookup"><span data-stu-id="41759-111">Sometimes, you want see how a particular entry arose, such as whether it came from posting a general journal or a purchase invoice.</span></span> <span data-ttu-id="41759-112">Код источника указывает на место создания операции.</span><span class="sxs-lookup"><span data-stu-id="41759-112">A source code indicates where an entry was created.</span></span> <span data-ttu-id="41759-113">Операции создаются при учете журналов и счетов, а также при выполнении определенных пакетных заданий.</span><span class="sxs-lookup"><span data-stu-id="41759-113">Entries are created when journals and invoices are posted and when certain batch jobs are executed.</span></span> <span data-ttu-id="41759-114">Для каждого типа учета существует определенный код источника, который назначается при создании отдельных операций.</span><span class="sxs-lookup"><span data-stu-id="41759-114">Each posting type has a specific source code that is assigned when individual entries are created.</span></span>  

<span data-ttu-id="41759-115">При учете журналов, заказов, счетов или кредит-нот, а также при выполнении различных пакетных заданий создаются операции в финансовой отчетности.</span><span class="sxs-lookup"><span data-stu-id="41759-115">Posting journals, orders, invoices, or credit memos, and running various batch jobs, creates entries in the financial statements.</span></span> <span data-ttu-id="41759-116">Страница **Настройка кодов источников** содержит несколько экспресс-вкладок, по одной для каждой области приложения.</span><span class="sxs-lookup"><span data-stu-id="41759-116">The **Source Code Setup** page contains several FastTabs, one for each application area.</span></span> <span data-ttu-id="41759-117">На каждой экспресс-вкладке содержатся коды источника, применимые для данной области приложения.</span><span class="sxs-lookup"><span data-stu-id="41759-117">Each FastTab contains the source codes that are applicable for that application area.</span></span>

<span data-ttu-id="41759-118">При учете или выполнении пакетного задания соответствующий код источника автоматически прикрепляется к операции.</span><span class="sxs-lookup"><span data-stu-id="41759-118">When you post or run a batch job, the correct source code is automatically attached to the entry.</span></span> <span data-ttu-id="41759-119">Например, когда учет производится из финансового журнала, операция кодируется как *ФИНЖУР*.</span><span class="sxs-lookup"><span data-stu-id="41759-119">For example, when you post from the general journal, the entry is coded as *GENJNL*.</span></span> <span data-ttu-id="41759-120">В этом случае вы сможете отфильтровать страницу **Операции главной книги** для отображения операций, которые были учтены из финансового журнала или из документов продажи, например.</span><span class="sxs-lookup"><span data-stu-id="41759-120">You can then filter the **General Ledger Entries** page to show which entries were posted from the general journal or from sales documents, for example</span></span>

### <a name="to-define-source-codes"></a><span data-ttu-id="41759-121">Определение кодов источников</span><span class="sxs-lookup"><span data-stu-id="41759-121">To define source codes</span></span>

1. <span data-ttu-id="41759-122">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Настройка кодов источников**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="41759-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Source Code Setup**, and then choose the related link.</span></span>  

2. <span data-ttu-id="41759-123">В окне **Настройка кодов источников** для каждого типа учета и пакетного задания укажите соответствующий код источника.</span><span class="sxs-lookup"><span data-stu-id="41759-123">In the **Source Code Setup** window, for each each posting type and batch job, specify the relevant source code.</span></span>  

<span data-ttu-id="41759-124">Вы можете изменить содержимое поля позже, и это изменение будет влиять на учет в будущем.</span><span class="sxs-lookup"><span data-stu-id="41759-124">You can change the contents of a field later, and that change will then impact future postings.</span></span>

## <a name="change-source-codes"></a><span data-ttu-id="41759-125">Изменение кодов источников</span><span class="sxs-lookup"><span data-stu-id="41759-125">Change source codes</span></span>

<span data-ttu-id="41759-126">Может возникнуть необходимость изменить код источника.</span><span class="sxs-lookup"><span data-stu-id="41759-126">You may want to change a source code.</span></span> <span data-ttu-id="41759-127">Например, может потребоваться изменить код источника (например, с *ФИНЖУР* на *GNJ*).</span><span class="sxs-lookup"><span data-stu-id="41759-127">For example, you want to change the source code *GENJNL* to *GNJ*.</span></span>

### <a name="to-change-source-codes"></a><span data-ttu-id="41759-128">Изменение кодов источников</span><span class="sxs-lookup"><span data-stu-id="41759-128">To change source codes</span></span>

1. <span data-ttu-id="41759-129">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Коды источников**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="41759-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Source Codes**, and then choose the related link.</span></span>

2. <span data-ttu-id="41759-130">В строке с кодом, который необходимо изменить, выберите код в поле **Код**.</span><span class="sxs-lookup"><span data-stu-id="41759-130">On the line with the code to be changed, select the code in the **Code** field.</span></span>

3. <span data-ttu-id="41759-131">Введите новый код, а затем выберите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="41759-131">Enter the new code, and then choose the **Yes** button.</span></span> <span data-ttu-id="41759-132">Можно также изменить содержимое поля **Описание**.</span><span class="sxs-lookup"><span data-stu-id="41759-132">You can also change the contents of the **Description** field.</span></span>

<span data-ttu-id="41759-133">Все последующие операции, учтенные из финансового журнала, будут иметь новый код источника.</span><span class="sxs-lookup"><span data-stu-id="41759-133">All new entries that are posted from the general journal will have the new source code.</span></span>

## <a name="define-reason-codes"></a><span data-ttu-id="41759-134">Определение кодов причин</span><span class="sxs-lookup"><span data-stu-id="41759-134">Define reason codes</span></span>

<span data-ttu-id="41759-135">Коды причин дополняют коды источников и используются для указания причины создания операции.</span><span class="sxs-lookup"><span data-stu-id="41759-135">Reason codes supplement the source codes and are used to indicate why an entry was created.</span></span> <span data-ttu-id="41759-136">Коды причин можно назначать отдельным операциям, а также назначать постоянные коды для конкретным шаблонам журналов и разделам журналов.</span><span class="sxs-lookup"><span data-stu-id="41759-136">You can assign reason codes on individual entries, and you can assign permanent codes to specific journal templates and journal batches.</span></span> <span data-ttu-id="41759-137">Если со строкой журнала или с заголовком продажи или покупки связан код причины, при учете все операции будут снабжены этим кодом причины.</span><span class="sxs-lookup"><span data-stu-id="41759-137">When a reason code is linked to a journal line or a sales or purchase header, all entries are marked with the reason code when they are posted.</span></span>  

### <a name="to-set-up-reason-codes"></a><span data-ttu-id="41759-138">Настройка кодов причин</span><span class="sxs-lookup"><span data-stu-id="41759-138">To set up reason codes</span></span>

1. <span data-ttu-id="41759-139">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Коды причин**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="41759-139">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon")  icon, enter **Reason Codes**, and then choose the related link.</span></span>

2. <span data-ttu-id="41759-140">В окне **Коды причин** в поле **Код** введите первый код.</span><span class="sxs-lookup"><span data-stu-id="41759-140">In the **Reason Codes** window, enter the first code in the **Code** field.</span></span> <span data-ttu-id="41759-141">В поле **Описание** введите пояснение.</span><span class="sxs-lookup"><span data-stu-id="41759-141">In the **Description** field, enter an explanatory text.</span></span>

<span data-ttu-id="41759-142">Повторите процедуру для каждого кода, который намереваетесь использовать.</span><span class="sxs-lookup"><span data-stu-id="41759-142">Repeat the procedure for each code you want to use.</span></span> <span data-ttu-id="41759-143">Можно настроить любое количество кодов.</span><span class="sxs-lookup"><span data-stu-id="41759-143">You can set up any number of codes.</span></span>

<span data-ttu-id="41759-144">Следующая процедура описывает, как добавить код причины к шаблону журнала, однако аналогичные шаги можно использовать для добавления кода причины к строке журнала или разделу журнала.</span><span class="sxs-lookup"><span data-stu-id="41759-144">The following procedure describes how to add a reason code to a journal template, but similar steps apply to adding a reason code to a journal line or journal batch.</span></span>  

### <a name="to-assign-reason-codes-to-journal-templates"></a><span data-ttu-id="41759-145">Назначение кодов причин шаблонам журналов</span><span class="sxs-lookup"><span data-stu-id="41759-145">To assign reason codes to journal templates</span></span>

1. <span data-ttu-id="41759-146">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Шаблоны финансового журнала**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="41759-146">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon")  icon, enter **General Journal Templates**, and then choose the related link.</span></span>

2. <span data-ttu-id="41759-147">В строке с выбранным шаблоном журнала введите соответствующий код в поле **Код причины**.</span><span class="sxs-lookup"><span data-stu-id="41759-147">On the line with the selected journal template, in the **Reason Code** field, specify the relevant code.</span></span>

3. <span data-ttu-id="41759-148">Закройте шаблон журнала.</span><span class="sxs-lookup"><span data-stu-id="41759-148">Close the journal template.</span></span>

<span data-ttu-id="41759-149">Выбранный код причины будет копироваться в новые разделы журнала, создаваемые на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="41759-149">The selected reason code will be copied to new journal batches created under this journal template.</span></span> <span data-ttu-id="41759-150">Аналогичным образом можно назначать коды причин шаблонам журналов в других областях приложения.</span><span class="sxs-lookup"><span data-stu-id="41759-150">You assign reason codes to journal templates in the other application areas in the same way.</span></span>

### <a name="to-use-reason-codes-on-sales-and-purchase-documents"></a><span data-ttu-id="41759-151">Использование кодов причин в документах продажи и покупки</span><span class="sxs-lookup"><span data-stu-id="41759-151">To use reason codes on sales and purchase documents</span></span>

1. <span data-ttu-id="41759-152">Откройте соответствующий документ продажи или покупки.</span><span class="sxs-lookup"><span data-stu-id="41759-152">Open the relevant sales or purchase document.</span></span>

2. <span data-ttu-id="41759-153">В заголовке документа продажи или покупки введите код в поле **Код причины**.</span><span class="sxs-lookup"><span data-stu-id="41759-153">On the sales or purchase header, enter the code in the **Reason Code** field.</span></span>

<span data-ttu-id="41759-154">При учете счета код причины копируется в каждую операцию главной книги, клиента и поставщика.</span><span class="sxs-lookup"><span data-stu-id="41759-154">When the invoice is posted, the reason code is copied to each general ledger, customer, and vendor entry.</span></span> <span data-ttu-id="41759-155">Поскольку все строки учитываются как одна операция, задать различные коды причин для отдельных строк покупок и продаж нельзя.</span><span class="sxs-lookup"><span data-stu-id="41759-155">You cannot assign different reason codes to the individual purchase and sales lines because all lines are posted as one entry.</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="41759-156">См. соответствующее обучение на странице [Microsoft Learn](/learn/paths/set-up-financial-management-dynamics-365-business-central/)</span><span class="sxs-lookup"><span data-stu-id="41759-156">See Related Training at [Microsoft Learn](/learn/paths/set-up-financial-management-dynamics-365-business-central/)</span></span>

## <a name="see-also"></a><span data-ttu-id="41759-157">См. также</span><span class="sxs-lookup"><span data-stu-id="41759-157">See Also</span></span>

[<span data-ttu-id="41759-158">Финансы</span><span class="sxs-lookup"><span data-stu-id="41759-158">Finance</span></span>](finance.md)  
[<span data-ttu-id="41759-159">Выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="41759-159">Reconciling Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="41759-160">Работа с измерениями</span><span class="sxs-lookup"><span data-stu-id="41759-160">Working with Dimensions</span></span>](finance-dimensions.md)  
[<span data-ttu-id="41759-161">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="41759-161">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
[<span data-ttu-id="41759-162">Анализ движения денежных средств в организации</span><span class="sxs-lookup"><span data-stu-id="41759-162">Analyzing Cash Flow in Your Company</span></span>](finance-analyze-cash-flow.md)  
<span data-ttu-id="41759-163">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="41759-163">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  
