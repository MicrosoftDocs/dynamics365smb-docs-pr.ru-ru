---
title: Расчет налога на имущество в России
description: Российские усовершенствования включают расчет налога на имущество.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 7654a860a04eec36489df3cad8a9d5f25889c535
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5382075"
---
# <a name="calculate-assessed-tax"></a><span data-ttu-id="80d54-103">Расчет налога на имущество</span><span class="sxs-lookup"><span data-stu-id="80d54-103">Calculate Assessed Tax</span></span>

<span data-ttu-id="80d54-104">Функция налога на имущество позволяет рассчитывать налог на имущество для основных средств.</span><span class="sxs-lookup"><span data-stu-id="80d54-104">The assessed tax feature enables you to calculate the assessed tax for fixed assets.</span></span> <span data-ttu-id="80d54-105">Налог на имущество рассчитывается на основе данных окна **Настройка модуля ОС**.</span><span class="sxs-lookup"><span data-stu-id="80d54-105">The assessed tax is based on the information provided in the **Fixed Asset Setup** window.</span></span> <span data-ttu-id="80d54-106">Также имеется возможность экспортировать результаты расчета налога в виде шаблона Microsoft Office Excel.</span><span class="sxs-lookup"><span data-stu-id="80d54-106">You can also export the results of the calculated tax as a Microsoft Office Excel template.</span></span>

<span data-ttu-id="80d54-107">Для работы с функцией расчета налога на имущество необходимо указать следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="80d54-107">To work with the functionality of calculating assessed tax, you must specify the following settings:</span></span>

<span data-ttu-id="80d54-108">\-параметры на странице **Настройка модуля ОС**</span><span class="sxs-lookup"><span data-stu-id="80d54-108">\- parameters in the **Fixed Asset Setup** page</span></span>

<span data-ttu-id="80d54-109">\- создать и заполнить страницу **Налоговые органы**</span><span class="sxs-lookup"><span data-stu-id="80d54-109">\- create and fill **Tax authorities** page</span></span>

<span data-ttu-id="80d54-110">\- заполнить информацию об организации</span><span class="sxs-lookup"><span data-stu-id="80d54-110">\- fill in information about the organization</span></span>

<span data-ttu-id="80d54-111">\- создать текущие каталоги</span><span class="sxs-lookup"><span data-stu-id="80d54-111">\- create current directories</span></span>

<span data-ttu-id="80d54-112">\- заполнить параметры в карточках основных средств</span><span class="sxs-lookup"><span data-stu-id="80d54-112">\- fill in the parameters in the fixed asset cards</span></span>

## <a name="to-calculate-assessed-tax"></a><span data-ttu-id="80d54-113">Расчет налога на имущество</span><span class="sxs-lookup"><span data-stu-id="80d54-113">To calculate assessed tax</span></span>

1. <span data-ttu-id="80d54-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Льготы по налогу на имущество**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="80d54-114">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assessed Tax Allowances**, and then choose the related link.</span></span>

2. <span data-ttu-id="80d54-115">Заполните поля в окне **Льготы по налогу на имущество**, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="80d54-115">In the **Assessed Tax Allowances** window, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="80d54-116">Поле</span><span class="sxs-lookup"><span data-stu-id="80d54-116">Field</span></span>    | <span data-ttu-id="80d54-117">Описание</span><span class="sxs-lookup"><span data-stu-id="80d54-117">Description</span></span>                                                  |
   | :------- | :----------------------------------------------------------- |
   | <span data-ttu-id="80d54-118">**Код**</span><span class="sxs-lookup"><span data-stu-id="80d54-118">**Code**</span></span> | <span data-ttu-id="80d54-119">Определяет код налога на имущество, связанного с основным средством.</span><span class="sxs-lookup"><span data-stu-id="80d54-119">Specifies the code for the assessed tax that is associated with the fixed asset.</span></span> |
   | <span data-ttu-id="80d54-120">**Название**</span><span class="sxs-lookup"><span data-stu-id="80d54-120">**Name**</span></span> | <span data-ttu-id="80d54-121">Определяет имя кода налога на имущество.</span><span class="sxs-lookup"><span data-stu-id="80d54-121">Specifies the name of the assessed tax code.</span></span>                 |

