---
title: Учет платежной квитанции по прямому дебету SEPA | Документы Майкрософт
description: При успешной обработке банком непосредственной операции сбора на дебетовом счете можно переходить к учету приемки оплаты для соответствующих счетов продажи.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: finance-collect-payments-with-sepa-direct-debit
ms.openlocfilehash: 6c646575ba803358aa00309ce02742423bcc7de8
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1242656"
---
# <a name="post-sepa-direct-debit-payment-receipts"></a><span data-ttu-id="cd9f0-103">Учет платежной квитанции по прямому дебету SEPA</span><span class="sxs-lookup"><span data-stu-id="cd9f0-103">Post SEPA Direct Debit Payment Receipts</span></span>
<span data-ttu-id="cd9f0-104">При успешной обработке банком непосредственной операции сбора на дебетовом счете можно переходить к учету приемки оплаты для соответствующих счетов продажи.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-104">When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.</span></span> <span data-ttu-id="cd9f0-105">Дополнительные сведения см. в разделе [Создание операций погашения прямого дебета SEPA и их экспорт в файл банка](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="cd9f0-105">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  

<span data-ttu-id="cd9f0-106">Учесть платежную квитанции можно непосредственно на странице **Коллекции прямого дебетования** или на странице **Операции коллекции прямого дебетования**.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-106">You can post the payment receipt directly from the **Direct Debit Collections** page or the **Direct Debit Collect. Entries** page.</span></span> <span data-ttu-id="cd9f0-107">Кроме того, можно передать работу другому пользователю путем подготовки связанных строк журнала.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-107">Alternatively, you can relay the work to another user by preparing the related journal lines.</span></span>  

## <a name="to-post-a-direct-debit-payment-receipt-from-the-direct-debit-collections-page"></a><span data-ttu-id="cd9f0-108">Учет платежной квитанции по прямому дебету на странице погашений прямого дебета</span><span class="sxs-lookup"><span data-stu-id="cd9f0-108">To post a direct-debit payment receipt from the Direct Debit Collections page</span></span>  
1. <span data-ttu-id="cd9f0-109">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сбор платежей с помощью прямого дебетования**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Direct Debit Collections**, and then choose the related link.</span></span>  
2. <span data-ttu-id="cd9f0-110">Выберите строку для коллекции прямого дебета, экспортированную в файл банка и успешно обработанную банком.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-110">Select a line for a direct debit collection that has been exported to a bank file and successfully processed by the bank.</span></span> <span data-ttu-id="cd9f0-111">Дополнительные сведения см. в разделе [Создание операций погашения прямого дебета SEPA и их экспорт в файл банка](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="cd9f0-111">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  
3. <span data-ttu-id="cd9f0-112">Выберите действие **Поступления после платежа**.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-112">Choose the **Post Payment Receipts** action.</span></span>  
4. <span data-ttu-id="cd9f0-113">На странице **Учет коллекции прямого дебетования** заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-113">On the **Post Direct Debit Collection** page, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="cd9f0-114">Поле</span><span class="sxs-lookup"><span data-stu-id="cd9f0-114">Field</span></span>|<span data-ttu-id="cd9f0-115">Описанием</span><span class="sxs-lookup"><span data-stu-id="cd9f0-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="cd9f0-116">**Номер коллекции прямого дебетования**</span><span class="sxs-lookup"><span data-stu-id="cd9f0-116">**Direct Debit Collection No.**</span></span>|<span data-ttu-id="cd9f0-117">Укажите погашение прямого дебета, для которого необходимо учесть платежную квитанцию.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-117">Specify the direct debit collection that you want to post payment receipt for.</span></span>|  
    |<span data-ttu-id="cd9f0-118">**Шаблон финансового журнала**</span><span class="sxs-lookup"><span data-stu-id="cd9f0-118">**General Journal Template**</span></span>|<span data-ttu-id="cd9f0-119">Укажите шаблон финансового журнала, который предполагается использовать для учета платежной квитанции, например шаблон для кассовых поступлений.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-119">Specify which general journal template to use for posting the payment receipt, such as the template for cash receipts.</span></span>|  
    |<span data-ttu-id="cd9f0-120">**Название раздела финансового журнала**</span><span class="sxs-lookup"><span data-stu-id="cd9f0-120">**General Journal Batch Name**</span></span>|<span data-ttu-id="cd9f0-121">Укажите раздел финансового журнала, который предполагается использовать для учета платежной квитанции.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-121">Specify which general journal batch to use for posting the payment receipt.</span></span>|  
    |<span data-ttu-id="cd9f0-122">**Создать только журнал**</span><span class="sxs-lookup"><span data-stu-id="cd9f0-122">**Create Journal Only**</span></span>|<span data-ttu-id="cd9f0-123">Установите этот флажок, если при нажатии кнопки **ОК** не нужно учитывать платежную квитанцию.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-123">Select this check box if you do not want to post the payment receipt when you choose the **OK** button.</span></span> <span data-ttu-id="cd9f0-124">Платежная квитанция будет подготовлена в конкретном журнале и не будет учтена, пока кто-либо не учтет соответствующие строки журнала.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-124">The payment receipt will be prepared in the specified journal and will not be posted until someone posts the journal lines in question.</span></span>|  

5. <span data-ttu-id="cd9f0-125">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="cd9f0-125">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cd9f0-126">См. также</span><span class="sxs-lookup"><span data-stu-id="cd9f0-126">See Also</span></span>  
 <span data-ttu-id="cd9f0-127">[Сбор платежей с прямым дебетом SEPA](finance-collect-payments-with-sepa-direct-debit.md) </span><span class="sxs-lookup"><span data-stu-id="cd9f0-127">[Collect Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span></span>  
 [<span data-ttu-id="cd9f0-128">Продажи</span><span class="sxs-lookup"><span data-stu-id="cd9f0-128">Sales</span></span>](sales-manage-sales.md)
