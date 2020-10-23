---
title: Предоплата для поставщиков и клиентов в России
description: Российские усовершенствования включают управление предоплатой поставщиков и клиентов.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 435a4359dbfd59086f1bb3c043e6e3a41df07a35
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3921294"
---
# <a name="posting-vendor-and-customer-prepayments"></a><span data-ttu-id="9dbf7-103">Учет предоплаты поставщиков и клиентов</span><span class="sxs-lookup"><span data-stu-id="9dbf7-103">Posting Vendor and Customer Prepayments</span></span>

<span data-ttu-id="9dbf7-104">В российской версии предоплаты работают не так, как в стандартной версии [!INCLUDE[prodshort](../../includes/prodshort.md)],</span><span class="sxs-lookup"><span data-stu-id="9dbf7-104">In the Russian version, prepayments work in a different way compared to the standard version of [!INCLUDE[prodshort](../../includes/prodshort.md)].</span></span> <span data-ttu-id="9dbf7-105">Когда мы получаем предоплату, по правилам бухгалтерского учета необходимо учесть предоплату на отдельном счете.</span><span class="sxs-lookup"><span data-stu-id="9dbf7-105">When we receive a prepayment, it is necessary by accounting rules to post the prepayment on a separate account.</span></span> <span data-ttu-id="9dbf7-106">Таким образом, группы учета поставщиков и клиентов имеют поле **Счет предоплаты**.</span><span class="sxs-lookup"><span data-stu-id="9dbf7-106">Therefore, the vendor and customer posting groups have the **Prepayment Account** field.</span></span>

[!INCLUDE[prodshort](../../includes/prodshort.md)] <span data-ttu-id="9dbf7-107">использует эти счета для операций предоплаты — платежей с отметкой "Предоплата".</span><span class="sxs-lookup"><span data-stu-id="9dbf7-107">uses this accounts for prepayment entries- Payment with Prepayment check mark.</span></span>

## <a name="to-post-a-prepayment"></a><span data-ttu-id="9dbf7-108">Для учета предоплаты</span><span class="sxs-lookup"><span data-stu-id="9dbf7-108">To post a prepayment</span></span>

1. <span data-ttu-id="9dbf7-109">На странице **Финансовый журнал** установите флажок **Тип документа - Платеж и предоплата**.</span><span class="sxs-lookup"><span data-stu-id="9dbf7-109">On the **General Journal** page, select the **Document Type - Payment and Prepayment** check box.</span></span>
2. <span data-ttu-id="9dbf7-110">Укажите тип и номер счета, тип и номер балансового счета.</span><span class="sxs-lookup"><span data-stu-id="9dbf7-110">Specify the account type and account number, the balance account type, and the balance account number.</span></span>
3. <span data-ttu-id="9dbf7-111">Выполните учет финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="9dbf7-111">Post the general journal.</span></span>

## <a name="to-apply-prepayments"></a><span data-ttu-id="9dbf7-112">Чтобы применить предоплаты</span><span class="sxs-lookup"><span data-stu-id="9dbf7-112">To apply prepayments</span></span>

1. <span data-ttu-id="9dbf7-113">Перейдите на страницу **Книга операций по поставщикам** или **Книга операций по клиентам**.</span><span class="sxs-lookup"><span data-stu-id="9dbf7-113">Go to the **Vendor Ledger Entries** or **Customer Ledger Entries** page.</span></span>
2. <span data-ttu-id="9dbf7-114">Выберите строку с учтенной предоплатой, затем выберите действие **Применить**.</span><span class="sxs-lookup"><span data-stu-id="9dbf7-114">Select a line with a posted prepayment, and then choose the **Apply** action.</span></span>
4. <span data-ttu-id="9dbf7-115">Выберите строку со счетом, к которому требуется применить предоплату, затем выберите действие **Установить код применения**.</span><span class="sxs-lookup"><span data-stu-id="9dbf7-115">Select the line with the invoice to which you want to apply the prepayment, and then choose the **Set applies-to ID** action.</span></span>
6. <span data-ttu-id="9dbf7-116">Выберите действие **Учет применения**.</span><span class="sxs-lookup"><span data-stu-id="9dbf7-116">Choose the **Post Application** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="9dbf7-117">См. также</span><span class="sxs-lookup"><span data-stu-id="9dbf7-117">See Also</span></span>

[<span data-ttu-id="9dbf7-118">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="9dbf7-118">Russia Local Functionality</span></span>](russia-local-functionality.md)  
