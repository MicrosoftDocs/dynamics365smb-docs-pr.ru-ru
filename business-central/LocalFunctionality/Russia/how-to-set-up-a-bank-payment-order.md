---
title: Настройка платежного поручения в России
description: Российские усовершенствования включают платежные поручения.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: a7fa18986d532cde0d64b9f3d7de7d34cf16437c
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738253"
---
# <a name="how-to-set-up-a-bank-payment-order"></a><span data-ttu-id="5128e-103">Практическое руководство. Настройка платежного поручения</span><span class="sxs-lookup"><span data-stu-id="5128e-103">How to: Set Up a Bank Payment Order</span></span>

<span data-ttu-id="5128e-104">Платежные поручения используются для банковских платежей в государственный бюджет.</span><span class="sxs-lookup"><span data-stu-id="5128e-104">Bank payment orders must be used if a bank payment is for the official state budget.</span></span> <span data-ttu-id="5128e-105">Чтобы использовать платежное поручение, необходимо создать шаблон финансового журнала, как описано в следующей процедуре.</span><span class="sxs-lookup"><span data-stu-id="5128e-105">To use a bank payment order, a general journal template must be created as described in the following procedure.</span></span>

## <a name="to-set-up-a-bank-payment-order"></a><span data-ttu-id="5128e-106">Настройка платежного поручения</span><span class="sxs-lookup"><span data-stu-id="5128e-106">To set up a bank payment order</span></span>

1. <span data-ttu-id="5128e-107">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Шаблоны финансовых журналов**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5128e-107">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal Templates**, and then choose the related link.</span></span>
2. <span data-ttu-id="5128e-108">Создайте раздел финансового журнала для каждой операции.</span><span class="sxs-lookup"><span data-stu-id="5128e-108">Create a general journal batch for every bank operation.</span></span>
3. <span data-ttu-id="5128e-109">В поле **Тип баланс. счета** выберите тип банковского счета.</span><span class="sxs-lookup"><span data-stu-id="5128e-109">In the **Bal. Account Type** field, select the bank account type.</span></span>
4. <span data-ttu-id="5128e-110">В поле **Номер баланс. счета** введите номер банковского счета.</span><span class="sxs-lookup"><span data-stu-id="5128e-110">In the **Bal. Account No.** field, enter the bank account.</span></span>
5. <span data-ttu-id="5128e-111">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Коды источников**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5128e-111">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Source Codes**, and then choose the related link.</span></span>
6. <span data-ttu-id="5128e-112">Создайте запись кода источника.</span><span class="sxs-lookup"><span data-stu-id="5128e-112">Create a source code record.</span></span>
7. <span data-ttu-id="5128e-113">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал кассовых ордеров КО-3**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5128e-113">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Source Code Setup**, and then choose the related link.</span></span>
8. <span data-ttu-id="5128e-114">На экспресс-вкладке **Общее** в поле **Банковские платежи** выберите код источника, который был введен в окне **Коды источников**.</span><span class="sxs-lookup"><span data-stu-id="5128e-114">On the **General** FastTab, in the **Bank Payments** field, select the source code that you entered in the **Source Codes** window.</span></span>

## <a name="see-also"></a><span data-ttu-id="5128e-115">См. также</span><span class="sxs-lookup"><span data-stu-id="5128e-115">See Also</span></span>

 [<span data-ttu-id="5128e-116">Управление банком</span><span class="sxs-lookup"><span data-stu-id="5128e-116">Bank Management</span></span>](Bank-Management.md)  
