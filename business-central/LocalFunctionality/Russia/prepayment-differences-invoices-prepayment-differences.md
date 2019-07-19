---
title: Авансовые разницы в России
description: Российские усовершенствования включают управление авансовыми разницами.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: fab5546571e73ce43164ab0c81a75ffc29f17e62
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738242"
---
# <a name="prepayment-differences-and-invoices-for-prepayment-differences"></a><span data-ttu-id="fd002-103">Авансовые разницы и счета по авансовым разницам</span><span class="sxs-lookup"><span data-stu-id="fd002-103">Prepayment Differences and Invoices for Prepayment Differences</span></span>

<span data-ttu-id="fd002-104">Когда вы применяете предоплату к счету в иностранной валюте, [!INCLUDE[prodshort](../../includes/prodshort.md)] рассчитывает разницу в суммах на основе курсов обмена валют между счетом и предоплатой и создает запись авансовой разницы для счета.</span><span class="sxs-lookup"><span data-stu-id="fd002-104">When you apply a prepayment to an invoice in a foreign currency, [!INCLUDE[prodshort](../../includes/prodshort.md)] calculates the difference in the amounts based on currency exchange rates between the invoice and the prepayment and create a prepayment difference entry for the invoice.</span></span>  

### <a name="setups-for-purchases"></a><span data-ttu-id="fd002-105">Настройки для покупок</span><span class="sxs-lookup"><span data-stu-id="fd002-105">Setups for Purchases</span></span>

<span data-ttu-id="fd002-106">На странице **Настройка модуля "Покупки"** заполните следующие поля:</span><span class="sxs-lookup"><span data-stu-id="fd002-106">In the **Purchases & payables Setup** page fill the fields:</span></span>

| <span data-ttu-id="fd002-107">Поле</span><span class="sxs-lookup"><span data-stu-id="fd002-107">Field</span></span>                      | <span data-ttu-id="fd002-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fd002-108">Description</span></span>                                                  |
| -------------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="fd002-109">**Использовать счет ГК предоплаты**</span><span class="sxs-lookup"><span data-stu-id="fd002-109">**Use Prepayment Account**</span></span> | <span data-ttu-id="fd002-110">Определяет, требуется ли учитывать предоплаты с помощью счета главной книги.</span><span class="sxs-lookup"><span data-stu-id="fd002-110">Specifies if you want to post prepayments using the general ledger account.</span></span> |
| <span data-ttu-id="fd002-111">**Учт. разн. по предопл. - серия ном. док.**</span><span class="sxs-lookup"><span data-stu-id="fd002-111">**Posted PD Doc. Nos.**</span></span>    | <span data-ttu-id="fd002-112">Определяет серию номеров, из которой присваиваются номера новых записей.</span><span class="sxs-lookup"><span data-stu-id="fd002-112">Specifies the number series from which numbers are assigned to new records.</span></span> |
| <span data-ttu-id="fd002-113">**Разн. по предопл. - тип серии номеров док.**</span><span class="sxs-lookup"><span data-stu-id="fd002-113">**PD Doc. Nos. Type**</span></span>      | <span data-ttu-id="fd002-114">Определяет, требуется ли использовать серию номеров или символ для идентификации операций транзакций предоплаты.</span><span class="sxs-lookup"><span data-stu-id="fd002-114">Specifies if you want to use a number series or symbol to identify prepayment transaction entries.</span></span> |
| <span data-ttu-id="fd002-115">**Символ для док. разн. по предопл.**</span><span class="sxs-lookup"><span data-stu-id="fd002-115">**Symbol for PD Doc**</span></span>      | <span data-ttu-id="fd002-116">Определяет символ, который идентифицирует связанные операции предоплаты.</span><span class="sxs-lookup"><span data-stu-id="fd002-116">Specifies the symbol that identifies prepayment related entries.</span></span> |

### <a name="setup-for-sales"></a><span data-ttu-id="fd002-117">Настройка для продаж.</span><span class="sxs-lookup"><span data-stu-id="fd002-117">Setup for Sales.</span></span>

<span data-ttu-id="fd002-118">На странице **Настройка модуля "Продажи"** заполните следующие поля:</span><span class="sxs-lookup"><span data-stu-id="fd002-118">In the **Sales & Receivables setup** page fill the fields:</span></span>

| <span data-ttu-id="fd002-119">Поле</span><span class="sxs-lookup"><span data-stu-id="fd002-119">Field</span></span>                     | <span data-ttu-id="fd002-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fd002-120">Description</span></span>                                                  |
| ------------------------- | ------------------------------------------------------------ |
| <span data-ttu-id="fd002-121">Использовать счет предоплаты</span><span class="sxs-lookup"><span data-stu-id="fd002-121">Use prepayment Account</span></span>    | <span data-ttu-id="fd002-122">Определяет, требуется ли учитывать предоплаты с помощью счета главной книги.</span><span class="sxs-lookup"><span data-stu-id="fd002-122">Specifies if you want to post prepayments using the general ledger account.</span></span> |
| <span data-ttu-id="fd002-123">Создание счета на предоплату</span><span class="sxs-lookup"><span data-stu-id="fd002-123">Create Prepayment Invoice</span></span> | <span data-ttu-id="fd002-124">Определяет, требуется ли создать счет на предоплату.</span><span class="sxs-lookup"><span data-stu-id="fd002-124">Specifies if you want to create an invoice for the prepayment.</span></span> |
| <span data-ttu-id="fd002-125">Серия номеров учт. предоплат</span><span class="sxs-lookup"><span data-stu-id="fd002-125">Posted Prepayment Nos.</span></span>    | <span data-ttu-id="fd002-126">Определяет серию номеров, из которой присваиваются номера новых записей.</span><span class="sxs-lookup"><span data-stu-id="fd002-126">Specifies the number series from which numbers are assigned to new records.</span></span> |
| <span data-ttu-id="fd002-127">Учт. разн. по предопл. - серия ном. док.</span><span class="sxs-lookup"><span data-stu-id="fd002-127">Posted PD Doc. Nos.</span></span>       | <span data-ttu-id="fd002-128">Определяет серию номеров, из которой присваиваются номера новых записей.</span><span class="sxs-lookup"><span data-stu-id="fd002-128">Specifies the number series from which numbers are assigned to new records.</span></span> |
| <span data-ttu-id="fd002-129">Разн. по предопл. - тип серии номеров док.</span><span class="sxs-lookup"><span data-stu-id="fd002-129">PD Doc. Nos. Type</span></span>         | <span data-ttu-id="fd002-130">Определяет, требуется ли использовать серию номеров или символ для идентификации операций транзакций предоплаты.</span><span class="sxs-lookup"><span data-stu-id="fd002-130">Specifies if you want to use a number series or symbol to identify prepayment transaction entries.</span></span> |
| <span data-ttu-id="fd002-131">Символ для док. разн. по предопл.</span><span class="sxs-lookup"><span data-stu-id="fd002-131">Symbol for PD Doc.</span></span>        | <span data-ttu-id="fd002-132">Определяет символ, который идентифицирует связанные операции предоплаты.</span><span class="sxs-lookup"><span data-stu-id="fd002-132">Specifies a symbol that identifies prepayment related entries.</span></span> |

## <a name="see-also"></a><span data-ttu-id="fd002-133">См. также</span><span class="sxs-lookup"><span data-stu-id="fd002-133">See Also</span></span>

[<span data-ttu-id="fd002-134">Функциональность локальной версии для России</span><span class="sxs-lookup"><span data-stu-id="fd002-134">Russia Local Functionality</span></span>](russia-local-functionality.md)  
