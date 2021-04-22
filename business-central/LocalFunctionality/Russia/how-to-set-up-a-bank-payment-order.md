---
title: Настройка платежного поручения в России
description: Российские усовершенствования включают платежные поручения.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 660d198e4da6c581d6ea2dfdf15513a37c8d64e9
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779180"
---
# <a name="set-up-a-bank-payment-order"></a><span data-ttu-id="9435f-103">Настройка платежного поручения</span><span class="sxs-lookup"><span data-stu-id="9435f-103">Set Up a Bank Payment Order</span></span>

<span data-ttu-id="9435f-104">Платежные поручения используются для банковских платежей в государственный бюджет.</span><span class="sxs-lookup"><span data-stu-id="9435f-104">Bank payment orders must be used if a bank payment is for the official state budget.</span></span> <span data-ttu-id="9435f-105">Чтобы использовать платежное поручение, необходимо создать шаблон финансового журнала, как описано в следующей процедуре.</span><span class="sxs-lookup"><span data-stu-id="9435f-105">To use a bank payment order, a general journal template must be created as described in the following procedure.</span></span>

## <a name="to-set-up-a-bank-payment-order"></a><span data-ttu-id="9435f-106">Настройка платежного поручения</span><span class="sxs-lookup"><span data-stu-id="9435f-106">To set up a bank payment order</span></span>

1. <span data-ttu-id="9435f-107">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Шаблоны финансового журнала**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="9435f-107">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal Templates**, and then choose the related link.</span></span>
2. <span data-ttu-id="9435f-108">Создайте раздел финансового журнала для каждой операции.</span><span class="sxs-lookup"><span data-stu-id="9435f-108">Create a general journal batch for every bank operation.</span></span>
3. <span data-ttu-id="9435f-109">В поле **Тип баланс. счета** выберите тип банковского счета.</span><span class="sxs-lookup"><span data-stu-id="9435f-109">In the **Bal. Account Type** field, select the bank account type.</span></span>
4. <span data-ttu-id="9435f-110">В поле **Номер баланс. счета** введите номер банковского счета.</span><span class="sxs-lookup"><span data-stu-id="9435f-110">In the **Bal. Account No.** field, enter the bank account.</span></span>
5. <span data-ttu-id="9435f-111">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Коды источников**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="9435f-111">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Source Codes**, and then choose the related link.</span></span>
6. <span data-ttu-id="9435f-112">Создайте запись кода источника.</span><span class="sxs-lookup"><span data-stu-id="9435f-112">Create a source code record.</span></span>
7. <span data-ttu-id="9435f-113">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка кодов источника**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="9435f-113">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Source Code Setup**, and then choose the related link.</span></span>
8. <span data-ttu-id="9435f-114">На экспресс-вкладке **Общее** в поле **Банковские платежи** выберите код источника, который был введен в окне **Коды источников**.</span><span class="sxs-lookup"><span data-stu-id="9435f-114">On the **General** FastTab, in the **Bank Payments** field, select the source code that you entered in the **Source Codes** window.</span></span>

## <a name="see-also"></a><span data-ttu-id="9435f-115">См. также</span><span class="sxs-lookup"><span data-stu-id="9435f-115">See Also</span></span>

 [<span data-ttu-id="9435f-116">Управление банком</span><span class="sxs-lookup"><span data-stu-id="9435f-116">Bank Management</span></span>](Bank-Management.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]