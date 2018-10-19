---
title: "Использование расширения для миграции данных QuickBooks | Microsoft Docs"
description: "Описывает, как использовать расширение для импорта клиентов, поставщиков, товаров и счетов из QuickBooks Desktop в Business Central."
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 583f6947acd3778710f0889736439322d9179ce6
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="the-quickbooks-data-migration-extension"></a><span data-ttu-id="50567-103">Расширение для миграции данных QuickBooks</span><span class="sxs-lookup"><span data-stu-id="50567-103">The QuickBooks Data Migration Extension</span></span>
<span data-ttu-id="50567-104">Это расширение облегчает миграцию клиентов, поставщиков, товаров и счетов из QuickBooks в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="50567-104">This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="50567-105">Если сейчас ваша компания использует QuickBooks, вы можете экспортировать требуемую информацию, а затем открыть руководство по сопровождаемой настройке, чтобы загрузить данные в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="50567-105">If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
<span data-ttu-id="50567-106">Дополнительные сведения см. в разделе [Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md).</span><span class="sxs-lookup"><span data-stu-id="50567-106">For more information, see [Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md).</span></span>

## <a name="exporting-data-from-quickbooks-desktop"></a><span data-ttu-id="50567-107">Экспорт данных из QuickBooks Desktop</span><span class="sxs-lookup"><span data-stu-id="50567-107">Exporting Data from QuickBooks Desktop</span></span>
<span data-ttu-id="50567-108">Вы должны были экспортировать часть или всех ваших существующих клиентов, поставщиков, складские товары и счета в файл Intuit Interchange Format (IIF).</span><span class="sxs-lookup"><span data-stu-id="50567-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to an Intuit Interchange Format (IIF) file.</span></span> <span data-ttu-id="50567-109">Расширение для миграции данных QuickBooks содержит сопоставление данных QuickBooks по умолчанию, чтобы вы могли использовать собственные данные для тестирования новой организации [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="50567-109">The QuickBooks Data Migration extension includes a default mapping of QuickBooks data so that you can use your existing data to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span></span> <span data-ttu-id="50567-110">Сопоставления по умолчанию будет в большинстве случаев достаточно, но можно изменить его с помощью руководства по настройке.</span><span class="sxs-lookup"><span data-stu-id="50567-110">The default mapping will be sufficient in the vast majority of cases, but you can change the mapping in the assisted setup guide.</span></span>  
<span data-ttu-id="50567-111">В QuickBooks в меню "Файл" есть служебная программа для экспорта списков.</span><span class="sxs-lookup"><span data-stu-id="50567-111">In QuickBooks, the File menu includes a utility to export lists.</span></span> <span data-ttu-id="50567-112">Для целей [!INCLUDE[d365fin](includes/d365fin_md.md)] можно экспортировать следующие списки:</span><span class="sxs-lookup"><span data-stu-id="50567-112">For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following lists:</span></span>

* <span data-ttu-id="50567-113">Список клиентов</span><span class="sxs-lookup"><span data-stu-id="50567-113">Customer List</span></span>  
* <span data-ttu-id="50567-114">Список поставщиков</span><span class="sxs-lookup"><span data-stu-id="50567-114">Vendor List</span></span>  
* <span data-ttu-id="50567-115">Список товаров</span><span class="sxs-lookup"><span data-stu-id="50567-115">Item List</span></span>  
* <span data-ttu-id="50567-116">Список счетов</span><span class="sxs-lookup"><span data-stu-id="50567-116">Account List</span></span>  

<span data-ttu-id="50567-117">Экспортируемые данные сохраняются в виде файла IIF, который затем можно загрузить в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="50567-117">The exported data is saved as an IIF file that you can then upload to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="finding-the-quickbooks-data-migration-extension"></a><span data-ttu-id="50567-118">Поиск расширения для миграции данных QuickBooks</span><span class="sxs-lookup"><span data-stu-id="50567-118">Finding the QuickBooks Data Migration Extension</span></span>
<span data-ttu-id="50567-119">Расширение миграции данных QuickBooks установлено и готово к работе как составная часть мастер настройки миграции данных.</span><span class="sxs-lookup"><span data-stu-id="50567-119">The QuickBooks Data Migration extension is installed and ready to go as an integrated part of the Data Migration assisted setup guide.</span></span> <span data-ttu-id="50567-120">Если вы готовы начать прямо сейчас и уже экспортировали свои данные из QuickBooks, выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Мастер настройки**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="50567-120">If you are ready to get started now, and have exported your data from QuickBooks, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose the related link.</span></span> <span data-ttu-id="50567-121">Выберите **Миграция бизнес-данных**, затем выполните шаги в руководстве.</span><span class="sxs-lookup"><span data-stu-id="50567-121">Choose **Migrate business data**, and then follow the steps in the guide.</span></span>  

## <a name="see-also"></a><span data-ttu-id="50567-122">См. также</span><span class="sxs-lookup"><span data-stu-id="50567-122">See Also</span></span>
[<span data-ttu-id="50567-123">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="50567-123">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="50567-124">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="50567-124">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span></span>  

