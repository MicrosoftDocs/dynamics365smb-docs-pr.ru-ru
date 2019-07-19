---
title: Настройка юрисдикций нормы в России
description: Российские усовершенствования включают юрисдикции нормы.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: b8939d249425ca4e52445873a6830fe277dad782
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738204"
---
# <a name="how-to-set-up-norm-jurisdictions"></a><span data-ttu-id="72960-103">Практическое руководство. Настройка юрисдикций нормы</span><span class="sxs-lookup"><span data-stu-id="72960-103">How to: Set Up Norm Jurisdictions</span></span>

<span data-ttu-id="72960-104">Юрисдикции нормы основаны на российском налоговом законодательстве, в которое определены различные ставки налогов.</span><span class="sxs-lookup"><span data-stu-id="72960-104">Norm jurisdictions are based on Russian tax laws that define a variety of tax rates.</span></span> <span data-ttu-id="72960-105">Юрисдикции номы используются для расчета налогооблагаемых прибылей и убытков в налоговом учете.</span><span class="sxs-lookup"><span data-stu-id="72960-105">Norm jurisdictions are used to calculate taxable profits and losses in tax accounting.</span></span> <span data-ttu-id="72960-106">В окне **Юрисдикции нормы** вы можете настроить и определить юрисдикции нормы, которые будут использоваться при расчете налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="72960-106">You can use the **Norm Jurisdictions** window to set up and define norm jurisdictions that can be used when you calculate tax differences.</span></span>

## <a name="to-set-up-norm-jurisdictions"></a><span data-ttu-id="72960-107">Настройка юрисдикций нормы</span><span class="sxs-lookup"><span data-stu-id="72960-107">To set up norm jurisdictions</span></span>

1. <span data-ttu-id="72960-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Юрисдикции нормы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="72960-108">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Norm Jurisdictions**, and then choose the related link.</span></span>

2. <span data-ttu-id="72960-109">Введите **Код** и **Описание** юрисдикции нормы, которую необходимо настроить.</span><span class="sxs-lookup"><span data-stu-id="72960-109">Enter an identifying **Code** and **Description** for the norm jurisdiction that you want to set up.</span></span>

3. <span data-ttu-id="72960-110">Выберите действие **Группы**, чтобы открыть окно **Группы норм**.</span><span class="sxs-lookup"><span data-stu-id="72960-110">Choose the **Groups** action to open the **Norm Groups** window.</span></span>

4. <span data-ttu-id="72960-111">В окне **Группы норм** введите следующие сведения.</span><span class="sxs-lookup"><span data-stu-id="72960-111">In the **Norm Groups** window, enter the following information.</span></span>

   | <span data-ttu-id="72960-112">Поле</span><span class="sxs-lookup"><span data-stu-id="72960-112">Field</span></span>              | <span data-ttu-id="72960-113">Описание</span><span class="sxs-lookup"><span data-stu-id="72960-113">Description</span></span>                                                  |
   | :----------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="72960-114">**Код**</span><span class="sxs-lookup"><span data-stu-id="72960-114">**Code**</span></span>           | <span data-ttu-id="72960-115">Введите код для идентификации группы норм.</span><span class="sxs-lookup"><span data-stu-id="72960-115">Enter a code to identify the norm group.</span></span>                     |
   | <span data-ttu-id="72960-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="72960-116">**Description**</span></span>    | <span data-ttu-id="72960-117">Введите описание группы норм.</span><span class="sxs-lookup"><span data-stu-id="72960-117">Enter a description for the norm group.</span></span>                      |
   | <span data-ttu-id="72960-118">**Есть подробности**</span><span class="sxs-lookup"><span data-stu-id="72960-118">**Has Details**</span></span>    | <span data-ttu-id="72960-119">Указывает, определены ли особенности расчета для группы норм.</span><span class="sxs-lookup"><span data-stu-id="72960-119">Specifies if calculation details are defined for the norm group.</span></span> |
   | <span data-ttu-id="72960-120">**Метод поиска**</span><span class="sxs-lookup"><span data-stu-id="72960-120">**Search Detail**</span></span>  | <span data-ttu-id="72960-121">Выберите метод, который можно использовать для поиска юрисдикций норм.</span><span class="sxs-lookup"><span data-stu-id="72960-121">Select the method that you use for norm jurisdiction search.</span></span> <span data-ttu-id="72960-122">Возможные значения: **До даты** и **По состоянию на дату.**</span><span class="sxs-lookup"><span data-stu-id="72960-122">The options include **To Date** and **As of Date.**</span></span> |
   | <span data-ttu-id="72960-123">**Метод хранения**</span><span class="sxs-lookup"><span data-stu-id="72960-123">**Storing Method**</span></span> | <span data-ttu-id="72960-124">Выберите **Расчет**, если юрисдикция нормы рассчитывается по заданной формуле.</span><span class="sxs-lookup"><span data-stu-id="72960-124">Select **Calculation** if the norm jurisdiction is calculated with a specific formula.</span></span> <span data-ttu-id="72960-125">Оставьте поле пустым, если норма постоянна.</span><span class="sxs-lookup"><span data-stu-id="72960-125">Leave this field blank if the norm is a constant value.</span></span> |

