---
title: Зачет НДС в России
description: Российские усовершенствования включают поддержку НДС в заказах на покупку.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 9a2cd9d026fac810017db1ecadfbc9f50557b2b0
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738231"
---
# <a name="vat-settlement"></a><span data-ttu-id="1408f-103">Зачет НДС</span><span class="sxs-lookup"><span data-stu-id="1408f-103">VAT Settlement</span></span>

<span data-ttu-id="1408f-104">Возможен полный зачет НДС или части НДС.</span><span class="sxs-lookup"><span data-stu-id="1408f-104">It is possible to settlement full VAT or part of VAT.</span></span>

## <a name="setup"></a><span data-ttu-id="1408f-105">Настройка</span><span class="sxs-lookup"><span data-stu-id="1408f-105">Setup</span></span>

<span data-ttu-id="1408f-106">Вы должны настроить учетные группы НДС на странице **Настройка учета НДС**.</span><span class="sxs-lookup"><span data-stu-id="1408f-106">You must set up VAT posting groups in the **VAT posting setup** page.</span></span> <span data-ttu-id="1408f-107">Вы можете указать НДС бизнес-группу или НДС товарную группу.</span><span class="sxs-lookup"><span data-stu-id="1408f-107">You can specify a VAT Business posting group and VAT product posting group.</span></span>  

- <span data-ttu-id="1408f-108">Тип расчета НДС - Обычный НДС</span><span class="sxs-lookup"><span data-stu-id="1408f-108">Type of VAT calculation – normal VAT</span></span>
- <span data-ttu-id="1408f-109">Тип транз. НДС - Сумма и налог</span><span class="sxs-lookup"><span data-stu-id="1408f-109">Type of transit VAT – Amount and tax</span></span>
- <span data-ttu-id="1408f-110">Вы можете указать транзитный счет НДС</span><span class="sxs-lookup"><span data-stu-id="1408f-110">You can specify a VAT transit account</span></span>
- <span data-ttu-id="1408f-111">В поле "Вид нереализованного НДС" - процент</span><span class="sxs-lookup"><span data-stu-id="1408f-111">In the field "Type of unrealized VAT" - percentage</span></span>
- <span data-ttu-id="1408f-112">Укажите счет НДС</span><span class="sxs-lookup"><span data-stu-id="1408f-112">Specify the VAT Account</span></span>
- <span data-ttu-id="1408f-113">Установлено "Зачет НДС вручную"</span><span class="sxs-lookup"><span data-stu-id="1408f-113">Checked the "VAT manual" installed</span></span>
- <span data-ttu-id="1408f-114">Указаны шаблон зачета НДС и раздел зачета НДС</span><span class="sxs-lookup"><span data-stu-id="1408f-114">The VAT settlement template and VAT settlement batch is specified</span></span>  
- <span data-ttu-id="1408f-115">Указан счет нереализованного</span><span class="sxs-lookup"><span data-stu-id="1408f-115">Specified Account Unreal.</span></span> <span data-ttu-id="1408f-116">НДС</span><span class="sxs-lookup"><span data-stu-id="1408f-116">VAT</span></span>

## <a name="vat-settlement"></a><span data-ttu-id="1408f-117">Зачет НДС</span><span class="sxs-lookup"><span data-stu-id="1408f-117">VAT settlement</span></span>

<span data-ttu-id="1408f-118">Чтобы вручную зачесть НДС, необходимо использовать рабочий лист для зачета НДС.</span><span class="sxs-lookup"><span data-stu-id="1408f-118">For manual settlement of VAT it is necessary to use the VAT settlement worksheet.</span></span>   

<span data-ttu-id="1408f-119">Рабочая дата должна быть в текущем месяце, за в котором нужно зачесть НДС.</span><span class="sxs-lookup"><span data-stu-id="1408f-119">The working date must be set to the current month in which VAT is to be settlement.</span></span>  

