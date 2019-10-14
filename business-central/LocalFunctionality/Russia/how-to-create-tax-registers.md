---
title: Создание налоговых регистров в России
description: Российские улучшения включают налоговые регистры.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 60f2a28796daa9a49dba5cbbb3b6e469cf68e33f
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301165"
---
# <a name="how-to-create-tax-registers"></a><span data-ttu-id="1b94a-103">Практическое руководство. Создание налоговых регистров</span><span class="sxs-lookup"><span data-stu-id="1b94a-103">How to: Create Tax Registers</span></span>

<span data-ttu-id="1b94a-104">В следующей процедуре показан порядок создания налоговых регистров.</span><span class="sxs-lookup"><span data-stu-id="1b94a-104">The following procedure shows how to create tax registers.</span></span> 

1. <span data-ttu-id="1b94a-105">Выберите **Финансовый менеджмент**, выберите **Налоговый учет**, выберите **Настройка**, выберите **Налоговые регистры**, затем выберите **Разделы**.</span><span class="sxs-lookup"><span data-stu-id="1b94a-105">Choose **Financial Management**, choose **Tax Accounting**, choose **Setup**, choose **Tax Register**s, and then choose **Sections**.</span></span>

2. <span data-ttu-id="1b94a-106">В окне **Секции налоговых регистров** нажмите кнопку **Функции**.</span><span class="sxs-lookup"><span data-stu-id="1b94a-106">In the **Tax Register Sections** window, choose the **Functions** button.</span></span>

3. <span data-ttu-id="1b94a-107">Выберите одно из следующих полей:</span><span class="sxs-lookup"><span data-stu-id="1b94a-107">Select one of the following fields:</span></span>

   - <span data-ttu-id="1b94a-108">**Копирование секции** — копируются данные из одного налогового регистра в другой.</span><span class="sxs-lookup"><span data-stu-id="1b94a-108">**Copy Section** -Copies data from one tax register to another.</span></span>
   - <span data-ttu-id="1b94a-109">**Очистить регистры** — очищает данные, уже созданные в налоговых регистрах, и используется для отладки условий пересчета налоговых регистров.</span><span class="sxs-lookup"><span data-stu-id="1b94a-109">**Clear Registers** -Clears data already created in the tax registers and is used for debugging conditions to re-count tax registers.</span></span>
   - <span data-ttu-id="1b94a-110">**Создать регистры** — создает данные в налоговых регистрах **.**</span><span class="sxs-lookup"><span data-stu-id="1b94a-110">**Create Registers** -Creates data in the tax registers **.**</span></span>

4. <span data-ttu-id="1b94a-111">Для создания данных выберите **Создать регистр**.</span><span class="sxs-lookup"><span data-stu-id="1b94a-111">To create data, choose **Create Register**.</span></span> <span data-ttu-id="1b94a-112">Будет открыто окно **Создание налогового регистра**.</span><span class="sxs-lookup"><span data-stu-id="1b94a-112">The **Tax Register Create** window opens.</span></span>

