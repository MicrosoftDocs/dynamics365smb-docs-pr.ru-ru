---
title: Практическое руководство. Перенос операций ГК в операции затрат | Документы Майкрософт
description: Можно перенести операции главной книги в операции затрат.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: 273a8c4341f621710819fd5fbc5cb8ce579c86f5
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "805061"
---
# <a name="transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="f6e0a-103">Перенос операций ГК в операции затрат</span><span class="sxs-lookup"><span data-stu-id="f6e0a-103">Transfer General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="f6e0a-104">Можно перенести операции главной книги в операции затрат.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-104">You can transfer general ledger entries to cost entries.</span></span>  

<span data-ttu-id="f6e0a-105">Перед запуском процесса перемещения операций Главной книги в операции затрат необходимо подготовить перемещение, чтобы избежать ручного учета коррекции.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-105">Before you run the process for transferring general ledger entries to cost entries, you must prepare the transfer to avoid manual correction posting.</span></span>  

## <a name="to-prepare-the-transfer"></a><span data-ttu-id="f6e0a-106">Подготовка перемещения</span><span class="sxs-lookup"><span data-stu-id="f6e0a-106">To prepare the transfer</span></span>  

1.  <span data-ttu-id="f6e0a-107">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка учета затрат**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Accounting Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f6e0a-108">На странице **Настройка учета затрат** убедитесь, что в поле **Начальная дата для перемещения ГК** установлено нужное значение.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-108">On the **Cost Accounting Setup** page, verify that the **Starting Date for G/L Transfer** field is set to the correct value.</span></span>  
3.  <span data-ttu-id="f6e0a-109">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Диаграмма типов затрат**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Types**, and then choose the related link.</span></span>  
4.  <span data-ttu-id="f6e0a-110">На странице **Карта типов затрат** убедитесь, что поле **Диапазон счетов ГК** правильно связано с каждым типом затрат для получения операций из главной книги.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-110">On the **Cost Type Card** page, verify that the **G/L Account Range** field is linked correctly for each cost type to take entries from the general ledger.</span></span>  
5.  <span data-ttu-id="f6e0a-111">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **План счетов**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="f6e0a-112">Для каждого соответствующего счета главной книги на странице **Карточка счета ГК** убедитесь, что поле **Номер типа затрат**</span><span class="sxs-lookup"><span data-stu-id="f6e0a-112">For each relevant general ledger account, on the **G/L Account Card** page, verify that the **Cost Type No.**</span></span> <span data-ttu-id="f6e0a-113">правильно связано с типом затрат.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-113">field is linked correctly to a cost type.</span></span> <span data-ttu-id="f6e0a-114">Дополнительные сведения см. в разделе [Настройка учета затрат](finance-set-up-cost-accounting.md).</span><span class="sxs-lookup"><span data-stu-id="f6e0a-114">For more information, see [Setting Up Cost Accounting](finance-set-up-cost-accounting.md).</span></span>  
7.  <span data-ttu-id="f6e0a-115">Удостоверьтесь, что для всех соответствующих операций главной книги указаны значения измерений, соответствующие месту возникновения затрат или объекту затрат.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-115">Verify that all relevant general ledger entries have dimension values that correspond to a cost center and a cost object.</span></span>  

## <a name="to-transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="f6e0a-116">Перенос операций ГК в операции затрат</span><span class="sxs-lookup"><span data-stu-id="f6e0a-116">To transfer general ledger entries to cost entries</span></span>  
1.  <span data-ttu-id="f6e0a-117">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Перенести записи ГК в учет затрат**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer GL Entries to CA**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f6e0a-118">Нажмите кнопку **Да** для запуска перемещения.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-118">Choose the **Yes** button to start the transfer.</span></span> <span data-ttu-id="f6e0a-119">Процесс переносит все операции главной книги, которые еще не были переданы.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-119">The process transfers all general ledger entries that have not already been transferred.</span></span>  

    <span data-ttu-id="f6e0a-120">Во время перемещения процесс создает связи в записях таблиц **Операция затрат** и **Регистр затрат**.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-120">During the transfer, the process creates connections in the entries in the **Cost Entry** table and the **Cost Register** table.</span></span> <span data-ttu-id="f6e0a-121">Это позволяет отслеживать источник операций себестоимости.</span><span class="sxs-lookup"><span data-stu-id="f6e0a-121">This makes it possible to trace the source of cost entries.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f6e0a-122">См. также</span><span class="sxs-lookup"><span data-stu-id="f6e0a-122">See Also</span></span>  
<span data-ttu-id="f6e0a-123">[Перемещение и операции учета затрат](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="f6e0a-123">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
[<span data-ttu-id="f6e0a-124">Настройка учета затрат</span><span class="sxs-lookup"><span data-stu-id="f6e0a-124">Setting Up Cost Accounting</span></span>](finance-set-up-cost-accounting.md)   
