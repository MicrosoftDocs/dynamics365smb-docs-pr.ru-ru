---
title: "Использование расширения импорта файла зарплаты QuickBooks | Документы Майкрософт"
description: "В этом разделе описывается использование расширения для импорта транзакция по зарплате из Quickbooks."
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, salary, wage
ms.date: 01/09/2019
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 79729b42b660399893aebe1116c80ef3b3209042
ms.openlocfilehash: ac68f8a4d67224ad55b1c34ff9b2e4ffa2c372aa
ms.contentlocale: ru-ru
ms.lasthandoff: 01/15/2019

---
# <a name="the-quickbooks-payroll-file-import-extension"></a><span data-ttu-id="59675-103">Расширение импорта файла зарплаты QuickBooks</span><span class="sxs-lookup"><span data-stu-id="59675-103">The QuickBooks Payroll File Import Extension</span></span>
<span data-ttu-id="59675-104">Используйте расширение импорта файла зарплаты QuickBooks для импорта транзакций зарплаты из QuickBooks в счета главной книги в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="59675-104">Use the QuickBooks Payroll File Import extension to import payroll transactions from QuickBooks to general ledger accounts in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="59675-105">Например, это может оказаться полезным при переходе с QuickBooks в [!INCLUDE[d365fin](includes/d365fin_md.md)] или если используются сторонние услуги расчета зарплаты, но вы хотите отслеживать зарплату в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="59675-105">For example, this is useful when you are transitioning from QuickBooks to [!INCLUDE[d365fin](includes/d365fin_md.md)], or if you outsource your payroll but also want to keep track of it in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="steps-to-import-payroll-data"></a><span data-ttu-id="59675-106">Действия для импорта данных по зарплате</span><span class="sxs-lookup"><span data-stu-id="59675-106">Steps to Import Payroll Data</span></span>
<span data-ttu-id="59675-107">Первым шагом вы или, возможно, ваш бухгалтер, должны использовать функции экспорта в QuickBooks для экспорта данных зарплаты в файл IIF.</span><span class="sxs-lookup"><span data-stu-id="59675-107">The first step is for you, or maybe your accountant, to use the export features in QuickBooks to export the payroll data to an .IIF file.</span></span> <span data-ttu-id="59675-108">На втором шаге необходимо открыть страницу **Финансовые журналы** в [!INCLUDE[d365fin](includes/d365fin_md.md)] и использовании действие **Импорт транзакций на зарплату** для импорта файла.</span><span class="sxs-lookup"><span data-stu-id="59675-108">The second step is to open the **General Journals** page in [!INCLUDE[d365fin](includes/d365fin_md.md)] and use the **Import Payroll Transactions** action to import the file.</span></span> <span data-ttu-id="59675-109">Во время процесса импорта можно сопоставить счета главной книги из QuickBooks с соответствующими счетами в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="59675-109">During the import process you map the general ledger accounts from QuickBooks to corresponding accounts in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="59675-110">Последний шаг — это учет транзакции зарплаты в [!INCLUDE[d365fin](includes/d365fin_md.md)] в соответствии с сопоставлением счетов.</span><span class="sxs-lookup"><span data-stu-id="59675-110">The final step is to post the payroll transactions in [!INCLUDE[d365fin](includes/d365fin_md.md)] according to the account mapping.</span></span> 

<span data-ttu-id="59675-111">Дополнительные сведения см. в разделе [Импорт транзакций зарплаты](finance-how-import-payroll-transactions.md).</span><span class="sxs-lookup"><span data-stu-id="59675-111">For more information, see [Import Payroll Transactions](finance-how-import-payroll-transactions.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="59675-112">См. также</span><span class="sxs-lookup"><span data-stu-id="59675-112">See Also</span></span>
<span data-ttu-id="59675-113">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="59675-113">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
<span data-ttu-id="59675-114">[Финансы](finance.md)  </span><span class="sxs-lookup"><span data-stu-id="59675-114">[Finance](finance.md)  </span></span>  
<span data-ttu-id="59675-115">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="59675-115">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

