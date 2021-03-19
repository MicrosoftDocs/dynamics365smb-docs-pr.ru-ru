---
title: Расширение для миграции данных QuickBooks | Документация Майкрософт
description: Описывает, как использовать расширение для импорта клиентов, поставщиков, товаров и счетов из QuickBooks Desktop в Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 990aabaaccbf32a5cbd95c09527657757e5182cb
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5391428"
---
# <a name="the-quickbooks-data-migration-extension"></a><span data-ttu-id="dd927-103">Расширение для миграции данных QuickBooks</span><span class="sxs-lookup"><span data-stu-id="dd927-103">The QuickBooks Data Migration Extension</span></span>

<span data-ttu-id="dd927-104">Это расширение облегчает миграцию клиентов, поставщиков, товаров и счетов из QuickBooks в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="dd927-104">This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="dd927-105">Если сейчас ваша компания использует QuickBooks, вы можете экспортировать требуемую информацию, а затем открыть руководство по сопровождаемой настройке, чтобы загрузить данные в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="dd927-105">If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  
<span data-ttu-id="dd927-106">Дополнительные сведения см. в разделе [Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md).</span><span class="sxs-lookup"><span data-stu-id="dd927-106">For more information, see [Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md).</span></span>

## <a name="data-from-quickbooks-desktop"></a><span data-ttu-id="dd927-107">Данные из QuickBooks Desktop</span><span class="sxs-lookup"><span data-stu-id="dd927-107">Data from QuickBooks Desktop</span></span>

<span data-ttu-id="dd927-108">Вы можете импортировать следующие данные из QuickBooks Online в Business Central:</span><span class="sxs-lookup"><span data-stu-id="dd927-108">You can import the following data from QuickBooks Online to Business Central:</span></span>

- <span data-ttu-id="dd927-109">Клиенты</span><span class="sxs-lookup"><span data-stu-id="dd927-109">Customers</span></span>  
- <span data-ttu-id="dd927-110">Поставщики</span><span class="sxs-lookup"><span data-stu-id="dd927-110">Vendors</span></span>  
- <span data-ttu-id="dd927-111">Товаров</span><span class="sxs-lookup"><span data-stu-id="dd927-111">Items</span></span>  
- <span data-ttu-id="dd927-112">План счетов</span><span class="sxs-lookup"><span data-stu-id="dd927-112">Chart of Accounts</span></span>  
- <span data-ttu-id="dd927-113">Транзакция начального сальдо в главной книге</span><span class="sxs-lookup"><span data-stu-id="dd927-113">Beginning Balance transactions in General Ledger</span></span>  
- <span data-ttu-id="dd927-114">Товары в наличии</span><span class="sxs-lookup"><span data-stu-id="dd927-114">On-hand Quantities for Inventory Items</span></span>  
- <span data-ttu-id="dd927-115">Открытые документы для клиентов и поставщиков, например счета, кредит-ноты и платежи</span><span class="sxs-lookup"><span data-stu-id="dd927-115">Open documents for customers and vendors, such as invoices, credit memos and payments</span></span>  

<span data-ttu-id="dd927-116">Мы переносим только полные суммы документов продажи и покупки.</span><span class="sxs-lookup"><span data-stu-id="dd927-116">We migrate only full amounts on sales and purchase documents.</span></span> <span data-ttu-id="dd927-117">Мы не обновляем частично оплаченные суммы.</span><span class="sxs-lookup"><span data-stu-id="dd927-117">We do not update partially paid amounts.</span></span> <span data-ttu-id="dd927-118">Например, если клиент оплатил 300 долларов из 500 по счету продажи, мы переносим 500 долларов.</span><span class="sxs-lookup"><span data-stu-id="dd927-118">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span></span> <span data-ttu-id="dd927-119">Если вы получили частичные платежи, их необходимо вручную обновить либо до миграции данных, либо после нее.</span><span class="sxs-lookup"><span data-stu-id="dd927-119">If you have received partial payments, you must update these manually, either before or after you migrate data.</span></span> <span data-ttu-id="dd927-120">Рекомендуется применить незакрытые транзакции перед миграцией, чтобы потом было проще работать.</span><span class="sxs-lookup"><span data-stu-id="dd927-120">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span></span>

