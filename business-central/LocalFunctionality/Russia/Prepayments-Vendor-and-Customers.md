---
title: Предоплата для поставщиков и клиентов в России
description: Российские усовершенствования включают управление предоплатой поставщиков и клиентов.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: e617026179b09fb2148ba401c26aab5cee36fa8d
ms.sourcegitcommit: 319023e53627dbe8e68643908aacc6fd594a4957
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/04/2019
ms.locfileid: "2554538"
---
# <a name="posting-vendor-and-customer-prepayments"></a><span data-ttu-id="af640-103">Учет предоплаты поставщиков и клиентов</span><span class="sxs-lookup"><span data-stu-id="af640-103">Posting Vendor and Customer Prepayments</span></span>

<span data-ttu-id="af640-104">В российской версии предоплаты работают не так, как в стандартной версии [!INCLUDE[prodshort](../../includes/prodshort.md)],</span><span class="sxs-lookup"><span data-stu-id="af640-104">In the Russian version, prepayments work in a different way compared to the standard version of [!INCLUDE[prodshort](../../includes/prodshort.md)].</span></span> <span data-ttu-id="af640-105">Когда мы получаем предоплату, по правилам бухгалтерского учета необходимо учесть предоплату на отдельном счете.</span><span class="sxs-lookup"><span data-stu-id="af640-105">When we receive a prepayment, it is necessary by accounting rules to post the prepayment on a separate account.</span></span> <span data-ttu-id="af640-106">Таким образом, группы учета поставщиков и клиентов имеют поле **Счет предоплаты**.</span><span class="sxs-lookup"><span data-stu-id="af640-106">Therefore, the vendor and customer posting groups have the **Prepayment Account** field.</span></span>

[!INCLUDE[prodshort](../../includes/prodshort.md)] <span data-ttu-id="af640-107">использует эти счета для операций предоплаты — платежей с отметкой "Предоплата".</span><span class="sxs-lookup"><span data-stu-id="af640-107">uses this accounts for prepayment entries- Payment with Prepayment check mark.</span></span>

## <a name="to-post-a-prepayment"></a><span data-ttu-id="af640-108">Для учета предоплаты</span><span class="sxs-lookup"><span data-stu-id="af640-108">To post a prepayment</span></span>

1. <span data-ttu-id="af640-109">На странице **Финансовый журнал** установите флажок **Тип документа - Платеж и предоплата**.</span><span class="sxs-lookup"><span data-stu-id="af640-109">On the **General Journal** page, select the **Document Type - Payment and Prepayment** check box.</span></span>
2. <span data-ttu-id="af640-110">Укажите тип и номер счета, тип и номер балансового счета.</span><span class="sxs-lookup"><span data-stu-id="af640-110">Specify the account type and account number, the balance account type, and the balance account number.</span></span>
3. <span data-ttu-id="af640-111">Выполните учет финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="af640-111">Post the general journal.</span></span>

## <a name="to-apply-prepayments"></a><span data-ttu-id="af640-112">Чтобы применить предоплаты</span><span class="sxs-lookup"><span data-stu-id="af640-112">To apply prepayments</span></span>

1. <span data-ttu-id="af640-113">Перейдите на страницу **Книга операций по поставщикам** или **Книга операций по клиентам**.</span><span class="sxs-lookup"><span data-stu-id="af640-113">Go to the **Vendor Ledger Entries** or **Customer Ledger Entries** page.</span></span>
2. <span data-ttu-id="af640-114">Выберите строку с учтенной предоплатой, затем выберите действие **Применить**.</span><span class="sxs-lookup"><span data-stu-id="af640-114">Select a line with a posted prepayment, and then choose the **Apply** action.</span></span>
4. <span data-ttu-id="af640-115">Выберите строку со счетом, к которому требуется применить предоплату, затем выберите действие **Установить код применения**.</span><span class="sxs-lookup"><span data-stu-id="af640-115">Select the line with the invoice to which you want to apply the prepayment, and then choose the **Set applies-to ID** action.</span></span>
6. <span data-ttu-id="af640-116">Выберите действие **Учет применения**.</span><span class="sxs-lookup"><span data-stu-id="af640-116">Choose the **Post Application** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="af640-117">См. также</span><span class="sxs-lookup"><span data-stu-id="af640-117">See Also</span></span>

[<span data-ttu-id="af640-118">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="af640-118">Russia Local Functionality</span></span>](russia-local-functionality.md)  