3. <span data-ttu-id="80d54-122">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="80d54-122">Choose the **OK** button.</span></span>

4. <span data-ttu-id="80d54-123">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Коды налога на имущество**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="80d54-123">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assessed Tax Codes**, and then choose the related link.</span></span>

5. <span data-ttu-id="80d54-124">Заполните поля в окне **Коды налога на имущество**, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="80d54-124">In the **Assessed Tax Codes** window, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="80d54-125">Поле</span><span class="sxs-lookup"><span data-stu-id="80d54-125">Field</span></span>                              | <span data-ttu-id="80d54-126">Описание</span><span class="sxs-lookup"><span data-stu-id="80d54-126">Description</span></span>                                                  |
   | :--------------------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="80d54-127">**Код**</span><span class="sxs-lookup"><span data-stu-id="80d54-127">**Code**</span></span>                           | <span data-ttu-id="80d54-128">Определяет код льготы по налогу на имущество.</span><span class="sxs-lookup"><span data-stu-id="80d54-128">Specifies a code for an assessed tax allowance.</span></span>              |
   | <span data-ttu-id="80d54-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80d54-129">**Description**</span></span>                    | <span data-ttu-id="80d54-130">Определяет описание кода налога на имущество.</span><span class="sxs-lookup"><span data-stu-id="80d54-130">Specifies a description for the assessed tax code.</span></span>           |
   | <span data-ttu-id="80d54-131">**Код Региона**</span><span class="sxs-lookup"><span data-stu-id="80d54-131">**Region Code**</span></span>                    | <span data-ttu-id="80d54-132">Определяет код региона из 2 символов, который используется вместе с полем "Код налог. органа"</span><span class="sxs-lookup"><span data-stu-id="80d54-132">Specifies a two-character region code that is used together with the Tax Authority No.</span></span> <span data-ttu-id="80d54-133">для определения кода ОКАТО.</span><span class="sxs-lookup"><span data-stu-id="80d54-133">field to determine the OKATO code.</span></span> |
   | <span data-ttu-id="80d54-134">**Ставка (%)**</span><span class="sxs-lookup"><span data-stu-id="80d54-134">**Rate %**</span></span>                         | <span data-ttu-id="80d54-135">Определяет ставку налога на имущество.</span><span class="sxs-lookup"><span data-stu-id="80d54-135">Specifies the tax rate for the assessed tax.</span></span> <span data-ttu-id="80d54-136">Если имеются льготы, уменьшающие ставку налога, они должны быть включены в процентах ставки.</span><span class="sxs-lookup"><span data-stu-id="80d54-136">If there are any tax allowances that reduce the tax rate, they must be included in the rate percentage.</span></span> |
   | <span data-ttu-id="80d54-137">**Код льготы для уменьшения ставки налога**</span><span class="sxs-lookup"><span data-stu-id="80d54-137">**Dec. Rate Tax Allowance Code**</span></span>   | <span data-ttu-id="80d54-138">Определяет код для кода льготы по налогу на имущество, которая сокращает вычисленную сумму налога на имущество согласно каталогу налогов на имущество.</span><span class="sxs-lookup"><span data-stu-id="80d54-138">Specifies a code for the assessed tax allowance code that reduces the calculated assessed tax amount according to the tax allowances directory.</span></span> <span data-ttu-id="80d54-139">Этот код определяется в таблице **Льготы налога на имущество**.</span><span class="sxs-lookup"><span data-stu-id="80d54-139">This code is defined in the **Assessed Tax Allowance** table.</span></span> |
   | <span data-ttu-id="80d54-140">**Код льготы для уменьшения суммы налога**</span><span class="sxs-lookup"><span data-stu-id="80d54-140">**Dec. Amount Tax Allowance Code**</span></span> | <span data-ttu-id="80d54-141">Определяет сумму льготы по налогу на имущество.</span><span class="sxs-lookup"><span data-stu-id="80d54-141">Specifies the amount of an assessed tax allowance.</span></span>           |
   | <span data-ttu-id="80d54-142">**Сумма уменьшения**</span><span class="sxs-lookup"><span data-stu-id="80d54-142">**Decreasing Amount**</span></span>              | <span data-ttu-id="80d54-143">Определяет значение, которое будет использоваться при расчете налога на имущество при наличии льготы по налогу, сокращающей налоги на имущество.</span><span class="sxs-lookup"><span data-stu-id="80d54-143">Specifies the value to be used in the assessed tax calculation if there is a tax allowance that reduces assessed taxes.</span></span> |
   | <span data-ttu-id="80d54-144">**Код освобождения от налога**</span><span class="sxs-lookup"><span data-stu-id="80d54-144">**Exemption Tax Allowance**</span></span>        | <span data-ttu-id="80d54-145">Определяет код освобождения от налога на имущество.</span><span class="sxs-lookup"><span data-stu-id="80d54-145">Specifies a code for an assessed tax allowance exemption.</span></span> <span data-ttu-id="80d54-146">Этот код определяется в таблице **Льготы налога на имущество**.</span><span class="sxs-lookup"><span data-stu-id="80d54-146">This code is defined in the **Assessed Tax Allowance** table.</span></span> |
   | <span data-ttu-id="80d54-147">**Тип суммы уменьшения**</span><span class="sxs-lookup"><span data-stu-id="80d54-147">**Decreasing Amount Type**</span></span>         | <span data-ttu-id="80d54-148">Определяет, является ли значение суммы уменьшения процентом или суммой.</span><span class="sxs-lookup"><span data-stu-id="80d54-148">Specifies whether the decreasing amount value is a percentage or an amount.</span></span> |

