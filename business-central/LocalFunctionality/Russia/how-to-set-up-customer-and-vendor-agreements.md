---
title: Настройка договоров с клиентами и поставщиками в России
description: Российские улучшения включают договоры с клиентами и поставщиками.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 5355662cb4ea1a74d343dff11b46bd71a3473eb9
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5382723"
---
# <a name="set-up-customer-and-vendor-agreements"></a><span data-ttu-id="a92ae-103">Настройка договоров с клиентами и поставщиками</span><span class="sxs-lookup"><span data-stu-id="a92ae-103">Set Up Customer and Vendor Agreements</span></span>

<span data-ttu-id="a92ae-104">Функции договоров с поставщиками и клиентами включает в себя следующие компоненты:</span><span class="sxs-lookup"><span data-stu-id="a92ae-104">The customer and vendor agreements feature provides the following:</span></span>

- <span data-ttu-id="a92ae-105">список договоров для клиентов и поставщиков;</span><span class="sxs-lookup"><span data-stu-id="a92ae-105">A list of agreements for customers and vendors</span></span>
- <span data-ttu-id="a92ae-106">карточка договора, в которой хранятся все нужные сведения о договоре;</span><span class="sxs-lookup"><span data-stu-id="a92ae-106">An agreement card where all the required information about agreements is stored</span></span>
- <span data-ttu-id="a92ae-107">синхронизация между договорами и измерениями, которая обеспечивает использование существующих отчетов и анализов измерений.</span><span class="sxs-lookup"><span data-stu-id="a92ae-107">Synchronization between agreements and dimensions, to enable use of existing reports and dimension analyses</span></span>

<span data-ttu-id="a92ae-108">Приведенная ниже процедура показывает, как настроить договор для клиента, но процедура для поставщика аналогична и начинается из окна **Покупки и расчеты с кредиторами**.</span><span class="sxs-lookup"><span data-stu-id="a92ae-108">The following procedure shows how to set up an agreement for a customer, but the procedure for a vendor is similar and starts from the **Purchases & Payables** window.</span></span>

## <a name="to-set-up-an-agreement"></a><span data-ttu-id="a92ae-109">Настройка договора</span><span class="sxs-lookup"><span data-stu-id="a92ae-109">To set up an agreement</span></span>

1. <span data-ttu-id="a92ae-110">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Продажи и дебитор. задолж."**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="a92ae-110">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>

2. <span data-ttu-id="a92ae-111">Чтобы настроить договор, на экспресс-вкладке **Измерения** и экспресс-вкладках **Нумерация** заполните поля, перечисленные в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="a92ae-111">To set up agreement, on the **Dimensions** FastTab and **Numbering** FastTabs, enter information in the fields listed in the following table.</span></span>

   | <span data-ttu-id="a92ae-112">Поле</span><span class="sxs-lookup"><span data-stu-id="a92ae-112">Field</span></span>                          | <span data-ttu-id="a92ae-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a92ae-113">Description</span></span>         |
   | :----------------------------- | :------------------ |
   | <span data-ttu-id="a92ae-114">**Измерение Договор**</span><span class="sxs-lookup"><span data-stu-id="a92ae-114">**Dimension Agreement**</span></span>        | <span data-ttu-id="a92ae-115">Выберите код измерения для договоров.</span><span class="sxs-lookup"><span data-stu-id="a92ae-115">Select a dimension code for agreements.</span></span>             |
   | <span data-ttu-id="a92ae-116">**Синхр. измерения договоров**</span><span class="sxs-lookup"><span data-stu-id="a92ae-116">**Synch. Agreement Dimension**</span></span> | <span data-ttu-id="a92ae-117">Установите этот флажок, чтобы создать код значения измерения после создания договоров. Коды значений измерений равны кодам договоров.</span><span class="sxs-lookup"><span data-stu-id="a92ae-117">Select this field to create a dimension value code after agreements is created, and the dimension value codes are equal to the agreement codes.</span></span> |
   | <span data-ttu-id="a92ae-118">**Серия номеров для договоров клиента**</span><span class="sxs-lookup"><span data-stu-id="a92ae-118">**Customer Agreement Nos.**</span></span>    | <span data-ttu-id="a92ae-119">Выберите серию номеров для договоров с клиентом.</span><span class="sxs-lookup"><span data-stu-id="a92ae-119">Select the customer agreement number series.</span></span>        | 

