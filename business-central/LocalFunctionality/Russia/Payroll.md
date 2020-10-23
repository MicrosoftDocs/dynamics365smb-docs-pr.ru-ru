---
title: Зарплата в России
description: Российские усовершенствования включают поддержку начисления заработной платы.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 02f9e00f1b243c46338abadaf1786bb3b509d947
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3921296"
---
# <a name="payroll"></a><span data-ttu-id="961bb-103">Зарплата</span><span class="sxs-lookup"><span data-stu-id="961bb-103">Payroll</span></span>

<span data-ttu-id="961bb-104">Основной единицей начисления заработной платы является **элемент заработной платы**.</span><span class="sxs-lookup"><span data-stu-id="961bb-104">The basic unit of payroll is the **salary element**.</span></span> <span data-ttu-id="961bb-105">Каждый элемент заработной платы имеет индивидуальную настройку, которая обеспечивает расчет начисления/удержания в соответствии с заранее определенными правилами.</span><span class="sxs-lookup"><span data-stu-id="961bb-105">Each salary element has an individual setting that provides calculation of accrual/deduction/deduction according to pre-defined rules.</span></span> 

<span data-ttu-id="961bb-106">Типы зарплатных элементов:</span><span class="sxs-lookup"><span data-stu-id="961bb-106">Types of salary element:</span></span>

- <span data-ttu-id="961bb-107">Оклад</span><span class="sxs-lookup"><span data-stu-id="961bb-107">Wage</span></span>
- <span data-ttu-id="961bb-108">Премия</span><span class="sxs-lookup"><span data-stu-id="961bb-108">Bonus</span></span>
- <span data-ttu-id="961bb-109">НДФЛ</span><span class="sxs-lookup"><span data-stu-id="961bb-109">Income tax</span></span>
- <span data-ttu-id="961bb-110">Налоговый вычет</span><span class="sxs-lookup"><span data-stu-id="961bb-110">Tax deduction</span></span>
- <span data-ttu-id="961bb-111">Удержание</span><span class="sxs-lookup"><span data-stu-id="961bb-111">Deduction</span></span>
- <span data-ttu-id="961bb-112">Прочее</span><span class="sxs-lookup"><span data-stu-id="961bb-112">Other</span></span>
- <span data-ttu-id="961bb-113">Фонды</span><span class="sxs-lookup"><span data-stu-id="961bb-113">Funds</span></span>

<span data-ttu-id="961bb-114">Элементы зарплаты, которые похожи по назначению, объединяются в **типы расчета**.</span><span class="sxs-lookup"><span data-stu-id="961bb-114">Salary elements that are similar in purpose are combined into **calculation types**.</span></span> <span data-ttu-id="961bb-115">Каждый тип расчета имеет определенный приоритет, который определяет его последовательность в общей платежной ведомости.</span><span class="sxs-lookup"><span data-stu-id="961bb-115">Each type of calculation has a certain priority, which determines its sequence in the overall payroll.</span></span>

<span data-ttu-id="961bb-116">Другие виды расчета, которые должны быть сделаны при расчете окончательных или промежуточных выплат заработной платы, образуют **Расчетную группа заработной платы** (или же **Группу расчетов**).</span><span class="sxs-lookup"><span data-stu-id="961bb-116">Other types of calculation that must be made when calculating the final or interim payments of wages, forms a **Calculated payroll group** (or **the calculation Group**).</span></span> <span data-ttu-id="961bb-117">Группа расчетов задается в карточке сотрудника.</span><span class="sxs-lookup"><span data-stu-id="961bb-117">The calculation group is set in the employee card.</span></span>

<span data-ttu-id="961bb-118">Основные функции модуля расчета заработной платы:</span><span class="sxs-lookup"><span data-stu-id="961bb-118">Main functions of the payroll module:</span></span>