6. <span data-ttu-id="80d54-149">Нажмите кнопку **Закрыть**.</span><span class="sxs-lookup"><span data-stu-id="80d54-149">Choose the **Close** button.</span></span>

7. <span data-ttu-id="80d54-150">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Коды ОКАТО**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="80d54-150">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OKATO Codes**, and then choose the related link.</span></span>

8. <span data-ttu-id="80d54-151">В окне **Коды ОКАТО** заполните поля **Код региона** и **Код налог. органа**</span><span class="sxs-lookup"><span data-stu-id="80d54-151">In the **OKATO Codes** window, fill in the **Region Code** and the **Tax Authority No.**</span></span> <span data-ttu-id="80d54-152">и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="80d54-152">fields, and then choose the **OK** button.</span></span>

9. <span data-ttu-id="80d54-153">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Основные средства**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="80d54-153">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>

10. <span data-ttu-id="80d54-154">На экспресс-вкладке **Налог на имущество** заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="80d54-154">On the **Assessed Tax** FastTab, fill in the fields as described in the following table.</span></span>

    | <span data-ttu-id="80d54-155">Поле</span><span class="sxs-lookup"><span data-stu-id="80d54-155">Field</span></span>                      | <span data-ttu-id="80d54-156">Описание</span><span class="sxs-lookup"><span data-stu-id="80d54-156">Description</span></span>                                                  |
    | :------------------------- | :----------------------------------------------------------- |
    | <span data-ttu-id="80d54-157">**Код налога на имущество**</span><span class="sxs-lookup"><span data-stu-id="80d54-157">**Assessed Tax Code**</span></span>      | <span data-ttu-id="80d54-158">Определяет код налога на имущество, связанный с основным средством.</span><span class="sxs-lookup"><span data-stu-id="80d54-158">Specifies the assessed tax code that is associated with the fixed asset.</span></span> |
    | <span data-ttu-id="80d54-159">**Вид имущества**</span><span class="sxs-lookup"><span data-stu-id="80d54-159">**Property Type**</span></span>          | <span data-ttu-id="80d54-160">Определяет вид имущества основного средства.</span><span class="sxs-lookup"><span data-stu-id="80d54-160">Specifies the property type of the fixed the fixed asset.</span></span> <span data-ttu-id="80d54-161">Возможные значения: **Недвижимое имущество ЕСГС**, **Недвижимое распределенное имущество**, **Прочее имущество** и **Имущество особой экономической зоны**.</span><span class="sxs-lookup"><span data-stu-id="80d54-161">Property types include: **Immovable UGSS Property**, **Immovable Distributed Property**, **Other Property**, and **Special Economic Zone Property**.</span></span> |
    | <span data-ttu-id="80d54-162">**Доля балансовой стоимости**</span><span class="sxs-lookup"><span data-stu-id="80d54-162">**Book Value per Share**</span></span>   | <span data-ttu-id="80d54-163">Определяет балансовую стоимость ОС на акцию.</span><span class="sxs-lookup"><span data-stu-id="80d54-163">Specifies the book value of the fixed asset, per share.</span></span>      |
    | <span data-ttu-id="80d54-164">**Код ОКАТО**</span><span class="sxs-lookup"><span data-stu-id="80d54-164">**OKATO Code**</span></span>             | <span data-ttu-id="80d54-165">Определяет регион, в котором находится текущее основное средство.</span><span class="sxs-lookup"><span data-stu-id="80d54-165">Specifies the region where the current fixed asset is situated.</span></span> |
    | <span data-ttu-id="80d54-166">**Сумма налога, уплаченная за рубежом**</span><span class="sxs-lookup"><span data-stu-id="80d54-166">**Tax Amount Paid Abroad**</span></span> | <span data-ttu-id="80d54-167">Определяет сумму налога, который был оплачен за основное средство за границей.</span><span class="sxs-lookup"><span data-stu-id="80d54-167">Specifies the amount of tax that was paid abroad for the fixed asset.</span></span> |

