---
title: "Использование расширения для миграции данных QuickBooks | Документы Майкрософт"
description: "Описывает, как использовать расширение для импорта клиентов, поставщиков, товаров и счетов из QuickBooks Desktop в Dynamics 365 for Financials."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 37d90316ea0be5489fb5abe33645de3fe0d3cf90
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="the-quickbooks-data-migration-extension-for-dynamics-365-for-financials"></a><span data-ttu-id="5b1e2-103">Расширение для миграции данных QuickBooks для Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="5b1e2-103">The QuickBooks Data Migration Extension for Dynamics 365 for Financials</span></span>
<span data-ttu-id="5b1e2-104">Это расширение облегчает миграцию клиентов, поставщиков, товаров и счетов из QuickBooks в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5b1e2-104">This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="5b1e2-105">Если сейчас ваша компания использует QuickBooks, вы можете экспортировать требуемую информацию, а затем открыть руководство по сопровождаемой настройке, чтобы загрузить данные в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5b1e2-105">If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
<span data-ttu-id="5b1e2-106">Дополнительные сведения см. в разделе [Импорт бизнес-данных из других финансовых систем](upload-data.md).</span><span class="sxs-lookup"><span data-stu-id="5b1e2-106">For more information, see [Importing Business Data from Other Finance Systems](upload-data.md).</span></span>

## <a name="exporting-data-from-quickbooks"></a><span data-ttu-id="5b1e2-107">Экспорт данных из QuickBooks</span><span class="sxs-lookup"><span data-stu-id="5b1e2-107">Exporting Data from QuickBooks</span></span>
<span data-ttu-id="5b1e2-108">Вы должны были экспортировать часть или всех ваших существующих клиентов, поставщиков, складские товары и счета в файл Intuit Interchange Format (IIF).</span><span class="sxs-lookup"><span data-stu-id="5b1e2-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to an Intuit Interchange Format (IIF) file.</span></span> <span data-ttu-id="5b1e2-109">Расширение для миграции данных QuickBooks содержит сопоставление данных QuickBooks по умолчанию, чтобы вы могли использовать собственные данные для тестирования новой организации [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5b1e2-109">The QuickBooks Data Migration extension includes a default mapping of QuickBooks data so that you can use your existing data to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span></span> <span data-ttu-id="5b1e2-110">Сопоставления по умолчанию будет в большинстве случаев достаточно, но можно изменить его с помощью руководства по настройке.</span><span class="sxs-lookup"><span data-stu-id="5b1e2-110">The default mapping will be sufficient in the vast majority of cases, but you can change the mapping in the assisted setup guide.</span></span>  
<span data-ttu-id="5b1e2-111">В QuickBooks в меню "Файл" есть служебная программа для экспорта списков.</span><span class="sxs-lookup"><span data-stu-id="5b1e2-111">In QuickBooks, the File menu includes a utility to export lists.</span></span> <span data-ttu-id="5b1e2-112">Для целей [!INCLUDE[d365fin](includes/d365fin_md.md)] можно экспортировать следующие списки:</span><span class="sxs-lookup"><span data-stu-id="5b1e2-112">For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following lists:</span></span>

* <span data-ttu-id="5b1e2-113">Список клиентов</span><span class="sxs-lookup"><span data-stu-id="5b1e2-113">Customer List</span></span>  
* <span data-ttu-id="5b1e2-114">Список поставщиков</span><span class="sxs-lookup"><span data-stu-id="5b1e2-114">Vendor List</span></span>  
* <span data-ttu-id="5b1e2-115">Список товаров</span><span class="sxs-lookup"><span data-stu-id="5b1e2-115">Item List</span></span>  
* <span data-ttu-id="5b1e2-116">Список счетов</span><span class="sxs-lookup"><span data-stu-id="5b1e2-116">Account List</span></span>  

<span data-ttu-id="5b1e2-117">Экспортируемые данные сохраняются в виде файла IIF, который затем можно загрузить в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5b1e2-117">The exported data is saved as an IIF file that you can then upload to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="see-also"></a><span data-ttu-id="5b1e2-118">См. также</span><span class="sxs-lookup"><span data-stu-id="5b1e2-118">See Also</span></span>
[<span data-ttu-id="5b1e2-119">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="5b1e2-119">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="5b1e2-120">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="5b1e2-120">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span></span>  