5. <span data-ttu-id="1b94a-113">На вкладке **Общее** введите значения в поля, описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="1b94a-113">On the **General** tab, enter the fields described in the following table.</span></span>

   | <span data-ttu-id="1b94a-114">Поле</span><span class="sxs-lookup"><span data-stu-id="1b94a-114">Field</span></span>                                                        | <span data-ttu-id="1b94a-115">Описание</span><span class="sxs-lookup"><span data-stu-id="1b94a-115">Description</span></span>                                                  |
   | :----------------------------------------------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="1b94a-116">**Периодичность**</span><span class="sxs-lookup"><span data-stu-id="1b94a-116">**Periodicity**</span></span>                                              | <span data-ttu-id="1b94a-117">Введите период для создания данных в регистрах налогового учета.</span><span class="sxs-lookup"><span data-stu-id="1b94a-117">Enter a period to create data in tax accounting registers.</span></span> <span data-ttu-id="1b94a-118">Допустимые значения:   -   **Месяц** -   **Квартал** -   **Год** **Примечание**. Если указан месяц, данные в выбранных регистрах будут созданы специально для этого месяца.</span><span class="sxs-lookup"><span data-stu-id="1b94a-118">The allowed values are:   -   **Month** -   **Quarter** -   **Year** **Note:**      If you select a month, the data in the selected registers will be created especially for that month.</span></span> <span data-ttu-id="1b94a-119">Если выбрать квартал, данные будут созданы для каждого из трех месяцев этого квартала.</span><span class="sxs-lookup"><span data-stu-id="1b94a-119">If you select a quarter, the data will be created for each of the three months of that quarter.</span></span> <span data-ttu-id="1b94a-120">Если выбрать год, данные будут созданы для каждого из 12 месяцев этого года.</span><span class="sxs-lookup"><span data-stu-id="1b94a-120">If you select a year, the data will be created for each of the 12 months of that year.</span></span> |
   | <span data-ttu-id="1b94a-121">**Учетный период**</span><span class="sxs-lookup"><span data-stu-id="1b94a-121">**Accounting Period**</span></span>                                        | <span data-ttu-id="1b94a-122">Значение, вводимое в это поле, зависит от значения, выбранного в поле "Периодичность".</span><span class="sxs-lookup"><span data-stu-id="1b94a-122">The value entered in this field depends on the value selected in the Periodicity field.</span></span> <span data-ttu-id="1b94a-123">Выберите учетный период (**Месяц**, **Квартал** или **Год**).</span><span class="sxs-lookup"><span data-stu-id="1b94a-123">Select the accounting period (**Month**, **Quarter**, or **Year**).</span></span> |
   | <span data-ttu-id="1b94a-124">**От, До**</span><span class="sxs-lookup"><span data-stu-id="1b94a-124">**From, To**</span></span>                                                 | <span data-ttu-id="1b94a-125">Эти поля заполняются автоматически и показывают дату начала и дату конца выбранного периода.</span><span class="sxs-lookup"><span data-stu-id="1b94a-125">These fields are filled in automatically and show start and end dates of the chosen period.</span></span> |
   | <span data-ttu-id="1b94a-126">**Операции ГК, Поставщики/Клиенты, Товары, Основные средства, РБП, Зарплата, Шаблоны**</span><span class="sxs-lookup"><span data-stu-id="1b94a-126">**G/L Entries, Vend's/Cust's, Items, Fixed Asset, Fut. Exp., Payroll, Templates**</span></span> | <span data-ttu-id="1b94a-127">Выберите поля для расчета регистров соответствующего типа.</span><span class="sxs-lookup"><span data-stu-id="1b94a-127">Select the fields to calculate registers of the appropriate type.</span></span> |
   | <span data-ttu-id="1b94a-128">**Статус**</span><span class="sxs-lookup"><span data-stu-id="1b94a-128">**Status**</span></span>                                                   | <span data-ttu-id="1b94a-129">В этом поле отображается информация о версии налогового регистра.</span><span class="sxs-lookup"><span data-stu-id="1b94a-129">This field displays information about the version of the tax register.</span></span> |
   | <span data-ttu-id="1b94a-130">**Дата начала, Дата окончания**</span><span class="sxs-lookup"><span data-stu-id="1b94a-130">**Starting Date, Ending Date**</span></span>                               | <span data-ttu-id="1b94a-131">В этом поле отображаются даты, указанные при настройке этой версии налогового регистра.</span><span class="sxs-lookup"><span data-stu-id="1b94a-131">This field displays the dates given when setting the tax register version.</span></span> |

6. <span data-ttu-id="1b94a-132">Выберите **ОК**, чтобы создать налоговый регистр.</span><span class="sxs-lookup"><span data-stu-id="1b94a-132">Choose **OK** to create the tax register.</span></span>

    > :speech_balloon: <span data-ttu-id="1b94a-133">Примечание</span><span class="sxs-lookup"><span data-stu-id="1b94a-133">Note</span></span>
    >
    > <span data-ttu-id="1b94a-134">Если выбрано создание регистра для уже рассчитанного периода, на экран выводится предупреждение.</span><span class="sxs-lookup"><span data-stu-id="1b94a-134">If the creation of registers for an already counted period is selected, a warning is displayed.</span></span> <span data-ttu-id="1b94a-135">На этом этапе создания налогового регистра можно либо продолжить расчет и удалить имеющиеся данные, либо прекратить создание.</span><span class="sxs-lookup"><span data-stu-id="1b94a-135">At this stage of the tax register     > creation, it is possible either to continue counting and delete all existing data, or stop.</span></span>