> [!NOTE]
> <span data-ttu-id="1408f-120">Перед расчетом НДС необходимо проверить данные документа НДС.</span><span class="sxs-lookup"><span data-stu-id="1408f-120">Before calculating VAT, you must check the data of the VAT document.</span></span> <span data-ttu-id="1408f-121">Если вы видите, что данные пусты, вы должны заполнить поля и использовать функцию "Изменить счета-фактуры поставщика".</span><span class="sxs-lookup"><span data-stu-id="1408f-121">If you see that the data is empty, you must fill in the fields and use the -> Change Vendor VAT Invoices function.</span></span>
> <span data-ttu-id="1408f-122">Дополнительный способ изменить данные счета НДС — использовать эту функцию в книге поставщиков.</span><span class="sxs-lookup"><span data-stu-id="1408f-122">An additional way to change the VAT invoice data is to use this function in the vendor Ledger.</span></span>

<span data-ttu-id="1408f-123">Нажмите "Предложить документы" и получите список документов для зачета НДС.</span><span class="sxs-lookup"><span data-stu-id="1408f-123">Click "Suggest documents" and get a list of documents to settlement VAT.</span></span>  

<span data-ttu-id="1408f-124">Затем нажмите кнопку "Копировать строки в журнал", чтобы перенести выбранные строки в журнал зачета НДС.</span><span class="sxs-lookup"><span data-stu-id="1408f-124">Next, click on the "Copy lines to journal" button to transfer the lines (which are selected) to the VAT settlement journal.</span></span>  

<span data-ttu-id="1408f-125">После учета журнала в регистре НДС появляется сформированная транзакция.</span><span class="sxs-lookup"><span data-stu-id="1408f-125">After posting the journal – formed transaction in the VAT register.</span></span>

### <a name="vat-allocation"></a><span data-ttu-id="1408f-126">Распределение НДС</span><span class="sxs-lookup"><span data-stu-id="1408f-126">VAT allocation</span></span>

<span data-ttu-id="1408f-127">Можно учесть только часть суммы НДС и списать оставшуюся часть.</span><span class="sxs-lookup"><span data-stu-id="1408f-127">It is possible to consider only part of the amount of the VAT and write off the other part.</span></span>

1. <span data-ttu-id="1408f-128">Вы должны использовать функцию **Распределение НДС** в **Журнале зачета НДС**.</span><span class="sxs-lookup"><span data-stu-id="1408f-128">You must use the **VAT Allocation** function in the **VAT settlement Journal**.</span></span>

2. <span data-ttu-id="1408f-129">Заполните поля:</span><span class="sxs-lookup"><span data-stu-id="1408f-129">Fill the fields:</span></span>

- <span data-ttu-id="1408f-130">Тип НДС — вы можете выбрать распределение НДС, списание или издержки.</span><span class="sxs-lookup"><span data-stu-id="1408f-130">Type of VAT, you can select whether this allocation of VAT, write-off or charge.</span></span>
- <span data-ttu-id="1408f-131">Номер счета — счет для распределения НДС.</span><span class="sxs-lookup"><span data-stu-id="1408f-131">Account No. - account for VAT allocation.</span></span>
- <span data-ttu-id="1408f-132">Укажите процент или сумму распределения.</span><span class="sxs-lookup"><span data-stu-id="1408f-132">Specify the percentage or amount of the allocation.</span></span>

3. <span data-ttu-id="1408f-133">Нажмите ОК.</span><span class="sxs-lookup"><span data-stu-id="1408f-133">Click OK.</span></span> <span data-ttu-id="1408f-134">Учтите журнал.</span><span class="sxs-lookup"><span data-stu-id="1408f-134">Post the journal.</span></span>

## <a name="see-also"></a><span data-ttu-id="1408f-135">См. также</span><span class="sxs-lookup"><span data-stu-id="1408f-135">See Also</span></span>

[<span data-ttu-id="1408f-136">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="1408f-136">Russia Local Functionality</span></span>](russia-local-functionality.md)  
