---
title: Как вводить данные в поля | Документы Майкрософт
description: Узнайте об общих функциях, помогающих ввести данные в поля.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: 00143454cf0b0da9b111f92bcdb7879c7e6743d2
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "929077"
---
# <a name="entering-data"></a><span data-ttu-id="14ec3-103">Ввод данных</span><span class="sxs-lookup"><span data-stu-id="14ec3-103">Entering Data</span></span>

<span data-ttu-id="14ec3-104">Имеется много общих функций, помогающих легче, быстрее и точнее вводить данные.</span><span class="sxs-lookup"><span data-stu-id="14ec3-104">There are many general features that help you enter data easier, faster, and more accurate.</span></span> <span data-ttu-id="14ec3-105">Общие функции ввода данных описаны в этой статье.</span><span class="sxs-lookup"><span data-stu-id="14ec3-105">The general features for entering data are described in this article.</span></span>  

<!-- The examples in this article use the demonstration data.-->

## <a name="keyboard-shortcuts"></a><span data-ttu-id="14ec3-106">Сочетания клавиш</span><span class="sxs-lookup"><span data-stu-id="14ec3-106">Keyboard Shortcuts</span></span>

<span data-ttu-id="14ec3-107">Предусмотрено несколько сочетаний клавиш, которые позволяют работать без использования мыши и ускоряют ввод данных, особенно в случае записей большого масштаба и повторяющихся задач ввода.</span><span class="sxs-lookup"><span data-stu-id="14ec3-107">There are several keyboard shortcuts that let you to work "mouse-free" and speed up your data entry, especially with large scale entries and repetitive typing tasks.</span></span>

<span data-ttu-id="14ec3-108">Дополнительные сведения о сочетаниях клавиш см. в разделе [Сочетания клавиш](keyboard-shortcuts.md).</span><span class="sxs-lookup"><span data-stu-id="14ec3-108">For more information about shortcuts, see [Keyboard Shortcuts](keyboard-shortcuts.md).</span></span> <span data-ttu-id="14ec3-109">Некоторые из сочетаний клавиш рассматриваются в этой статье.</span><span class="sxs-lookup"><span data-stu-id="14ec3-109">A few of the shortcuts are discussed in this article.</span></span>

## <a name="QuickEntry"></a><span data-ttu-id="14ec3-110">Ускорение ввода с помощью экспресс-ввода</span><span class="sxs-lookup"><span data-stu-id="14ec3-110">Accelerating Data Entry Using Quick Entry</span></span>

<span data-ttu-id="14ec3-111">Функция экспресс-ввода предназначена для ввода данных при использовании клавиатуры.</span><span class="sxs-lookup"><span data-stu-id="14ec3-111">Quick Entry is a feature designed for data entry when using the keyboard.</span></span> <span data-ttu-id="14ec3-112">Экспресс-ввод работает с полями (например, на страницах карточек) и в списках (строки и столбцы).</span><span class="sxs-lookup"><span data-stu-id="14ec3-112">Quick Entry works on fields (like on card pages) and in lists (rows and columns).</span></span> <span data-ttu-id="14ec3-113">Он полезен при выполнении повторяющихся задач ввода, которые требуют последовательного создания нескольких записей, например партия заказов на продажу или регистрация новых товаров.</span><span class="sxs-lookup"><span data-stu-id="14ec3-113">It is beneficial when performing repetitive typing tasks that require creating multiple records in sequence, such as a batch of sales orders or registering new items.</span></span>

<span data-ttu-id="14ec3-114">Вероятно, вы уже знакомы с использованием клавиши табуляции для перехода из одного поля на странице к следующему редактируемому полю.</span><span class="sxs-lookup"><span data-stu-id="14ec3-114">You might already be familiar with using the Tab key to navigate from one field on a page to the next editable field.</span></span> <span data-ttu-id="14ec3-115">Недостаток использования клавиши табуляции заключается в том, что по ней всегда производится последовательный переход к следующему полю.</span><span class="sxs-lookup"><span data-stu-id="14ec3-115">A disadvantage of using Tab is that it always goes sequentially to the next field.</span></span> <!-- even if the field is non-editable or seldom filled it in.--><span data-ttu-id="14ec3-116">Экспресс-ввод, позволяет изменить этот путь.</span><span class="sxs-lookup"><span data-stu-id="14ec3-116">Quick Entry lets you change this path.</span></span> <span data-ttu-id="14ec3-117">При экспресс-вводе используется клавиша ВВОД для переход только между теми полями, которые вам нужны, пропуская все недоступные для редактирования поля и поля, которые обычно не заполняются.</span><span class="sxs-lookup"><span data-stu-id="14ec3-117">With Quick Entry, you use the Enter key to navigate through only those fields that you are interested in, skipping non-editable fields and fields that you typically do not fill in.</span></span> <span data-ttu-id="14ec3-118">Возможно, вы уже заметили такое поведение на некоторых страницах.</span><span class="sxs-lookup"><span data-stu-id="14ec3-118">You might have already noticed this behavior on some pages.</span></span> <span data-ttu-id="14ec3-119">Это происходит из-за того, что в приложении уже назначено, какие поля включать при нажатии клавиши ВВОД, а какие пропускать.</span><span class="sxs-lookup"><span data-stu-id="14ec3-119">This is because the application already designates which fields to include when pressing Enter and which ones to skip.</span></span> <span data-ttu-id="14ec3-120">Экспресс-ввод можно настроить, персонализировав рабочую область и выполнив оптимизацию способа ввода данных на каждой странице.</span><span class="sxs-lookup"><span data-stu-id="14ec3-120">You can customize Quick Entry by personalizing your workspace and optimizing how you enter data on each page.</span></span>

### <a name="how-quick-entry-works"></a><span data-ttu-id="14ec3-121">Как работает экспресс-ввод</span><span class="sxs-lookup"><span data-stu-id="14ec3-121">How Quick Entry Works</span></span>

<span data-ttu-id="14ec3-122">Каждое поле может быть помечено как *включенное в экспресс-ввод* или как *исключенное из экспресс-ввода*.</span><span class="sxs-lookup"><span data-stu-id="14ec3-122">Every field can be marked as either being *included in Quick Entry* or *excluded from Quick Entry*.</span></span> <span data-ttu-id="14ec3-123">Поля, которые включены в экспресс-ввод, будут включены в путь при нажатии клавиши ВВОД; поля, исключенные из экспресс-ввода, не включаются.</span><span class="sxs-lookup"><span data-stu-id="14ec3-123">Fields that are included in Quick Entry, will be included in the path when you press Enter; fields that are excluded from Quick Entry, will not.</span></span>

