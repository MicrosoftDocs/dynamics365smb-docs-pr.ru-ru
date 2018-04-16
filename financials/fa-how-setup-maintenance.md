---
title: "Настройка обслуживания ОС | Документы Майкрософт"
description: "Для управления сервисом и ремонтом основных средств необходимо определить общие сведения об обслуживании, коды видов работ и счет учета затрат."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: repair, service
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: 0eccdafe78c74de05269af9a8b4132e4bcc9be57
ms.contentlocale: ru-ru
ms.lasthandoff: 04/16/2018

---
# <a name="set-up-fixed-asset-maintenance"></a><span data-ttu-id="c8e4a-103">Настройка обслуживания основного средства</span><span class="sxs-lookup"><span data-stu-id="c8e4a-103">Set Up Fixed Asset Maintenance</span></span>
<span data-ttu-id="c8e4a-104">Для управления обслуживанием основных средств следует сначала настроить некоторые общие сведения об обслуживании, счета учета для затрат на обслуживание, а также коды обслуживания для различных типов работ, например планового обслуживания или ремонта.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-104">To manage fixed asset maintenance, you must first set up some general maintenance information, a posting account for maintenance costs, and maintenance codes for types of work, such as Routine Service or Repair.</span></span>

## <a name="to-set-up-general-maintenance-information"></a><span data-ttu-id="c8e4a-105">Настройка общей информации об обслуживании</span><span class="sxs-lookup"><span data-stu-id="c8e4a-105">To set up general maintenance information</span></span>
<span data-ttu-id="c8e4a-106">Если устанавливаются поля для обслуживания, то можно учитывать расходы на обслуживание из журнала основных средств.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-106">If you set up the fields for maintenance, you can post maintenance expenses from the fixed asset journal.</span></span>

1. <span data-ttu-id="c8e4a-107">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Основные средства**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="c8e4a-108">Выберите основное средство, для которого определяется страховое покрытие, затем выберите действие **Правка**.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-108">Select the fixed asset that you to define insurance coverage for, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="c8e4a-109">На экспресс-вкладке **Обслуживание** заполните необходимые поля.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-109">On the **Maintenance** FastTab, fill in the fields as necessary.</span></span> [!INCLUDE [tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-maintenance-codes"></a><span data-ttu-id="c8e4a-110">Настройка кодов обслуживания</span><span class="sxs-lookup"><span data-stu-id="c8e4a-110">To set up maintenance codes</span></span>
<span data-ttu-id="c8e4a-111">При учете затрат на обслуживание из финансового журнала заполняется поле **Код обслуживания**, чтобы зарегистрировать тип выполненного обслуживания, например плановое обслуживание или ремонт.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-111">When you post maintenance costs from a general journal, you fill in the **Maintenance Code** field to record what kind of maintenance has been performed, such as routine service or repair.</span></span>

1. <span data-ttu-id="c8e4a-112">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Обслуживание**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Maintenance**, and then choose the related link.</span></span>
2. <span data-ttu-id="c8e4a-113">В окне **Обслуживание** настройте коды для различных типов работ по техническому обслуживанию.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-113">In the **Maintenance** window, set up codes for different types of maintenance work.</span></span>

## <a name="to-set-up-maintenance-expense-accounts"></a><span data-ttu-id="c8e4a-114">Настройка счетов расходов на обслуживание</span><span class="sxs-lookup"><span data-stu-id="c8e4a-114">To set up maintenance expense accounts</span></span>
<span data-ttu-id="c8e4a-115">Чтобы учитывать затраты на обслуживание, следует сначала ввести номер счета в окне **ОС - учетные группы**.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-115">To post maintenance costs, you must first enter an account number in the **FA Posting Groups** window.</span></span>

1. <span data-ttu-id="c8e4a-116">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Учетные группы ОС**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA Posting Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="c8e4a-117">Заполните поле **Обслуживание - счет расходов** для каждой учетной группы.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-117">Fill in the **Maintenance Expense Account** field for each posting group.</span></span>

> [!NOTE]  
>   <span data-ttu-id="c8e4a-118">Чтобы задать распределение стоимости обслуживания между отделами или проектами, необходимо настроить ключи распределения.</span><span class="sxs-lookup"><span data-stu-id="c8e4a-118">To define that maintenance costs are allocated to departments or projects, set up an allocation keys.</span></span> <span data-ttu-id="c8e4a-119">Дополнительные сведения см. в разделе [Настройка общих параметров основных средств](fa-how-setup-general.md).</span><span class="sxs-lookup"><span data-stu-id="c8e4a-119">For more information, see [Set Up General Fixed Assets Features](fa-how-setup-general.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="c8e4a-120">См. также</span><span class="sxs-lookup"><span data-stu-id="c8e4a-120">See Also</span></span>
[<span data-ttu-id="c8e4a-121">Настройка основных средств</span><span class="sxs-lookup"><span data-stu-id="c8e4a-121">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="c8e4a-122">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="c8e4a-122">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="c8e4a-123">Финансы</span><span class="sxs-lookup"><span data-stu-id="c8e4a-123">Finance</span></span>](finance.md)  
<span data-ttu-id="c8e4a-124">[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="c8e4a-124">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
<span data-ttu-id="c8e4a-125">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c8e4a-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

