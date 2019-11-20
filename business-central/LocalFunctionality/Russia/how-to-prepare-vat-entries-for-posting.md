---
title: Подготовка операций НДС к учету в России
description: Российские улучшения включают возможность периодически предоставлять в налоговые органы данные о чистой сумме НДС покупок или продаж.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 111ea1015f3f85603a1a5b6aaa8d47b866ed0914
ms.sourcegitcommit: 319023e53627dbe8e68643908aacc6fd594a4957
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/04/2019
ms.locfileid: "2554509"
---
# <a name="prepare-vat-entries-for-posting"></a><span data-ttu-id="b0ae4-103">Подготовка операций НДС к учету</span><span class="sxs-lookup"><span data-stu-id="b0ae4-103">Prepare VAT Entries for Posting</span></span>

<span data-ttu-id="b0ae4-104">Необходимо периодически предоставлять в налоговые органы данные о чистой сумме НДС.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-104">You may want to periodically remit the net VAT from sales and purchase transactions to the tax authorities.</span></span> <span data-ttu-id="b0ae4-105">Можно использовать **Журнал НДС** для подготовки транзакций с открытыми суммами НДС к учету и для копирования операций в соответствующий журнал НДС.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-105">You can use the **VAT Settlement Worksheet** to prepare transactions with open VAT amounts for posting and copy the entries to the appropriate VAT settlement journal.</span></span> <span data-ttu-id="b0ae4-106">Обычно это нужно перед запуском пакетного задания **Вычисление и учет зачета НДС** для учета и закрытия операций НДС.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-106">This is typically done before you run the **Calc. and Post VAT Settlement** batch job to post and close VAT entries.</span></span>

## <a name="to-prepare-vat-entries-for-posting"></a><span data-ttu-id="b0ae4-107">Подготовка операций НДС к учету</span><span class="sxs-lookup"><span data-stu-id="b0ae4-107">To prepare VAT entries for posting</span></span>

1. <span data-ttu-id="b0ae4-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал НДС**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-108">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Settlement Worksheet**, and then choose the related link.</span></span>

2. <span data-ttu-id="b0ae4-109">Выберите фильтры, которые определяют связанные с НДС транзакции, которые требуется включить в зачет НДС.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-109">Select the filters that define the VAT related transactions that you want to include in the VAT settlement.</span></span>

   | <span data-ttu-id="b0ae4-110">Поле</span><span class="sxs-lookup"><span data-stu-id="b0ae4-110">Field</span></span>       | <span data-ttu-id="b0ae4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b0ae4-111">Description</span></span>                                                  |
   | :---------- | :----------------------------------------------------------- |
   | <span data-ttu-id="b0ae4-112">**Тип**</span><span class="sxs-lookup"><span data-stu-id="b0ae4-112">**Type**</span></span>    | <span data-ttu-id="b0ae4-113">Выберите типы транзакций, которые требуется включить в зачет НДС.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-113">Select the type of transactions that you want to include in the VAT settlement.</span></span> |
   | <span data-ttu-id="b0ae4-114">**Просмотр по**</span><span class="sxs-lookup"><span data-stu-id="b0ae4-114">**View by**</span></span> | <span data-ttu-id="b0ae4-115">Выберите период времени для зачета НДС.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-115">Select the time period for the VAT settlement.</span></span>               |
   | <span data-ttu-id="b0ae4-116">**Просмотр как**</span><span class="sxs-lookup"><span data-stu-id="b0ae4-116">**View as**</span></span> | <span data-ttu-id="b0ae4-117">Выберите способ просмотра чистой суммы НДС.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-117">Select how you want to view the net VAT.</span></span> <span data-ttu-id="b0ae4-118">Возможные варианты: **Оборот** и **Сальдо на дату**.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-118">The options include **Net Change** and **Balance at Date**.</span></span> |

3. <span data-ttu-id="b0ae4-119">Выберите **Предложить документы**.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-119">Choose **Suggest Documents**.</span></span> <span data-ttu-id="b0ae4-120">Будут показаны транзакции с открытыми операциями НДС, которые соответствуют выбранным фильтрам.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-120">Transactions with open VAT entries that match the filters that you selected will be displayed.</span></span>

4. <span data-ttu-id="b0ae4-121">Проверьте выбранные транзакции.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-121">Review the transactions that are included to ensure accuracy.</span></span> <span data-ttu-id="b0ae4-122">При необходимости скорректируйте фильтр.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-122">If necessary, adjust your filter selection.</span></span>

5. <span data-ttu-id="b0ae4-123">Выберите **Копировать строки в журнал**.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-123">Choose **Copy Lines to Journal**.</span></span>

<span data-ttu-id="b0ae4-124">Операции копируется в соответствующие журналы НДС.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-124">The entries are copied to the appropriate VAT settlement journals.</span></span> <span data-ttu-id="b0ae4-125">Теперь можно запустить пакетное задание **Вычисление и учет зачета НДС**, чтобы закрыть операции НДС.</span><span class="sxs-lookup"><span data-stu-id="b0ae4-125">You can now run the **Calc. and Post VAT Settlement** batch job to close the VAT entries.</span></span>

## <a name="see-also"></a><span data-ttu-id="b0ae4-126">См. также</span><span class="sxs-lookup"><span data-stu-id="b0ae4-126">See Also</span></span>

[<span data-ttu-id="b0ae4-127">Подача отчета об НДС в налоговые органы</span><span class="sxs-lookup"><span data-stu-id="b0ae4-127">Report VAT to Tax Authorities</span></span>](../../finance-how-report-vat.md)  