- <span data-ttu-id="961bb-119">Назначение окладов;</span><span class="sxs-lookup"><span data-stu-id="961bb-119">Appointment of wages;</span></span> 
- <span data-ttu-id="961bb-120">Осуществление компенсационных и стимулирующих выплат (премий);</span><span class="sxs-lookup"><span data-stu-id="961bb-120">Implementation of compensation and incentive payments (bonuses);</span></span> 
- <span data-ttu-id="961bb-121">Расчет среднего заработка;</span><span class="sxs-lookup"><span data-stu-id="961bb-121">Calculation of average earnings;</span></span>
- <span data-ttu-id="961bb-122">Предоставление основных типов удержаний, определенных действующим законодательством;</span><span class="sxs-lookup"><span data-stu-id="961bb-122">Provision of basic types of deduction defined by the current legislation;</span></span> 
- <span data-ttu-id="961bb-123">Предоставление налоговых вычетов в соответствии с действующим законодательством;</span><span class="sxs-lookup"><span data-stu-id="961bb-123">Provision of tax deductions according to the current legislation;</span></span> 
- <span data-ttu-id="961bb-124">Расчет налога на доходы физических лиц и отчислений в фонды в соответствии с действующим законодательством.</span><span class="sxs-lookup"><span data-stu-id="961bb-124">Calculation of personal income tax and payments to funds according to the current legislation.</span></span>

## <a name="payroll-accounting-groups"></a><span data-ttu-id="961bb-125">Учетные группы заработной платы</span><span class="sxs-lookup"><span data-stu-id="961bb-125">Payroll accounting groups</span></span>

<span data-ttu-id="961bb-126">Учетная группа заработной платы относится к категории специальных учетных групп.</span><span class="sxs-lookup"><span data-stu-id="961bb-126">Accounting payroll group belongs to the category of special accounting groups.</span></span>

<span data-ttu-id="961bb-127">Для каждой позиции платежной ведомости можно определить учетную группу заработной платы, включающую счета ГК, которые будут использоваться при генерации транзакций.</span><span class="sxs-lookup"><span data-stu-id="961bb-127">For each payroll item, a payroll accounting group can be defined, the setup  determines the Ledger accounts to be used when generating transactions.</span></span> <span data-ttu-id="961bb-128">Настраиваемая при этом учетная группа может быть переопределена типом расчета (чтобы можно было распределять расходы на заработную плату на разные счета ГК).</span><span class="sxs-lookup"><span data-stu-id="961bb-128">The posting group that is set up for the item can be overridden in the calculation type (to enable payroll expenses to be allocated to different Ledger accounts).</span></span> <span data-ttu-id="961bb-129">Учетная группа, указанная в типе расчета, имеет более высокий приоритет.</span><span class="sxs-lookup"><span data-stu-id="961bb-129">The accounting group specified in the calculation type has a higher priority.</span></span> <span data-ttu-id="961bb-130">По умолчанию все позиции заработной платы используют учетную группу, указанную на карточке сотрудника (поле "Учетная группа"), которая имеет самый низкий приоритет.</span><span class="sxs-lookup"><span data-stu-id="961bb-130">By default, all payroll items use the posting group specified on the employee card (the Posting group field), which has the lowest priority.</span></span>

## <a name="payroll"></a><span data-ttu-id="961bb-131">Зарплата</span><span class="sxs-lookup"><span data-stu-id="961bb-131">Payroll</span></span>

<span data-ttu-id="961bb-132">Расчет заработной платы осуществляется по специальному зарплатному документу, индивидуальному для каждого работника.</span><span class="sxs-lookup"><span data-stu-id="961bb-132">Payroll is performed by a special salary document, individual for each employee.</span></span>

[!INCLUDE[prodshort](../../includes/prodshort.md)] <span data-ttu-id="961bb-133">поддерживает два типа зарплатных документов:</span><span class="sxs-lookup"><span data-stu-id="961bb-133">supports two types of payroll documents:</span></span> 

- <span data-ttu-id="961bb-134">Выплата заработной платы между периодами;</span><span class="sxs-lookup"><span data-stu-id="961bb-134">Payment of salary in interperiod;</span></span> 
- <span data-ttu-id="961bb-135">Базовая заработная плата.</span><span class="sxs-lookup"><span data-stu-id="961bb-135">Basic payroll.</span></span> 

