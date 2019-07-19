---
title: Настройка налогового учета в России
description: Российские улучшения включают налоговый учет.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: db63dbaf0dc6eb8217e727f8ad57a5829213795e
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738248"
---
# <a name="how-to-set-up-tax-accounting"></a><span data-ttu-id="32f06-103">Практическое руководство. Настройка налогового учета</span><span class="sxs-lookup"><span data-stu-id="32f06-103">How to: Set Up Tax Accounting</span></span>

<span data-ttu-id="32f06-104">Налоговый учет позволяет применять правила признания доходов и расходов в соответствии с местным законодательством.</span><span class="sxs-lookup"><span data-stu-id="32f06-104">Tax accounting lets you apply rules for recognizing income and expenses that follow your local tax laws.</span></span> <span data-ttu-id="32f06-105">Вы можете активировать функции налогового учета в [!INCLUDE[prodshort](../../includes/prodshort.md)], настроив налоговые регистры.</span><span class="sxs-lookup"><span data-stu-id="32f06-105">You can activate tax accounting features in [!INCLUDE[prodshort](../../includes/prodshort.md)] by setting up tax registers.</span></span>

## <a name="to-activate-tax-accounting"></a><span data-ttu-id="32f06-106">Активация налогового учета</span><span class="sxs-lookup"><span data-stu-id="32f06-106">To activate tax accounting</span></span>

1. <span data-ttu-id="32f06-107">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка налоговых регистров**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="32f06-107">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Tax Register Setup**, and then choose the related link.</span></span>

2. <span data-ttu-id="32f06-108">На экспресс-вкладке **Общее** выберите коды для следующих измерений.</span><span class="sxs-lookup"><span data-stu-id="32f06-108">On the **General** FastTab, select codes for the following dimensions.</span></span>

   | <span data-ttu-id="32f06-109">Поле</span><span class="sxs-lookup"><span data-stu-id="32f06-109">Field</span></span>                        | <span data-ttu-id="32f06-110">Описание</span><span class="sxs-lookup"><span data-stu-id="32f06-110">Description</span></span>                                                  |
   | :--------------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="32f06-111">**Условие - код измерения**</span><span class="sxs-lookup"><span data-stu-id="32f06-111">**Condition Dimension Code**</span></span> | <span data-ttu-id="32f06-112">Выберите код измерения, описывающий условие налогового регистра.</span><span class="sxs-lookup"><span data-stu-id="32f06-112">Select a dimension code that describes the condition of the tax register.</span></span> |
   | <span data-ttu-id="32f06-113">**Вид - код измерения**</span><span class="sxs-lookup"><span data-stu-id="32f06-113">**Kind Dimension Code**</span></span>      | <span data-ttu-id="32f06-114">Выберите код измерения, описывающий тип налогового регистра.</span><span class="sxs-lookup"><span data-stu-id="32f06-114">Select a dimension code that describes the type of tax register.</span></span> |

3. <span data-ttu-id="32f06-115">Выберите следующие поля, чтобы активировать операции в налоговом регистре.</span><span class="sxs-lookup"><span data-stu-id="32f06-115">Select the following fields to activate entries in the tax register.</span></span>

   | <span data-ttu-id="32f06-116">Поле</span><span class="sxs-lookup"><span data-stu-id="32f06-116">Field</span></span>                             | <span data-ttu-id="32f06-117">Описание</span><span class="sxs-lookup"><span data-stu-id="32f06-117">Description</span></span>                                            |
   | :-------------------------------- | :----------------------------------------------------- |
   | <span data-ttu-id="32f06-118">**Создавать приобр. ОС в НУ**</span><span class="sxs-lookup"><span data-stu-id="32f06-118">**Create Acquis. FA Tax Ledger**</span></span>  | <span data-ttu-id="32f06-119">Выберите, чтобы создать операции приобретения ОС.</span><span class="sxs-lookup"><span data-stu-id="32f06-119">Select to create fixed asset acquisition entries.</span></span>      |
   | <span data-ttu-id="32f06-120">**Создавать рекласс. ОС в НУ**</span><span class="sxs-lookup"><span data-stu-id="32f06-120">**Create Reclass. FA Tax Ledger**</span></span> | <span data-ttu-id="32f06-121">Выберите, чтобы создать операции реклассификации ОС.</span><span class="sxs-lookup"><span data-stu-id="32f06-121">Select to create fixed asset reclassification entries.</span></span> |
   | <span data-ttu-id="32f06-122">**Создавать РБП по приобр. в НУ**</span><span class="sxs-lookup"><span data-stu-id="32f06-122">**Create Acquis. FE Tax Ledger**</span></span>  | <span data-ttu-id="32f06-123">Выберите, чтобы создать операции приобретения с учетом в будущих периодах.</span><span class="sxs-lookup"><span data-stu-id="32f06-123">Select to create future expense acquisition entries.</span></span>   |

4. <span data-ttu-id="32f06-124">Выберите соответствующие книги амортизации в полях **Книга амортизации для налогового учета** и **Расх. буд. пер. - книга аморт.**.</span><span class="sxs-lookup"><span data-stu-id="32f06-124">Select the appropriate depreciation books in the **Tax Depreciation Book** and **Future Exp. Depreciation Book** fields.</span></span> <span data-ttu-id="32f06-125">Книги амортизации, которые вы выбрали, должны быть интегрированы с модулем финансов [!INCLUDE[prodshort](../../includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="32f06-125">The depreciation books that you select should not be integrated with the [!INCLUDE[prodshort](../../includes/prodshort.md)] finance module.</span></span>

5. <span data-ttu-id="32f06-126">Установите флажок **Создать данные для печати форм**, чтобы разрешить печать подробных данных налогового регистра в отчетах и формах.</span><span class="sxs-lookup"><span data-stu-id="32f06-126">Select the **Create Data for Printing Forms** check box to enable detailed tax register entry information to be printed on reports and forms.</span></span>

6. <span data-ttu-id="32f06-127">Нажмите кнопку **Закрыть**, чтобы закрыть окно и сохранить введенные данные.</span><span class="sxs-lookup"><span data-stu-id="32f06-127">Choose the **Close** button to close the window and save your entries.</span></span>

<span data-ttu-id="32f06-128">Дополнительные сведения о том, как настроить налоговые регистры, см. в разделе [Практическое руководство. Создание налоговых регистров](How-to-Create-Tax-Registers.md).</span><span class="sxs-lookup"><span data-stu-id="32f06-128">For more information about how to set up and customize tax registers, see [How to: Create Tax Registers](How-to-Create-Tax-Registers.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="32f06-129">См. также</span><span class="sxs-lookup"><span data-stu-id="32f06-129">See Also</span></span>

[<span data-ttu-id="32f06-130">Налоговый учет</span><span class="sxs-lookup"><span data-stu-id="32f06-130">Tax Accounting</span></span>](Tax-Accounting.md)  
[<span data-ttu-id="32f06-131">Налоговые регистры</span><span class="sxs-lookup"><span data-stu-id="32f06-131">Tax Registers</span></span>](Tax-Registers.md)  
[<span data-ttu-id="32f06-132">Практическое руководство. Создание налоговых регистров</span><span class="sxs-lookup"><span data-stu-id="32f06-132">How to: Create Tax Registers</span></span>](How-to-Create-Tax-Registers.md)  
[<span data-ttu-id="32f06-133">Налоговые разницы</span><span class="sxs-lookup"><span data-stu-id="32f06-133">Tax Differences</span></span>](Tax-Differences.md)  
