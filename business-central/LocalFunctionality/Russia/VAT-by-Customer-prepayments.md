---
title: НДС по предоплатам клиентов в России
description: Российские улучшения включают отчетность по НДС по предоплатам клиентов.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: caaeb90a8bd4448fbf95d4d56cf31302c18eaa27
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738228"
---
# <a name="vat-by-customer-prepayment"></a><span data-ttu-id="b852e-103">НДС по предоплатам клиентов</span><span class="sxs-lookup"><span data-stu-id="b852e-103">VAT by Customer Prepayment</span></span>

<span data-ttu-id="b852e-104">Когда компания получает предоплату от клиента, вы должны создать счет НДС и запись и запись НДС на сумму НДС.</span><span class="sxs-lookup"><span data-stu-id="b852e-104">When a company receives a prepayment from a Customer, you must create a VAT invoice and a VAT record for the amount of VAT.</span></span> 

## <a name="setup"></a><span data-ttu-id="b852e-105">Настройка</span><span class="sxs-lookup"><span data-stu-id="b852e-105">Setup</span></span>

1. <span data-ttu-id="b852e-106">Включите нереализованный НДС в окне **Настройка ГК**.</span><span class="sxs-lookup"><span data-stu-id="b852e-106">To enable the unrealized VAT in the window **General Ledger Setup**.</span></span>
2. <span data-ttu-id="b852e-107">Настройте тип "Нереализованный НДС" и выберите учетную счет, по которой будет осуществляться операция нереализованного НДС — **Настройка учета НДС**.</span><span class="sxs-lookup"><span data-stu-id="b852e-107">Setup the unrealized VAT type and choose the account which will be taken of the operation of unrealized VAT **VAT posting setup**.</span></span>
3. <span data-ttu-id="b852e-108">Для настройки учетных групп клиентов: установите счет, по которому будет осуществляться операция предоплаты.</span><span class="sxs-lookup"><span data-stu-id="b852e-108">To configure the customer posting groups: set account, which will be taken of the operation of the prepayment.</span></span> 
4. <span data-ttu-id="b852e-109">Для каждого счета в плане счетов назначьте:</span><span class="sxs-lookup"><span data-stu-id="b852e-109">For each account in the chart of accounts, assign:</span></span> 

- <span data-ttu-id="b852e-110">Общий тип учета</span><span class="sxs-lookup"><span data-stu-id="b852e-110">General type of accounting</span></span> 
- <span data-ttu-id="b852e-111">НДС бизнес-группу</span><span class="sxs-lookup"><span data-stu-id="b852e-111">VAT business group</span></span>  
- <span data-ttu-id="b852e-112">НДС товарную группу</span><span class="sxs-lookup"><span data-stu-id="b852e-112">VAT product posting group</span></span>  

4. <span data-ttu-id="b852e-113">Настройте учет НДС на странице **Настройка учета НДС**.</span><span class="sxs-lookup"><span data-stu-id="b852e-113">Setup the VAT posting in **VAT Posting setup** page.</span></span>

## <a name="receiving-prepayment"></a><span data-ttu-id="b852e-114">Получение предоплаты</span><span class="sxs-lookup"><span data-stu-id="b852e-114">Receiving prepayment</span></span>

<span data-ttu-id="b852e-115">После получения предоплаты от клиента система создает записи нереализованного НДС и счета НДС.</span><span class="sxs-lookup"><span data-stu-id="b852e-115">After you receive prepayment from a customer, the system creates unrealized VAT records and VAT invoices.</span></span> 

<span data-ttu-id="b852e-116">Выполните учет предоплаты в финансовом журнале (см. [Предоплата продавца и покупателя](Prepayments-Vendor-and-Customers.md)).</span><span class="sxs-lookup"><span data-stu-id="b852e-116">Post prepayment in the General journal (see [Prepayment to the vendor and customers](Prepayments-Vendor-and-Customers.md)).</span></span>

