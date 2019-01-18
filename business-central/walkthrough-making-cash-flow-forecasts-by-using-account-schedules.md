---
title: "Пошаговое руководство. Создание прогнозов движения денежных средств с использованием финансовых отчетов | Документы Майкрософт"
description: "В этом пошаговом руководстве описывается использование финансовых отчетов для создания прогнозов движения денежных средств. Финансовые отчеты выполняют расчеты, которые невозможно выполнить непосредственно в диаграмме счетов движения денежных средств. В финансовых отчетах можно настроить промежуточные итоги для приема и распределения движения денежных средств. Эти подытоги могут включаться в новые итоговые значения, которые затем можно использовать при создании прогнозов движения денежных средств."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 652a151ff50c8492b3dc7df5d17c04ff2d00faad
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="walkthrough-making-cash-flow-forecasts-by-using-account-schedules"></a><span data-ttu-id="7e0ef-106">Пошаговое руководство: создание прогнозов движения денежных средств с использованием финансовых отчетов</span><span class="sxs-lookup"><span data-stu-id="7e0ef-106">Walkthrough: Making Cash Flow Forecasts by Using Account Schedules</span></span>
<span data-ttu-id="7e0ef-107">В этом пошаговом руководстве описывается использование финансовых отчетов для создания прогнозов движения денежных средств.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-107">This walkthrough describes how you can use account schedules to make cash flow forecasts.</span></span> <span data-ttu-id="7e0ef-108">Финансовые отчеты выполняют расчеты, которые невозможно выполнить непосредственно в диаграмме счетов движения денежных средств.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-108">Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts.</span></span> <span data-ttu-id="7e0ef-109">В финансовых отчетах можно настроить промежуточные итоги для приема и распределения движения денежных средств.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-109">In the account schedules, you can set up subtotals for cash flow receipts and disbursements.</span></span> <span data-ttu-id="7e0ef-110">Эти подытоги могут включаться в новые итоговые значения, которые затем можно использовать при создании прогнозов движения денежных средств.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-110">These subtotals can be included in new totals that can then be used in making cash flow forecasts.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="7e0ef-111">Об этом пошаговом руководстве</span><span class="sxs-lookup"><span data-stu-id="7e0ef-111">About This Walkthrough</span></span>  
<span data-ttu-id="7e0ef-112">В этом пошаговом руководстве описываются следующие задачи:</span><span class="sxs-lookup"><span data-stu-id="7e0ef-112">This walkthrough describes the following tasks:</span></span>  

- <span data-ttu-id="7e0ef-113">Настройте новое название финансового отчета о движении денежных средств.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-113">Setting up a new cash flow account schedule name.</span></span>  
- <span data-ttu-id="7e0ef-114">Настройка строк финансового отчета.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-114">Setting up account schedule lines.</span></span>  
- <span data-ttu-id="7e0ef-115">Настройка новой раскладки столбцов.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-115">Setting up a new column layout.</span></span>  
- <span data-ttu-id="7e0ef-116">Назначение раскладки столбцов финансовому отчету.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-116">Assigning a column layout to an account schedule.</span></span>  
- <span data-ttu-id="7e0ef-117">Просмотр и печать прогноза движения денежных средств.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-117">Viewing and printing the cash flow forecast.</span></span>  

### <a name="prerequisites"></a><span data-ttu-id="7e0ef-118">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="7e0ef-118">Prerequisites</span></span>  
<span data-ttu-id="7e0ef-119">Для выполнения данного пошагового руководства необходимо выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-119">To complete this walkthrough, you will need:</span></span>  

