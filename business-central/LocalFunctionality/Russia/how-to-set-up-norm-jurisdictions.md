---
title: Настройка юрисдикций нормы в России
description: Российские усовершенствования включают юрисдикции нормы.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 8e96414ee6d1680b06c33ae4ab7f72e064464f3c
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5774227"
---
# <a name="set-up-norm-jurisdictions"></a><span data-ttu-id="ed027-103">Настройка юрисдикций нормы</span><span class="sxs-lookup"><span data-stu-id="ed027-103">Set Up Norm Jurisdictions</span></span>

<span data-ttu-id="ed027-104">Юрисдикции нормы основаны на российском налоговом законодательстве, в которое определены различные ставки налогов.</span><span class="sxs-lookup"><span data-stu-id="ed027-104">Norm jurisdictions are based on Russian tax laws that define a variety of tax rates.</span></span> <span data-ttu-id="ed027-105">Юрисдикции номы используются для расчета налогооблагаемых прибылей и убытков в налоговом учете.</span><span class="sxs-lookup"><span data-stu-id="ed027-105">Norm jurisdictions are used to calculate taxable profits and losses in tax accounting.</span></span> <span data-ttu-id="ed027-106">В окне **Юрисдикции нормы** вы можете настроить и определить юрисдикции нормы, которые будут использоваться при расчете налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="ed027-106">You can use the **Norm Jurisdictions** window to set up and define norm jurisdictions that can be used when you calculate tax differences.</span></span>

## <a name="to-set-up-norm-jurisdictions"></a><span data-ttu-id="ed027-107">Настройка юрисдикций нормы</span><span class="sxs-lookup"><span data-stu-id="ed027-107">To set up norm jurisdictions</span></span>

1. <span data-ttu-id="ed027-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Юрисдикции нормы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="ed027-108">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Norm Jurisdictions**, and then choose the related link.</span></span>

2. <span data-ttu-id="ed027-109">Введите **Код** и **Описание** юрисдикции нормы, которую необходимо настроить.</span><span class="sxs-lookup"><span data-stu-id="ed027-109">Enter an identifying **Code** and **Description** for the norm jurisdiction that you want to set up.</span></span>

3. <span data-ttu-id="ed027-110">Выберите действие **Группы**, чтобы открыть окно **Группы норм**.</span><span class="sxs-lookup"><span data-stu-id="ed027-110">Choose the **Groups** action to open the **Norm Groups** window.</span></span>

4. <span data-ttu-id="ed027-111">В окне **Группы норм** введите следующие сведения.</span><span class="sxs-lookup"><span data-stu-id="ed027-111">In the **Norm Groups** window, enter the following information.</span></span>

   | <span data-ttu-id="ed027-112">Поле</span><span class="sxs-lookup"><span data-stu-id="ed027-112">Field</span></span>              | <span data-ttu-id="ed027-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ed027-113">Description</span></span>                                                  |
   | :----------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="ed027-114">**Код**</span><span class="sxs-lookup"><span data-stu-id="ed027-114">**Code**</span></span>           | <span data-ttu-id="ed027-115">Введите код для идентификации группы норм.</span><span class="sxs-lookup"><span data-stu-id="ed027-115">Enter a code to identify the norm group.</span></span>                     |
   | <span data-ttu-id="ed027-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ed027-116">**Description**</span></span>    | <span data-ttu-id="ed027-117">Введите описание группы норм.</span><span class="sxs-lookup"><span data-stu-id="ed027-117">Enter a description for the norm group.</span></span>                      |
   | <span data-ttu-id="ed027-118">**Есть подробности**</span><span class="sxs-lookup"><span data-stu-id="ed027-118">**Has Details**</span></span>    | <span data-ttu-id="ed027-119">Указывает, определены ли особенности расчета для группы норм.</span><span class="sxs-lookup"><span data-stu-id="ed027-119">Specifies if calculation details are defined for the norm group.</span></span> |
   | <span data-ttu-id="ed027-120">**Метод поиска**</span><span class="sxs-lookup"><span data-stu-id="ed027-120">**Search Detail**</span></span>  | <span data-ttu-id="ed027-121">Выберите метод, который можно использовать для поиска юрисдикций норм.</span><span class="sxs-lookup"><span data-stu-id="ed027-121">Select the method that you use for norm jurisdiction search.</span></span> <span data-ttu-id="ed027-122">Возможные значения: **До даты** и **По состоянию на дату.**</span><span class="sxs-lookup"><span data-stu-id="ed027-122">The options include **To Date** and **As of Date.**</span></span> |
   | <span data-ttu-id="ed027-123">**Метод хранения**</span><span class="sxs-lookup"><span data-stu-id="ed027-123">**Storing Method**</span></span> | <span data-ttu-id="ed027-124">Выберите **Расчет**, если юрисдикция нормы рассчитывается по заданной формуле.</span><span class="sxs-lookup"><span data-stu-id="ed027-124">Select **Calculation** if the norm jurisdiction is calculated with a specific formula.</span></span> <span data-ttu-id="ed027-125">Оставьте поле пустым, если норма постоянна.</span><span class="sxs-lookup"><span data-stu-id="ed027-125">Leave this field blank if the norm is a constant value.</span></span> |

