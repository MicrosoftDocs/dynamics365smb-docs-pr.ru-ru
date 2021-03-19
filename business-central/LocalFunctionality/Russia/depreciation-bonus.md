---
title: Амортизационная премия в России
description: Российские улучшения включают амортизацию.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 6c43e68b63a39089bb9ce6ee3814e59d9251f6d3
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5382087"
---
# <a name="depreciation-bonus"></a><span data-ttu-id="37b90-103">Амортизационная премия</span><span class="sxs-lookup"><span data-stu-id="37b90-103">Depreciation Bonus</span></span>

<span data-ttu-id="37b90-104">Амортизационная премия представляет собой метод ускоренной амортизации, применяемый в налоговом учете в связи с положениями налогового законодательства России.</span><span class="sxs-lookup"><span data-stu-id="37b90-104">Depreciation bonus is an accelerated depreciation method applied in tax accounting because of provisions in the Russian tax laws.</span></span> <span data-ttu-id="37b90-105">Амортизационная премия позволяет включить затраты на основные средства и капиталовложения в текущий период по ставке, равной 10 или 30 процентам.</span><span class="sxs-lookup"><span data-stu-id="37b90-105">A depreciation bonus enables you to include fixed asset and capital investment expenses in the current period at the rate of 10 percent or 30 percent.</span></span>

## <a name="depreciation-bonus-calculation"></a><span data-ttu-id="37b90-106">Расчет амортизационной премии</span><span class="sxs-lookup"><span data-stu-id="37b90-106">Depreciation Bonus Calculation</span></span>

<span data-ttu-id="37b90-107">Амортизационная премия может рассчитываться и применяться для следующих типов транзакций:</span><span class="sxs-lookup"><span data-stu-id="37b90-107">A depreciation bonus can be calculated and applied for the following types of transactions:</span></span>

- <span data-ttu-id="37b90-108">Затраты на приобретение основных средств.</span><span class="sxs-lookup"><span data-stu-id="37b90-108">Acquisition costs of fixed assets.</span></span>
- <span data-ttu-id="37b90-109">Затраты на приобретение и повышение оценочной стоимости капиталовложений для всех предшествующих периодов, исключая текущий.</span><span class="sxs-lookup"><span data-stu-id="37b90-109">Acquisition costs and appreciation of capital investments for all previous periods excluding the current period.</span></span> 

<span data-ttu-id="37b90-110">Ставка амортизационной премии составляет 10 или 30 процентов в зависимости от класса основных средств.</span><span class="sxs-lookup"><span data-stu-id="37b90-110">The rate of the depreciation bonus is 10 percent or 30 percent, depending on the class of the fixed asset.</span></span> <span data-ttu-id="37b90-111">Ставка установлена для группы амортизации с помощью поля **Процент амортизационной премии** в окне **Группа амортизации**.</span><span class="sxs-lookup"><span data-stu-id="37b90-111">The rate is set for a depreciation group using the **Depr. Bonus Percentage** field in the **Depreciation Group** window.</span></span> 

<span data-ttu-id="37b90-112">После того как амортизационная премия рассчитана и учтена для периода, все транзакции очищаются для подготовки к следующему периоду.</span><span class="sxs-lookup"><span data-stu-id="37b90-112">After the depreciation bonus is calculated and posted for a period, all transactions are cleared in preparation for the next period.</span></span>

## <a name="depreciation-bonus-settings"></a><span data-ttu-id="37b90-113">Параметры амортизационной премии</span><span class="sxs-lookup"><span data-stu-id="37b90-113">Depreciation Bonus Settings</span></span>

<span data-ttu-id="37b90-114">Перед расчетом амортизационной премии необходимо убедиться в том, были применены соответствующие параметры в окне **Настройка налоговых регистров**.</span><span class="sxs-lookup"><span data-stu-id="37b90-114">Before depreciation bonus is calculated, you will have to make sure that the appropriate settings have been applied in the **Tax Register Setup** window.</span></span> <span data-ttu-id="37b90-115">Используйте информацию в следующей таблице для применения параметров амортизационной премии.</span><span class="sxs-lookup"><span data-stu-id="37b90-115">Use the information in the following table to apply depreciation bonus settings.</span></span>

