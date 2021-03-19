---
title: Использование расширения импорта файла зарплаты QuickBooks | Документация Майкрософт
description: В этом разделе описывается использование расширения для импорта транзакция по зарплате из Quickbooks.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, salary, wage
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: fc8767f1e6a33f957b33f9076a8cee485b2f1412
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5386378"
---
# <a name="the-quickbooks-payroll-file-import-extension"></a><span data-ttu-id="4b3c0-103">Расширение импорта файла зарплаты QuickBooks</span><span class="sxs-lookup"><span data-stu-id="4b3c0-103">The QuickBooks Payroll File Import Extension</span></span>
<span data-ttu-id="4b3c0-104">Используйте расширение импорта файла зарплаты QuickBooks для импорта транзакций зарплаты из QuickBooks в счета главной книги в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="4b3c0-104">Use the QuickBooks Payroll File Import extension to import payroll transactions from QuickBooks to general ledger accounts in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="4b3c0-105">Например, это может оказаться полезным при переходе с QuickBooks в [!INCLUDE[prod_short](includes/prod_short.md)] или если используются сторонние услуги расчета зарплаты, но вы хотите отслеживать зарплату в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="4b3c0-105">For example, this is useful when you are transitioning from QuickBooks to [!INCLUDE[prod_short](includes/prod_short.md)], or if you outsource your payroll but also want to keep track of it in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

## <a name="steps-to-import-payroll-data"></a><span data-ttu-id="4b3c0-106">Действия для импорта данных по зарплате</span><span class="sxs-lookup"><span data-stu-id="4b3c0-106">Steps to Import Payroll Data</span></span>
<span data-ttu-id="4b3c0-107">Первым шагом вы или, возможно, ваш бухгалтер, должны использовать функции экспорта в QuickBooks для экспорта данных зарплаты в файл IIF.</span><span class="sxs-lookup"><span data-stu-id="4b3c0-107">The first step is for you, or maybe your accountant, to use the export features in QuickBooks to export the payroll data to an .IIF file.</span></span> <span data-ttu-id="4b3c0-108">На втором шаге необходимо открыть страницу **Финансовые журналы** в [!INCLUDE[prod_short](includes/prod_short.md)] и использовании действие **Импорт транзакций на зарплату** для импорта файла.</span><span class="sxs-lookup"><span data-stu-id="4b3c0-108">The second step is to open the **General Journals** page in [!INCLUDE[prod_short](includes/prod_short.md)] and use the **Import Payroll Transactions** action to import the file.</span></span> <span data-ttu-id="4b3c0-109">Во время процесса импорта можно сопоставить счета главной книги из QuickBooks с соответствующими счетами в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="4b3c0-109">During the import process you map the general ledger accounts from QuickBooks to corresponding accounts in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="4b3c0-110">Последний шаг — это учет транзакции зарплаты в [!INCLUDE[prod_short](includes/prod_short.md)] в соответствии с сопоставлением счетов.</span><span class="sxs-lookup"><span data-stu-id="4b3c0-110">The final step is to post the payroll transactions in [!INCLUDE[prod_short](includes/prod_short.md)] according to the account mapping.</span></span> 

<span data-ttu-id="4b3c0-111">Дополнительные сведения см. в разделе [Импорт транзакций зарплаты](finance-how-import-payroll-transactions.md).</span><span class="sxs-lookup"><span data-stu-id="4b3c0-111">For more information, see [Import Payroll Transactions](finance-how-import-payroll-transactions.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="4b3c0-112">См. также</span><span class="sxs-lookup"><span data-stu-id="4b3c0-112">See Also</span></span>
<span data-ttu-id="4b3c0-113">[Настройка [!INCLUDE[prod_short](includes/prod_short.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="4b3c0-113">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions ](ui-extensions.md)  </span></span>  
<span data-ttu-id="4b3c0-114">[Финансы](finance.md)  </span><span class="sxs-lookup"><span data-stu-id="4b3c0-114">[Finance](finance.md)  </span></span>  
<span data-ttu-id="4b3c0-115">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4b3c0-115">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]