<span data-ttu-id="961bb-136">Первый тип документов используется для расчета выплат сотрудникам в течение месяца (аванс, отпуск, больничный, увольнение).</span><span class="sxs-lookup"><span data-stu-id="961bb-136">The first type of document is used to calculate employee payments during the month (prepayment, vacation, sick leave, dismissal).</span></span> <span data-ttu-id="961bb-137">При публикации документа расчета зарплаты этого типа никакие транзакции в Главной книге и в книге зарплаты не создаются.</span><span class="sxs-lookup"><span data-stu-id="961bb-137">When you post a payroll document of this type, no transactions are generated in the General Ledger and transactions in the payroll Ledger.</span></span> <span data-ttu-id="961bb-138">На основании документов этого типа могут быть сформированы платежные документы для оплаты физическому лицу.</span><span class="sxs-lookup"><span data-stu-id="961bb-138">On the basis of documents of this type can be formed payment documents for payment to an individual.</span></span> 

<span data-ttu-id="961bb-139">Второй тип документов — базовая зарплата — должен формироваться для каждого сотрудника в конце каждого месяца после учета всех приказов об отсутствии и утверждения табеля учета рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="961bb-139">The second type of document – the basic payroll – should be formed for each employee at the end of each month after taking into account all types of orders for the absence and approval of the timesheet.</span></span> <span data-ttu-id="961bb-140">При учете документа расчета зарплаты второго типа создаются транзакции в книге зарплаты, а также финансовые транзакции в Главной книге. Полученная задолженность по зарплате отражается на соответствующей карточке отдельного поставщика.</span><span class="sxs-lookup"><span data-stu-id="961bb-140">When you post a payroll document of the second type, transactions are generated in the payroll Ledger, as well as financial transactions in the Ledger; the resulting wage arrears are reflected on the corresponding card of the individual vendor.</span></span> <span data-ttu-id="961bb-141">На основании существующей задолженности могут формироваться платежные документы для каждого сотрудника.</span><span class="sxs-lookup"><span data-stu-id="961bb-141">On the basis of the existing debt can be formed for each individual employee payment documents.</span></span>

<span data-ttu-id="961bb-142">Организация и принцип расчета для документов обоих типов одинаковы:</span><span class="sxs-lookup"><span data-stu-id="961bb-142">The organization and principle of calculation of both types of documents is the same:</span></span>

1. <span data-ttu-id="961bb-143">Выберите **Персонал > Зарплата > Зарплатные документы**</span><span class="sxs-lookup"><span data-stu-id="961bb-143">Go to **Human Resources > Payrol > Payroll documents**</span></span>
2. <span data-ttu-id="961bb-144">Чтобы автоматически сгенерировать зарплатные документы, запустите функцию **Предложить документы**.</span><span class="sxs-lookup"><span data-stu-id="961bb-144">To automatically generate payroll documents, run the **Suggest documents** function.</span></span>
3. <span data-ttu-id="961bb-145">Заполните поля:</span><span class="sxs-lookup"><span data-stu-id="961bb-145">Fill in the fields:</span></span>

