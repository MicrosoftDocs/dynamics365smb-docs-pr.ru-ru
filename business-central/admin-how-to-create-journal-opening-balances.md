---
title: Создание входящего сальдо журнала | Документация Майкрософт
description: Business Central включает несколько пакетных заданий, которые помогают перенести предыдущие сальдо счетов в заново настроенную организацию. Можно легко перенести эти данные с помощью учета в журналах.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 9e1d936901f1a42991895c9e4b797a3238a24710
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5378277"
---
# <a name="create-journal-opening-balances"></a><span data-ttu-id="3f67a-104">Создание входящего сальдо журнала</span><span class="sxs-lookup"><span data-stu-id="3f67a-104">Create Journal Opening Balances</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="3f67a-105">включает несколько пакетных заданий, которые помогают перенести предыдущие сальдо счетов в заново настроенную организацию.</span><span class="sxs-lookup"><span data-stu-id="3f67a-105">includes several batch jobs that are provided to help in the transfer of legacy account balances to a newly configured company.</span></span> <span data-ttu-id="3f67a-106">Можно легко перенести эти данные с помощью журнала клиентов, журнала поставщиков, журнала товаров или журнала ГК.</span><span class="sxs-lookup"><span data-stu-id="3f67a-106">You can easily transfer this data with the customer journal, the vendor journal, the item journal, or the G/L journal.</span></span>

<span data-ttu-id="3f67a-107">Первым этапом является создание пакета конфигурации, включающего таблицы настройки таких журналов.</span><span class="sxs-lookup"><span data-stu-id="3f67a-107">The first step is to create a configuration package that includes the setup tables for those journals.</span></span> <span data-ttu-id="3f67a-108">Следующая процедура предполагает, что этот шаг выполнен.</span><span class="sxs-lookup"><span data-stu-id="3f67a-108">The following procedure assumes that this step is completed.</span></span> <span data-ttu-id="3f67a-109">Дополнительные сведения см. в разделе [Настройка конфигурации организации](admin-set-up-company-configuration.md).</span><span class="sxs-lookup"><span data-stu-id="3f67a-109">For more information, see [Set Up Company Configuration](admin-set-up-company-configuration.md).</span></span> <span data-ttu-id="3f67a-110">Эта процедура описывает последовательные действия, в число которых включается применение пакета, предоставленного партнером.</span><span class="sxs-lookup"><span data-stu-id="3f67a-110">This procedure describes the subsequent steps, which include applying the package that is provided by a partner.</span></span>  