## <a name="to-create-a-customer-or-vendor-agreement"></a><span data-ttu-id="a92ae-120">Создание договора с клиентом или поставщиком</span><span class="sxs-lookup"><span data-stu-id="a92ae-120">To create a customer or vendor agreement</span></span> 

1. <span data-ttu-id="a92ae-121">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиенты**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="a92ae-121">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span></span>

2. <span data-ttu-id="a92ae-122">Выберите клиента из списка и выберите действие **Правка**.</span><span class="sxs-lookup"><span data-stu-id="a92ae-122">Select a customer from the list, and then choose the **Edit** action.</span></span>

3. <span data-ttu-id="a92ae-123">Разверните экспресс-вкладку **Договоры** и измените поле **Учет договоров**.</span><span class="sxs-lookup"><span data-stu-id="a92ae-123">Expand the **Agreements** FastTab, and modify the **Agreement Posting** field.</span></span>

4. <span data-ttu-id="a92ae-124">Выберите действие **Договоры**.</span><span class="sxs-lookup"><span data-stu-id="a92ae-124">Choose the **Agreements** action.</span></span> <span data-ttu-id="a92ae-125">В окне **Договоры клиентов** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="a92ae-125">In the **Customer Agreements** window, choose the **New** action.</span></span>

5. <span data-ttu-id="a92ae-126">В карточке **Договоры с клиентом или поставщиком** заполните поля, перечисленные в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="a92ae-126">In the **Customer or Vendor Agreement** card, enter the information in the following fields listed in the table.</span></span>

   | <span data-ttu-id="a92ae-127">Поле</span><span class="sxs-lookup"><span data-stu-id="a92ae-127">Field</span></span>                    | <span data-ttu-id="a92ae-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a92ae-128">Description</span></span>                                                  |
   | :----------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="a92ae-129">**Код**</span><span class="sxs-lookup"><span data-stu-id="a92ae-129">**Code**</span></span>                 | <span data-ttu-id="a92ae-130">Введите код договора.</span><span class="sxs-lookup"><span data-stu-id="a92ae-130">Enter the code for an agreement.</span></span> <span data-ttu-id="a92ae-131">Введите до 20 буквенно-цифровых знаков.</span><span class="sxs-lookup"><span data-stu-id="a92ae-131">Enter a maximum of 20 characters, both numbers and letters.</span></span> <span data-ttu-id="a92ae-132">По умолчанию код создается из серии номеров, настроенной в форме "Настройка ГК".</span><span class="sxs-lookup"><span data-stu-id="a92ae-132">It is created by default from the number series set up in the General Ledger Setup form.</span></span> |
   | <span data-ttu-id="a92ae-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a92ae-133">**Description**</span></span>          | <span data-ttu-id="a92ae-134">Введите описание договора.</span><span class="sxs-lookup"><span data-stu-id="a92ae-134">Enter the description of the agreement.</span></span> <span data-ttu-id="a92ae-135">Введите до 250 буквенно-цифровых знаков.</span><span class="sxs-lookup"><span data-stu-id="a92ae-135">Enter a maximum of 250 characters, both numbers and letters.</span></span> |
   | <span data-ttu-id="a92ae-136">**Номер источника**</span><span class="sxs-lookup"><span data-stu-id="a92ae-136">**Source No.**</span></span>           | <span data-ttu-id="a92ae-137">Выберите это поле, чтобы видеть номер поставщика или клиента, для которого создается данный договор.</span><span class="sxs-lookup"><span data-stu-id="a92ae-137">Select this field to see the number of the vendor or customer for whom the agreement is created.</span></span> |
   | <span data-ttu-id="a92ae-138">**Название источника**</span><span class="sxs-lookup"><span data-stu-id="a92ae-138">**Source Name**</span></span>          | <span data-ttu-id="a92ae-139">Введите название поставщика или клиента, для которого создается данное соглашение.</span><span class="sxs-lookup"><span data-stu-id="a92ae-139">Enter the name of the vendor or customer for whom the agreement is created.</span></span> <span data-ttu-id="a92ae-140">Название источника автоматически извлекается из таблицы "Поставщик" или "Клиент".</span><span class="sxs-lookup"><span data-stu-id="a92ae-140">The source name is automatically retrieved from the Vendor or Customer table.</span></span> |
   | <span data-ttu-id="a92ae-141">**Код Значения Измерения**</span><span class="sxs-lookup"><span data-stu-id="a92ae-141">**Dimension Value Code**</span></span> | <span data-ttu-id="a92ae-142">Введите код значения измерения.</span><span class="sxs-lookup"><span data-stu-id="a92ae-142">Enter the dimension value code.</span></span> <span data-ttu-id="a92ae-143">Укажите функции соглашения и измерения.</span><span class="sxs-lookup"><span data-stu-id="a92ae-143">Enter agreement and dimension functionality.</span></span> <span data-ttu-id="a92ae-144">Код значения измерения равен коду договора, если выбрано поле **Синхр. измерения договоров** в окне **Настройка модуля "Продажи"**.</span><span class="sxs-lookup"><span data-stu-id="a92ae-144">The dimension value code is equal to the agreement code when the **Synch. Agreement Dimensions** field is selected in the **Sales & Receivables Setup** window.</span></span> |
   | <span data-ttu-id="a92ae-145">**Дата начала**</span><span class="sxs-lookup"><span data-stu-id="a92ae-145">**Starting Date**</span></span>        | <span data-ttu-id="a92ae-146">Введите начальную дату периода, в течение которого предполагается использовать данный договор.</span><span class="sxs-lookup"><span data-stu-id="a92ae-146">Enter starting date of the period for which you want to use the agreement.</span></span> |
   | <span data-ttu-id="a92ae-147">**Дата окончания**</span><span class="sxs-lookup"><span data-stu-id="a92ae-147">**Expire Date**</span></span>          | <span data-ttu-id="a92ae-148">Введите дату окончания срока действия данного договора.</span><span class="sxs-lookup"><span data-stu-id="a92ae-148">Enter the expiration date of the agreement.</span></span>                  |
   | <span data-ttu-id="a92ae-149">**Заблокировано**</span><span class="sxs-lookup"><span data-stu-id="a92ae-149">**Blocked**</span></span>              | <span data-ttu-id="a92ae-150">Установите этот флажок, чтобы избежать учета операций в договоре.</span><span class="sxs-lookup"><span data-stu-id="a92ae-150">Select this field to prevent posting of entries on the agreement.</span></span> <span data-ttu-id="a92ae-151">При попытке создания документа с заблокированным договором будет выведено сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="a92ae-151">When you try to create a document with a blocked agreement, an error message is displayed.</span></span> <span data-ttu-id="a92ae-152">Обычно договор блокируется после даты окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="a92ae-152">An agreement is usually blocked after the expiration date.</span></span> |

