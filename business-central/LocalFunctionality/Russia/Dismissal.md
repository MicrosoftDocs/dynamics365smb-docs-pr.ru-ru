---
title: Увольнение в России
description: Российские улучшения включают увольнение сотрудников.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: c1a9dc2d5cfde36279b1ba47390e5fcd2bfc5a41
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3921308"
---
# <a name="dismissal"></a><span data-ttu-id="dc669-103">Увольнение</span><span class="sxs-lookup"><span data-stu-id="dc669-103">Dismissal</span></span>

<span data-ttu-id="dc669-104">Для уволенного создается дополнительная строка трудового договора, где **Тип операции** — *Увольнение*.</span><span class="sxs-lookup"><span data-stu-id="dc669-104">For the dismissed is created additional line of the employment contract with **Operation type** *Dismissal*.</span></span> 

<span data-ttu-id="dc669-105">Оформление приказа об увольнении осуществляется в следующей последовательности.</span><span class="sxs-lookup"><span data-stu-id="dc669-105">Registration of the order on dismissal is carried out in the following sequence.</span></span> 

1. <span data-ttu-id="dc669-106">Для бессрочных трудовых договоров заполните поле **Дата окончания** в заголовке трудового договора.</span><span class="sxs-lookup"><span data-stu-id="dc669-106">For indefinite employment contracts, fill the **end date** field in the employment contract header.</span></span> <span data-ttu-id="dc669-107">Поле должно содержать дату увольнения сотрудника.</span><span class="sxs-lookup"><span data-stu-id="dc669-107">The field must contain the employee's dismissal date.</span></span>
2. <span data-ttu-id="dc669-108">Создайте новую строку и укажите *Увольнение* в поле **Тип операции**.</span><span class="sxs-lookup"><span data-stu-id="dc669-108">Create a new line and specify *Dismissal* in the **Operation Type** field.</span></span>
3. <span data-ttu-id="dc669-109">Заполните поля договора:</span><span class="sxs-lookup"><span data-stu-id="dc669-109">Fill the contract fields:</span></span>

| <span data-ttu-id="dc669-110">Поле</span><span class="sxs-lookup"><span data-stu-id="dc669-110">Field</span></span>              | <span data-ttu-id="dc669-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dc669-111">Description</span></span>                                                  |
| ------------------ | ------------------------------------------------------------ |
| <span data-ttu-id="dc669-112">Причина увольнения</span><span class="sxs-lookup"><span data-stu-id="dc669-112">Dismissal Reason</span></span>   | <span data-ttu-id="dc669-113">Код причины увольнения</span><span class="sxs-lookup"><span data-stu-id="dc669-113">Code of  Dismissal Reason</span></span>                                    |
| <span data-ttu-id="dc669-114">Документ увольнения</span><span class="sxs-lookup"><span data-stu-id="dc669-114">Dismissal Document</span></span> | <span data-ttu-id="dc669-115">В этом поле вы можете указать документ о причине увольнения, если это необходимо</span><span class="sxs-lookup"><span data-stu-id="dc669-115">In the field, you can enter a document of reason for dismissal, if necessary</span></span> |

<span data-ttu-id="dc669-116">Если работнику при увольнении полагаются компенсационные выплаты, они должны быть указаны в условиях договора.</span><span class="sxs-lookup"><span data-stu-id="dc669-116">If the employee at dismissal rely compensation payments, they should be specified in the terms of the contract.</span></span>

<span data-ttu-id="dc669-117">Код обязательной компенсационной выплаты также связан с причиной расторжения трудового договора.</span><span class="sxs-lookup"><span data-stu-id="dc669-117">The code of obligatory compensation payment is also linked to the reason of termination of the employment contract.</span></span>

4. <span data-ttu-id="dc669-118">Утвердите строку договора (Функция - **Утвердить строку**).</span><span class="sxs-lookup"><span data-stu-id="dc669-118">Approve the contract line (Function – **Approve line**).</span></span> 

5. <span data-ttu-id="dc669-119">Следующая последовательность действий будет выполнена во время утверждения строки трудового договора с типом "Увольнение".</span><span class="sxs-lookup"><span data-stu-id="dc669-119">The following sequence of actions will be performed during the approval of the employment contract line with the type dismissal.</span></span> 

- <span data-ttu-id="dc669-120">Трудовому договору будет присвоен статус "Закрыт".</span><span class="sxs-lookup"><span data-stu-id="dc669-120">The employment contract will be assigned the closed status.</span></span>
- <span data-ttu-id="dc669-121">Создает новую запись об увольнении в истории работника на предприятии.</span><span class="sxs-lookup"><span data-stu-id="dc669-121">Creates a new record of dismissal in the history of the employee at the enterprise.</span></span> 

6. <span data-ttu-id="dc669-122">Карточка сотрудника содержит информацию об увольнении (в поле **Статус** установлено значение *Уволен*, заполнены поля **Дата увольнения** и **Код причины увольнения**).</span><span class="sxs-lookup"><span data-stu-id="dc669-122">The employee card contains information about the dismissal (in the field **Status** set the value *Dismissed*, filled in the fields **date of dismissal** and **Code of the reason for dismissal**.</span></span>

## <a name="see-also"></a><span data-ttu-id="dc669-123">См. также</span><span class="sxs-lookup"><span data-stu-id="dc669-123">See Also</span></span>

[<span data-ttu-id="dc669-124">Персонал</span><span class="sxs-lookup"><span data-stu-id="dc669-124">Human Resources</span></span>](Human-Resources.md)