## <a name="return-prepayment"></a><span data-ttu-id="b852e-117">Возврат предоплаты</span><span class="sxs-lookup"><span data-stu-id="b852e-117">Return prepayment</span></span>

<span data-ttu-id="b852e-118">Для возврата предоплаты необходимо создать запись реализованного НДС.</span><span class="sxs-lookup"><span data-stu-id="b852e-118">To return a prepayment, you must create a realized VAT record.</span></span> 

<span data-ttu-id="b852e-119">Выберите **Книга операций по клиентам** -> выберите возвращенную предоплату -> нажмите **Возврат платежа**.</span><span class="sxs-lookup"><span data-stu-id="b852e-119">Go to **Customer ledger entries** -> select returned prepayment -> press **return payment.**</span></span> 

<span data-ttu-id="b852e-120">Заполните поля:</span><span class="sxs-lookup"><span data-stu-id="b852e-120">Fill in the fields:</span></span>

| <span data-ttu-id="b852e-121">Поле</span><span class="sxs-lookup"><span data-stu-id="b852e-121">Field</span></span>               | <span data-ttu-id="b852e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b852e-122">Description</span></span>                                                  |
| ------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="b852e-123">Дата учета</span><span class="sxs-lookup"><span data-stu-id="b852e-123">Posting Date</span></span>        | <span data-ttu-id="b852e-124">Определяет дату учета операций, которые следует включить в отчет или пакетное задание.</span><span class="sxs-lookup"><span data-stu-id="b852e-124">Specifies the posting date of the entries that you want to include in the report or batch job.</span></span> |
| <span data-ttu-id="b852e-125">Номер документа</span><span class="sxs-lookup"><span data-stu-id="b852e-125">Document No.</span></span>        | <span data-ttu-id="b852e-126">Определяет номер связанного документа.</span><span class="sxs-lookup"><span data-stu-id="b852e-126">Specifies the number of the related document.</span></span>                |
| <span data-ttu-id="b852e-127">Новая дата учета</span><span class="sxs-lookup"><span data-stu-id="b852e-127">New posting Date</span></span>    | <span data-ttu-id="b852e-128">Определяет новую дату учета.</span><span class="sxs-lookup"><span data-stu-id="b852e-128">Specifies the new posting date.</span></span>                              |
| <span data-ttu-id="b852e-129">Номер нового документа</span><span class="sxs-lookup"><span data-stu-id="b852e-129">New Document No.</span></span>    | <span data-ttu-id="b852e-130">Определяет номер нового документа для предоплаты.</span><span class="sxs-lookup"><span data-stu-id="b852e-130">Specifies the new document number for the prepayment.</span></span>        |
| <span data-ttu-id="b852e-131">Описание учета</span><span class="sxs-lookup"><span data-stu-id="b852e-131">Posting Description</span></span> | <span data-ttu-id="b852e-132">Определяет описание, которое будет добавлено в итоговый учет.</span><span class="sxs-lookup"><span data-stu-id="b852e-132">Specifies the description that will be added to the resulting posting.</span></span> |
| <span data-ttu-id="b852e-133">Корректировка</span><span class="sxs-lookup"><span data-stu-id="b852e-133">Correction</span></span>          | <span data-ttu-id="b852e-134">Указывает, что операция является корректирующей.</span><span class="sxs-lookup"><span data-stu-id="b852e-134">Specifies the operation is corrective.</span></span>                       |

<span data-ttu-id="b852e-135">Нажмите "ОК".</span><span class="sxs-lookup"><span data-stu-id="b852e-135">Click "OK".</span></span> <span data-ttu-id="b852e-136">Система автоматически создаст корректирующие операции.</span><span class="sxs-lookup"><span data-stu-id="b852e-136">The system will automatically create corrective entries.</span></span>

## <a name="see-also"></a><span data-ttu-id="b852e-137">См. также</span><span class="sxs-lookup"><span data-stu-id="b852e-137">See Also</span></span>

[<span data-ttu-id="b852e-138">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="b852e-138">Russia Local Functionality</span></span>](russia-local-functionality.md)  