> [!NOTE]
> <span data-ttu-id="dd927-121">Мы не переносим заказы на покупку и заказы на продажу.</span><span class="sxs-lookup"><span data-stu-id="dd927-121">We do not migrate purchase orders or sales orders.</span></span>

## <a name="before-you-start"></a><span data-ttu-id="dd927-122">Перед началом работы</span><span class="sxs-lookup"><span data-stu-id="dd927-122">Before You Start</span></span>

<span data-ttu-id="dd927-123">Важной частью процесса миграции является указание счетов, на которые должны быть перенесены транзакции.</span><span class="sxs-lookup"><span data-stu-id="dd927-123">An important part of the migration process is to specify the accounts to migrate transactions to.</span></span> <span data-ttu-id="dd927-124">Рекомендуется задать сопоставление до переноса данных.</span><span class="sxs-lookup"><span data-stu-id="dd927-124">It's a good idea to plan this mapping before you migrate data.</span></span> <span data-ttu-id="dd927-125">Например, задать счета, на которых вы учитываете транзакции для:</span><span class="sxs-lookup"><span data-stu-id="dd927-125">For example, the accounts where you post transactions for:</span></span>

- <span data-ttu-id="dd927-126">Продажи товаров или услуг клиентам</span><span class="sxs-lookup"><span data-stu-id="dd927-126">The sale of items or services to customers</span></span>  
- <span data-ttu-id="dd927-127">Покупки товаров или услуг у поставщиков</span><span class="sxs-lookup"><span data-stu-id="dd927-127">The purchase of items or services from vendors</span></span>  
- <span data-ttu-id="dd927-128">Коррекции в главной книге</span><span class="sxs-lookup"><span data-stu-id="dd927-128">Adjustments in the general ledger</span></span>  

<span data-ttu-id="dd927-129">Business Central требует, чтобы счетам главной книги были назначены номера.</span><span class="sxs-lookup"><span data-stu-id="dd927-129">Business Central requires that general ledger accounts have account numbers assigned to them.</span></span> <span data-ttu-id="dd927-130">Убедитесь, что номера счетов назначены в QuickBooks.</span><span class="sxs-lookup"><span data-stu-id="dd927-130">Make sure that account numbers are assigned to your accounts in QuickBooks.</span></span>
<span data-ttu-id="dd927-131">Если транзакции в QuickBooks содержат суммы налога, необходимо настроить налоговый счет в налоговых юрисдикциях в Business Central, прежде чем вы сможете учитывать транзакции.</span><span class="sxs-lookup"><span data-stu-id="dd927-131">If transactions in QuickBooks have tax amounts, you must set up a tax account for your tax jurisdictions in Business Central before you can post transactions.</span></span>

<span data-ttu-id="dd927-132">Чтобы получить данные из приложения QuickBooks Desktop, необходимо загрузить средство экспорта данных Microsoft.</span><span class="sxs-lookup"><span data-stu-id="dd927-132">In order to get your data out of the QuickBooks desktop application you will need to download the Microsoft Data Exporter Tool.</span></span>  <span data-ttu-id="dd927-133">Инструкции для этого средства приведены в мастере миграции данных в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="dd927-133">The instructions for the tool are in the Data Migration Wizard in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="dd927-134">Средство подключится к вашему приложению QuickBooks и экспортирует соответствующие данные в виде файла ZIP.</span><span class="sxs-lookup"><span data-stu-id="dd927-134">The tool will connect to your QuickBooks application and export the applicable data to a .zip file.</span></span>  

> [!NOTE]
> <span data-ttu-id="dd927-135">В данный момент средство экспорта данных можно использовать только с QuickBooks 2017 и 2018.</span><span class="sxs-lookup"><span data-stu-id="dd927-135">Currently the data exporter tool only works with QuickBooks 2017 and 2018.</span></span>

## <a name="finding-the-quickbooks-data-migration-extension"></a><span data-ttu-id="dd927-136">Поиск расширения для миграции данных QuickBooks</span><span class="sxs-lookup"><span data-stu-id="dd927-136">Finding the QuickBooks Data Migration Extension</span></span>

