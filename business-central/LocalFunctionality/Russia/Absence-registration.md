---
title: Регистрация отсутствия в России
description: Российские улучшения включают регистрацию отсутствия.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: cdd5e3efac3b8b95eaed9e56ae3cab4ee88b71e2
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738286"
---
# <a name="absence-registration"></a><span data-ttu-id="faae2-103">Регистрация отсутствия</span><span class="sxs-lookup"><span data-stu-id="faae2-103">Absence registration</span></span>

<span data-ttu-id="faae2-104">Все виды отсутствия, которые оплачиваются в соответствии с законодательством о среднем заработке, должны регистрироваться в соответствующих типах приказов.</span><span class="sxs-lookup"><span data-stu-id="faae2-104">All types of absence which are paid according to the legislation on average earnings shall be registered by the corresponding types of orders.</span></span> 

<span data-ttu-id="faae2-105">Есть четыре типа приказов в [!INCLUDE[prodshort](../../includes/prodshort.md)]:</span><span class="sxs-lookup"><span data-stu-id="faae2-105">There are four types of orders in [!INCLUDE[prodshort](../../includes/prodshort.md)]:</span></span>

- <span data-ttu-id="faae2-106">Отпуск;</span><span class="sxs-lookup"><span data-stu-id="faae2-106">Vacation;</span></span> 
- <span data-ttu-id="faae2-107">Командировка;</span><span class="sxs-lookup"><span data-stu-id="faae2-107">Travel;</span></span> 
- <span data-ttu-id="faae2-108">Больничный;</span><span class="sxs-lookup"><span data-stu-id="faae2-108">Sick leave;</span></span> 
- <span data-ttu-id="faae2-109">Другие типы отсутствия.</span><span class="sxs-lookup"><span data-stu-id="faae2-109">Other types of absence.</span></span> 

<span data-ttu-id="faae2-110">Все виды приказов оформляются аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="faae2-110">All types of orders are issued in a similar way.</span></span> 

1. <span data-ttu-id="faae2-111">Выберите **Подразделения > Управление персоналом > Приказы на отсутствия**</span><span class="sxs-lookup"><span data-stu-id="faae2-111">Go to **Departments > Human resources > Absence Orders**</span></span> 
2. <span data-ttu-id="faae2-112">Заполните заголовок приказа:</span><span class="sxs-lookup"><span data-stu-id="faae2-112">Fill the header of order:</span></span>

| <span data-ttu-id="faae2-113">Поле</span><span class="sxs-lookup"><span data-stu-id="faae2-113">Field</span></span>         | <span data-ttu-id="faae2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="faae2-114">Description</span></span>                                                  |
| ------------- | ------------------------------------------------------------ |
| <span data-ttu-id="faae2-115">Номер</span><span class="sxs-lookup"><span data-stu-id="faae2-115">No.</span></span>           | <span data-ttu-id="faae2-116">Определяет номер соответствующей записи или операции в соответствии с указанной серией номеров.</span><span class="sxs-lookup"><span data-stu-id="faae2-116">Specifies the number of the involved entry or record, according to the specified number series.</span></span> |
| <span data-ttu-id="faae2-117">Код сотрудника</span><span class="sxs-lookup"><span data-stu-id="faae2-117">Employee No.</span></span>  | <span data-ttu-id="faae2-118">Определяет номер сотрудника.</span><span class="sxs-lookup"><span data-stu-id="faae2-118">Specifies the number of the involved employee.</span></span>               |
| <span data-ttu-id="faae2-119">Дата Документа</span><span class="sxs-lookup"><span data-stu-id="faae2-119">Document Date</span></span> | <span data-ttu-id="faae2-120">Определяет дату создания связанного документа.</span><span class="sxs-lookup"><span data-stu-id="faae2-120">Specifies the date when the related document was created.</span></span>    |
| <span data-ttu-id="faae2-121">Дата учета</span><span class="sxs-lookup"><span data-stu-id="faae2-121">Posting Date</span></span>  | <span data-ttu-id="faae2-122">Определяет дату учета операции.</span><span class="sxs-lookup"><span data-stu-id="faae2-122">Specifies the entry's posting date.</span></span>                          |
| <span data-ttu-id="faae2-123">Номер кадрового приказа</span><span class="sxs-lookup"><span data-stu-id="faae2-123">HR Order No.</span></span>  | <span data-ttu-id="faae2-124">Номер приказа на отсутствие, который будет отображен в соответствующей печатной форме документа.</span><span class="sxs-lookup"><span data-stu-id="faae2-124">Number of the order for absence which will be displayed in the corresponding printed form of the document.</span></span> <span data-ttu-id="faae2-125">По умолчанию значение поля совпадает со значением поля "Номер",</span><span class="sxs-lookup"><span data-stu-id="faae2-125">By default, the value of the field is the same as the value of the No.</span></span> <span data-ttu-id="faae2-126">но его можно изменить вручную.</span><span class="sxs-lookup"><span data-stu-id="faae2-126">field, but can be changed manually</span></span> |
| <span data-ttu-id="faae2-127">Дата кадрового приказа</span><span class="sxs-lookup"><span data-stu-id="faae2-127">HR Order Date</span></span> | <span data-ttu-id="faae2-128">Дата приказа на отсутствие, которая будет отображена в печатной форме документа.</span><span class="sxs-lookup"><span data-stu-id="faae2-128">Date of the order for absence, which will be displayed in the printed form of the document.</span></span> <span data-ttu-id="faae2-129">По умолчанию значение поля совпадает с полем даты документа, но может быть изменено вручную</span><span class="sxs-lookup"><span data-stu-id="faae2-129">By default, the field value is the same as the document date field, but can be changed manually</span></span> |
| <span data-ttu-id="faae2-130">Код периода</span><span class="sxs-lookup"><span data-stu-id="faae2-130">Period Code</span></span>   | <span data-ttu-id="faae2-131">Код периода, в котором текущий документ должен быть включен в зарплатный документ.</span><span class="sxs-lookup"><span data-stu-id="faae2-131">The period code in which the current document must be included in the payroll document.</span></span> <span data-ttu-id="faae2-132">По умолчанию поле заполняется автоматически кодом периода, который соответствует дате учета</span><span class="sxs-lookup"><span data-stu-id="faae2-132">By default, the field is filled in automatically with a period code that corresponds to the posting date</span></span> |

