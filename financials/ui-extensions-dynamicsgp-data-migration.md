---
title: "Миграция данных из Dynamics GP с помощью расширения для миграции данных | Документы Майкрософт"
description: "Используйте расширение для миграции данных Dynamics GP, чтобы перенести клиентов, поставщиков, товары и счета из Dynamics GP в Dynamics 365 for Financials."
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
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 31b698aea884da162cc18f16a912ebd57e35aed9
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="the-dynamics-gp-data-migration-extension-for-dynamics-365-for-financials"></a><span data-ttu-id="e8bb0-103">Расширение для миграции данных Dynamics GP для Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="e8bb0-103">The Dynamics GP Data Migration Extension for Dynamics 365 for Financials</span></span>
<span data-ttu-id="e8bb0-104">Это расширение облегчает миграцию клиентов, поставщиков, складских товаров и счетов из Dynamics GP в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e8bb0-104">This extension makes it easy to migrate customers, vendors, inventory items, and accounts from Dynamics GP to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="e8bb0-105">Если сейчас ваша компания использует Dynamics GP, вы можете экспортировать соответствующие основные записи, а затем открыть руководство по сопровождаемой настройке, чтобы добавить данные в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e8bb0-105">If your business uses Dynamics GP today, you can export the relevant master records and then open an assisted setup guide to add the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="e8bb0-106">Дополнительные сведения см. в разделе [Миграция бизнес-данных из других финансовых систем](upload-data.md).</span><span class="sxs-lookup"><span data-stu-id="e8bb0-106">For more information, see [Migrate Business Data from Other Finance Systems](upload-data.md).</span></span>

## <a name="exporting-data-from-dynamics-gp"></a><span data-ttu-id="e8bb0-107">Экспорт данных из Dynamics GP</span><span class="sxs-lookup"><span data-stu-id="e8bb0-107">Exporting Data from Dynamics GP</span></span>
<span data-ttu-id="e8bb0-108">Чтобы экспортировать данный, вы должны экспортировать некоторые или все существующие клиенты, поставщики, складские товары и счета в файл с помощью функции Dynamics GP.</span><span class="sxs-lookup"><span data-stu-id="e8bb0-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to a file, using the Dynamics GP functionality for data export.</span></span> <span data-ttu-id="e8bb0-109">Для целей [!INCLUDE[d365fin](includes/d365fin_md.md)] можно экспортировать следующие типы данных:</span><span class="sxs-lookup"><span data-stu-id="e8bb0-109">For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following types of data:</span></span>

* <span data-ttu-id="e8bb0-110">Организация</span><span class="sxs-lookup"><span data-stu-id="e8bb0-110">Account</span></span>  
* <span data-ttu-id="e8bb0-111">Клиент</span><span class="sxs-lookup"><span data-stu-id="e8bb0-111">Customer</span></span>  
* <span data-ttu-id="e8bb0-112">Пункт меню</span><span class="sxs-lookup"><span data-stu-id="e8bb0-112">Item</span></span>  
* <span data-ttu-id="e8bb0-113">Поставщик</span><span class="sxs-lookup"><span data-stu-id="e8bb0-113">Vendor</span></span>  

<span data-ttu-id="e8bb0-114">Расширение переноса данных Dynamics GP автоматически сопоставляет экспортированные данные, чтобы вы могли быстро получить данные в новой организации в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e8bb0-114">The Dynamics GP Data Migration extension automatically maps the exported data so that your data is quickly available to you in your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span></span> <span data-ttu-id="e8bb0-115">В ходе процесса создается информация по настройке, например учетные группы.</span><span class="sxs-lookup"><span data-stu-id="e8bb0-115">During the process, supporting setup information is created, such as posting groups.</span></span> <span data-ttu-id="e8bb0-116">Складские товары будут добавлены в систему по методу оценки себестоимости FIFO.</span><span class="sxs-lookup"><span data-stu-id="e8bb0-116">Inventory items will be brought into the system with FIFO as the cost valuation method.</span></span> <span data-ttu-id="e8bb0-117">Счета будут настроены как сегмент главного счета из Dynamics GP с измерениями, поскольку [!INCLUDE[d365fin](includes/d365fin_long_md.md)] не имеет сегменты счета.</span><span class="sxs-lookup"><span data-stu-id="e8bb0-117">Accounts will be set up as the main account segment from Dynamics GP with dimensions, because [!INCLUDE[d365fin](includes/d365fin_long_md.md)] does not have account segments.</span></span>

## <a name="see-also"></a><span data-ttu-id="e8bb0-118">См. также</span><span class="sxs-lookup"><span data-stu-id="e8bb0-118">See Also</span></span>
[<span data-ttu-id="e8bb0-119">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="e8bb0-119">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="e8bb0-120">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="e8bb0-120">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span></span>  