- <span data-ttu-id="7e0ef-120">Установлен [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="7e0ef-120">[!INCLUDE[d365fin](includes/d365fin_md.md)] installed.</span></span>  
- <span data-ttu-id="7e0ef-121">Строки журнала движения денежных средств регистрируются.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-121">The cash flow worksheet lines are registered.</span></span>  

## <a name="roles"></a><span data-ttu-id="7e0ef-122">Роли</span><span class="sxs-lookup"><span data-stu-id="7e0ef-122">Roles</span></span>  
<span data-ttu-id="7e0ef-123">В этом пошаговом руководстве демонстрируются задачи, выполняемые исполнителем следующей роли:</span><span class="sxs-lookup"><span data-stu-id="7e0ef-123">This walkthrough demonstrates tasks that are performed by the following user role:</span></span>  

- <span data-ttu-id="7e0ef-124">Контроллер</span><span class="sxs-lookup"><span data-stu-id="7e0ef-124">Controller</span></span>  

## <a name="story"></a><span data-ttu-id="7e0ef-125">Сюжет</span><span class="sxs-lookup"><span data-stu-id="7e0ef-125">Story</span></span>  
<span data-ttu-id="7e0ef-126">Иван — контролер в CRONUS, который делает ежемесячные прогнозы движения денежных средств.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-126">Ken is a controller at CRONUS who makes monthly cash flow forecasts.</span></span> <span data-ttu-id="7e0ef-127">Он включает в финансы, продажи, покупки, а также основные средства в прогнозе, а затем представляет в CFO Sara для рассмотрения.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-127">He includes finance, sales, purchase, and fixed assets in the forecast, and then he presents it to CFO Sara for business insight.</span></span>  

## <a name="setting-up-a-new-account-schedule-name"></a><span data-ttu-id="7e0ef-128">Настройки нового названия финансового отчета</span><span class="sxs-lookup"><span data-stu-id="7e0ef-128">Setting Up a New Account Schedule Name</span></span>  
<span data-ttu-id="7e0ef-129">Финансовый отчет состоит из названия финансового отчета о движении денежных средств с серией строк и раскладкой столбцов.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-129">An account schedule consists of a cash flow account schedule name with a series of lines and a column layout.</span></span>  

### <a name="to-set-up-a-new-account-schedule-name"></a><span data-ttu-id="7e0ef-130">Задание нового названия финансового отчета</span><span class="sxs-lookup"><span data-stu-id="7e0ef-130">To set up a new account schedule name</span></span>  

1.  <span data-ttu-id="7e0ef-131">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовые отчеты**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Schedules**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7e0ef-132">На странице **Названия финансовых отчетов** на выберите действие **Создать**, чтобы создать новое название графика счета движения денежных средств.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-132">On the **Account Schedule Names** page, choose the **New** to create a new cash flow account schedule name.</span></span>  
3.  <span data-ttu-id="7e0ef-133">В поле **Имя** введите **Прогноз**.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-133">In the **Name** field, enter **Forecast**.</span></span>  
4.  <span data-ttu-id="7e0ef-134">В поле **Описание** введите **Прогноз движения денежных средств**.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-134">In the **Description** field, enter **Cash Flow Forecast**.</span></span>  
5.  <span data-ttu-id="7e0ef-135">Оставьте пустыми поля **Раскладка столбцов по умолчанию** и **Название аналитического отчета**.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-135">Leave the **Default Column Layout** and **Analysis View Name** fields blank.</span></span>  

## <a name="setting-up-account-schedule-lines"></a><span data-ttu-id="7e0ef-136">Настройка строк финансового отчета</span><span class="sxs-lookup"><span data-stu-id="7e0ef-136">Setting Up Account Schedule Lines</span></span>  
<span data-ttu-id="7e0ef-137">После настройки названия финансового отчета Кен определяет каждую строку, которая отображается в финансовом отчете о движении денежных средств.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-137">After an account schedule name is set up, Ken defines each line that appears in the cash flow account schedule.</span></span> <span data-ttu-id="7e0ef-138">Иван, определяет строки, которые могут отображаться в отчетах в дополнение к строкам, предназначенным только для вычислений.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-138">Ken defines lines that can be shown in reports in addition to lines that are only for calculation purposes.</span></span>  

### <a name="to-set-up-account-schedule-lines"></a><span data-ttu-id="7e0ef-139">Процедура настройки строк финансового отчета</span><span class="sxs-lookup"><span data-stu-id="7e0ef-139">To set up account schedule lines</span></span>  

1.  <span data-ttu-id="7e0ef-140">На странице **Названия финансовых отчетов** выберите новое название созданного финансового отчета **Прогноз**.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-140">On the **Account Schedule Names** page, select the new **Forecast** account schedule name that you have created.</span></span> <span data-ttu-id="7e0ef-141">На вкладке **Главная** в группе **Процесс** выберите **Изменение финансового отчета**.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-141">On the **Home** tab, in the **Process** group, choose **Edit Account Schedule**.</span></span>  
2.  <span data-ttu-id="7e0ef-142">На странице **Финансовый отчет** заполните каждую строку, как показано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-142">On the **Account Schedule** page, enter each line exactly as shown in the following table.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="7e0ef-143">С помощью функции **Вставить счета CF** можно быстро отмечать счета движения денежных средств в диаграмме счетов движения денежных средств и копировать их в строки финансового отчета.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-143">Using the **Insert CF Accounts** function, you can quickly mark the cash flow accounts from the chart of cash flow accounts and copy them to account schedule lines.</span></span>  

    <span data-ttu-id="7e0ef-144">|Номер строки|Описание|Тип группировки|Группировка|Тип строки|Тип суммы|Показать|</span><span class="sxs-lookup"><span data-stu-id="7e0ef-144">|Row No.|Description|Totaling Type|Totaling|Row Type|Amount Type|Show|</span></span>  
    <span data-ttu-id="7e0ef-145">|-------|-----------|-------------|--------|--------|---  ------|----| |C10|Сумма|Оборот|Операции|Чистая сумма|Всегда|</span><span class="sxs-lookup"><span data-stu-id="7e0ef-145">|-------|-----------|-------------|--------|--------|---  ------|----| |C10|Amount|Net Change|Entries|Net Amount|Always|</span></span>  
    <span data-ttu-id="7e0ef-146">|C20|Сумма до даты|Сальдо на дату|Операции|Чистая сумма|Всегда|</span><span class="sxs-lookup"><span data-stu-id="7e0ef-146">|C20|Amount until Date|Balance at Date|Entries|Net Amount|Always|</span></span>  
    <span data-ttu-id="7e0ef-147">|C30|Весь фин. год|Весь фин. год|Операции|Чистая сумма|Всегда|</span><span class="sxs-lookup"><span data-stu-id="7e0ef-147">|C30|Entire Fiscal Year|Entire Fiscal Year|Entries|Net Amount|Always|</span></span>  

4.  <span data-ttu-id="7e0ef-148">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-148">Choose the **OK** button.</span></span>  

## <a name="assigning-the-column-layout-to-the-account-schedule-name"></a><span data-ttu-id="7e0ef-149">Назначение раскладки столбцов названию финансового отчета</span><span class="sxs-lookup"><span data-stu-id="7e0ef-149">Assigning the Column Layout to the Account Schedule Name</span></span>  
<span data-ttu-id="7e0ef-150">Иван теперь готов назначить шаблон столбцов названию финансового отчета.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-150">Ken is now ready to assign the column layout to the account schedule name.</span></span>  

### <a name="to-assign-the-column-layout-to-the-account-schedule-name"></a><span data-ttu-id="7e0ef-151">Присвоение раскладки столбцов названию финансового отчета</span><span class="sxs-lookup"><span data-stu-id="7e0ef-151">To assign the column layout to the account schedule name</span></span>  

1.  <span data-ttu-id="7e0ef-152">На странице **Названия финансовых отчетов** выберите **Прогноз** в поле **Название**.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-152">On the **Account Schedule Names** page, select **Forecast** in the **Name** field.</span></span>  
2.  <span data-ttu-id="7e0ef-153">В поле **Раскладка столбцов по умолчанию** выберите раскладку столбцов **Движение денежных средств** в качестве раскладки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-153">In the **Default Column Layout** field, choose the column layout **Cash Flow** to assign as the default column layout.</span></span>  

### <a name="to-view-and-print-the-cash-flow-forecast"></a><span data-ttu-id="7e0ef-154">Просмотр и печать прогноза движения денежных средств</span><span class="sxs-lookup"><span data-stu-id="7e0ef-154">To view and print the cash flow forecast</span></span>  
1.  <span data-ttu-id="7e0ef-155">На странице **Названия финансовых отчетов** выберите действие **Обзор**, чтобы просмотреть прогноз движения денежных средств.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-155">On the **Account Schedule Names** page, choose the **Overview** action to view the cash flow forecast.</span></span>  
2.  <span data-ttu-id="7e0ef-156">На странице **Просмотр финансового отчета** можно выбрать сумму, а затем просмотреть записи прогноза движения денежных средств, которые составляют сумму.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-156">On the **Acc. Schedule Overview** page, you can select an amount and then view the cash flow forecast entries that make up the amount.</span></span> <span data-ttu-id="7e0ef-157">Кроме того, можно просмотреть используемую формулу для расчета суммы.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-157">In addition, you can view the formula that is used to calculate the amount.</span></span> <span data-ttu-id="7e0ef-158">Можно также фильтровать суммы по дате и измерению.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-158">You can also filter the amounts by date and dimension.</span></span>  
3.  <span data-ttu-id="7e0ef-159">Выберите действие **Печать** для печати прогноза движения денежных средств.</span><span class="sxs-lookup"><span data-stu-id="7e0ef-159">Choose the **Print** action to print the cash flow forecast.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7e0ef-160">См. также</span><span class="sxs-lookup"><span data-stu-id="7e0ef-160">See Also</span></span>  
 <span data-ttu-id="7e0ef-161">[Работа с финансовыми отчетами](bi-how-work-account-schedule.md) </span><span class="sxs-lookup"><span data-stu-id="7e0ef-161">[Work with Account Schedules](bi-how-work-account-schedule.md) </span></span>  
 [<span data-ttu-id="7e0ef-162">Пошаговые описания бизнес-процессов</span><span class="sxs-lookup"><span data-stu-id="7e0ef-162">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="7e0ef-163">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7e0ef-163">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

