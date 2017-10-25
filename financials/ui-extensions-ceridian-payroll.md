---
title: "Импорт данных о зарплате с помощью расширения \"Зарплата Ceridian\" | Документы Майкрософт"
description: "Это расширение позволяет импортировать транзакции зарплаты из служб Ceridian HR/Payroll (США) и Ceridian PowerPay (Канада)."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, salary, wage
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 18b1dcd66b6816adc9fcb8b86d4f55834f51fd02
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="the-ceridian-payroll-extension-to-dynamics-365-for-financials"></a><span data-ttu-id="130c9-103">Расширение "Зарплата Ceridian" для Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="130c9-103">The Ceridian Payroll Extension to Dynamics 365 for Financials</span></span>
<span data-ttu-id="130c9-104">Для учета выплаты зарплаты и связанных транзакций необходимо импортировать и учесть финансовые транзакции, сделанные поставщиком системы зарплаты, в главную книгу.</span><span class="sxs-lookup"><span data-stu-id="130c9-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span>

<span data-ttu-id="130c9-105">Чтобы это сделать, следует сначала импортировать файл, полученный от поставщика системы зарплаты, в окно **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="130c9-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="130c9-106">Затем следует сопоставить внешние счета в файле зарплаты с соответствующими счетами ГК.</span><span class="sxs-lookup"><span data-stu-id="130c9-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="130c9-107">Наконец требуется учесть транзакции зарплаты в соответствии с сопоставлением счетов.</span><span class="sxs-lookup"><span data-stu-id="130c9-107">Lastly, you post the payroll transactions according to the account mapping.</span></span> <span data-ttu-id="130c9-108">Дополнительные сведения см. в разделе [Практическое руководство. Импорт транзакций зарплаты](finance-how-import-payroll-transactions.md).</span><span class="sxs-lookup"><span data-stu-id="130c9-108">For more information, see [How to: Import Payroll Transactions](finance-how-import-payroll-transactions.md).</span></span>

<span data-ttu-id="130c9-109">Расширение "Зарплата Ceridian" позволяет импортировать транзакции зарплаты из служб Ceridian HR/Payroll (США) и Ceridian PowerPay (Канада).</span><span class="sxs-lookup"><span data-stu-id="130c9-109">The Ceridian Payroll extension allows you to import payroll transactions from the Ceridian HR/Payroll (US) and Ceridian PowerPay (Canada) services.</span></span>

## <a name="see-also"></a><span data-ttu-id="130c9-110">См. также</span><span class="sxs-lookup"><span data-stu-id="130c9-110">See Also</span></span>
<span data-ttu-id="130c9-111">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="130c9-111">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
<span data-ttu-id="130c9-112">[Финансы](finance.md)  </span><span class="sxs-lookup"><span data-stu-id="130c9-112">[Finance](finance.md)  </span></span>  
<span data-ttu-id="130c9-113">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="130c9-113">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