3. <span data-ttu-id="faae2-133">Заполните строку:</span><span class="sxs-lookup"><span data-stu-id="faae2-133">Fill the line:</span></span>

| <span data-ttu-id="faae2-134">Поле</span><span class="sxs-lookup"><span data-stu-id="faae2-134">Field</span></span>              | <span data-ttu-id="faae2-135">Описание</span><span class="sxs-lookup"><span data-stu-id="faae2-135">Description</span></span>                                                  |
| ------------------ | ------------------------------------------------------------ |
| <span data-ttu-id="faae2-136">Код временной активности</span><span class="sxs-lookup"><span data-stu-id="faae2-136">Time Activity Code</span></span> | <span data-ttu-id="faae2-137">Код временной активности, соответствующий типу приказа</span><span class="sxs-lookup"><span data-stu-id="faae2-137">Temporary activity code corresponding to the type of order</span></span>   |
| <span data-ttu-id="faae2-138">Код элемента</span><span class="sxs-lookup"><span data-stu-id="faae2-138">Element Code</span></span>       | <span data-ttu-id="faae2-139">Определяет код связанного зарплатного элемента для целей налоговой регистрации.</span><span class="sxs-lookup"><span data-stu-id="faae2-139">Specifies the code of the related payroll element for tax registration purposes.</span></span> |
| <span data-ttu-id="faae2-140">Описание</span><span class="sxs-lookup"><span data-stu-id="faae2-140">Description</span></span>        | <span data-ttu-id="faae2-141">Определяет описание, связанное с этой строкой.</span><span class="sxs-lookup"><span data-stu-id="faae2-141">Specifies the description associated with this line.</span></span>         |
| <span data-ttu-id="faae2-142">Дата начала</span><span class="sxs-lookup"><span data-stu-id="faae2-142">Start Date</span></span>         | <span data-ttu-id="faae2-143">Определяет первый день действия.</span><span class="sxs-lookup"><span data-stu-id="faae2-143">Specifies the first day of the activity in question.</span></span>         |
| <span data-ttu-id="faae2-144">Дата окончания</span><span class="sxs-lookup"><span data-stu-id="faae2-144">End Date</span></span>           | <span data-ttu-id="faae2-145">Определяет последний день действия.</span><span class="sxs-lookup"><span data-stu-id="faae2-145">Specifies the last day of the activity in question.</span></span>          |

4. <span data-ttu-id="faae2-146">Для формирования транзакций в книгах документ должен быть учтен.</span><span class="sxs-lookup"><span data-stu-id="faae2-146">For the formation of transactions in the books document should be post.</span></span> 

<span data-ttu-id="faae2-147">Типы отсутствия, определенные рассматриваемым приказом, записываются в записях книги сотрудников.</span><span class="sxs-lookup"><span data-stu-id="faae2-147">Absence types defined by a considered order, recorded in the Employee Ledger Entries.</span></span> 

<span data-ttu-id="faae2-148">Рассмотренный приказ может быть отменен.</span><span class="sxs-lookup"><span data-stu-id="faae2-148">The considered order can be cancelled.</span></span> <span data-ttu-id="faae2-149">Функция доступна в виде карточки рассматриваемого приказа.</span><span class="sxs-lookup"><span data-stu-id="faae2-149">The function is available in the form of a card of the considered order.</span></span> <span data-ttu-id="faae2-150">Только приказы, по которым не рассчитывается заработная плата, могут быть отменены.</span><span class="sxs-lookup"><span data-stu-id="faae2-150">Only orders for which wages are not calculated may be cancelled.</span></span>

## <a name="see-also"></a><span data-ttu-id="faae2-151">См. также</span><span class="sxs-lookup"><span data-stu-id="faae2-151">See Also</span></span>

[<span data-ttu-id="faae2-152">Персонал</span><span class="sxs-lookup"><span data-stu-id="faae2-152">Human Resources</span></span>](Human-Resources.md)
