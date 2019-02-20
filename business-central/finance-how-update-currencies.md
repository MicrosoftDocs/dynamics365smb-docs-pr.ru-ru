---
title: "Обновление валютных курсов | Документы Майкрософт"
description: "Для использования в бизнесе нескольких валют, можно настроить код по каждой используемой валюте и использовать внешний сервис валютного курса."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies
ms.date: 12/19/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: aa1e7b13cf6cc56df1a6922a9b123e7cc19580c6
ms.openlocfilehash: 7fafae0cba12ba985de2faa795b434d4c670a8ca
ms.contentlocale: ru-ru
ms.lasthandoff: 12/19/2018

---
# <a name="update-currency-exchange-rates"></a><span data-ttu-id="3d7cd-103">Обновление валютных курсов</span><span class="sxs-lookup"><span data-stu-id="3d7cd-103">Update Currency Exchange Rates</span></span>
<span data-ttu-id="3d7cd-104">Поскольку сфера действия организаций включает все новые и новые страны и регионы, растет необходимость в торговле и составлении финансовых отчетов в нескольких валютах.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-104">As companies operate in increasingly more countries/regions, it becomes more important that they be able to trade and report financials in more than one currency.</span></span> <span data-ttu-id="3d7cd-105">Следует настраивать код по каждой используемой валюте при покупке или продаже в валютах, отличных от местной валюты, при поступлениях или платежах в других валютах или при записи транзакций ГК в других валютах.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-105">You must set up a code for each currency you use if you buy or sell in currencies other than your local currency, have receivables or payables in other currencies, or record G/L transactions in different currencies.</span></span>

<span data-ttu-id="3d7cd-106">Главная книга настраивается на использование локальной валюты (руб.), но можно также задать использование другой валюты с назначением текущего валютного курса.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-106">Your general ledger is set up to use your local currency (LCY), but you can set it up to also use another currency with a current exchange rate assigned.</span></span> <span data-ttu-id="3d7cd-107">В случае указания второй валюты в качестве так называемой дополнительной валюты отчетности [!INCLUDE[d365fin](includes/d365fin_md.md)] будет автоматически регистрировать суммы как в рублях, так и в дополнительной валюте по каждой операции в ГК и в других операциях, таких как операции НДС.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-107">By designating a second currency as a so-called additional reporting currency, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically record amounts in both LCY and this additional reporting currency on each G/L entry and other entries, such as VAT entries.</span></span> <span data-ttu-id="3d7cd-108">Дополнительные сведения см. в разделе [Настройка дополнительной отчетной валюты](finance-how-setup-additional-currencies.md).</span><span class="sxs-lookup"><span data-stu-id="3d7cd-108">For more information, see [Set Up an Additional Reporting Currency](finance-how-setup-additional-currencies.md).</span></span>

## <a name="adjusting-exchange-rates"></a><span data-ttu-id="3d7cd-109">Коррекция валютных курсов</span><span class="sxs-lookup"><span data-stu-id="3d7cd-109">Adjusting Exchange Rates</span></span>
<span data-ttu-id="3d7cd-110">В связи с постоянным колебанием курсов валют, возникает необходимость в периодической корректировке дополнительной валюты.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-110">Because exchange rates fluctuate constantly, additional currency equivalents in your system must be adjusted periodically.</span></span> <span data-ttu-id="3d7cd-111">Если данные корректировки не будут производиться, суммы, конвертированные из иностранных (или дополнительных) валют и разнесенные в главной книге в рублях, могут оказаться неточными.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-111">If these adjustments are not done, amounts that have been converted from foreign (or additional) currencies and posted to the general ledger in LCY may be misleading.</span></span> <span data-ttu-id="3d7cd-112">К тому же, ежедневные операции, учтенные до момента ввода ежедневного курса валют, следует обновлять после ввода информации о ежедневном курсе валют.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-112">In addition, daily entries posted before a daily exchange rate is entered into the program must be updated after the daily exchange rate information is entered.</span></span> <span data-ttu-id="3d7cd-113">Пакетное задание Коррекция валютных курсов используется для корректировки курсов валют учтенных операций по клиентам, поставщикам и банковским счетам.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-113">The Adjust Exchange Rates batch job is used to adjust the exchange rates of posted customer, vendor and bank account entries.</span></span> <span data-ttu-id="3d7cd-114">Также может быть выполнена корректировка сумм в дополнительной отчетной валюте в операциях ГК.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-114">It can also update additional reporting currency amounts on G/L entries.</span></span>

## <a name="to-set-up-a-currency-exchange-rate-service"></a><span data-ttu-id="3d7cd-115">Настройка служб валютных курсов</span><span class="sxs-lookup"><span data-stu-id="3d7cd-115">To set up a currency exchange rate service</span></span>
<span data-ttu-id="3d7cd-116">Для обновления валютных курсов можно использовать внешнюю службу, например FloatRates.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-116">You can use an external service to keep your currency exchange rates up to date, such as FloatRates.</span></span>

1. <span data-ttu-id="3d7cd-117">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Службы валютных курсов**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currency Exchange Rate Services**, and then choose the related link.</span></span>
2. <span data-ttu-id="3d7cd-118">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-118">Choose the **New** action.</span></span>
3. <span data-ttu-id="3d7cd-119">На странице **Служба валютных курсов** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-119">On the **Currency Exchange Rate Service** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="3d7cd-120">Установите флажок **Включено** для включения службы.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-120">Choose the **Enabled** check box to enable the service.</span></span>

## <a name="to-update-currency-exchange-rates-through-a-service"></a><span data-ttu-id="3d7cd-121">Обновление валютных курсов с использованием службы</span><span class="sxs-lookup"><span data-stu-id="3d7cd-121">To update currency exchange rates through a service</span></span>
1. <span data-ttu-id="3d7cd-122">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Валюты**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currencies**, and then choose the related link.</span></span>
2. <span data-ttu-id="3d7cd-123">Выберите действие **Обновить валютные курсы**.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-123">Choose the **Update Exchange Rates** action.</span></span>

<span data-ttu-id="3d7cd-124">Значение в поле **Валютный курс** на странице **Валюты** обновляется до самого актуального валютного курса.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-124">The value in the **Exchange Rate** field on the **Currencies** page is updated with the latest currency exchange rate.</span></span>

## <a name="see-also"></a><span data-ttu-id="3d7cd-125">См. также</span><span class="sxs-lookup"><span data-stu-id="3d7cd-125">See Also</span></span>
[<span data-ttu-id="3d7cd-126">Настройка дополнительной отчетной валюты</span><span class="sxs-lookup"><span data-stu-id="3d7cd-126">Set Up an Additional Reporting Currency</span></span>](finance-how-setup-additional-currencies.md)  
[<span data-ttu-id="3d7cd-127">Закрытие года и периодов</span><span class="sxs-lookup"><span data-stu-id="3d7cd-127">Closing Years and Periods</span></span>](year-close-years-periods.md)  
<span data-ttu-id="3d7cd-128">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3d7cd-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