11. <span data-ttu-id="80d54-168">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="80d54-168">Choose the **OK** button.</span></span>

12. <span data-ttu-id="80d54-169">Чтобы напечатать декларацию по налогу на имущество, следует сначала импортировать шаблон декларации.</span><span class="sxs-lookup"><span data-stu-id="80d54-169">To print the assessed tax declaration, you have to first import the declaration template.</span></span> <span data-ttu-id="80d54-170">В окне **Настройка модуля ОС** выберите шаблон на экспресс-вкладке **Шаблоны**.</span><span class="sxs-lookup"><span data-stu-id="80d54-170">In the **Fixed Asset Setup** window, select the template name from the **Templates** FastTab.</span></span>

13. <span data-ttu-id="80d54-171">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Расчет налога на имущество**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="80d54-171">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Calculate Assessed Tax**, and then choose the related link.</span></span>

14. <span data-ttu-id="80d54-172">В окне **Расчет налога на имущество** заполните поля **Код налог. органа**, **Год** и **Отчетный период**.</span><span class="sxs-lookup"><span data-stu-id="80d54-172">In the **Calculate Assessed Tax** window, fill in the **Tax Authority No.**, **Year**, and the **Reporting Period** fields.</span></span>

15. <span data-ttu-id="80d54-173">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="80d54-173">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="80d54-174">См. также</span><span class="sxs-lookup"><span data-stu-id="80d54-174">See Also</span></span>

[<span data-ttu-id="80d54-175">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="80d54-175">Fixed Assets</span></span>](../../fa-manage.md)  
[<span data-ttu-id="80d54-176">Настройка основных средств</span><span class="sxs-lookup"><span data-stu-id="80d54-176">Setting Up Fixed Assets</span></span>](../../fa-setup.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]