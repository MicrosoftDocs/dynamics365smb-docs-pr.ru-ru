---
title: Импорт данных о зарплате с помощью расширения "Зарплата Ceridian" | Microsoft Docs
description: Это расширение позволяет импортировать транзакции зарплаты из служб Ceridian HR/Payroll (США) и Ceridian PowerPay (Канада).
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, salary, wage
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 6bf5796a5e438995d039f2e40d7dbec3ccdc8cf1
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1250139"
---
# <a name="the-ceridian-payroll-extension"></a><span data-ttu-id="36b0f-103">Расширение зарплаты Ceridian</span><span class="sxs-lookup"><span data-stu-id="36b0f-103">The Ceridian Payroll Extension</span></span>
<span data-ttu-id="36b0f-104">Для учета выплаты зарплаты и связанных транзакций необходимо импортировать и учесть финансовые транзакции, сделанные поставщиком системы зарплаты, в главную книгу.</span><span class="sxs-lookup"><span data-stu-id="36b0f-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span>

<span data-ttu-id="36b0f-105">Чтобы это сделать, следует сначала импортировать файл, полученный от поставщика системы зарплаты, на страницу **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="36b0f-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** page.</span></span> <span data-ttu-id="36b0f-106">Затем следует сопоставить внешние счета в файле зарплаты с соответствующими счетами ГК.</span><span class="sxs-lookup"><span data-stu-id="36b0f-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="36b0f-107">Наконец требуется учесть транзакции зарплаты в соответствии с сопоставлением счетов.</span><span class="sxs-lookup"><span data-stu-id="36b0f-107">Lastly, you post the payroll transactions according to the account mapping.</span></span> <span data-ttu-id="36b0f-108">Дополнительные сведения см. в разделе [Импорт транзакций зарплаты](finance-how-import-payroll-transactions.md).</span><span class="sxs-lookup"><span data-stu-id="36b0f-108">For more information, see [Import Payroll Transactions](finance-how-import-payroll-transactions.md).</span></span>

<span data-ttu-id="36b0f-109">Расширение "Зарплата Ceridian" позволяет импортировать транзакции зарплаты из служб Ceridian HR/Payroll (США) и Ceridian PowerPay (Канада).</span><span class="sxs-lookup"><span data-stu-id="36b0f-109">The Ceridian Payroll extension allows you to import payroll transactions from the Ceridian HR/Payroll (US) and Ceridian PowerPay (Canada) services.</span></span>

## <a name="see-also"></a><span data-ttu-id="36b0f-110">См. также</span><span class="sxs-lookup"><span data-stu-id="36b0f-110">See Also</span></span>
<span data-ttu-id="36b0f-111">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="36b0f-111">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
<span data-ttu-id="36b0f-112">[Финансы](finance.md)  </span><span class="sxs-lookup"><span data-stu-id="36b0f-112">[Finance](finance.md)  </span></span>  
<span data-ttu-id="36b0f-113">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="36b0f-113">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
