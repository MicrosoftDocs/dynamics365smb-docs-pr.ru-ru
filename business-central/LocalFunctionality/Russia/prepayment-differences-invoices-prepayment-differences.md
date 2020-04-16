---
title: Авансовые разницы в России
description: Российские усовершенствования включают управление авансовыми разницами.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 5377561f41e4f96b738c22b031af11d114f1d229
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3189215"
---
# <a name="prepayment-differences"></a><span data-ttu-id="659d1-103">Авансовые разницы</span><span class="sxs-lookup"><span data-stu-id="659d1-103">Prepayment Differences</span></span>

<span data-ttu-id="659d1-104">Когда вы применяете предоплату к счету в иностранной валюте, [!INCLUDE[prodshort](../../includes/prodshort.md)] рассчитывает разницу в суммах на основе курсов обмена валют между счетом и предоплатой и создает запись авансовой разницы для счета.</span><span class="sxs-lookup"><span data-stu-id="659d1-104">When you apply a prepayment to an invoice in a foreign currency, [!INCLUDE[prodshort](../../includes/prodshort.md)] calculates the difference in the amounts based on currency exchange rates between the invoice and the prepayment and create a prepayment difference entry for the invoice.</span></span>  

### <a name="setup-for-purchases"></a><span data-ttu-id="659d1-105">Настройка для покупок</span><span class="sxs-lookup"><span data-stu-id="659d1-105">Setup for Purchases</span></span>

<span data-ttu-id="659d1-106">На странице **Настройка модуля "Покупки и кредиторская задолженность"** заполните следующие поля:</span><span class="sxs-lookup"><span data-stu-id="659d1-106">On the **Purchases & Payables Setup** page, fill in the fields:</span></span>

| <span data-ttu-id="659d1-107">Поле</span><span class="sxs-lookup"><span data-stu-id="659d1-107">Field</span></span>                      | <span data-ttu-id="659d1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="659d1-108">Description</span></span>                                                  |
| -------------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="659d1-109">**Использовать счет ГК предоплаты**</span><span class="sxs-lookup"><span data-stu-id="659d1-109">**Use Prepayment Account**</span></span> | <span data-ttu-id="659d1-110">Определяет, требуется ли учитывать предоплаты с помощью счета главной книги.</span><span class="sxs-lookup"><span data-stu-id="659d1-110">Specifies if you want to post prepayments using the general ledger account.</span></span> |
| <span data-ttu-id="659d1-111">**Учт. разн. по предопл. - серия ном. док.**</span><span class="sxs-lookup"><span data-stu-id="659d1-111">**Posted PD Doc. Nos.**</span></span>    | <span data-ttu-id="659d1-112">Определяет серию номеров, из которой присваиваются номера новых записей.</span><span class="sxs-lookup"><span data-stu-id="659d1-112">Specifies the number series from which numbers are assigned to new records.</span></span> |
| <span data-ttu-id="659d1-113">**Разн. по предопл. - тип серии номеров док.**</span><span class="sxs-lookup"><span data-stu-id="659d1-113">**PD Doc. Nos. Type**</span></span>      | <span data-ttu-id="659d1-114">Определяет, требуется ли использовать серию номеров или символ для идентификации операций транзакций предоплаты.</span><span class="sxs-lookup"><span data-stu-id="659d1-114">Specifies if you want to use a number series or symbol to identify prepayment transaction entries.</span></span> |
| <span data-ttu-id="659d1-115">**Символ для док. разн. по предопл.**</span><span class="sxs-lookup"><span data-stu-id="659d1-115">**Symbol for PD Doc**</span></span>      | <span data-ttu-id="659d1-116">Определяет символ, который идентифицирует связанные операции предоплаты.</span><span class="sxs-lookup"><span data-stu-id="659d1-116">Specifies the symbol that identifies prepayment related entries.</span></span> |

### <a name="setup-for-sales"></a><span data-ttu-id="659d1-117">Настройка для продаж</span><span class="sxs-lookup"><span data-stu-id="659d1-117">Setup for Sales</span></span>

<span data-ttu-id="659d1-118">На странице **Настройка модуля "Продажи и дебиторская задолженность"** заполните следующие поля:</span><span class="sxs-lookup"><span data-stu-id="659d1-118">On the **Sales & Receivables Setup** page, fill in the fields:</span></span>

| <span data-ttu-id="659d1-119">Поле</span><span class="sxs-lookup"><span data-stu-id="659d1-119">Field</span></span>                     | <span data-ttu-id="659d1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="659d1-120">Description</span></span>                                                  |
| ------------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="659d1-121">**Использовать счет ГК предоплаты**</span><span class="sxs-lookup"><span data-stu-id="659d1-121">**Use Prepayment Account**</span></span>    | <span data-ttu-id="659d1-122">Определяет, требуется ли учитывать предоплаты с помощью счета главной книги.</span><span class="sxs-lookup"><span data-stu-id="659d1-122">Specifies if you want to post prepayments using the general ledger account.</span></span> |
| <span data-ttu-id="659d1-123">**Создание счета на предоплату**</span><span class="sxs-lookup"><span data-stu-id="659d1-123">**Create Prepayment Invoice**</span></span> | <span data-ttu-id="659d1-124">Определяет, требуется ли создать счет на предоплату.</span><span class="sxs-lookup"><span data-stu-id="659d1-124">Specifies if you want to create an invoice for the prepayment.</span></span> |
| <span data-ttu-id="659d1-125">**Серия номеров учт. предоплат**</span><span class="sxs-lookup"><span data-stu-id="659d1-125">**Posted Prepayment Nos.**</span></span>    | <span data-ttu-id="659d1-126">Определяет серию номеров, из которой присваиваются номера новых записей.</span><span class="sxs-lookup"><span data-stu-id="659d1-126">Specifies the number series from which numbers are assigned to new records.</span></span> |
| <span data-ttu-id="659d1-127">**Учт. разн. по предопл. - серия ном. док.**</span><span class="sxs-lookup"><span data-stu-id="659d1-127">**Posted PD Doc. Nos.**</span></span>       | <span data-ttu-id="659d1-128">Определяет серию номеров, из которой присваиваются номера новых записей.</span><span class="sxs-lookup"><span data-stu-id="659d1-128">Specifies the number series from which numbers are assigned to new records.</span></span> |
| <span data-ttu-id="659d1-129">**Разн. по предопл. - тип серии номеров док.**</span><span class="sxs-lookup"><span data-stu-id="659d1-129">**PD Doc. Nos. Type**</span></span>         | <span data-ttu-id="659d1-130">Определяет, требуется ли использовать серию номеров или символ для идентификации операций транзакций предоплаты.</span><span class="sxs-lookup"><span data-stu-id="659d1-130">Specifies if you want to use a number series or symbol to identify prepayment transaction entries.</span></span> |
| <span data-ttu-id="659d1-131">**Символ для док. разн. по предопл.**</span><span class="sxs-lookup"><span data-stu-id="659d1-131">**Symbol for PD Doc.**</span></span>        | <span data-ttu-id="659d1-132">Определяет символ, который идентифицирует связанные операции предоплаты.</span><span class="sxs-lookup"><span data-stu-id="659d1-132">Specifies a symbol that identifies prepayment related entries.</span></span> |

## <a name="see-also"></a><span data-ttu-id="659d1-133">См. также</span><span class="sxs-lookup"><span data-stu-id="659d1-133">See Also</span></span>

[<span data-ttu-id="659d1-134">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="659d1-134">Russia Local Functionality</span></span>](russia-local-functionality.md)  
