---
title: Печать отчета "Кассовая книга КО-4" в России
description: Улучшения в России включают поддержку отчета "Кассовая книга КО-4"
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 6ab4cbfb5232fc0f3a99abea50207f0a4009a280
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5773226"
---
# <a name="print-the-cash-report-co-4-report"></a><span data-ttu-id="b7972-103">Печать отчета "Кассовая книга КО-4"</span><span class="sxs-lookup"><span data-stu-id="b7972-103">Print the Cash Report CO-4 Report</span></span>

<span data-ttu-id="b7972-104">Отчет **Кассовая книга КО-4** содержит унифицированную стандартную форму для кассиров с отчетом об одном дне работы счета кассы.</span><span class="sxs-lookup"><span data-stu-id="b7972-104">The **Cash Report CO-4** report shows the unified standard printing form for cashiers reporting for one operational day of the cash account.</span></span> <span data-ttu-id="b7972-105">Он обязателен и может печататься только для каждого дня.</span><span class="sxs-lookup"><span data-stu-id="b7972-105">It is required and can only be printed per day.</span></span> 

<span data-ttu-id="b7972-106">Этот отчет содержит открывающее сальдо всех учтенных приходных и расходных кассовых ордеров и закрывающее сальдо операционного дня для счета кассы.</span><span class="sxs-lookup"><span data-stu-id="b7972-106">This report shows the opening balance of all the posted ingoing and outgoing cash orders, and the closing balance of an operational day for one cash account.</span></span>  

## <a name="to-print-the-cash-report-co-4"></a><span data-ttu-id="b7972-107">Печать отчета "Кассовая книга КО-4"</span><span class="sxs-lookup"><span data-stu-id="b7972-107">To print the cash report CO-4</span></span>

1. <span data-ttu-id="b7972-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Кассовая книга КО-4**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b7972-108">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cash Report CO-4**, and then choose the related link.</span></span>

2. <span data-ttu-id="b7972-109">В окне **Кассовая книга КО-4** заполните поля.</span><span class="sxs-lookup"><span data-stu-id="b7972-109">In the **Cash Report CO-4** window, fill in the fields.</span></span>

   | <span data-ttu-id="b7972-110">Поле</span><span class="sxs-lookup"><span data-stu-id="b7972-110">Field</span></span>                 | <span data-ttu-id="b7972-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b7972-111">Description</span></span>                                                  |
   | :-------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="b7972-112">**Код кассы**</span><span class="sxs-lookup"><span data-stu-id="b7972-112">**Cash Account No.**</span></span>  | <span data-ttu-id="b7972-113">Выберите номер кассового счета.</span><span class="sxs-lookup"><span data-stu-id="b7972-113">Select a cash account number.</span></span>                                |
   | <span data-ttu-id="b7972-114">**Тип отчета**</span><span class="sxs-lookup"><span data-stu-id="b7972-114">**Report Type**</span></span>       | <span data-ttu-id="b7972-115">Выберите тип отчета.</span><span class="sxs-lookup"><span data-stu-id="b7972-115">Select the type of report to run.</span></span> <span data-ttu-id="b7972-116">Возможные типы: **Кассовая книга КО-4** и **Лист Кассовой Книги**.</span><span class="sxs-lookup"><span data-stu-id="b7972-116">Reports include **Cash Report CO-4** and **Cash Additional Sheet**.</span></span> |
   | <span data-ttu-id="b7972-117">**Дата**</span><span class="sxs-lookup"><span data-stu-id="b7972-117">**Date**</span></span>              | <span data-ttu-id="b7972-118">Введите дату, за которую необходимо сформировать отчет о кассовых операциях.</span><span class="sxs-lookup"><span data-stu-id="b7972-118">Enter the operational date of the cash account transactions to be reported.</span></span> |
   | <span data-ttu-id="b7972-119">**Кассир**</span><span class="sxs-lookup"><span data-stu-id="b7972-119">**Cashier**</span></span>           | <span data-ttu-id="b7972-120">Выберите сотрудника, которые является контактом для этого счета кассы.</span><span class="sxs-lookup"><span data-stu-id="b7972-120">Select the employee who is the contact for this cash account.</span></span> <span data-ttu-id="b7972-121">Этот сотрудник должен поставить свою подпись в конце отчета.</span><span class="sxs-lookup"><span data-stu-id="b7972-121">This employee must sign the end of the report.</span></span> |
   | <span data-ttu-id="b7972-122">**Печать титульного листа**</span><span class="sxs-lookup"><span data-stu-id="b7972-122">**Print Title Sheet**</span></span> | <span data-ttu-id="b7972-123">Выберите, чтобы напечатать титульный лист.</span><span class="sxs-lookup"><span data-stu-id="b7972-123">Select to print a title sheet.</span></span>                               |
   | <span data-ttu-id="b7972-124">**Печать последнего листа**</span><span class="sxs-lookup"><span data-stu-id="b7972-124">**Print Last Sheet**</span></span>  | <span data-ttu-id="b7972-125">Выберите, чтобы напечатать последний лист.</span><span class="sxs-lookup"><span data-stu-id="b7972-125">Select to print a last sheet.</span></span>                                |
   | <span data-ttu-id="b7972-126">**Предварительный просмотр**</span><span class="sxs-lookup"><span data-stu-id="b7972-126">**Preview**</span></span>           | <span data-ttu-id="b7972-127">Установите флажок для предварительного просмотра отчета.</span><span class="sxs-lookup"><span data-stu-id="b7972-127">Select the check box to see a preview of the report.</span></span>         |

3. <span data-ttu-id="b7972-128">Нажмите кнопку **Печать**, чтобы распечатать отчет, или кнопку **Просмотр**, чтобы отобразить его на экране.</span><span class="sxs-lookup"><span data-stu-id="b7972-128">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span></span> <span data-ttu-id="b7972-129">Нажмите кнопку **Отмена** для сохранения информации без печати отчета.</span><span class="sxs-lookup"><span data-stu-id="b7972-129">Choose the **Cancel** button to save the information without printing the report.</span></span>

## <a name="see-also"></a><span data-ttu-id="b7972-130">См. также</span><span class="sxs-lookup"><span data-stu-id="b7972-130">See Also</span></span>

[<span data-ttu-id="b7972-131">Настройка запасов</span><span class="sxs-lookup"><span data-stu-id="b7972-131">Setting Up Inventory</span></span>](../../inventory-setup-inventory.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]