5. <span data-ttu-id="ed027-126">Выберите действие **Сведения**, чтобы открыть окно **Подробности нормы**.</span><span class="sxs-lookup"><span data-stu-id="ed027-126">Choose the **Details** action to open the **Norm Details** window.</span></span> <span data-ttu-id="ed027-127">В этом окне определите постоянную ставку налога для нормы.</span><span class="sxs-lookup"><span data-stu-id="ed027-127">In this window, you will define a constant tax rate for the norm.</span></span>

6. <span data-ttu-id="ed027-128">В окне **Подробности нормы** введите следующие сведения.</span><span class="sxs-lookup"><span data-stu-id="ed027-128">In the **Norm Details** window, enter the following information.</span></span>

   | <span data-ttu-id="ed027-129">Поле</span><span class="sxs-lookup"><span data-stu-id="ed027-129">Field</span></span>              | <span data-ttu-id="ed027-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ed027-130">Description</span></span>                                                  |
   | :----------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="ed027-131">**Дата вступления в силу**</span><span class="sxs-lookup"><span data-stu-id="ed027-131">**Effective Date**</span></span> | <span data-ttu-id="ed027-132">Введите дату начала срока действия нормы.</span><span class="sxs-lookup"><span data-stu-id="ed027-132">Enter an effective date for the norm.</span></span>                        |
   | <span data-ttu-id="ed027-133">**Норма**</span><span class="sxs-lookup"><span data-stu-id="ed027-133">**Norm**</span></span>           | <span data-ttu-id="ed027-134">Введите значение нормы.</span><span class="sxs-lookup"><span data-stu-id="ed027-134">Enter a value for the norm.</span></span> <span data-ttu-id="ed027-135">Это значение используется для расчета налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="ed027-135">This value is used to calculate tax differences.</span></span> |

7. <span data-ttu-id="ed027-136">Нажмите кнопку **Закрыть**, чтобы закрыть окно **Подробности нормы** и сохранить введенные данные.</span><span class="sxs-lookup"><span data-stu-id="ed027-136">Choose the **Close** button to close the **Norm Details** window and save your entries.</span></span>

<span data-ttu-id="ed027-137">Настроенная юрисдикция нормы теперь доступна для расчета налоговых разниц.</span><span class="sxs-lookup"><span data-stu-id="ed027-137">The norm jurisdiction that you set up is now available for use in calculating tax differences.</span></span>

## <a name="see-also"></a><span data-ttu-id="ed027-138">См. также</span><span class="sxs-lookup"><span data-stu-id="ed027-138">See Also</span></span>

[<span data-ttu-id="ed027-139">Налоговые разницы</span><span class="sxs-lookup"><span data-stu-id="ed027-139">Tax Differences</span></span>](Tax-Differences.md)  
[<span data-ttu-id="ed027-140">Настройка расчета налоговых разниц</span><span class="sxs-lookup"><span data-stu-id="ed027-140">Setting up Tax Difference Calculation</span></span>](Setting-up-Tax-Difference-Calculation.md)  
[<span data-ttu-id="ed027-141">Налоговый учет</span><span class="sxs-lookup"><span data-stu-id="ed027-141">Tax Accounting</span></span>](Tax-Accounting.md)  
[<span data-ttu-id="ed027-142">Налоговые регистры</span><span class="sxs-lookup"><span data-stu-id="ed027-142">Tax Registers</span></span>](Tax-Registers.md)  
[<span data-ttu-id="ed027-143">Расчет налоговых регистров</span><span class="sxs-lookup"><span data-stu-id="ed027-143">Create Tax Registers</span></span>](How-to-Create-Tax-Registers.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]