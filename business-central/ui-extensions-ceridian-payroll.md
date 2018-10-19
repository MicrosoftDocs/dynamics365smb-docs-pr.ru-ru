---
title: "Импорт данных о зарплате с помощью расширения \"Зарплата Ceridian\" | Microsoft Docs"
description: "Это расширение позволяет импортировать транзакции зарплаты из служб Ceridian HR/Payroll (США) и Ceridian PowerPay (Канада)."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, salary, wage
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 7df17702abafd834976527978f1caadffb590ab4
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="the-ceridian-payroll-extension"></a><span data-ttu-id="be9ee-103">Расширение зарплаты Ceridian</span><span class="sxs-lookup"><span data-stu-id="be9ee-103">The Ceridian Payroll Extension</span></span>
<span data-ttu-id="be9ee-104">Для учета выплаты зарплаты и связанных транзакций необходимо импортировать и учесть финансовые транзакции, сделанные поставщиком системы зарплаты, в главную книгу.</span><span class="sxs-lookup"><span data-stu-id="be9ee-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span>

<span data-ttu-id="be9ee-105">Чтобы это сделать, следует сначала импортировать файл, полученный от поставщика системы зарплаты, в окно **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="be9ee-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="be9ee-106">Затем следует сопоставить внешние счета в файле зарплаты с соответствующими счетами ГК.</span><span class="sxs-lookup"><span data-stu-id="be9ee-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="be9ee-107">Наконец требуется учесть транзакции зарплаты в соответствии с сопоставлением счетов.</span><span class="sxs-lookup"><span data-stu-id="be9ee-107">Lastly, you post the payroll transactions according to the account mapping.</span></span> <span data-ttu-id="be9ee-108">Дополнительные сведения см. в разделе [Импорт транзакций зарплаты](finance-how-import-payroll-transactions.md).</span><span class="sxs-lookup"><span data-stu-id="be9ee-108">For more information, see [Import Payroll Transactions](finance-how-import-payroll-transactions.md).</span></span>

<span data-ttu-id="be9ee-109">Расширение "Зарплата Ceridian" позволяет импортировать транзакции зарплаты из служб Ceridian HR/Payroll (США) и Ceridian PowerPay (Канада).</span><span class="sxs-lookup"><span data-stu-id="be9ee-109">The Ceridian Payroll extension allows you to import payroll transactions from the Ceridian HR/Payroll (US) and Ceridian PowerPay (Canada) services.</span></span>

## <a name="see-also"></a><span data-ttu-id="be9ee-110">См. также</span><span class="sxs-lookup"><span data-stu-id="be9ee-110">See Also</span></span>
<span data-ttu-id="be9ee-111">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="be9ee-111">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
<span data-ttu-id="be9ee-112">[Финансы](finance.md)  </span><span class="sxs-lookup"><span data-stu-id="be9ee-112">[Finance](finance.md)  </span></span>  
<span data-ttu-id="be9ee-113">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="be9ee-113">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