<span data-ttu-id="3f67a-111">Перед началом убедитесь, что вы используете страницу ролевого центра администрирования, так как она дает правильный контекст для вашей работы по конфигурации.</span><span class="sxs-lookup"><span data-stu-id="3f67a-111">Before you start, make sure that you are using the Administration Role Center page because it provides the correct context for your configuration work.</span></span> <span data-ttu-id="3f67a-112">Дополнительные сведения см. в разделе [Изменение базовых настроек](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="3f67a-112">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span></span>

## <a name="to-apply-the-entries-in-a-journal-to-a-new-company"></a><span data-ttu-id="3f67a-113">Применение журнальных записей к новой организации</span><span class="sxs-lookup"><span data-stu-id="3f67a-113">To apply the entries in a journal to a new company</span></span>

1. <span data-ttu-id="3f67a-114">Настройте новую организацию и примените к ней пакет конфигурации.</span><span class="sxs-lookup"><span data-stu-id="3f67a-114">Configure a new company and apply a configuration package to it.</span></span> <span data-ttu-id="3f67a-115">Дополнительные сведения см. в разделе [Настройка организации с помощью мастера RapidStart](admin-how-to-configure-a-company-with-the-rapidstart-wizard.md).</span><span class="sxs-lookup"><span data-stu-id="3f67a-115">For more information, see [Configure a Company with the RapidStart Wizard](admin-how-to-configure-a-company-with-the-rapidstart-wizard.md).</span></span>  

    <span data-ttu-id="3f67a-116">Новая организация не содержит информацию о входящем сальдо журнала.</span><span class="sxs-lookup"><span data-stu-id="3f67a-116">The new company does not contain information about journal opening balances.</span></span>  

2. <span data-ttu-id="3f67a-117">Откройте журнал конфигураций и импортируйте существующие данные о товарах, клиентах, поставщиках и Главной книге.</span><span class="sxs-lookup"><span data-stu-id="3f67a-117">Open the configuration worksheet and import existing data about customers, items, vendors, and the general ledger.</span></span> <span data-ttu-id="3f67a-118">Дополнительные сведения см. в разделе [Миграция данных клиента](admin-migrate-customer-data.md).</span><span class="sxs-lookup"><span data-stu-id="3f67a-118">For more information, see [Migrate Customer Data](admin-migrate-customer-data.md).</span></span>  

    <span data-ttu-id="3f67a-119">Теперь у вас есть основные данные.</span><span class="sxs-lookup"><span data-stu-id="3f67a-119">Now you have master data in place.</span></span> <span data-ttu-id="3f67a-120">Затем вы добавляете начальные сальдо.</span><span class="sxs-lookup"><span data-stu-id="3f67a-120">Next, you add the opening balances.</span></span> <span data-ttu-id="3f67a-121">Следующие шаги описывают, как создать строки журнала для счетов ГК, но то же самое применимо к созданию строк журнала для клиентов, поставщиков и товаров.</span><span class="sxs-lookup"><span data-stu-id="3f67a-121">The following steps describe how to create journal lines for G/L accounts, but the same apply to creating journal lines for customers, vendors, and items.</span></span>  
3. <span data-ttu-id="3f67a-122">Выберите действие **Создать строки журнала счетов ГК**.</span><span class="sxs-lookup"><span data-stu-id="3f67a-122">Choose the **Create G/L Acct. Journal Lines** action.</span></span>  
4. <span data-ttu-id="3f67a-123">Заполните экспресс-вкладку **Параметры** должным образом и по мере необходимости настройте фильтры.</span><span class="sxs-lookup"><span data-stu-id="3f67a-123">Fill in the **Options** FastTab as appropriate, and set filters as needed.</span></span> <span data-ttu-id="3f67a-124">Например, в поле **Шаблон журнала** введите описательное имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="3f67a-124">For example, in the **Journal Template** field, enter a name.</span></span>  
5. <span data-ttu-id="3f67a-125">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="3f67a-125">Choose the **OK** button.</span></span> <span data-ttu-id="3f67a-126">Записи теперь находятся в журнале, но суммы не указаны.</span><span class="sxs-lookup"><span data-stu-id="3f67a-126">The records are now in the journal, but the amounts are empty.</span></span>  
6. <span data-ttu-id="3f67a-127">Экспортируйте таблицу журнала в Excel и вручную введите информацию об учете и балансирующем счете из унаследованных данных.</span><span class="sxs-lookup"><span data-stu-id="3f67a-127">Export the journal table to Excel and manually enter the posting and balancing account information from the legacy data.</span></span>
7. <span data-ttu-id="3f67a-128">Импортируйте и примените информацию о таблице в новой организации.</span><span class="sxs-lookup"><span data-stu-id="3f67a-128">Import and apply the table information into the new company.</span></span> <span data-ttu-id="3f67a-129">Строки журнала готовы к учету.</span><span class="sxs-lookup"><span data-stu-id="3f67a-129">The journal lines are ready for posting.</span></span>  
8. <span data-ttu-id="3f67a-130">В журнале конфигураций выберите таблицу строки журнала, затем выберите действие **Данные базы данных**.</span><span class="sxs-lookup"><span data-stu-id="3f67a-130">In the configuration worksheet, select the journal line table, and then choose the **Database Data** action.</span></span>  
9. <span data-ttu-id="3f67a-131">Проверьте информацию, затем выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="3f67a-131">Review the information, and then choose the **Post** action.</span></span>  
10. <span data-ttu-id="3f67a-132">Повторите эти шаги для импорта и учета всех других начальных балансов.</span><span class="sxs-lookup"><span data-stu-id="3f67a-132">Repeat the steps to import and post any other opening balances.</span></span>  

> [!TIP]
> <span data-ttu-id="3f67a-133">Вы можете использовать те же пакетные задания для добавления начальных балансов всякий раз, когда вы регистрируете нового клиента или поставщика, с которым вы работали ранее, но не зарегистрировали в [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="3f67a-133">You can use the same batch jobs to add opening balances whenever you register a new customer or vendor that you have done business with before but not registered in [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="3f67a-134">Просто найдите соответствующую задачу, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="3f67a-134">Just search for the relevant task, and then choose the relevant link.</span></span>

## <a name="see-also"></a><span data-ttu-id="3f67a-135">См. также</span><span class="sxs-lookup"><span data-stu-id="3f67a-135">See Also</span></span>

[<span data-ttu-id="3f67a-136">Применение конфигураций к новым организациям</span><span class="sxs-lookup"><span data-stu-id="3f67a-136">Apply Configurations to New Companies</span></span>](admin-apply-configuration-to-new-companies.md)  
[<span data-ttu-id="3f67a-137">Настройка организации со службами RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="3f67a-137">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="3f67a-138">Администрация</span><span class="sxs-lookup"><span data-stu-id="3f67a-138">Administration</span></span>](admin-setup-and-administration.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]