---
title: "Обновление валютных курсов | Документы Майкрософт"
description: "Для использования в бизнесе нескольких валют, можно настроить код по каждой используемой валюте и использовать внешний сервис валютного курса, например Yahoo."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, Yahoo
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: cc60569091b3aa37d17e981f1fae8f46c4a004df
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-update-currency-exchange-rates"></a><span data-ttu-id="6d37b-103">Практическое руководство. Обновление валютных курсов</span><span class="sxs-lookup"><span data-stu-id="6d37b-103">How to: Update Currency Exchange Rates</span></span>
<span data-ttu-id="6d37b-104">Следует настраивать код по каждой используемой валюте при покупке или продаже в валютах, отличных от местной валюты, при поступлениях или платежах в других валютах или при записи транзакций ГК в других валютах.</span><span class="sxs-lookup"><span data-stu-id="6d37b-104">You must set up a code for each currency you use if you buy or sell in currencies other than your local currency, have receivables or payables in other currencies, or record G/L transactions in different currencies.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="6d37b-105">Эта функция требует, чтобы было задано значение **Пакет**.</span><span class="sxs-lookup"><span data-stu-id="6d37b-105">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="6d37b-106">Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="6d37b-106">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

<span data-ttu-id="6d37b-107">Для обновления валютных курсов можно использовать внешнюю службу.</span><span class="sxs-lookup"><span data-stu-id="6d37b-107">You can use an external service to keep your currency exchange rates up to date.</span></span> <span data-ttu-id="6d37b-108">Служба валютных курсов Yahoo предустановлена и готова к использованию.</span><span class="sxs-lookup"><span data-stu-id="6d37b-108">The Yahoo Currency Exchange Rates service is preinstalled and ready to enable.</span></span>

## <a name="to-set-up-a-currency-exchange-rate-service"></a><span data-ttu-id="6d37b-109">Настройка служб валютных курсов</span><span class="sxs-lookup"><span data-stu-id="6d37b-109">To set up a currency exchange rate service</span></span>
1. <span data-ttu-id="6d37b-110">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Службы валютных курсов**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6d37b-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Currency Exchange Rate Services**, and then choose the related link.</span></span>
2. <span data-ttu-id="6d37b-111">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="6d37b-111">Choose the **New** action.</span></span>
3. <span data-ttu-id="6d37b-112">В окне **Служба валютных курсов** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="6d37b-112">In the **Currency Exchange Rate Service** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="6d37b-113">Установите флажок **Включено** для включения службы.</span><span class="sxs-lookup"><span data-stu-id="6d37b-113">Choose the **Enabled** check box to enable the service.</span></span>

## <a name="to-update-currency-exchange-rates-through-a-service"></a><span data-ttu-id="6d37b-114">Обновление валютных курсов с использованием службы</span><span class="sxs-lookup"><span data-stu-id="6d37b-114">To update currency exchange rates through a service</span></span>
1. <span data-ttu-id="6d37b-115">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Валюты**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6d37b-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Currencies**, and then choose the related link.</span></span>
2. <span data-ttu-id="6d37b-116">Выберите действие **Обновить валютные курсы**.</span><span class="sxs-lookup"><span data-stu-id="6d37b-116">Choose the **Update Exchange Rates** action.</span></span>

<span data-ttu-id="6d37b-117">Значение в поле **Валютный курс** в окне **Валюты** обновляется до самого актуального валютного курса.</span><span class="sxs-lookup"><span data-stu-id="6d37b-117">The value in the **Exchange Rate** field in the **Currencies** window is updated with the latest currency exchange rate.</span></span>

## <a name="see-also"></a><span data-ttu-id="6d37b-118">См. также</span><span class="sxs-lookup"><span data-stu-id="6d37b-118">See Also</span></span>
[<span data-ttu-id="6d37b-119">Закрытие года и периодов</span><span class="sxs-lookup"><span data-stu-id="6d37b-119">Closing Years and Periods</span></span>](year-close-years-periods.md)  
<span data-ttu-id="6d37b-120">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6d37b-120">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

