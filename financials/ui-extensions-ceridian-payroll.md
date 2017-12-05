---
title: "Импорт данных о зарплате с помощью расширения \"Зарплата Ceridian\" | Microsoft Docs"
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
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 3c67d6bd4d24d5b58462fa05168f2ac764b2c695
ms.contentlocale: ru-ru
ms.lasthandoff: 11/10/2017

---
# <a name="the-ceridian-payroll-extension-to-dynamics-365-business-edition"></a><span data-ttu-id="23b78-103">Расширение "Зарплата Ceridian" для Dynamics 365 Business edition</span><span class="sxs-lookup"><span data-stu-id="23b78-103">The Ceridian Payroll Extension to Dynamics 365 Business edition</span></span> 
<span data-ttu-id="23b78-104">Для учета выплаты зарплаты и связанных транзакций необходимо импортировать и учесть финансовые транзакции, сделанные поставщиком системы зарплаты, в главную книгу.</span><span class="sxs-lookup"><span data-stu-id="23b78-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span>

<span data-ttu-id="23b78-105">Чтобы это сделать, следует сначала импортировать файл, полученный от поставщика системы зарплаты, в окно **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="23b78-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="23b78-106">Затем следует сопоставить внешние счета в файле зарплаты с соответствующими счетами ГК.</span><span class="sxs-lookup"><span data-stu-id="23b78-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="23b78-107">Наконец требуется учесть транзакции зарплаты в соответствии с сопоставлением счетов.</span><span class="sxs-lookup"><span data-stu-id="23b78-107">Lastly, you post the payroll transactions according to the account mapping.</span></span> <span data-ttu-id="23b78-108">Дополнительные сведения см. в разделе [Практическое руководство. Импорт транзакций зарплаты](finance-how-import-payroll-transactions.md).</span><span class="sxs-lookup"><span data-stu-id="23b78-108">For more information, see [How to: Import Payroll Transactions](finance-how-import-payroll-transactions.md).</span></span>

<span data-ttu-id="23b78-109">Расширение "Зарплата Ceridian" позволяет импортировать транзакции зарплаты из служб Ceridian HR/Payroll (США) и Ceridian PowerPay (Канада).</span><span class="sxs-lookup"><span data-stu-id="23b78-109">The Ceridian Payroll extension allows you to import payroll transactions from the Ceridian HR/Payroll (US) and Ceridian PowerPay (Canada) services.</span></span>

## <a name="see-also"></a><span data-ttu-id="23b78-110">См. также</span><span class="sxs-lookup"><span data-stu-id="23b78-110">See Also</span></span>
<span data-ttu-id="23b78-111">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="23b78-111">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
<span data-ttu-id="23b78-112">[Финансы](finance.md)  </span><span class="sxs-lookup"><span data-stu-id="23b78-112">[Finance](finance.md)  </span></span>  
<span data-ttu-id="23b78-113">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="23b78-113">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

