---
title: Настройка отчетов и печать на конкретных принтерах | Документы Майкрософт
description: Узнайте о том, как задать принтер для отчета и использовать страница "Выбор принтера".
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online printing
ms.date: 10/01/2018
ms.author: solsen
ms.openlocfilehash: bc3a7ab7a61e7a51a58494c3f5892c22b6867333
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "804899"
---
# <a name="specify-printer-selection-for-reports"></a><span data-ttu-id="7177c-103">Выбор принтера для отчета</span><span class="sxs-lookup"><span data-stu-id="7177c-103">Specify Printer Selection for Reports</span></span>
<span data-ttu-id="7177c-104">Эта страница пустая, поскольку еще невозможно настроить определенные принтеры для конкретных отчетов.</span><span class="sxs-lookup"><span data-stu-id="7177c-104">This page is empty because you cannot yet set up specific printers for specific reports.</span></span> <span data-ttu-id="7177c-105">Мы работаем над разрешением этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="7177c-105">We are working on solving this.</span></span>

<span data-ttu-id="7177c-106">Между тем, если вам требуется напечатать отчет, вам следует сначала загрузить отчет как PDF-документ, нажав кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="7177c-106">In the meantime, when you want to print a report, you have to download the report as a PDF document first by choosing the **Send to** button.</span></span> <span data-ttu-id="7177c-107">Затем выберите тип файла для загрузки отчета, в данном случае — **Документ PDF**.</span><span class="sxs-lookup"><span data-stu-id="7177c-107">Then you select the type of file to download the report as, and here you should pick **PDF Document**.</span></span> <span data-ttu-id="7177c-108">Теперь можно либо открыть PDF-документ сразу же и напечатать его, либо сохранить документ и напечатать его позже.</span><span class="sxs-lookup"><span data-stu-id="7177c-108">Now, you can either open the PDF document right-away and print it, or save it and print it later.</span></span>

<!--

You can set up reports so that they must be printed on a specific printer. The following are some uses of printer selection:

- You can print reports on special company letterhead.
- You can print reports on different paper sizes.
- You can print reports on the default printer of a specified employee.

You use the **Printer Selections** page to set different values to obtain different output. If you set a specific printer selection, then it takes precedence over a more general printer selection. For example, you can set a printer selection that has values in the **User ID**, **Report ID**, and **Printer Name** fields. This printer selection takes precedence over a printer selection that has blank entries in the **User ID** or **Report ID** fields.

The following table describes the combination of values to specify when you set up printer selections for a report.

|To                                                 |Set the following values                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|Print a report to a specific printer for all users |Specify values in the **Report ID** and **Printer Name** fields and leave the **User ID** field blank.|
|Print all reports to a specific printer for a specific user|Specify values in the **User ID** and **Printer Name** fields and leave the **Report ID** field blank.|
|Set the default printer for all reports|Specify a value in the **Printer Name** field and leave the **User ID** and **Report ID** fields blank.|
|Print a specific report to the user’s default printer|Specify a value in the **Report ID** field and leave the **Printer Name** and **User ID** fields blank.|
|Print a specific report to a specific printer for a specific user|Specify values in all three fields.|
-->

## <a name="see-also"></a><span data-ttu-id="7177c-109">См. также</span><span class="sxs-lookup"><span data-stu-id="7177c-109">See Also</span></span>
<span data-ttu-id="7177c-110">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7177c-110">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="7177c-111">Запуск пакетных заданий</span><span class="sxs-lookup"><span data-stu-id="7177c-111">Run Batch Jobs</span></span>](ui-how-run-batch-jobs.md)  
[<span data-ttu-id="7177c-112">Отправка документов по электронной почте</span><span class="sxs-lookup"><span data-stu-id="7177c-112">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