<span data-ttu-id="dd927-137">Расширение миграции данных QuickBooks установлено и готово к работе как составная часть мастер настройки миграции данных.</span><span class="sxs-lookup"><span data-stu-id="dd927-137">The QuickBooks Data Migration extension is installed and ready to go as an integrated part of the Data Migration assisted setup guide.</span></span> <span data-ttu-id="dd927-138">Если вы готовы начать прямо сейчас и уже экспортировали свои данные из QuickBooks, выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Мастер настройки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="dd927-138">If you are ready to get started now, and have exported your data from QuickBooks, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose the related link.</span></span> <span data-ttu-id="dd927-139">Выберите **Миграция бизнес-данных**, затем выполните шаги в руководстве.</span><span class="sxs-lookup"><span data-stu-id="dd927-139">Choose **Migrate business data**, and then follow the steps in the guide.</span></span>  

## <a name="what-do-i-do-after-i-migrate-data"></a><span data-ttu-id="dd927-140">Что нужно сделать после переноса данных?</span><span class="sxs-lookup"><span data-stu-id="dd927-140">What do I do after I migrate Data?</span></span>

<span data-ttu-id="dd927-141">После переноса данных транзакции имеют статус Неучтенные, чтобы их можно было проверить и внести корректировки.</span><span class="sxs-lookup"><span data-stu-id="dd927-141">After you migrate data, transactions have the status Unposted, so you can review them and make adjustments.</span></span> <span data-ttu-id="dd927-142">Чтобы проверить транзакции, откройте страницу, на которой они должны находиться.</span><span class="sxs-lookup"><span data-stu-id="dd927-142">To review the transactions, go to the page where you would normally find them.</span></span> <span data-ttu-id="dd927-143">Например, чтобы проверить неучтенные счета продажи, перейдите на страницу Счета продажи.</span><span class="sxs-lookup"><span data-stu-id="dd927-143">For example, to review unposted sales invoices, go to the Sales Invoices page.</span></span> <span data-ttu-id="dd927-144">Чтобы проверить журналы платежей, перейдите на страницу Журналы платежей.</span><span class="sxs-lookup"><span data-stu-id="dd927-144">To review payment journals, go to the Payment Journals page.</span></span>
<span data-ttu-id="dd927-145">Есть несколько важных вещей, которые нужно сделать. Если для транзакций в QuickBooks Online были заданы суммы наценки или скидки, их необходимо вручную добавить в соответствующие транзакции в Business Central, прежде чем учитывать их.</span><span class="sxs-lookup"><span data-stu-id="dd927-145">There are a few things in particular that you should do: If the transactions in QuickBooks had markup or discount amounts, you must manually add the amounts to the related transactions in Business Central before you post them.</span></span>
<span data-ttu-id="dd927-146">Если вы используете налог на добавленную стоимость (НДС), вы можете добавить учетные бизнес-группы или товарные группы в параметры учета, чтобы вы могли учитывать суммы НДС.</span><span class="sxs-lookup"><span data-stu-id="dd927-146">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span></span>
<span data-ttu-id="dd927-147">Проверьте начальные сальдо счетов в главной книге.</span><span class="sxs-lookup"><span data-stu-id="dd927-147">Verify the beginning balances for accounts in the general ledger.</span></span> <span data-ttu-id="dd927-148">В QuickBooks не хранится текущее сальдо для всех счетов, поэтому вам может потребоваться исправить начальные сальдо.</span><span class="sxs-lookup"><span data-stu-id="dd927-148">QuickBooks does not store the current balance for all accounts, so you might need to correct beginning balances.</span></span>

## <a name="see-also"></a><span data-ttu-id="dd927-149">См. также</span><span class="sxs-lookup"><span data-stu-id="dd927-149">See Also</span></span>

[<span data-ttu-id="dd927-150">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="dd927-150">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="dd927-151">[Настройка [!INCLUDE[prod_short](includes/prod_short.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="dd927-151">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions ](ui-extensions.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]