---
title: "Выбор метода электронных платежей | Документы Майкрософт"
description: "Обрабатывайте платежи поставщикам путем экспорта файла со сведениями о платежах из строк журнала."
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
ms.sourcegitcommit: 8b2e20e694279a8c06188e0e429ef3b4fb43aea2
ms.openlocfilehash: 20ae505bc76b8971c678de9e2664653aa5032d6e
ms.contentlocale: ru-ru
ms.lasthandoff: 09/27/2017

---
# <a name="make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a><span data-ttu-id="f29fe-103">Выполнение платежей с помощью службы конвертации банковских данных или кредитового перевода SEPA</span><span class="sxs-lookup"><span data-stu-id="f29fe-103">Make Payments with Bank Data Conversion Service or SEPA Credit Transfer</span></span>
<span data-ttu-id="f29fe-104">В окне **Журнал платежей** можно обработать платежи поставщикам путем экспорта файла со сведениями о платежах из строк журнала.</span><span class="sxs-lookup"><span data-stu-id="f29fe-104">In the **Payment Journal** window, you can process payments to your vendors by exporting a file together with the payment information from the journal lines.</span></span> <span data-ttu-id="f29fe-105">Затем можно загрузить файл в электронный банк для обработки соответствующих денежных переводов.</span><span class="sxs-lookup"><span data-stu-id="f29fe-105">You can then upload the file to your electronic bank where the related money transfers are processed.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="f29fe-106"> поддерживает формат кредитового перевода SEPA, но в вашей стране или регионе могут быть доступны другие форматы электронных платежей.</span><span class="sxs-lookup"><span data-stu-id="f29fe-106"> supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.</span></span>   

 <span data-ttu-id="f29fe-107">Чтобы включить кредитные переносы SEPA, необходимо сначала настроить банковский счет, поставщика и общий раздел журнала, на котором будет основан журнал оплаты.</span><span class="sxs-lookup"><span data-stu-id="f29fe-107">To enable SEPA credit transfers, you must first set up a bank account, a vendor, and the general journal batch that the payment journal is based on.</span></span> <span data-ttu-id="f29fe-108">Затем подготавливаются платежи поставщикам путем автоматического заполнения окна **Журнал платежей** сведениями о платежах с подошедшим сроком с указанием дат учета.</span><span class="sxs-lookup"><span data-stu-id="f29fe-108">You then prepare payments to vendors by automatically filling the **Payment Journal** window with due payments with specified posting dates.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="f29fe-109">Убедившись, что платежи успешно обработаны банком, можно переходить к учету строк журнала платежей.</span><span class="sxs-lookup"><span data-stu-id="f29fe-109">When you have verified that the payments are successfully processed by the bank, you can proceed to post the payment journal lines.</span></span>  

 <span data-ttu-id="f29fe-110">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="f29fe-110">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="f29fe-111">**Задача**</span><span class="sxs-lookup"><span data-stu-id="f29fe-111">**To**</span></span>|<span data-ttu-id="f29fe-112">**Ссылка**</span><span class="sxs-lookup"><span data-stu-id="f29fe-112">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="f29fe-113">Активация службы обработки данных банка для преобразования любого файла банковской выписки в формат, который можно импортировать, или для преобразования экспортируемых файлов платежей в требуемый банком формат.</span><span class="sxs-lookup"><span data-stu-id="f29fe-113">Activate the Bank Data Conversion Service feature to have any bank statement file converted to a format that you can import or to have your exported payment files converted to the format that your bank requires.</span></span>|[<span data-ttu-id="f29fe-114">Практическое руководство. Настройка службы конвертации банковских данных</span><span class="sxs-lookup"><span data-stu-id="f29fe-114">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-statement-service.md)|  
|<span data-ttu-id="f29fe-115">Настройка банковского счета, поставщика и журнала платежей для кредитового перевода SEPA.</span><span class="sxs-lookup"><span data-stu-id="f29fe-115">Set up a bank account, a vendor, and a payment journal for SEPA credit transfer.</span></span>|[<span data-ttu-id="f29fe-116">Практическое руководство. Настройка кредитового перевода SEPA</span><span class="sxs-lookup"><span data-stu-id="f29fe-116">How to: Set Up SEPA Credit Transfer</span></span>](finance-how-to-set-up-sepa-credit-transfer.md)|  
|<span data-ttu-id="f29fe-117">Заполнение журнал платежей строками по задолженностям перед поставщиками с возможностью вставить даты учета на основании срока оплаты в связанных документах покупки.</span><span class="sxs-lookup"><span data-stu-id="f29fe-117">Fill the payment journal with lines for due payments to vendors, with the option to insert posting dates based on the due date of the related purchase documents.</span></span>|[<span data-ttu-id="f29fe-118">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="f29fe-118">Manage Payables</span></span>](payables-manage-payables.md)|  
|<span data-ttu-id="f29fe-119">Экспорт строк журнала платежей в файл в формате кредитового перевода SEPA.</span><span class="sxs-lookup"><span data-stu-id="f29fe-119">Export payment journal lines to a file in the SEPA Credit Transfer format.</span></span>|[<span data-ttu-id="f29fe-120">Практическое руководство. Экспорт платежей в банковский файл</span><span class="sxs-lookup"><span data-stu-id="f29fe-120">How to: Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|  
|<span data-ttu-id="f29fe-121">Просмотр того, какие платежи были экспортированы и в какие файлы.</span><span class="sxs-lookup"><span data-stu-id="f29fe-121">Review which payments have been exported and into which files.</span></span>|<span data-ttu-id="f29fe-122">Регистры кредитовых переводов</span><span class="sxs-lookup"><span data-stu-id="f29fe-122">Credit Transfer Registers</span></span>|  
|<span data-ttu-id="f29fe-123">Если электронный платеж успешно обрабатывается банком, выполняется учет платежей.</span><span class="sxs-lookup"><span data-stu-id="f29fe-123">When the electronic payment is successfully processed by the bank, post the payments.</span></span>|[<span data-ttu-id="f29fe-124">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="f29fe-124">Working with General Journals</span></span>](ui-work-general-journals.md)|  

## <a name="see-also"></a><span data-ttu-id="f29fe-125">См. также</span><span class="sxs-lookup"><span data-stu-id="f29fe-125">See Also</span></span>  
[<span data-ttu-id="f29fe-126">Практическое руководство. Настройка службы конвертации банковских данных</span><span class="sxs-lookup"><span data-stu-id="f29fe-126">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-statement-service.md)  
[<span data-ttu-id="f29fe-127">Практическое руководство. Настройка кредитового перевода SEPA</span><span class="sxs-lookup"><span data-stu-id="f29fe-127">How to: Set Up SEPA Credit Transfer</span></span>](finance-how-to-set-up-sepa-credit-transfer.md)  
<span data-ttu-id="f29fe-128">[Управление кредиторской задолженностью](payables-manage-payables.md) </span><span class="sxs-lookup"><span data-stu-id="f29fe-128">[Manage Payables](payables-manage-payables.md) </span></span>  
[<span data-ttu-id="f29fe-129">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="f29fe-129">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="f29fe-130">Сбор платежей с прямым дебетом SEPA</span><span class="sxs-lookup"><span data-stu-id="f29fe-130">Collecting Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)   

