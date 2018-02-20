---
title: "Учет платежной квитанции по прямому дебету SEPA | Документы Майкрософт"
description: "При успешной обработке банком непосредственной операции сбора на дебетовом счете можно переходить к учету приемки оплаты для соответствующих счетов продажи."
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 0031017c96172dca76b50542e52c6a437c01427a
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="post-sepa-direct-debit-payment-receipts"></a><span data-ttu-id="3b93d-103">Учет платежной квитанции по прямому дебету SEPA</span><span class="sxs-lookup"><span data-stu-id="3b93d-103">Post SEPA Direct Debit Payment Receipts</span></span>
<span data-ttu-id="3b93d-104">При успешной обработке банком непосредственной операции сбора на дебетовом счете можно переходить к учету приемки оплаты для соответствующих счетов продажи.</span><span class="sxs-lookup"><span data-stu-id="3b93d-104">When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.</span></span> <span data-ttu-id="3b93d-105">Дополнительные сведения см. в разделе [Создание операций погашения прямого дебета SEPA и их экспорт в файл банка](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="3b93d-105">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  

<span data-ttu-id="3b93d-106">Учесть платежную квитанции можно непосредственно в окне **Коллекции прямого дебетования** или в окне **Операции коллекции прямого дебетования**.</span><span class="sxs-lookup"><span data-stu-id="3b93d-106">You can post the payment receipt directly from the **Direct Debit Collections** window or the **Direct Debit Collect. Entries** window.</span></span> <span data-ttu-id="3b93d-107">Кроме того, можно передать работу другому пользователю путем подготовки связанных строк журнала.</span><span class="sxs-lookup"><span data-stu-id="3b93d-107">Alternatively, you can relay the work to another user by preparing the related journal lines.</span></span>  

## <a name="to-post-a-direct-debit-payment-receipt-from-the-direct-debit-collections-window"></a><span data-ttu-id="3b93d-108">Учет платежной квитанции по прямому дебету в окне погашений прямого дебета</span><span class="sxs-lookup"><span data-stu-id="3b93d-108">To post a direct-debit payment receipt from the Direct Debit Collections window</span></span>  
1. <span data-ttu-id="3b93d-109">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Коллекции прямого дебетования**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3b93d-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Direct Debit Collections**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3b93d-110">Выберите строку для коллекции прямого дебета, экспортированную в файл банка и успешно обработанную банком.</span><span class="sxs-lookup"><span data-stu-id="3b93d-110">Select a line for a direct debit collection that has been exported to a bank file and successfully processed by the bank.</span></span> <span data-ttu-id="3b93d-111">Дополнительные сведения см. в разделе [Создание операций погашения прямого дебета SEPA и их экспорт в файл банка](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="3b93d-111">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  
3. <span data-ttu-id="3b93d-112">Выберите действие **Поступления после платежа**.</span><span class="sxs-lookup"><span data-stu-id="3b93d-112">Choose the **Post Payment Receipts** action.</span></span>  
4. <span data-ttu-id="3b93d-113">В окне **Учет коллекции прямого дебетования** заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="3b93d-113">In the **Post Direct Debit Collection** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="3b93d-114">Поле</span><span class="sxs-lookup"><span data-stu-id="3b93d-114">Field</span></span>|<span data-ttu-id="3b93d-115">Описанием</span><span class="sxs-lookup"><span data-stu-id="3b93d-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="3b93d-116">**Номер коллекции прямого дебетования**</span><span class="sxs-lookup"><span data-stu-id="3b93d-116">**Direct Debit Collection No.**</span></span>|<span data-ttu-id="3b93d-117">Укажите погашение прямого дебета, для которого необходимо учесть платежную квитанцию.</span><span class="sxs-lookup"><span data-stu-id="3b93d-117">Specify the direct debit collection that you want to post payment receipt for.</span></span>|  
    |<span data-ttu-id="3b93d-118">**Шаблон финансового журнала**</span><span class="sxs-lookup"><span data-stu-id="3b93d-118">**General Journal Template**</span></span>|<span data-ttu-id="3b93d-119">Укажите шаблон финансового журнала, который предполагается использовать для учета платежной квитанции, например шаблон для кассовых поступлений.</span><span class="sxs-lookup"><span data-stu-id="3b93d-119">Specify which general journal template to use for posting the payment receipt, such as the template for cash receipts.</span></span>|  
    |<span data-ttu-id="3b93d-120">**Название раздела финансового журнала**</span><span class="sxs-lookup"><span data-stu-id="3b93d-120">**General Journal Batch Name**</span></span>|<span data-ttu-id="3b93d-121">Укажите раздел финансового журнала, который предполагается использовать для учета платежной квитанции.</span><span class="sxs-lookup"><span data-stu-id="3b93d-121">Specify which general journal batch to use for posting the payment receipt.</span></span>|  
    |<span data-ttu-id="3b93d-122">**Создать только журнал**</span><span class="sxs-lookup"><span data-stu-id="3b93d-122">**Create Journal Only**</span></span>|<span data-ttu-id="3b93d-123">Установите этот флажок, если при нажатии кнопки **OK** не нужно учитывать платежную квитанцию.</span><span class="sxs-lookup"><span data-stu-id="3b93d-123">Select this check box if you do not want to post the payment receipt when you choose the **OK** button.</span></span> <span data-ttu-id="3b93d-124">Платежная квитанция будет подготовлена в конкретном журнале и не будет учтена, пока кто-либо не учтет соответствующие строки журнала.</span><span class="sxs-lookup"><span data-stu-id="3b93d-124">The payment receipt will be prepared in the specified journal and will not be posted until someone posts the journal lines in question.</span></span>|  

5. <span data-ttu-id="3b93d-125">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="3b93d-125">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3b93d-126">См. также</span><span class="sxs-lookup"><span data-stu-id="3b93d-126">See Also</span></span>  
 <span data-ttu-id="3b93d-127">[Сбор платежей с прямым дебетом SEPA](finance-collect-payments-with-sepa-direct-debit.md) </span><span class="sxs-lookup"><span data-stu-id="3b93d-127">[Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span></span>  
 [<span data-ttu-id="3b93d-128">Продажи</span><span class="sxs-lookup"><span data-stu-id="3b93d-128">Sales</span></span>](sales-manage-sales.md)