5. <span data-ttu-id="72960-126">Выберите действие **Сведения**, чтобы открыть окно **Подробности нормы**.</span><span class="sxs-lookup"><span data-stu-id="72960-126">Choose the **Details** action to open the **Norm Details** window.</span></span> <span data-ttu-id="72960-127">В этом окне определите постоянную ставку налога для нормы.</span><span class="sxs-lookup"><span data-stu-id="72960-127">In this window, you will define a constant tax rate for the norm.</span></span>

6. <span data-ttu-id="72960-128">В окне **Подробности нормы** введите следующие сведения.</span><span class="sxs-lookup"><span data-stu-id="72960-128">In the **Norm Details** window, enter the following information.</span></span>

   | <span data-ttu-id="72960-129">Поле</span><span class="sxs-lookup"><span data-stu-id="72960-129">Field</span></span>              | <span data-ttu-id="72960-130">Описание</span><span class="sxs-lookup"><span data-stu-id="72960-130">Description</span></span>                                                  |
   | :----------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="72960-131">**Дата вступления в силу**</span><span class="sxs-lookup"><span data-stu-id="72960-131">**Effective Date**</span></span> | <span data-ttu-id="72960-132">Введите дату начала срока действия нормы.</span><span class="sxs-lookup"><span data-stu-id="72960-132">Enter an effective date for the norm.</span></span>                        |
   | <span data-ttu-id="72960-133">**Норма**</span><span class="sxs-lookup"><span data-stu-id="72960-133">**Norm**</span></span>           | <span data-ttu-id="72960-134">Введите значение нормы.</span><span class="sxs-lookup"><span data-stu-id="72960-134">Enter a value for the norm.</span></span> <span data-ttu-id="72960-135">Это значение используется для расчета налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="72960-135">This value is used to calculate tax differences.</span></span> |

7. <span data-ttu-id="72960-136">Нажмите кнопку **Закрыть**, чтобы закрыть окно **Подробности нормы** и сохранить введенные данные.</span><span class="sxs-lookup"><span data-stu-id="72960-136">Choose the **Close** button to close the **Norm Details** window and save your entries.</span></span>

<span data-ttu-id="72960-137">Настроенная юрисдикция нормы теперь доступна для расчета налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="72960-137">The norm jurisdiction that you set up is now available for use in calculating tax differences.</span></span>

## <a name="see-also"></a><span data-ttu-id="72960-138">См. также</span><span class="sxs-lookup"><span data-stu-id="72960-138">See Also</span></span>

[<span data-ttu-id="72960-139">Налоговые разницы</span><span class="sxs-lookup"><span data-stu-id="72960-139">Tax Differences</span></span>](Tax-Differences.md)  
[<span data-ttu-id="72960-140">Настройка расчета налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="72960-140">Setting up Tax Difference Calculation</span></span>](Setting-up-Tax-Difference-Calculation.md)  
[<span data-ttu-id="72960-141">Налоговый учет</span><span class="sxs-lookup"><span data-stu-id="72960-141">Tax Accounting</span></span>](Tax-Accounting.md)  
[<span data-ttu-id="72960-142">Налоговые регистры</span><span class="sxs-lookup"><span data-stu-id="72960-142">Tax Registers</span></span>](Tax-Registers.md)  
[<span data-ttu-id="72960-143">Практическое руководство. Создание налоговых регистров</span><span class="sxs-lookup"><span data-stu-id="72960-143">How to: Create Tax Registers</span></span>](How-to-Create-Tax-Registers.md)  