| <span data-ttu-id="961bb-146">Поле</span><span class="sxs-lookup"><span data-stu-id="961bb-146">Field</span></span>                  | <span data-ttu-id="961bb-147">Описание</span><span class="sxs-lookup"><span data-stu-id="961bb-147">Description</span></span>                                                  |
| ---------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="961bb-148">Расчетный период</span><span class="sxs-lookup"><span data-stu-id="961bb-148">Calculation Period</span></span>     | <span data-ttu-id="961bb-149">Укажите период, за который будет рассчитываться зарплата.</span><span class="sxs-lookup"><span data-stu-id="961bb-149">Specify the period for which the salary will be calculated.</span></span>  |
| <span data-ttu-id="961bb-150">Дата расчета</span><span class="sxs-lookup"><span data-stu-id="961bb-150">Calculation Date</span></span>       | <span data-ttu-id="961bb-151">Дата расчета устанавливается равной последнему дню месяца выбранного расчетного периода и соответствует дате учета зарплатного документа (дата расчета заработной платы сотрудника).</span><span class="sxs-lookup"><span data-stu-id="961bb-151">The calculation date is set equal to the last day of the month of the selected calculation period and corresponds to the date of accounting of the salary document (date of payroll employee).</span></span> |
| <span data-ttu-id="961bb-152">Код группы расчета</span><span class="sxs-lookup"><span data-stu-id="961bb-152">Calculation Group Code</span></span> | <span data-ttu-id="961bb-153">Не заполняйте поле для окончательного расчета в конце месяца.</span><span class="sxs-lookup"><span data-stu-id="961bb-153">Do not fill the field for the final payroll at the end of the month.</span></span> <span data-ttu-id="961bb-154">Группа расчета будет подставлена из карточки сотрудника.</span><span class="sxs-lookup"><span data-stu-id="961bb-154">Calculation group will be used from imployee card.</span></span> <span data-ttu-id="961bb-155">Для оплаты между периодами введите код нужной группы расчета.</span><span class="sxs-lookup"><span data-stu-id="961bb-155">To pay in the interperiod, enter the code of the desired calculation group.</span></span> |
| <span data-ttu-id="961bb-156">Создать новые документы</span><span class="sxs-lookup"><span data-stu-id="961bb-156">Create New Documents</span></span>   | <span data-ttu-id="961bb-157">Установите флажок, если вы хотите создать новые документы по зарплате в любом случае.</span><span class="sxs-lookup"><span data-stu-id="961bb-157">Select the check box if you want to create new payroll documents in any case.</span></span> <span data-ttu-id="961bb-158">Если поле не отмечено, система попытается использовать ранее созданные документы заработной платы для этого сотрудника (поля "Код сотрудника" и "Код периода" должны соответствовать параметрам текущего расчета)</span><span class="sxs-lookup"><span data-stu-id="961bb-158">If the field is not marked, the system will try to use previously created payroll documents for this employee (the employee Code and period Code fields must match the parameters of the current calculation)</span></span> |
| <span data-ttu-id="961bb-159">Показать сообщения</span><span class="sxs-lookup"><span data-stu-id="961bb-159">Show Messages</span></span>          | <span data-ttu-id="961bb-160">Установите флажок для отображения подробных сообщений об ошибках, возникающих во время расчета.</span><span class="sxs-lookup"><span data-stu-id="961bb-160">Select the check box to display detailed messages about errors that occur at the time of calculation.</span></span> <span data-ttu-id="961bb-161">Если поле не помечено, сообщения об ошибках не будут отображаться, а некорректные документы заработной платы не будут создаваться.</span><span class="sxs-lookup"><span data-stu-id="961bb-161">If the field is not marked, error messages will not be displayed, and incorrect payroll documents will not be generated</span></span> |

4. <span data-ttu-id="961bb-162">Чтобы создать зарплатные документы, нажмите ОК.</span><span class="sxs-lookup"><span data-stu-id="961bb-162">To generate salary documents, click OK.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="961bb-163">Если вы создали документы, но не нашли никаких новых документов в списке, попробуйте обновить страницу (Действия - Обновить).</span><span class="sxs-lookup"><span data-stu-id="961bb-163">If you have generated documents but have not found any new documents in the list, try to update the page (Actions – Update).</span></span>

5. <span data-ttu-id="961bb-164">Для формирования транзакций в Главной книге и возможности выплаты заработной платы между периодами, необходимо выполнить учет зарплатных документов.</span><span class="sxs-lookup"><span data-stu-id="961bb-164">For the formation of transactions in the Ledger and the possibility of payment of wages in the inter-period salary documents must be post.</span></span>

## <a name="see-also"></a><span data-ttu-id="961bb-165">См. также</span><span class="sxs-lookup"><span data-stu-id="961bb-165">See Also</span></span>

[<span data-ttu-id="961bb-166">Персонал</span><span class="sxs-lookup"><span data-stu-id="961bb-166">Human Resources</span></span>](Human-Resources.md)  
