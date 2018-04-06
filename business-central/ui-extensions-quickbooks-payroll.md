---
title: "Использование расширение импорта файла зарплаты | Microsoft Docs"
description: "Описывает использование расширения для импорта транзакция по зарплате из службы Quickbooks Payroll."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, salary, wage
ms.date: 03/29/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 7e85ed50320089209c6bf66c45bc67801de5dbb6
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="the-quickbooks-payroll-file-import-extension-to-business-central"></a><span data-ttu-id="be0a6-103">Расширения импорта файла зарплаты Quickbooks в Business Central</span><span class="sxs-lookup"><span data-stu-id="be0a6-103">The Quickbooks Payroll File Import Extension to Business Central</span></span> 
<span data-ttu-id="be0a6-104">Для учета выплаты зарплаты и связанных транзакций необходимо импортировать и учесть финансовые транзакции, сделанные поставщиком системы зарплаты, в главную книгу.</span><span class="sxs-lookup"><span data-stu-id="be0a6-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span>

<span data-ttu-id="be0a6-105">Чтобы это сделать, следует сначала импортировать файл, полученный от поставщика системы зарплаты, в окно **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="be0a6-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="be0a6-106">Затем следует сопоставить внешние счета в файле зарплаты с соответствующими счетами ГК.</span><span class="sxs-lookup"><span data-stu-id="be0a6-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="be0a6-107">Наконец требуется учесть транзакции зарплаты в соответствии с сопоставлением счетов.</span><span class="sxs-lookup"><span data-stu-id="be0a6-107">Lastly, you post the payroll transactions according to the account mapping.</span></span> <span data-ttu-id="be0a6-108">Дополнительные сведения см. в разделе [Импорт транзакций зарплаты](finance-how-import-payroll-transactions.md).</span><span class="sxs-lookup"><span data-stu-id="be0a6-108">For more information, see [Import Payroll Transactions](finance-how-import-payroll-transactions.md).</span></span>

<span data-ttu-id="be0a6-109">Расширение импорта файла зарплаты Quickbooks позволяет импортировать транзакции зарплаты из службы зарплаты Quickbooks.</span><span class="sxs-lookup"><span data-stu-id="be0a6-109">The Quickbooks Payroll File Import extension allows you to import payroll transaction from the Quickbooks Payroll service.</span></span>

## <a name="see-also"></a><span data-ttu-id="be0a6-110">См. также</span><span class="sxs-lookup"><span data-stu-id="be0a6-110">See Also</span></span>
<span data-ttu-id="be0a6-111">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="be0a6-111">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
<span data-ttu-id="be0a6-112">[Финансы](finance.md)  </span><span class="sxs-lookup"><span data-stu-id="be0a6-112">[Finance](finance.md)  </span></span>  
<span data-ttu-id="be0a6-113">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="be0a6-113">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