| <span data-ttu-id="37b90-116">Поле</span><span class="sxs-lookup"><span data-stu-id="37b90-116">Field</span></span>                              | <span data-ttu-id="37b90-117">Описание</span><span class="sxs-lookup"><span data-stu-id="37b90-117">Description</span></span>                                                  |
| :--------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="37b90-118">**Вкл. акт ввода в эксп. в расчет аморт. премии**</span><span class="sxs-lookup"><span data-stu-id="37b90-118">**Rel. Act as Depr. Bonus Base**</span></span>   | <span data-ttu-id="37b90-119">Выберите, требуется ли использовать прием-передачу ОС для расчета базы амортизационной премии.</span><span class="sxs-lookup"><span data-stu-id="37b90-119">Select if you want fixed asset releases to be used to calculate the depreciation bonus base.</span></span> |
| <span data-ttu-id="37b90-120">**Код нал. разн. по аморт. премии**</span><span class="sxs-lookup"><span data-stu-id="37b90-120">**Depr. Bonus TD Code**</span></span>            | <span data-ttu-id="37b90-121">Введите код налоговой разницы, который используется для вычисления амортизационной премии.</span><span class="sxs-lookup"><span data-stu-id="37b90-121">Enter a tax difference code that is used to calculate the depreciation bonus.</span></span> <span data-ttu-id="37b90-122">Выбранный код налоговой разницы должен быть задан как амортизационная премия во время настройки налоговой разницы.</span><span class="sxs-lookup"><span data-stu-id="37b90-122">The selected tax difference code should be identified as a depreciation bonus during tax difference setup.</span></span> |
| <span data-ttu-id="37b90-123">**Восстановление аморт. премии c**</span><span class="sxs-lookup"><span data-stu-id="37b90-123">**Depr. Bonus Recovery from**</span></span>      | <span data-ttu-id="37b90-124">Введите начальную дату восстановления амортизации в случае продажи ОС.</span><span class="sxs-lookup"><span data-stu-id="37b90-124">Enter the starting date from which depreciation is recovered if the fixed asset is sold.</span></span> <span data-ttu-id="37b90-125">Если основное средство продано до этой даты и уже была применена амортизационная премия, амортизационная премия не будет восстанавливаться.</span><span class="sxs-lookup"><span data-stu-id="37b90-125">If the fixed asset is sold before this date and the depreciation bonus has already been applied, the depreciation bonus will not be recovered.</span></span> |
| <span data-ttu-id="37b90-126">**Период восстановл. аморт. премии (лет)**</span><span class="sxs-lookup"><span data-stu-id="37b90-126">**Depr. Bonus Recov. Per. (Year)**</span></span> | <span data-ttu-id="37b90-127">Введите период, в который производится восстановления амортизационной премии в случае продажи ОС.</span><span class="sxs-lookup"><span data-stu-id="37b90-127">Enter the period in which the depreciation bonus is recovered if the fixed asset is sold.</span></span> |
| <span data-ttu-id="37b90-128">**Код нал.разн. для восстановл. аморт.премии**</span><span class="sxs-lookup"><span data-stu-id="37b90-128">**Depr. Bonus Recovery TD Code**</span></span>   | <span data-ttu-id="37b90-129">Ведите код налоговой разницы, который используется для вычисления суммы восстановления амортизационной премии в налоговом учете.</span><span class="sxs-lookup"><span data-stu-id="37b90-129">Enter the tax difference code that is used to calculate the depreciation bonus recovery amount in tax accounting.</span></span> |

## <a name="selecting-and-canceling-depreciation-bonus-transactions"></a><span data-ttu-id="37b90-130">Выбор и отмена транзакций амортизационной премии</span><span class="sxs-lookup"><span data-stu-id="37b90-130">Selecting and Canceling Depreciation Bonus Transactions</span></span> 

<span data-ttu-id="37b90-131">Транзакции амортизационной премии должны учитываться до расчета и учета суммы ежемесячной амортизации.</span><span class="sxs-lookup"><span data-stu-id="37b90-131">Depreciation bonus transactions should be posted before the monthly depreciation amount is calculated and posted.</span></span>

<span data-ttu-id="37b90-132">Для выбора транзакций амортизационной премии публикации для учета за период выберите **Аморт. премия** в окне **Журнал ОС** и окне **Журнал ГК основных средств**.</span><span class="sxs-lookup"><span data-stu-id="37b90-132">To select depreciation bonus transactions for posting for a period, select **Depr. Bonus** in the **Fixed Asset Journal** window and the **Fixed Asset G/L Journal** window.</span></span> 

<span data-ttu-id="37b90-133">Можно отменять транзакции амортизационной премии путем выполнения пакетного задания **Отменить операции книги ОС**.</span><span class="sxs-lookup"><span data-stu-id="37b90-133">You can cancel depreciation bonus transactions by running the **Cancel FA Ledger Entries** batch job.</span></span> <span data-ttu-id="37b90-134">После учета отмены амортизационной премии все операции, включенные в базу амортизационной премии, необходимо вручную выбрать как базу амортизационной премии.</span><span class="sxs-lookup"><span data-stu-id="37b90-134">After posting the depreciation bonus cancellation, all operations that are included in the depreciation bonus base must be manually selected as the depreciation bonus base.</span></span>

## <a name="see-also"></a><span data-ttu-id="37b90-135">См. также</span><span class="sxs-lookup"><span data-stu-id="37b90-135">See Also</span></span>

[<span data-ttu-id="37b90-136">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="37b90-136">Fixed Assets</span></span>](fixed-assets.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]