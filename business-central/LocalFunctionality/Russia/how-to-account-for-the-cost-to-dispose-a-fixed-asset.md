---
title: Учет себестоимости реализации основного средства в России
description: Российские усовершенствования включают учет себестоимости реализации основных средств.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 2839cb903308bbc0d20672db511e6283de5a486a
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301172"
---
# <a name="how-to-account-for-the-cost-to-dispose-a-fixed-asset"></a><span data-ttu-id="1cf51-103">Практическое руководство. Учет себестоимости реализации основного средства</span><span class="sxs-lookup"><span data-stu-id="1cf51-103">How to: Account for the Cost to Dispose a Fixed Asset</span></span>

<span data-ttu-id="1cf51-104">Функция обслуживания при реализации позволяет отчитываться за сумму, потраченную на реализацию основного средства (ОС), как за расходы.</span><span class="sxs-lookup"><span data-stu-id="1cf51-104">The maintenance on disposal feature enables you to account for the amount spent to dispose a fixed asset (FA) as an expense.</span></span> <span data-ttu-id="1cf51-105">Можно учесть операции, которые относятся к затратам на реализацию основного средства, так чтобы эти операции были отражены в формах актов списания ОС.</span><span class="sxs-lookup"><span data-stu-id="1cf51-105">You can post operations related to spending for the disposal of a fixed asset so that they will be reflected in the FA Write-Off Act forms.</span></span> 

<span data-ttu-id="1cf51-106">Расходы на реализацию основного средства можно учесть из финансовых журналов, журналов ОС и документов покупки.</span><span class="sxs-lookup"><span data-stu-id="1cf51-106">The expenses of a fixed asset disposal can be posted from general ledger journals, fixed asset journals, and purchase documents.</span></span> <span data-ttu-id="1cf51-107">Ниже показано, как учесть расходы на реализацию основного средства с помощью финансового журнала основных средств.</span><span class="sxs-lookup"><span data-stu-id="1cf51-107">The following procedure shows how to post the expenses for a fixed asset disposal by using the Fixed Asset General Ledger Journal.</span></span> 

<span data-ttu-id="1cf51-108">Расходы на реализацию основного средства можно распечатать в отчете по акту списания ОС-4 и в отчете по акту списания ОС-4a.</span><span class="sxs-lookup"><span data-stu-id="1cf51-108">The expenses on a fixed asset disposal can be printed in the FA Write-off Act FA-4 report and the FA Writeoff Act FA-4a report.</span></span>

## <a name="to-set-up-a-maintenance-code"></a><span data-ttu-id="1cf51-109">Настройки кодов обслуживания</span><span class="sxs-lookup"><span data-stu-id="1cf51-109">To set up a maintenance code</span></span>

1. <span data-ttu-id="1cf51-110">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка ОС**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1cf51-110">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="1cf51-111">В окне **Настройка модуля ОС** на экспресс-вкладке **Общее** введите код обслуживания в поле **Код обслуживания при реализации**.</span><span class="sxs-lookup"><span data-stu-id="1cf51-111">In the **Fixed Asset Setup** window, on the **General** FastTab, enter a maintenance code in the **On Disposal Maintenance Code** field.</span></span>
3. <span data-ttu-id="1cf51-112">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="1cf51-112">Choose the **OK** button.</span></span>

## <a name="to-post-expenses-on-a-fixed-asset-disposal"></a><span data-ttu-id="1cf51-113">Учет расходов на реализацию основного средства</span><span class="sxs-lookup"><span data-stu-id="1cf51-113">To post expenses on a fixed asset disposal</span></span>

1. <span data-ttu-id="1cf51-114">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы ГК для ОС**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1cf51-114">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA G/L Journals**, and then choose the related link.</span></span>

