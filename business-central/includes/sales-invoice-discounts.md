---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 01/20/2021
ms.author: edupont
ms.openlocfilehash: 718845561c1a18701d20b93ebdc8339308ce7ac8
ms.sourcegitcommit: adf1a87a677b8197c68bb28c44b7a58250d6fc51
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2021
ms.locfileid: "5035793"
---
<span data-ttu-id="fe88e-101">Если все товары введены в строки заказа на продажу, можно вычислить скидку по счету для документа продажи в целом, выбрав действие **Вычислить скидку по счету**.</span><span class="sxs-lookup"><span data-stu-id="fe88e-101">When all the items have been entered on the sales order lines, you can calculate the invoice discount for the entire sales document by choosing the **Calculate Invoice Discount** action.</span></span>

<span data-ttu-id="fe88e-102">Если поле **Расчет скидки по счету** выбрано в окне **Настройка продаж и расчетов с клиентами**, то скидка вычисляется автоматически, если выполнено одно из перечисленных ниже действий в документе по продаже:</span><span class="sxs-lookup"><span data-stu-id="fe88e-102">If the **Calc. Inv. Discount** field is selected in the **Sales and Receivables Setup** window, then the invoice discount is calculated automatically when you do either of the following on a sales document:</span></span>

* <span data-ttu-id="fe88e-103">Просмотр статистики</span><span class="sxs-lookup"><span data-stu-id="fe88e-103">View statistics</span></span>
* <span data-ttu-id="fe88e-104">Просмотр тестового отчета</span><span class="sxs-lookup"><span data-stu-id="fe88e-104">View a test report</span></span>
* <span data-ttu-id="fe88e-105">Печать</span><span class="sxs-lookup"><span data-stu-id="fe88e-105">Print</span></span>
* <span data-ttu-id="fe88e-106">Почта</span><span class="sxs-lookup"><span data-stu-id="fe88e-106">Post</span></span>

<span data-ttu-id="fe88e-107">Скидка должна соразмерно распределяться по всем строкам документа продажи для товаров, в которых поле **Разрешить скидку по счету** в строке заказа на продажу содержит **Да**.</span><span class="sxs-lookup"><span data-stu-id="fe88e-107">The discount is apportioned over all the lines in the sales document for items where the **Allow Invoice Disc.** field on the sales order line contains **Yes**.</span></span> <span data-ttu-id="fe88e-108">Это настройка по умолчанию для товаров.</span><span class="sxs-lookup"><span data-stu-id="fe88e-108">This is the default setting for items.</span></span>

<span data-ttu-id="fe88e-109">Определены условия предоставления скидки по счету на странице **Клиент - скидки по счету** для вычисления скидки по счету.</span><span class="sxs-lookup"><span data-stu-id="fe88e-109">The invoice discount terms are defined in the **Cust. Invoice Discounts** page to calculate the invoice discount.</span></span> <span data-ttu-id="fe88e-110">Код валюты в документе продажи используется для поиска условий предоставления скидки по счету в соответствующей валюте.</span><span class="sxs-lookup"><span data-stu-id="fe88e-110">The currency code on the sales document is used to find the invoice discount terms in the corresponding currency.</span></span>

<span data-ttu-id="fe88e-111">Если скидки по счету не определены для иностранных валют, то будут использоваться условия скидки для счета, определенные на странице **Клиент - скидки счета** с суммами в местной валюте, и валютный курс на дату учета в документе продажи используется для расчета скидки по счету в иностранной валюте.</span><span class="sxs-lookup"><span data-stu-id="fe88e-111">If invoice discounts have not been defined for foreign currencies, then the invoice discount terms defined in the **Cust. Invoice Discounts** page with amounts in your local currency and the exchange rate on the posting date on the sales document are used to calculate the invoice discount in the foreign currency.</span></span>
