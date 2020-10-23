---
title: Импорт данных о зарплате с помощью расширения "Зарплата Ceridian" | Документация Майкрософт
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
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 29dfaaa1cefe2bdc55fd68b1efd752be2c11cbc8
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3912357"
---
# <a name="the-ceridian-payroll-extension"></a><span data-ttu-id="72a6b-103">Расширение зарплаты Ceridian</span><span class="sxs-lookup"><span data-stu-id="72a6b-103">The Ceridian Payroll Extension</span></span>
<span data-ttu-id="72a6b-104">Для учета выплаты зарплаты и связанных транзакций необходимо импортировать и учесть финансовые транзакции, сделанные поставщиком системы зарплаты, в главную книгу.</span><span class="sxs-lookup"><span data-stu-id="72a6b-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span>

<span data-ttu-id="72a6b-105">Чтобы это сделать, следует сначала импортировать файл, полученный от поставщика системы зарплаты, на страницу **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="72a6b-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** page.</span></span> <span data-ttu-id="72a6b-106">Затем следует сопоставить внешние счета в файле зарплаты с соответствующими счетами ГК.</span><span class="sxs-lookup"><span data-stu-id="72a6b-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="72a6b-107">Наконец требуется учесть транзакции зарплаты в соответствии с сопоставлением счетов.</span><span class="sxs-lookup"><span data-stu-id="72a6b-107">Lastly, you post the payroll transactions according to the account mapping.</span></span> <span data-ttu-id="72a6b-108">Дополнительные сведения см. в разделе [Импорт транзакций зарплаты](finance-how-import-payroll-transactions.md).</span><span class="sxs-lookup"><span data-stu-id="72a6b-108">For more information, see [Import Payroll Transactions](finance-how-import-payroll-transactions.md).</span></span>

<span data-ttu-id="72a6b-109">Расширение "Зарплата Ceridian" позволяет импортировать транзакции зарплаты из служб Ceridian HR/Payroll (США) и Ceridian PowerPay (Канада).</span><span class="sxs-lookup"><span data-stu-id="72a6b-109">The Ceridian Payroll extension allows you to import payroll transactions from the Ceridian HR/Payroll (US) and Ceridian PowerPay (Canada) services.</span></span>

## <a name="see-also"></a><span data-ttu-id="72a6b-110">См. также</span><span class="sxs-lookup"><span data-stu-id="72a6b-110">See Also</span></span>
<span data-ttu-id="72a6b-111">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="72a6b-111">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
<span data-ttu-id="72a6b-112">[Финансы](finance.md)  </span><span class="sxs-lookup"><span data-stu-id="72a6b-112">[Finance](finance.md)  </span></span>  
<span data-ttu-id="72a6b-113">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="72a6b-113">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
