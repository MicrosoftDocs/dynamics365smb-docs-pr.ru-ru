---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 95121642b62f33ea1fc160c103ee845816706530
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5778651"
---
<span data-ttu-id="4150b-101">Если все товары введены как строки, можно вычислить скидку по счету для документа продажи в целом, выбрав действие **Вычислить скидку по счету**.</span><span class="sxs-lookup"><span data-stu-id="4150b-101">When all the items have been entered as lines, you can calculate the invoice discount for the entire sales document by choosing the **Calculate Invoice Discount** action.</span></span>

<span data-ttu-id="4150b-102">Скидка рассчитывается по всем строкам документа продажи для товаров, в которых поле **Разрешить скидку по счету** в строке заказа на продажу содержит **Да**.</span><span class="sxs-lookup"><span data-stu-id="4150b-102">The discount is calculated based on all the lines in the sales document for items where the **Allow Invoice Disc.** field on the sales order line contains **Yes**.</span></span> <span data-ttu-id="4150b-103">Это настройка по умолчанию для товаров.</span><span class="sxs-lookup"><span data-stu-id="4150b-103">This is the default setting for items.</span></span> <span data-ttu-id="4150b-104">Например, строки с товарными издержками не включаются в расчет скидки по счету.</span><span class="sxs-lookup"><span data-stu-id="4150b-104">Lines with item charges, for example, are not included in the calculation of the invoice discount.</span></span> <span data-ttu-id="4150b-105">Если вы хотите применить скидку к таким строкам, вы должны установить поле **Скидка строки (%)** в соответствующих строках.</span><span class="sxs-lookup"><span data-stu-id="4150b-105">If you want to apply a discount to such lines, you must set the **Line Discount %** field on the relevant lines.</span></span>  

> [!TIP]
> <span data-ttu-id="4150b-106">Если поле **Расчет скидки по счету** выбрано на странице **Настройка продаж и расчетов с клиентами**, то скидка вычисляется автоматически, если выполнено одно из перечисленных ниже действий в документе по продаже:</span><span class="sxs-lookup"><span data-stu-id="4150b-106">If the **Calc. Inv. Discount** field is selected in the **Sales and Receivables Setup** page, then the invoice discount is calculated automatically when you do either of the following on a sales document:</span></span>
>
> * <span data-ttu-id="4150b-107">Просмотр статистики</span><span class="sxs-lookup"><span data-stu-id="4150b-107">View statistics</span></span>
> * <span data-ttu-id="4150b-108">Просмотр тестового отчета</span><span class="sxs-lookup"><span data-stu-id="4150b-108">View a test report</span></span>
> * <span data-ttu-id="4150b-109">Печать</span><span class="sxs-lookup"><span data-stu-id="4150b-109">Print</span></span>
> * <span data-ttu-id="4150b-110">Почта</span><span class="sxs-lookup"><span data-stu-id="4150b-110">Post</span></span>

<span data-ttu-id="4150b-111">Условия предоставления скидки для клиента задаются на странице **Клиент — скидки по счету** для клиента.</span><span class="sxs-lookup"><span data-stu-id="4150b-111">The invoice discount terms for a customer are defined in the **Cust. Invoice Discounts** page for the customer.</span></span> <span data-ttu-id="4150b-112">Код валюты в документе продажи используется для поиска условий предоставления скидки по счету в соответствующей валюте.</span><span class="sxs-lookup"><span data-stu-id="4150b-112">The currency code on the sales document is used to find the invoice discount terms in the corresponding currency.</span></span>

<span data-ttu-id="4150b-113">Если скидки по счету не определены для иностранных валют, то будут использоваться условия скидки для счета, определенные на странице **Клиент - скидки счета** с суммами в местной валюте, и валютный курс на дату учета в документе продажи используется для расчета скидки по счету в иностранной валюте.</span><span class="sxs-lookup"><span data-stu-id="4150b-113">If invoice discounts have not been defined for foreign currencies, then the invoice discount terms defined in the **Cust. Invoice Discounts** page with amounts in your local currency and the exchange rate on the posting date on the sales document are used to calculate the invoice discount in the foreign currency.</span></span>