7. <span data-ttu-id="1b94a-136">Для просмотра результата расчетов в окне **Накопление налогового регистра** выберите **Финансовый менеджмент**, выберите **Налоговый учет**, выберите **Отчетность**, затем выберите **Налог на прибыль**.</span><span class="sxs-lookup"><span data-stu-id="1b94a-136">To view the calculated information in the **Tax Register Accumulation** window, choose **Financial Management**, choose **Tax Accounting**, choose **Reporting,** and then choose **Profit Tax**.</span></span>

8. <span data-ttu-id="1b94a-137">Используя список регистров, можно просматривать содержимое любого регистра; используя стрелки вверху окна, можно просматривать информацию, переходя от одного регистра к другому.</span><span class="sxs-lookup"><span data-stu-id="1b94a-137">Using the register list, you can view the contents of any register or using the arrows at the top of the window, you can view the information going from one register to another.</span></span>

9. <span data-ttu-id="1b94a-138">При помощи стрелок и кнопок в нижнем левом углу окна можно просматривать содержимое регистров для рассчитанных ранее периодов.</span><span class="sxs-lookup"><span data-stu-id="1b94a-138">With the arrows and buttons in the lower-left corner of the window, you can view the contents of the registers for previously counted periods.</span></span>

10. <span data-ttu-id="1b94a-139">Выберите кнопку **Раскрытие** в поле **Сумма** для просмотра источников, на основе которых был выполнен этот расчет.</span><span class="sxs-lookup"><span data-stu-id="1b94a-139">Choose the **Drill-down** button in the **Amount** field to view the sources based on which this was counted.</span></span> <span data-ttu-id="1b94a-140">Источником может являться налоговый регистр или список транзакций, сформировавших эту сумму, в зависимости от настроек.</span><span class="sxs-lookup"><span data-stu-id="1b94a-140">A source can be a tax register or a list of transactions forming this amount, depending on the settings.</span></span> <span data-ttu-id="1b94a-141">Если источником формирования этой суммы является налоговый регистр, выберите кнопку **Раскрытие**, чтобы открыть окно с информацией об исходном налоговом регистре.</span><span class="sxs-lookup"><span data-stu-id="1b94a-141">If the source forming the sum is a tax register, choose the **Drill-down** button to open the window where the source tax register information is displayed.</span></span> <span data-ttu-id="1b94a-142">После этого выберите кнопку **Раскрытие** в поле **Сумма** этой формы, чтобы получить список транзакций, сформировавших данную сумму.</span><span class="sxs-lookup"><span data-stu-id="1b94a-142">Then choose the **Drill-down** button in the **Amount** field on this form to get a list of transactions forming the amount.</span></span>

11. <span data-ttu-id="1b94a-143">Выберите документ и выберите **Навигация**, чтобы получить все транзакции выбранного документа.</span><span class="sxs-lookup"><span data-stu-id="1b94a-143">Select a document and choose **Navigate** to get all the transactions of the selected document.</span></span>

12. <span data-ttu-id="1b94a-144">Выберите **Показать** для просмотра всех транзакций любой созданной книги операций.</span><span class="sxs-lookup"><span data-stu-id="1b94a-144">Choose **Show** to view all the transactions of any entry ledger that is created.</span></span>

## <a name="see-also"></a><span data-ttu-id="1b94a-145">См. также</span><span class="sxs-lookup"><span data-stu-id="1b94a-145">See Also</span></span>

[<span data-ttu-id="1b94a-146">Налоговый учет</span><span class="sxs-lookup"><span data-stu-id="1b94a-146">Tax Accounting</span></span>](Tax-Accounting.md)  
[<span data-ttu-id="1b94a-147">Налоговые регистры</span><span class="sxs-lookup"><span data-stu-id="1b94a-147">Tax Registers</span></span>](Tax-Registers.md)  
[<span data-ttu-id="1b94a-148">Практическое руководство. Настройка секций налогового регистра</span><span class="sxs-lookup"><span data-stu-id="1b94a-148">How to: Set Up Tax Register Sections</span></span>](How-to-Set-Up-Tax-Register-Sections.md)  
[<span data-ttu-id="1b94a-149">Сбор сведений о налоге на прибыль для налоговой декларации</span><span class="sxs-lookup"><span data-stu-id="1b94a-149">Collecting Profit Tax Information for Tax Declaration</span></span>](Collecting-Profit-Tax-Information-for-Tax-Declaration.md)  
