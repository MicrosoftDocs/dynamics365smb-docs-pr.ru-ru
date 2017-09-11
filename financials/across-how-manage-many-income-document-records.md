---
title: "Определение входящих документов, которые должны быть видны| Документы Майкрософт"
description: "Корректируйте представление по умолчанию для входящих документов, например для электронных счетов, чтобы иметь лучшее представление обработанных и необработанных записей."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2016
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: d840981dcceb54c74ac70ed0ddd05b3d3fa9bfc8
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-manage-many-incoming-document-records"></a><span data-ttu-id="b139e-103">Практическое руководство. Управление большим количеством записей входящих документов</span><span class="sxs-lookup"><span data-stu-id="b139e-103">How to: Manage Many Incoming Document Records</span></span>
<span data-ttu-id="b139e-104">По мере создания или обработки записей входящих документов количество строк в окне **Входящие документы** может увеличиться настолько, что вам сложно будет иметь общее представление об этих документах.</span><span class="sxs-lookup"><span data-stu-id="b139e-104">As you create or process incoming document records, the number of lines in the **Incoming Documents** window may grow to an extent where you lose overview.</span></span> <span data-ttu-id="b139e-105">Поэтому вы можете установить для записей входящих документов статус "Обработано", чтобы они не отображались в представлении по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b139e-105">Therefore, you can set incoming document records to Processed to remove them from the default view.</span></span> <span data-ttu-id="b139e-106">При выборе действий **Показать все** вы можете просматривать как обработанные, так и необработанные записи.</span><span class="sxs-lookup"><span data-stu-id="b139e-106">When you choose the **Show All** action, you can view both processed and unprocessed records.</span></span>

> [!NOTE]  
>   <span data-ttu-id="b139e-107">Изменить информацию, добавить файлы или выполнить другие действия над записями входящих документов, имеющих статус "Обработано" невозможно.</span><span class="sxs-lookup"><span data-stu-id="b139e-107">You cannot edit information, attach files, or perform other processes on incoming document records that are set to Processed.</span></span> <span data-ttu-id="b139e-108">Для этого сначала следует установить его на "Не обработано".</span><span class="sxs-lookup"><span data-stu-id="b139e-108">You must first set it to Unprocessed.</span></span>

<span data-ttu-id="b139e-109">Флажок **Обработано** автоматически устанавливается для записей входящих документов, которые были обработаны, но вы можете также устанавливать и снимать его вручную.</span><span class="sxs-lookup"><span data-stu-id="b139e-109">The **Processed** check box is automatically selected on incoming document records that have been processed, but you can also select or deselect the check box manually.</span></span> <span data-ttu-id="b139e-110">В зависимости от ваших бизнес-процессов записи входящих документов могут обрабатываться при создании для них соответствующих документов или при прикреплении файла.</span><span class="sxs-lookup"><span data-stu-id="b139e-110">Depending on your business process, an incoming document record may be processed when a related document has been created for it or a file has been attached.</span></span>

> [!NOTE]  
>   <span data-ttu-id="b139e-111">При открытии окна **Входящие документы** с помощью действия **Мои входящие документы** в ролевом центре по умолчанию отображаются только необработанные записи входящих документов.</span><span class="sxs-lookup"><span data-stu-id="b139e-111">When you open the **Incoming Documents** window with the **My Incoming Documents** action on the Role Center, only unprocessed incoming document records are shown by default.</span></span> <span data-ttu-id="b139e-112">Такое представление в этом разделе называется "представлением по умолчанию".</span><span class="sxs-lookup"><span data-stu-id="b139e-112">This is referred to in this topic as "the default view".</span></span>

## <a name="to-remove-incoming-document-records-from-the-default-view"></a><span data-ttu-id="b139e-113">Удаление записей входящих документов из представления по умолчанию</span><span class="sxs-lookup"><span data-stu-id="b139e-113">To remove incoming document records from the default view</span></span>
1. <span data-ttu-id="b139e-114">В окне **Входящие документы** выберите одну или несколько строк записей входящих документов, которые требуется удалить из представления по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b139e-114">In the **Incoming Documents** window, select one or more lines for incoming document records that you want to remove from the default view.</span></span>
2. <span data-ttu-id="b139e-115">Выберите действие **Установить состояние "Обработано"**.</span><span class="sxs-lookup"><span data-stu-id="b139e-115">Choose the **Set to Processed** action.</span></span>

<span data-ttu-id="b139e-116">Записи входящих документов будут удалены из представления по умолчанию и для них будет установлен флажок **Обработано**.</span><span class="sxs-lookup"><span data-stu-id="b139e-116">The incoming document records are removed from the default view, and the **Processed** check box is selected on the lines.</span></span>

> [!NOTE]  
>   <span data-ttu-id="b139e-117">Это действие можно выполнить для отдельной записи в окне **Карточка входящего документа**.</span><span class="sxs-lookup"><span data-stu-id="b139e-117">You can also perform this action for the individual record in the **Incoming Document Card** window.</span></span>

## <a name="to-view-all-incoming-document-records"></a><span data-ttu-id="b139e-118">Просмотр всех записей входящих документов</span><span class="sxs-lookup"><span data-stu-id="b139e-118">To view all incoming document records</span></span>
1. <span data-ttu-id="b139e-119">В окне **Входящие документы** выберите действие **Показать все**.</span><span class="sxs-lookup"><span data-stu-id="b139e-119">In the **Incoming Documents** window, choose the **Show All** action.</span></span>

<span data-ttu-id="b139e-120">Будут показаны все записи входящих документов, включая те, для которых флажок **Обработано** не установлен.</span><span class="sxs-lookup"><span data-stu-id="b139e-120">All incoming document records are displayed, including those where the **Processed** check box is not selected.</span></span>

## <a name="to-add-incoming-document-records-to-the-default-view"></a><span data-ttu-id="b139e-121">Добавление записей входящих документов в представление по умолчанию</span><span class="sxs-lookup"><span data-stu-id="b139e-121">To add incoming document records to the default view</span></span>
1. <span data-ttu-id="b139e-122">В окне **Входящие документы** выберите действие **Показать все**.</span><span class="sxs-lookup"><span data-stu-id="b139e-122">In the **Incoming Documents** window, choose the **Show All** action.</span></span>
2. <span data-ttu-id="b139e-123">Выберите одну или несколько строк для записей входящих документов, которые должны отображаться в представлении по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b139e-123">Select one or more lines for incoming document records that you want to appear in the default view.</span></span>
3. <span data-ttu-id="b139e-124">Выберите действие **Установить состояние "Не обработано"**.</span><span class="sxs-lookup"><span data-stu-id="b139e-124">Choose the **Set to Unprocessed** action.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="b139e-125">Это действие можно выполнить для отдельной записи в окне **Карточка входящего документа**.</span><span class="sxs-lookup"><span data-stu-id="b139e-125">You can also perform this action for the individual record in the **Incoming Document Card** window.</span></span>

## <a name="see-also"></a><span data-ttu-id="b139e-126">См. также</span><span class="sxs-lookup"><span data-stu-id="b139e-126">See Also</span></span>
[<span data-ttu-id="b139e-127">Обработка входящих документов</span><span class="sxs-lookup"><span data-stu-id="b139e-127">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="b139e-128">Входящие документы</span><span class="sxs-lookup"><span data-stu-id="b139e-128">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="b139e-129">Покупки</span><span class="sxs-lookup"><span data-stu-id="b139e-129">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="b139e-130">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b139e-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