2. <span data-ttu-id="1cf51-115">Заполните поля в окне **Журнал ГК основных средств**, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="1cf51-115">In the **Fixed Asset G/L Journal** window, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="1cf51-116">Поле</span><span class="sxs-lookup"><span data-stu-id="1cf51-116">Field</span></span>                | <span data-ttu-id="1cf51-117">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf51-117">Description</span></span>                                                  |
   | :------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="1cf51-118">**Тип счета**</span><span class="sxs-lookup"><span data-stu-id="1cf51-118">**Account Type**</span></span>     | <span data-ttu-id="1cf51-119">Выберите **Основное средство** в качестве типа счета.</span><span class="sxs-lookup"><span data-stu-id="1cf51-119">Select **Fixed Asset** as the account type.</span></span>                  |
   | <span data-ttu-id="1cf51-120">**Номер счета**</span><span class="sxs-lookup"><span data-stu-id="1cf51-120">**Account No.**</span></span>      | <span data-ttu-id="1cf51-121">Определяет номер основного средства, реализация которого потребовала расходов.</span><span class="sxs-lookup"><span data-stu-id="1cf51-121">Specifies the number of the fixed asset for disposal for which the expenses are made.</span></span> |
   | <span data-ttu-id="1cf51-122">**Тип учета ОС**</span><span class="sxs-lookup"><span data-stu-id="1cf51-122">**FA Posting Type**</span></span>  | <span data-ttu-id="1cf51-123">Выберите **Обслуживание** в качестве типа учета основного средства.</span><span class="sxs-lookup"><span data-stu-id="1cf51-123">Select **Maintenance** as the fixed asset posting type.</span></span>      |
   | <span data-ttu-id="1cf51-124">**Код обслуживания**</span><span class="sxs-lookup"><span data-stu-id="1cf51-124">**Maintenance Code**</span></span> | <span data-ttu-id="1cf51-125">Определяет код обслуживания, введенный в поле **Код обслуживания при реализации** в окне **Настройка модуля ОС**.</span><span class="sxs-lookup"><span data-stu-id="1cf51-125">Specifies the maintenance code that is entered in the **On Disposal Maintenance Code** field of the **Fixed Asset Setup** window.</span></span> |

3. <span data-ttu-id="1cf51-126">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="1cf51-126">Choose the **OK** button.</span></span>

## <a name="to-print-a-report-with-expenses-on-a-fixed-asset-disposal"></a><span data-ttu-id="1cf51-127">Печать отчета с расходами на реализацию основного средства</span><span class="sxs-lookup"><span data-stu-id="1cf51-127">To print a report with expenses on a fixed asset disposal</span></span>

1. <span data-ttu-id="1cf51-128">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Акт списания ОС**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1cf51-128">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Writeoff Act**, and then choose the related link.</span></span>

2. <span data-ttu-id="1cf51-129">В окне **Акт списания ОС** введите расходы, учтенные для данного основного средства.</span><span class="sxs-lookup"><span data-stu-id="1cf51-129">In the **FA Writeoff Act** window, enter the expenses that are posted for the fixed asset.</span></span>

3. <span data-ttu-id="1cf51-130">Нажмите кнопку **Печать**, чтобы распечатать отчет, или кнопку **Просмотр**, чтобы отобразить его на экране.</span><span class="sxs-lookup"><span data-stu-id="1cf51-130">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span></span> <span data-ttu-id="1cf51-131">Нажмите кнопку **Отмена** для сохранения информации без печати отчета.</span><span class="sxs-lookup"><span data-stu-id="1cf51-131">Choose the **Cancel** button to save the information without printing the report.</span></span>

    > [!NOTE]
    > <span data-ttu-id="1cf51-132">Если расходы на реализацию основного средства производятся авансом, они будут показаны на второй странице отчета.</span><span class="sxs-lookup"><span data-stu-id="1cf51-132">If the expenses on the disposal of the fixed asset are made in advance, they are displayed on the second page of the report.</span></span>

<span data-ttu-id="1cf51-133">После того как отчет о реализации основного средства учтен, он становится учтенным отчетом о списании основного средства.</span><span class="sxs-lookup"><span data-stu-id="1cf51-133">After the fixed asset write-off report is posted, it becomes the posted fixed asset write-off report.</span></span>

## <a name="see-also"></a><span data-ttu-id="1cf51-134">См. также</span><span class="sxs-lookup"><span data-stu-id="1cf51-134">See Also</span></span>

[<span data-ttu-id="1cf51-135">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="1cf51-135">Fixed Assets</span></span>](../../fa-manage.md)  