<span data-ttu-id="a92ae-153">На вкладке **Навигатор** можно найти следующие функции:</span><span class="sxs-lookup"><span data-stu-id="a92ae-153">On the **Navigate** tab, you can find the following functions:</span></span> 

- <span data-ttu-id="a92ae-154">Список — показать список договоров с клиентом или поставщиком.</span><span class="sxs-lookup"><span data-stu-id="a92ae-154">List - Shows a list of customer or vendor agreements.</span></span>
- <span data-ttu-id="a92ae-155">Книга операций — показать операции книги для клиента или поставщика, учтенные с данным кодом договора.</span><span class="sxs-lookup"><span data-stu-id="a92ae-155">Ledger Entries - Shows customer or vendor ledger entries posted with this agreement code.</span></span> 

<span data-ttu-id="a92ae-156">Договоры полностью синхронизированы с измерениями.</span><span class="sxs-lookup"><span data-stu-id="a92ae-156">The agreements are fully synchronized with dimensions.</span></span> <span data-ttu-id="a92ae-157">Можно учесть транзакции и выбрать код значения измерения соответствующего договора из списка договоров.</span><span class="sxs-lookup"><span data-stu-id="a92ae-157">You can post transactions and choose the dimension value code of the appropriate agreement from the list of agreements.</span></span>

## <a name="see-also"></a><span data-ttu-id="a92ae-158">См. также</span><span class="sxs-lookup"><span data-stu-id="a92ae-158">See Also</span></span>

[<span data-ttu-id="a92ae-159">Отчеты по расчетам с клиентами (Россия)</span><span class="sxs-lookup"><span data-stu-id="a92ae-159">Russian Receivables Reports</span></span>](Russian-Receivables-Reports.md)  
[<span data-ttu-id="a92ae-160">Отчеты о платежах (Россия)</span><span class="sxs-lookup"><span data-stu-id="a92ae-160">Russian Payables Reports</span></span>](Russian-Payables-Reports.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]