<span data-ttu-id="14ec3-124">После завершения ввода данных в поле, вы просто нажимаете клавишу ВВОД для подтверждения изменений и переходите к следующему полю.</span><span class="sxs-lookup"><span data-stu-id="14ec3-124">When you are finished entering data in a field, you simply press Enter to confirm the changes and go to the next field.</span></span> <span data-ttu-id="14ec3-125">Если требуется обратить направление и перейти к предыдущему полю, нажмите Shift+ВВОД.</span><span class="sxs-lookup"><span data-stu-id="14ec3-125">If you want to reverse direction, and go the previous field, press Shift+Enter.</span></span> <span data-ttu-id="14ec3-126">Дополнительные сведения о сочетаниях клавиш см. в разделе [Сочетания клавиш экспресс-ввода](keyboard-shortcuts.md#QuickEntry).</span><span class="sxs-lookup"><span data-stu-id="14ec3-126">For more information about shortcuts, see [Quick Entry keyboard shortcuts](keyboard-shortcuts.md#QuickEntry).</span></span>

#### <a name="tips-and-tricks"></a><span data-ttu-id="14ec3-127">Советы и подсказки</span><span class="sxs-lookup"><span data-stu-id="14ec3-127">Tips and tricks</span></span>
<span data-ttu-id="14ec3-128">Ниже приводятся некоторые полезные сведения об использовании экспресс-ввода.</span><span class="sxs-lookup"><span data-stu-id="14ec3-128">The following provides some useful information about using Quick Entry.</span></span>

- <span data-ttu-id="14ec3-129">Он доступен для всех полей, которые можно редактировать.</span><span class="sxs-lookup"><span data-stu-id="14ec3-129">It is available for any editable fields.</span></span>
- <span data-ttu-id="14ec3-130">Он также работает между столбцами и строками.</span><span class="sxs-lookup"><span data-stu-id="14ec3-130">It also works across columns and rows.</span></span>
- <span data-ttu-id="14ec3-131">Он не запрещает доступ к другим элементам страницы, таким как действия.</span><span class="sxs-lookup"><span data-stu-id="14ec3-131">It does not prevent accessing other elements of a page, such as actions.</span></span> <span data-ttu-id="14ec3-132">Они по-прежнему доступны с помощью клавиш Tab и Shift+Tab.</span><span class="sxs-lookup"><span data-stu-id="14ec3-132">These are still accessible by using Tab and Shift+Tab.</span></span>  
- <span data-ttu-id="14ec3-133">Для работы экспресс-ввода экспресс-вкладки не обязательно должны быть развернутыми.</span><span class="sxs-lookup"><span data-stu-id="14ec3-133">FastTabs do not have to be expanded for Quick Entry to work.</span></span> <span data-ttu-id="14ec3-134">Если следующее поле экспресс-ввода находится на свернутой экспресс-вкладке, эта экспресс-вкладка автоматически разворачивается с фокусом на назначенном поле.</span><span class="sxs-lookup"><span data-stu-id="14ec3-134">If the next Quick Entry field is located in a collapsed FastTab, that FastTab will automatically expand and focus on the designated field.</span></span>
- <span data-ttu-id="14ec3-135">Экспресс-ввод работает независимо от того, являются ли поля обязательными.</span><span class="sxs-lookup"><span data-stu-id="14ec3-135">Quick Entry works irrespective of whether fields are mandatory.</span></span> <span data-ttu-id="14ec3-136">Поэтому рекомендуется убедиться, что обязательные поля включены в экспресс-ввод.</span><span class="sxs-lookup"><span data-stu-id="14ec3-136">So it is a good idea to ensure that mandatory fields are included in Quick Entry.</span></span>
- <span data-ttu-id="14ec3-137">По умолчанию большинство полей включено в экспресс-ввод.</span><span class="sxs-lookup"><span data-stu-id="14ec3-137">By default, most fields are automatically included in Quick Entry.</span></span> <span data-ttu-id="14ec3-138">Поэтому сначала вам скорее всего потребуется исключать поля из экспресс-ввода.</span><span class="sxs-lookup"><span data-stu-id="14ec3-138">So initially your task will most likely be excluding fields from Quick Entry.</span></span>

### <a name="how-to-change-quick-entry-fields"></a><span data-ttu-id="14ec3-139">Изменение полей экспресс-ввода</span><span class="sxs-lookup"><span data-stu-id="14ec3-139">How to Change Quick Entry Fields</span></span>

<span data-ttu-id="14ec3-140">Для изменения того, какие поля на странице включены в экспресс-ввод или исключены из него, следует использовать персонализацию.</span><span class="sxs-lookup"><span data-stu-id="14ec3-140">To change which fields are included in or excluded from Quick Entry on a page, you use personalization.</span></span>

1. <span data-ttu-id="14ec3-141">Для начала персонализации выберите ![Настройка](media/ui-experience/settings_icon_small.png "Значок настроек для ролевого центра"), затем **Персонализировать**.</span><span class="sxs-lookup"><span data-stu-id="14ec3-141">Start personalization by selecting the ![Settings](media/ui-experience/settings_icon_small.png "Settings icon for role center") icon, and then **Personalize**.</span></span>
2. <span data-ttu-id="14ec3-142">Выберите поле, которое необходимо изменить, или в списках, выберите соответствующий заголовок столбца, затем выберите **Включить в экспресс-ввод** или **Исключить из экспресс-ввода**.</span><span class="sxs-lookup"><span data-stu-id="14ec3-142">Select a field that you want change, or in lists, select the corresponding column heading, and then choose either **Include in Quick Entry** or **Exclude from Quick Entry**.</span></span>

<span data-ttu-id="14ec3-143">Дополнительные сведения о персонализации см. в разделе [Персонализация рабочей области](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="14ec3-143">For more information about personalization, see [Personalizing Your Workspace](ui-personalization-user.md).</span></span>

## <a name="mandatory-fields"></a><span data-ttu-id="14ec3-144">Обязательные поля</span><span class="sxs-lookup"><span data-stu-id="14ec3-144">Mandatory Fields</span></span>

<span data-ttu-id="14ec3-145">При вводе данных на страницах некоторые поля помечаются красной звездочкой.</span><span class="sxs-lookup"><span data-stu-id="14ec3-145">When you enter data on pages, certain fields are marked with a red asterisk.</span></span> <span data-ttu-id="14ec3-146">Красная звездочка означает, что необходимо заполнить поле, чтобы завершить определенную процедуру, в которой используется это поле, например учесть транзакцию, в которой используется значение в поле.</span><span class="sxs-lookup"><span data-stu-id="14ec3-146">The red asterisk means that the field must be filled to complete a certain process that uses the field, such as posting a transaction that uses the value in the field.</span></span>  

<span data-ttu-id="14ec3-147">Даже если в поле содержится красная звездочка, не обязательно заполнять поле, чтобы перейти к другим полям или закрыть страницу.</span><span class="sxs-lookup"><span data-stu-id="14ec3-147">Even though the field contains a red asterisk, you are not forced to fill the field before you continue to other fields or close the page.</span></span> <span data-ttu-id="14ec3-148">Красная звездочка исключительно служит напоминанием, что определенный процесс будет заблокирован.</span><span class="sxs-lookup"><span data-stu-id="14ec3-148">The red asterisk only serves as a reminder that you will be blocked from completing a certain process.</span></span>  

## <a name="finding-data-as-you-type"></a><span data-ttu-id="14ec3-149">Поиск данных по мере ввода</span><span class="sxs-lookup"><span data-stu-id="14ec3-149">Finding Data As You Type</span></span>

 <span data-ttu-id="14ec3-150">С началом ввода символов в поле отображается раскрывающийся список с возможными значениями.</span><span class="sxs-lookup"><span data-stu-id="14ec3-150">When you start to type characters in a field, a drop-down list is displayed and shows possible field values.</span></span> <span data-ttu-id="14ec3-151">Содержимое списка меняется по мере ввода, и когда в нем отобразится нужное значение, его можно будет выбрать.</span><span class="sxs-lookup"><span data-stu-id="14ec3-151">The list changes as you type more characters, and you can select the correct value when it is displayed.</span></span>  

 <span data-ttu-id="14ec3-152">Многие поля содержат кнопку со стрелкой вниз, которую можно выбрать.</span><span class="sxs-lookup"><span data-stu-id="14ec3-152">Many fields have a down arrow button that you can choose.</span></span> <span data-ttu-id="14ec3-153">При выборе этой стрелки отображается список данных, которые можно ввести в этом поле.</span><span class="sxs-lookup"><span data-stu-id="14ec3-153">You choose the arrow to get a list of data that is available to enter in the field.</span></span> <span data-ttu-id="14ec3-154">В зависимости от типа поля эта кнопка выполняет две функции:</span><span class="sxs-lookup"><span data-stu-id="14ec3-154">The button has two functions depending on the type of field:</span></span>  

-   <span data-ttu-id="14ec3-155">Поиск: отображение информации из другой таблицы, которую можно ввести в данное поле.</span><span class="sxs-lookup"><span data-stu-id="14ec3-155">Lookup - Displays information from another table that you can enter in the field.</span></span> <span data-ttu-id="14ec3-156">Одновременно можно выбрать только один фрагмент данных.</span><span class="sxs-lookup"><span data-stu-id="14ec3-156">You can select one piece of data at a time.</span></span>  

-   <span data-ttu-id="14ec3-157">Раскрывающийся список — отображает набор существующих параметров для поля.</span><span class="sxs-lookup"><span data-stu-id="14ec3-157">Drop-down - Displays the set of options that exist for the field.</span></span> <span data-ttu-id="14ec3-158">Можно выбрать только один параметр.</span><span class="sxs-lookup"><span data-stu-id="14ec3-158">You can select only one of the options.</span></span>  

## <a name="copying-and-pasting-fields-and-lines"></a><span data-ttu-id="14ec3-159">Копирование и вставка полей и строк</span><span class="sxs-lookup"><span data-stu-id="14ec3-159">Copying and Pasting Fields and Lines</span></span>

<span data-ttu-id="14ec3-160">Можно скопировать один или несколько строк из списка или одно поле на странице, а затем вставить скопированное на ту же страницу, другую страницу или во внешний документ (например, Microsoft Excel или сообщение электронной почты Outlook).</span><span class="sxs-lookup"><span data-stu-id="14ec3-160">You can copy one or more rows from a list or a single field on a page, and then paste what you copied into the same page, another page, or an external document (like Microsoft Excel and Outlook email).</span></span> <span data-ttu-id="14ec3-161">Вкратце, чтобы скопировать, нажмите CTRL+C (cmd+C в macOS) на клавиатуре.</span><span class="sxs-lookup"><span data-stu-id="14ec3-161">In short, to copy, you press CTRL+C (cmd+C in macOS) on your keyboard.</span></span> <span data-ttu-id="14ec3-162">Для вставки нажмите CTRL+V (cmd+V в macOS).</span><span class="sxs-lookup"><span data-stu-id="14ec3-162">To paste, you press CTRL+V (cmd+V in macOS).</span></span>

<span data-ttu-id="14ec3-163">В списке чтобы скопировать поле в том же столбце строки выше и вставить его в текущую строку, просто нажмите F8.</span><span class="sxs-lookup"><span data-stu-id="14ec3-163">In a list, to copy the field in the same column of the row above, and paste it into the current row, just press F8.</span></span>

<span data-ttu-id="14ec3-164">Дополнительную информацию см. в разделе [Копирование и вставка в Business Central](ui-copy-paste.md).</span><span class="sxs-lookup"><span data-stu-id="14ec3-164">For more information, see [Copying and Pasting in Business Central](ui-copy-paste.md).</span></span>

## <a name="Focus"></a><span data-ttu-id="14ec3-165">Фокусировка на позициях строк</span><span class="sxs-lookup"><span data-stu-id="14ec3-165">Focusing on Line Items</span></span>

<span data-ttu-id="14ec3-166">При работе в документах, которые содержат часть с элементами строк, такими как заказ на продажу или страница счетов, можно переключить представление, значительно расширяя часть позиций строк, чтобы она занимала значительную часть всей рабочей области — скрывая другие части страницы, за исключением области действий в верхней части.</span><span class="sxs-lookup"><span data-stu-id="14ec3-166">When working on documents that include a line items part, like a sales order or invoice page, you can switch your view to focus only on the line items, essentially expanding the line items part so that it occupies pretty much the entire workspace - hiding other parts of the page except the actions area at the top.</span></span> <span data-ttu-id="14ec3-167">Это дает лучший обзор позиций строк, а также обеспечивает больше места для работы с ними.</span><span class="sxs-lookup"><span data-stu-id="14ec3-167">This gives you a better overview of the lines items, and provides more room to work on them.</span></span> <span data-ttu-id="14ec3-168">Это особенно полезно, если при работе с большими списками позиций строк требуется быстрый ввода данных.</span><span class="sxs-lookup"><span data-stu-id="14ec3-168">This is particularly beneficial when working with large line item lists and fast data entry is desired.</span></span>

<span data-ttu-id="14ec3-169">Другое преимущество заключается в том, что она также предоставляет дополнительные возможности фильтрации, такие как другие списки, чтобы просмотр и поиск в позициях строк были еще проще.</span><span class="sxs-lookup"><span data-stu-id="14ec3-169">Another advantage is that it also provides advanced filtering capability, like on other lists, so browsing and searching through line items becomes even easier.</span></span>

### <a name="switch-the-focus-on-and-off"></a><span data-ttu-id="14ec3-170">Включение и выключение фокусировки</span><span class="sxs-lookup"><span data-stu-id="14ec3-170">Switch the Focus On and Off</span></span>

<span data-ttu-id="14ec3-171">Чтобы сфокусироваться на позиции строки, выберите в любом месте части позиций строк, затем выберите ![Значок режима фокусировки](media/focus-mode.png "Значок режима фокусировки") в правом верхнем углу или нажмите клавиши Ctrl+Shift+F12.</span><span class="sxs-lookup"><span data-stu-id="14ec3-171">To focus on lines items, select anywhere in the line item part, and then choose ![Focus Mode icon](media/focus-mode.png "Focus mode icon") in the upper right corner or press Ctrl+Shift+F12.</span></span>

<span data-ttu-id="14ec3-172">Чтобы перейти обратно в обычное представление, снова выберите ![Значок режима фокусировки](media/focus-mode.png "Значок режима фокусировки") или нажмите клавиши Ctrl+Shift+F12.</span><span class="sxs-lookup"><span data-stu-id="14ec3-172">To switch back to the normal view, choose ![Focus Mode icon](media/focus-mode.png "Focus mode icon") or press Ctrl+Shift+F12 again.</span></span>

### <a name="filtering-the-line-items"></a><span data-ttu-id="14ec3-173">Фильтрация позиций строк</span><span class="sxs-lookup"><span data-stu-id="14ec3-173">Filtering the Line Items</span></span>

<span data-ttu-id="14ec3-174">Чтобы начать фильтрацию, выберите ![Значок области фильтрации](media/open-filter-pane-icon.png "Значок области фильтрации") вверху списка или нажмите клавиши **Shift+F3**, чтобы открыть область фильтрации.</span><span class="sxs-lookup"><span data-stu-id="14ec3-174">To start filtering, select ![Filter pane icon](media/open-filter-pane-icon.png "Filter pane icon") at the top of the list or press **Shift+F3** to open the filter pane.</span></span> <span data-ttu-id="14ec3-175">Вы работаете с областью фильтров точно также, как и случае любого другого списка.</span><span class="sxs-lookup"><span data-stu-id="14ec3-175">You work with the filter pane as you do on any other list.</span></span> <span data-ttu-id="14ec3-176">Дополнительные сведения см. в разделе [Фильтрация](ui-enter-criteria-filters.md#Filtering).</span><span class="sxs-lookup"><span data-stu-id="14ec3-176">For more information, see [Filtering](ui-enter-criteria-filters.md#Filtering).</span></span>

<span data-ttu-id="14ec3-177">Фильтрация особенно полезна при просмотре и анализе длинных документов.</span><span class="sxs-lookup"><span data-stu-id="14ec3-177">Filtering is especially helpful when viewing and analysing longer documents.</span></span> <span data-ttu-id="14ec3-178">Например, представьте, что вы открыли учтенный счет продажи и фильтруете позиции строк, чтобы отобразить все позиции строк с индивидуальной скидкой более 5% или фильтруете для отображения только принадлежностей для велосипеда со словом "Pro" в названии.</span><span class="sxs-lookup"><span data-stu-id="14ec3-178">For example, imagine you open a posted sales invoice and filter the line items to display all line items that have an individual discount above 5%, or filter to display only bike accessories with 'pro' in the name.</span></span>

## <a name="entering-quantities-by-calculation"></a><span data-ttu-id="14ec3-179">Ввод количества путем вычисления</span><span class="sxs-lookup"><span data-stu-id="14ec3-179">Entering Quantities by Calculation</span></span>

<span data-ttu-id="14ec3-180">При вводе чисел в поля количества, например в поле **Кол-во** в строке журнала товаров, вместо суммарного количества можно ввести формулу.</span><span class="sxs-lookup"><span data-stu-id="14ec3-180">When entering numbers into quantity fields, such as the **Quantity** field on an item journal line, you can enter the formula instead of the sum quantity.</span></span>  

### <a name="examples"></a><span data-ttu-id="14ec3-181">Примеры</span><span class="sxs-lookup"><span data-stu-id="14ec3-181">Examples</span></span>  

-   <span data-ttu-id="14ec3-182">Если ввести 19+19, вычисленное значение поля будет равняться 38.</span><span class="sxs-lookup"><span data-stu-id="14ec3-182">If you enter 19+19, the field is calculated to 38.</span></span>  

-   <span data-ttu-id="14ec3-183">Если ввести 41-9, вычисленное значение поля будет равняться 32.</span><span class="sxs-lookup"><span data-stu-id="14ec3-183">If you enter 41-9, the field is calculated to 32.</span></span>  

-   <span data-ttu-id="14ec3-184">Если ввести 12\*4, вычисленное значение поля будет равняться 48.</span><span class="sxs-lookup"><span data-stu-id="14ec3-184">If you enter 12\*4, the field is calculated to 48.</span></span>  

-   <span data-ttu-id="14ec3-185">Если ввести 12/4, вычисленное значение поля будет равняться 3.</span><span class="sxs-lookup"><span data-stu-id="14ec3-185">If you enter 12/4, the field is calculated to 3.</span></span>  

## <a name="entering-negative-numbers"></a><span data-ttu-id="14ec3-186">Ввод отрицательных чисел</span><span class="sxs-lookup"><span data-stu-id="14ec3-186">Entering Negative Numbers</span></span>

<span data-ttu-id="14ec3-187">Отрицательные числа можно ввести двумя способами.</span><span class="sxs-lookup"><span data-stu-id="14ec3-187">You can enter negative numbers in two ways.</span></span> <span data-ttu-id="14ec3-188">Число -20,5 можно ввести следующим образом:</span><span class="sxs-lookup"><span data-stu-id="14ec3-188">The number -20.5 can be entered as:</span></span>  

-   <span data-ttu-id="14ec3-189">-20,5</span><span class="sxs-lookup"><span data-stu-id="14ec3-189">-20.5</span></span>  

    <span data-ttu-id="14ec3-190">Или</span><span class="sxs-lookup"><span data-stu-id="14ec3-190">or</span></span>
-   <span data-ttu-id="14ec3-191">20,5-</span><span class="sxs-lookup"><span data-stu-id="14ec3-191">20.5-</span></span>  

 <span data-ttu-id="14ec3-192">В обоих случаях сумма будет записана как -20,5.</span><span class="sxs-lookup"><span data-stu-id="14ec3-192">In both cases, the amount will be recorded in as -20.5.</span></span>  

 <span data-ttu-id="14ec3-193">Если последний символ в выражении представляет собой **+** или **-**, все выражение будет записано с данным знаком.</span><span class="sxs-lookup"><span data-stu-id="14ec3-193">If the last character of the expression is a **+** or a **-**, the entire expression will be recorded with that sign.</span></span> <span data-ttu-id="14ec3-194">Например, **10-20+** приведет к значению 10, а не -10.</span><span class="sxs-lookup"><span data-stu-id="14ec3-194">An example, **10-20+** will result in 10 and not -10.</span></span>  

## <a name="entering-dates-and-times"></a><span data-ttu-id="14ec3-195">Ввода дат и времени</span><span class="sxs-lookup"><span data-stu-id="14ec3-195">Entering Dates and Times</span></span>

<span data-ttu-id="14ec3-196">Дату и время можно вводить во всех полях, которые специально предназначены для дат (полях дат).</span><span class="sxs-lookup"><span data-stu-id="14ec3-196">You can enter dates and times in all the fields that are specifically assigned to dates (date fields).</span></span> <span data-ttu-id="14ec3-197">Даты можно вводить с разделителями и без них.</span><span class="sxs-lookup"><span data-stu-id="14ec3-197">You can enter dates with or without separators.</span></span>

> [!NOTE]  
> <span data-ttu-id="14ec3-198">Способ ввода дат и времени зависит от настроек **Регион**.</span><span class="sxs-lookup"><span data-stu-id="14ec3-198">How you enter dates and times depends on your **Region** settings.</span></span> <span data-ttu-id="14ec3-199">Дополнительные сведения см. в разделе [Изменение базовых настроек](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="14ec3-199">For more information, see [Changing Basic Settings](ui-change-basic-settings.md).</span></span>  

### <a name="entering-dates"></a><span data-ttu-id="14ec3-200">Ввод дат</span><span class="sxs-lookup"><span data-stu-id="14ec3-200">Entering Dates</span></span>

<span data-ttu-id="14ec3-201">Чтобы задавать дату в полях, можно использовать средство выбора даты, которое позволяет выбрать дату в календаре, или ввести даты вручную.</span><span class="sxs-lookup"><span data-stu-id="14ec3-201">For date fields, you can either use the data picker, which lets you select a date from a calender, or you can enter dates manually.</span></span> <span data-ttu-id="14ec3-202">В этом разделе представлен быстрый обзор порядка ввода дат.</span><span class="sxs-lookup"><span data-stu-id="14ec3-202">This section provides a brief overview of how to enter dates.</span></span> <span data-ttu-id="14ec3-203">Дополнительные сведения см. в разделе [Работа с календарными датами и значениями времени](ui-enter-date-ranges.md).</span><span class="sxs-lookup"><span data-stu-id="14ec3-203">For more details, see [Working with Calendar Dates and Times](ui-enter-date-ranges.md).</span></span>

<span data-ttu-id="14ec3-204">Для ввода даты вручную можно ввести две, четыре, шесть или восемь цифр:</span><span class="sxs-lookup"><span data-stu-id="14ec3-204">For manually date entry, you can enter two, four, six, or eight digits:</span></span>  

-   <span data-ttu-id="14ec3-205">Если введены только две цифры, они будут интерпретированы как день, а месяц и год будут добавлены к рабочей даты.</span><span class="sxs-lookup"><span data-stu-id="14ec3-205">If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.</span></span>  

-   <span data-ttu-id="14ec3-206">Если введены четыре цифры, они будут интерпретированы как день и месяц, к которым будет добавлен год рабочей даты.</span><span class="sxs-lookup"><span data-stu-id="14ec3-206">If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.</span></span>  

-   <span data-ttu-id="14ec3-207">При вводе даты в интервале от 01.01.1930 до 31.12.2029 можно ввести две цифры года; в противном случае необходимо ввести все четыре цифры.</span><span class="sxs-lookup"><span data-stu-id="14ec3-207">If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.</span></span>  

<span data-ttu-id="14ec3-208">В качестве даты можно также ввести название дня недели, за которым следует номер недели и (необязательно) год (например, значение «Пн25» или «пн25» указывает на понедельник 25-й недели года).</span><span class="sxs-lookup"><span data-stu-id="14ec3-208">You can also enter a date as a weekday followed by a week number and, optionally, a year (for example, Mon25 or mon25 means Monday in week 25).</span></span>  

<span data-ttu-id="14ec3-209">Вместо ввода определенной даты можно ввести один из следующих кодов.</span><span class="sxs-lookup"><span data-stu-id="14ec3-209">Instead of entering a specific date, you can enter one of these codes.</span></span>  

|<span data-ttu-id="14ec3-210">Код</span><span class="sxs-lookup"><span data-stu-id="14ec3-210">Code</span></span>|<span data-ttu-id="14ec3-211">Результат</span><span class="sxs-lookup"><span data-stu-id="14ec3-211">Result</span></span>|  
|--------------|----------------|  
|<span data-ttu-id="14ec3-212">t</span><span class="sxs-lookup"><span data-stu-id="14ec3-212">t</span></span>|<span data-ttu-id="14ec3-213">Это указывает текущую дату (системная дата компьютера).</span><span class="sxs-lookup"><span data-stu-id="14ec3-213">This specifies today's date (the system date for the computer).</span></span>|  
|<span data-ttu-id="14ec3-214">p</span><span class="sxs-lookup"><span data-stu-id="14ec3-214">p</span></span>|<span data-ttu-id="14ec3-215">Это определяет учетный период, где `p` означает первый учетный период, `p2` означает второй учетный период и так далее.</span><span class="sxs-lookup"><span data-stu-id="14ec3-215">This specifies an accounting period´, where `p`means the first accounting period, `p2` means the second accountin period, and so on.</span></span> |
|<span data-ttu-id="14ec3-216">w</span><span class="sxs-lookup"><span data-stu-id="14ec3-216">w</span></span>|<span data-ttu-id="14ec3-217">Это задает рабочую дату, которая настроена в приложении.</span><span class="sxs-lookup"><span data-stu-id="14ec3-217">This specifies the work date that is setup in the application.</span></span> <span data-ttu-id="14ec3-218">Для изменения рабочей даты см. раздел [Изменение базовых настроек](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="14ec3-218">To change the work date, see [Changing Basic Settings](ui-change-basic-settings.md).</span></span> <span data-ttu-id="14ec3-219">Необходимость в использовании рабочей даты возникает при наличии большого количества транзакций, дата которых отличается от текущей.</span><span class="sxs-lookup"><span data-stu-id="14ec3-219">You may want to use a work date if you have many transactions with a date other than today's date.</span></span>|
|<span data-ttu-id="14ec3-220">c</span><span class="sxs-lookup"><span data-stu-id="14ec3-220">c</span></span>|<span data-ttu-id="14ec3-221">Это задает, что дата после `c` является датой закрытия, например `C123101`.</span><span class="sxs-lookup"><span data-stu-id="14ec3-221">This specifies that the date after `c`is a closing date, for example `C123101`.</span></span>|  

## <a name="entering-times"></a><span data-ttu-id="14ec3-222">Ввод времени</span><span class="sxs-lookup"><span data-stu-id="14ec3-222">Entering Times</span></span>

<span data-ttu-id="14ec3-223">При вводе времени можно вставить любой разделитель между единицами измерения, но это не обязательно.</span><span class="sxs-lookup"><span data-stu-id="14ec3-223">When you enter times, you can insert any separator sign that you want between the units, but it is not required.</span></span> <span data-ttu-id="14ec3-224">Минуты и секунды можно не указывать.</span><span class="sxs-lookup"><span data-stu-id="14ec3-224">You do not have to write minutes, seconds, or AM/PM.</span></span>  

<span data-ttu-id="14ec3-225">В следующей таблице представлены способы ввода времени и их интерпретация.</span><span class="sxs-lookup"><span data-stu-id="14ec3-225">The following table lists the various ways in which times can be entered and how they are interpreted.</span></span>  

|<span data-ttu-id="14ec3-226">Формат ввода</span><span class="sxs-lookup"><span data-stu-id="14ec3-226">Entry</span></span>|<span data-ttu-id="14ec3-227">Интерпретация</span><span class="sxs-lookup"><span data-stu-id="14ec3-227">Interpretation</span></span>|  
|---------------|------------------------|  
|<span data-ttu-id="14ec3-228">5</span><span class="sxs-lookup"><span data-stu-id="14ec3-228">5</span></span>|<span data-ttu-id="14ec3-229">05:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-229">05:00:00</span></span>|  
|<span data-ttu-id="14ec3-230">5:30</span><span class="sxs-lookup"><span data-stu-id="14ec3-230">5:30</span></span>|<span data-ttu-id="14ec3-231">05:30:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-231">05:30:00</span></span>|  
|<span data-ttu-id="14ec3-232">0530</span><span class="sxs-lookup"><span data-stu-id="14ec3-232">0530</span></span>|<span data-ttu-id="14ec3-233">05:30:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-233">05:30:00</span></span>|  
|<span data-ttu-id="14ec3-234">5:30:5</span><span class="sxs-lookup"><span data-stu-id="14ec3-234">5:30:5</span></span>|<span data-ttu-id="14ec3-235">05:30:05</span><span class="sxs-lookup"><span data-stu-id="14ec3-235">05:30:05</span></span>|  
|<span data-ttu-id="14ec3-236">053005</span><span class="sxs-lookup"><span data-stu-id="14ec3-236">053005</span></span>|<span data-ttu-id="14ec3-237">05:30:05</span><span class="sxs-lookup"><span data-stu-id="14ec3-237">05:30:05</span></span>|  
|<span data-ttu-id="14ec3-238">5:30:5,50</span><span class="sxs-lookup"><span data-stu-id="14ec3-238">5:30:5,50</span></span>|<span data-ttu-id="14ec3-239">05:30:05,5</span><span class="sxs-lookup"><span data-stu-id="14ec3-239">05:30:05.5</span></span>|  
|<span data-ttu-id="14ec3-240">053005050</span><span class="sxs-lookup"><span data-stu-id="14ec3-240">053005050</span></span>|<span data-ttu-id="14ec3-241">05:30:05.05</span><span class="sxs-lookup"><span data-stu-id="14ec3-241">05:30:05.05</span></span>|  

 <span data-ttu-id="14ec3-242">Если между единицами измерения времени не вводится разделитель, то для каждой единицы необходимо вводить две цифры.</span><span class="sxs-lookup"><span data-stu-id="14ec3-242">You must enter two digits for each unit of time if you do not enter a separator.</span></span>  

## <a name="entering-datetimes"></a><span data-ttu-id="14ec3-243">Ввод даты и времени</span><span class="sxs-lookup"><span data-stu-id="14ec3-243">Entering Datetimes</span></span>

<span data-ttu-id="14ec3-244">При вводе даты и времени между ними необходимо оставлять пробел.</span><span class="sxs-lookup"><span data-stu-id="14ec3-244">When you enter datetimes you must enter a space between the date and the time.</span></span>  

<span data-ttu-id="14ec3-245">В следующей таблице представлены способы ввода даты и времени и их интерпретация.</span><span class="sxs-lookup"><span data-stu-id="14ec3-245">The following table lists the various ways in which you can enter datetimes and how they are interpreted.</span></span>  

|<span data-ttu-id="14ec3-246">Формат ввода</span><span class="sxs-lookup"><span data-stu-id="14ec3-246">Entry</span></span>|<span data-ttu-id="14ec3-247">Интерпретация</span><span class="sxs-lookup"><span data-stu-id="14ec3-247">Interpretation</span></span>|  
|---------------|------------------------|  
|<span data-ttu-id="14ec3-248">131202 132455</span><span class="sxs-lookup"><span data-stu-id="14ec3-248">131202 132455</span></span>|<span data-ttu-id="14ec3-249">13.12.02 13:24:55</span><span class="sxs-lookup"><span data-stu-id="14ec3-249">13-12-02 13:24:55</span></span>|  
|<span data-ttu-id="14ec3-250">1-12-02 10</span><span class="sxs-lookup"><span data-stu-id="14ec3-250">1-12-02 10</span></span>|<span data-ttu-id="14ec3-251">01.12.02 10:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-251">01-12-02 10:00:00</span></span>|  
|<span data-ttu-id="14ec3-252">1.12.02 5</span><span class="sxs-lookup"><span data-stu-id="14ec3-252">1.12.02 5</span></span>|<span data-ttu-id="14ec3-253">12.01.02 05:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-253">01-12-02 05:00:00</span></span>|  
|<span data-ttu-id="14ec3-254">1.12.02</span><span class="sxs-lookup"><span data-stu-id="14ec3-254">1.12.02</span></span>|<span data-ttu-id="14ec3-255">12.01.02 00:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-255">01-12-02 00:00:00</span></span>|  
|<span data-ttu-id="14ec3-256">11 12</span><span class="sxs-lookup"><span data-stu-id="14ec3-256">11 12</span></span>|<span data-ttu-id="14ec3-257">11-е число текущего месяца и года, 12:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-257">11-current month-current year 12:00:00</span></span>|  
|<span data-ttu-id="14ec3-258">1112 12</span><span class="sxs-lookup"><span data-stu-id="14ec3-258">1112 12</span></span>|<span data-ttu-id="14ec3-259">11 декабря текущего года, 12:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-259">11-12-current year 12:00:00</span></span>|  
|<span data-ttu-id="14ec3-260">t или сегодня</span><span class="sxs-lookup"><span data-stu-id="14ec3-260">t or today</span></span>|<span data-ttu-id="14ec3-261">текущая дата, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-261">today's date 00:00:00</span></span>|  
|<span data-ttu-id="14ec3-262">t время</span><span class="sxs-lookup"><span data-stu-id="14ec3-262">t time</span></span>|<span data-ttu-id="14ec3-263">текущая дата, фактическое время</span><span class="sxs-lookup"><span data-stu-id="14ec3-263">today's date actual time</span></span>|  
|<span data-ttu-id="14ec3-264">t 10:30</span><span class="sxs-lookup"><span data-stu-id="14ec3-264">t 10:30</span></span>|<span data-ttu-id="14ec3-265">текущая дата, 10:30:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-265">today's date 10:30:00</span></span>|  
|<span data-ttu-id="14ec3-266">t 3:3:3</span><span class="sxs-lookup"><span data-stu-id="14ec3-266">t 3:3:3</span></span>|<span data-ttu-id="14ec3-267">текущая дата, 03:03:03</span><span class="sxs-lookup"><span data-stu-id="14ec3-267">today's date 03:03:03</span></span>|  
|<span data-ttu-id="14ec3-268">w или рабочая дата</span><span class="sxs-lookup"><span data-stu-id="14ec3-268">w or workdate</span></span>|<span data-ttu-id="14ec3-269">рабочая дата, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-269">the working date 00:00:00</span></span>|  
|<span data-ttu-id="14ec3-270">m или понедельник</span><span class="sxs-lookup"><span data-stu-id="14ec3-270">m or Monday</span></span>|<span data-ttu-id="14ec3-271">понедельник текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-271">Monday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="14ec3-272">tu или вторник</span><span class="sxs-lookup"><span data-stu-id="14ec3-272">tu or Tuesday</span></span>|<span data-ttu-id="14ec3-273">вторник текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-273">Tuesday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="14ec3-274">we или среда</span><span class="sxs-lookup"><span data-stu-id="14ec3-274">we or Wednesday</span></span>|<span data-ttu-id="14ec3-275">среда текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-275">Wednesday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="14ec3-276">th или четверг</span><span class="sxs-lookup"><span data-stu-id="14ec3-276">th or Thursday</span></span>|<span data-ttu-id="14ec3-277">четверг текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-277">Thursday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="14ec3-278">f или пятница</span><span class="sxs-lookup"><span data-stu-id="14ec3-278">f or Friday</span></span>|<span data-ttu-id="14ec3-279">пятница текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-279">Friday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="14ec3-280">s или суббота</span><span class="sxs-lookup"><span data-stu-id="14ec3-280">s or Saturday</span></span>|<span data-ttu-id="14ec3-281">суббота текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-281">Saturday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="14ec3-282">su или воскресенье</span><span class="sxs-lookup"><span data-stu-id="14ec3-282">su or Sunday</span></span>|<span data-ttu-id="14ec3-283">воскресенье текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-283">Sunday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="14ec3-284">tu 10:30</span><span class="sxs-lookup"><span data-stu-id="14ec3-284">tu 10:30</span></span>|<span data-ttu-id="14ec3-285">вторник текущей недели, 10:30:00</span><span class="sxs-lookup"><span data-stu-id="14ec3-285">Tuesday of the current week 10:30:00</span></span>|  
|<span data-ttu-id="14ec3-286">tu 3:3:3</span><span class="sxs-lookup"><span data-stu-id="14ec3-286">tu 3:3:3</span></span>|<span data-ttu-id="14ec3-287">вторник текущей недели, 03:03:03</span><span class="sxs-lookup"><span data-stu-id="14ec3-287">Tuesday of the current week 03:03:03</span></span>|  

## <a name="entering-duration"></a><span data-ttu-id="14ec3-288">Ввод продолжительности</span><span class="sxs-lookup"><span data-stu-id="14ec3-288">Entering Duration</span></span>

<span data-ttu-id="14ec3-289">Длительность вводится в виде числа, за которым следует единица измерения.</span><span class="sxs-lookup"><span data-stu-id="14ec3-289">You enter a duration as a number followed by its unit of measure.</span></span>  

<span data-ttu-id="14ec3-290">Примеры:</span><span class="sxs-lookup"><span data-stu-id="14ec3-290">Here are some examples.</span></span>  

|<span data-ttu-id="14ec3-291">Длительность</span><span class="sxs-lookup"><span data-stu-id="14ec3-291">Duration</span></span>|<span data-ttu-id="14ec3-292">Единица измерения\*\*</span><span class="sxs-lookup"><span data-stu-id="14ec3-292">Unit of measure\*\*</span></span>|  
|------------------|-------------------------|  
|<span data-ttu-id="14ec3-293">2ч</span><span class="sxs-lookup"><span data-stu-id="14ec3-293">2h</span></span>|<span data-ttu-id="14ec3-294">2 часа</span><span class="sxs-lookup"><span data-stu-id="14ec3-294">2 hrs</span></span>|  
|<span data-ttu-id="14ec3-295">6ч 30мин</span><span class="sxs-lookup"><span data-stu-id="14ec3-295">6h 30 m</span></span>|<span data-ttu-id="14ec3-296">6 часов 30 минут</span><span class="sxs-lookup"><span data-stu-id="14ec3-296">6 hrs 30 mins</span></span>|  
|<span data-ttu-id="14ec3-297">6,5ч</span><span class="sxs-lookup"><span data-stu-id="14ec3-297">6.5h</span></span>|<span data-ttu-id="14ec3-298">6 часов 30 минут</span><span class="sxs-lookup"><span data-stu-id="14ec3-298">6 hrs 30 mins</span></span>|  
|<span data-ttu-id="14ec3-299">90мин</span><span class="sxs-lookup"><span data-stu-id="14ec3-299">90m</span></span>|<span data-ttu-id="14ec3-300">1 час 30 минут</span><span class="sxs-lookup"><span data-stu-id="14ec3-300">1 hr 30 mins</span></span>|  
|<span data-ttu-id="14ec3-301">2дн 6ч 30мин</span><span class="sxs-lookup"><span data-stu-id="14ec3-301">2d 6h 30m</span></span>|<span data-ttu-id="14ec3-302">2 дня 6 часов 30 минут</span><span class="sxs-lookup"><span data-stu-id="14ec3-302">2 days 6 hrs 30 mins</span></span>|  
|<span data-ttu-id="14ec3-303">2дн 6ч 30мин 56сек 600мс</span><span class="sxs-lookup"><span data-stu-id="14ec3-303">2d 6h 30m 56s 600ms</span></span>|<span data-ttu-id="14ec3-304">2 дня 6 часов 30 минут 56 секунд 600 миллисекунд</span><span class="sxs-lookup"><span data-stu-id="14ec3-304">2 days 6 hrs 30 mins 56 secs 600 msecs</span></span>|  

 <span data-ttu-id="14ec3-305">Можно также ввести число; оно будет автоматически преобразовано во временной интервал.</span><span class="sxs-lookup"><span data-stu-id="14ec3-305">You can also enter a number and it is automatically converted to a duration.</span></span> <span data-ttu-id="14ec3-306">При этом по умолчанию используется единица измерения, указанная в поле «Длительность».</span><span class="sxs-lookup"><span data-stu-id="14ec3-306">The number you enter is converted according to the default unit of measure that has been specified for the duration field.</span></span>  

 <span data-ttu-id="14ec3-307">Чтобы узнать, какая единица измерения указана в поле "Длительность", введите любое число и посмотрите, в какую единицу измерения оно преобразуется.</span><span class="sxs-lookup"><span data-stu-id="14ec3-307">To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.</span></span>  

 <span data-ttu-id="14ec3-308">Если по умолчанию используются часы, число 5 будет преобразовано в 5 часов.</span><span class="sxs-lookup"><span data-stu-id="14ec3-308">The number 5 is converted to 5 hrs, if the unit of measure is hours.</span></span>  

<!--OnPrem  ##  <a name="BKMK_SettingDateRanges"></a> Setting Date Ranges  
 You can set filters containing a start date and an end date to display only the data contained in that date range or time interval. Special rules apply to the way you set date ranges.  

|**Meaning**|**Sample expression**|**Entries included**|  
|-----------------|---------------------------|--------------------------|  
|**Equal to**|12 15 00|Only those posted on 12 15 00.|  
|**Interval**|12 15 00..01 15 01<br /><br /> ..12 15 00|Those posted on dates between and including 12 15 00 and 01 15 01.<br /><br /> Those posted on 12 15 00 or earlier.|  
|**Either/or**|12 15 00&#124;12 16 00|Those posted on either 12 15 00 or 12 16 00. If there are entries posted on both days, they will all be displayed.|  

 You can also combine the various format types.  

|**Sample expression**|**Entries included**|  
|---------------------------|--------------------------|  
|12 15 00&#124;12 01 00..12 10 00|Entries posted either on 12 15 00 or on dates between and including 12 01 00 and 12 10 00.|  
|..12 14 00&#124;12 30 00..|Entries posted on 12 14 00 or earlier, or entries posted on 12 30 00 or later - that is, all entries except those posted on dates between and including 12 15 00 and 12 29 00.|

## Using Date Formulas

 A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates. You can enter date formulas in various date calculation fields and in recurring frequency fields in recurring journals.  

> [!NOTE]  
>  In all data formula fields, one day is automatically included to cover today as the day when the period starts. Accordingly, if you enter 1W, for example, then the period is actually eight days because today is included. To specify a period of seven days (one true week) including the period starting date, then you must enter 6D or 1W-1D.  

 Here are some examples of how date formulas can be used:  

-   The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.  

-   The date formula in the Grace Period field for a specified reminder level determines the period of time that must pass from the due date (or from the date of the previous reminder) before a reminder will be created.  

-   The date formula in the Due Date Calculation field determines how to calculate the due date on the reminder.  

 The date calculation formula can contain a maximum of 20 characters, both numbers and letters. You can use the following letters, which are abbreviations for time specifications.  

|||  
|-|-|  
|C|Current|  
|D|Day(s)|  
|W|Week(s)|  
|M|Month(s)|  
|Q|Quarter(s)|  
|Y|Year(s)|  

 You can construct a date formula in three ways.  

 The following example shows how current plus a time unit.  

|||  
|-|-|  
|CW|Current week|  
|CM|Current month|  

 The following example shows how a number and a time unit. A number cannot be larger than 9999.  

|||  
|-|-|  
|10D|10 days from today|  
|2W|2 weeks from today|  

 The following example shows how a time unit and a number.  

|||  
|-|-|  
|D10|The next 10th day of a month|  
|WD4|The next 4th day of a week (Thursday)|  

 The following example shows how you can combine these three forms as needed.  

|||  
|-|-|  
|CM+10D|Current month + 10 days|  

 The following example shows how you can use a minus sign to indicate a date in the past.  

|||  
|-|-|  
|-1Y|1 year ago from today|

[!CAUTION]  
>  If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days. For example, a 1W means seven working days. For more information, see Base Calendar Card.-->

## <a name="see-also"></a><span data-ttu-id="14ec3-309">См. также</span><span class="sxs-lookup"><span data-stu-id="14ec3-309">See Also</span></span>  
 [<span data-ttu-id="14ec3-310">Сортировка, поиск и фильтрация списков</span><span class="sxs-lookup"><span data-stu-id="14ec3-310">Sorting, Searching, and Filtering Lists</span></span>](ui-enter-criteria-filters.md)  
 <span data-ttu-id="14ec3-311">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="14ec3-311">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
