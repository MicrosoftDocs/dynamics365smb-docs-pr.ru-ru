---
title: Использование профилей для классификации контактов
description: Настройка анкет профилей для облегчения классификации бизнес-контактов
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: contacts, profiles
ms.author: edupont
ms.date: 10/01/2018
ms.openlocfilehash: 1007bdb689b72cf3eccfc5c15c2df9e3c760d8b3
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "804367"
---
# <a name="use-profile-questionnaires-to-classify-business-contacts"></a><span data-ttu-id="c3adf-103">Использование анкет профилей для классификации бизнес-контактов</span><span class="sxs-lookup"><span data-stu-id="c3adf-103">Use Profile Questionnaires to Classify Business Contacts</span></span>
<span data-ttu-id="c3adf-104">Можно настроить анкеты профиля, которые будут использоваться при вводе информации о профиле контакта.</span><span class="sxs-lookup"><span data-stu-id="c3adf-104">You can set up profile questionnaires that you want to use when entering information about your contacts' profiles.</span></span> <span data-ttu-id="c3adf-105">В каждой анкете можно настроить разные вопросы, которые планируется задавать контактам.</span><span class="sxs-lookup"><span data-stu-id="c3adf-105">Within each questionnaire, you can set up the different questions you intend to ask your contacts.</span></span>  

<span data-ttu-id="c3adf-106">Также можно указать, чтобы ответы на некоторые из этих вопросов заполнялись автоматически на основе данных о контакте, заказчике или поставщике.</span><span class="sxs-lookup"><span data-stu-id="c3adf-106">You can also run the questionnaire to answer some of the questions based on contact, customer, or vendor data automatically.</span></span>  

## <a name="to-add-a-profile-questionnaire"></a><span data-ttu-id="c3adf-107">Добавление анкеты профиля</span><span class="sxs-lookup"><span data-stu-id="c3adf-107">To add a profile questionnaire</span></span>
1.  <span data-ttu-id="c3adf-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка анкеты**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="c3adf-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Questionnaire Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c3adf-109">На вкладке **Главная** в группе **Создать** выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="c3adf-109">On the **Home** tab, in the **New** group, choose **New**.</span></span>  
3.  <span data-ttu-id="c3adf-110">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="c3adf-110">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-add-questions-to-a-profile-questionnaire"></a><span data-ttu-id="c3adf-111">Добавление вопросов в анкету профиля</span><span class="sxs-lookup"><span data-stu-id="c3adf-111">To add questions to a profile questionnaire</span></span>
1.  <span data-ttu-id="c3adf-112">Выберите соответствующую анкету профиля, после чего на вкладке **Главная** в группе **Процесс** выберите пункт **Изменение настройки анкеты**.</span><span class="sxs-lookup"><span data-stu-id="c3adf-112">Choose the relevant profile questionnaire, and then on the **Home** tab, in the **Process** group, choose **Edit Questionnaire Setup**.</span></span>  
2.  <span data-ttu-id="c3adf-113">На первой пустой строке в поле **Тип** выберите **Вопрос** и введите вопрос в поле **Описание**.</span><span class="sxs-lookup"><span data-stu-id="c3adf-113">On the first empty line, in the **Type** field, choose **Question** and type your question in the **Description** field.</span></span> <span data-ttu-id="c3adf-114">Заполните остальные поля в этой строке.</span><span class="sxs-lookup"><span data-stu-id="c3adf-114">Fill in the other fields on this line.</span></span>  
3.  <span data-ttu-id="c3adf-115">Находясь на следующей пустой строке, в поле **Тип**, выберите **Ответ** и введите ответ в поле **Описание**.</span><span class="sxs-lookup"><span data-stu-id="c3adf-115">On the next empty line, in the **Type** field, choose **Answer** and type your answer in the **Description** field.</span></span>  
4.  <span data-ttu-id="c3adf-116">В поле **Приоритет** выберите приоритет.</span><span class="sxs-lookup"><span data-stu-id="c3adf-116">In the **Priority** field, select the priority.</span></span> <span data-ttu-id="c3adf-117">Введите диапазон значений полях **От значения** и **До значения**.</span><span class="sxs-lookup"><span data-stu-id="c3adf-117">In the **From Value** and **To Value** fields, define a point range.</span></span> <span data-ttu-id="c3adf-118">Контакты, которые получат баллы в заданном диапазоне, получат ответ.</span><span class="sxs-lookup"><span data-stu-id="c3adf-118">Contacts that receive points within the defined range will get the answer.</span></span>  

<span data-ttu-id="c3adf-119">Повторите эти шаги, чтобы ввести все вопросы и ответы в анкете профиля.</span><span class="sxs-lookup"><span data-stu-id="c3adf-119">Repeat these steps to enter all the questions and answers within the profile questionnaire.</span></span>

<span data-ttu-id="c3adf-120">После создания анкеты необходимо создать рейтинги контактов для классификации ваших контактов.</span><span class="sxs-lookup"><span data-stu-id="c3adf-120">After you have created a questionnaire, you must create contact ratings to classify your contacts.</span></span> <span data-ttu-id="c3adf-121">Можно также настроить вопросы, которые расклассифицированы автоматически в соответствии с информацией в карточке контакта.</span><span class="sxs-lookup"><span data-stu-id="c3adf-121">You can also set up questions that are rated automatically based on information in the contact card.</span></span>  

> [!NOTE]
> <span data-ttu-id="c3adf-122">При вводе вопроса, на который программа будет отвечать автоматически, щелкните <STRONG>Строка</STRONG> и выберите <STRONG>Вопрос - подробности</STRONG>, чтобы ввести критерии, которые будут использоваться для автоматического ответа на вопрос.</span><span class="sxs-lookup"><span data-stu-id="c3adf-122">If you enter a question that is automatically answered, choose <STRONG>Line</STRONG>, and then choose <STRONG>Question Details</STRONG>, to enter the criteria to automatically answer the question.</span></span>

## <a name="the-automatic-classification-of-contacts"></a><span data-ttu-id="c3adf-123">Автоматическая классификация контактов</span><span class="sxs-lookup"><span data-stu-id="c3adf-123">The Automatic Classification of Contacts</span></span>
<span data-ttu-id="c3adf-124">Вы можете автоматически классифицировать свои контакты по клиенту, поставщику и контактной информации путем настройки профильных вопросов, на которые программа отвечает автоматически, на странице **Настройка анкеты профиля**.</span><span class="sxs-lookup"><span data-stu-id="c3adf-124">You can automatically classify your contacts according to customer, vendor, and contact information, by setting up automatically answered profile questions on the **Profile Questionnaire Setup** page.</span></span>  

> [!NOTE]
> <span data-ttu-id="c3adf-125">Только зарегистрированным в качестве клиентов контактам может быть назначена классификация, основанная на данных клиентов, и только зарегистрированным в качестве поставщиков контактам может быть назначена классификация, основанная на данных поставщиков.</span><span class="sxs-lookup"><span data-stu-id="c3adf-125">Only contacts that are recorded as customers can be assigned a classification based on customer data and only contacts that are recorded as vendors can be assigned a classification based on vendor data.</span></span> <span data-ttu-id="c3adf-126">Автоматическая классификация не обновляется автоматически.</span><span class="sxs-lookup"><span data-stu-id="c3adf-126">The automatic classification is not updated automatically.</span></span> <span data-ttu-id="c3adf-127">Впоследствии может понадобиться обновить профиль анкет после обновления данных клиента, поставщика или контакта, на которых они основаны.</span><span class="sxs-lookup"><span data-stu-id="c3adf-127">Consequently, you may want to update the profile questionnaires, after you have updated the customer, vendor or contact data they are based on.</span></span>  

<span data-ttu-id="c3adf-128">После настройки вопросов, на которые программа отвечает автоматически, при назначении профильной анкеты контакту [!INCLUDE[d365fin](includes/d365fin_md.md)] автоматически назначит контакту правильные ответы.</span><span class="sxs-lookup"><span data-stu-id="c3adf-128">After you have set up automatically answered profile questions, if you assign the profile questionnaire containing these questions to a contact, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically assign the right answers for the contact.</span></span>  

## <a name="example"></a><span data-ttu-id="c3adf-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c3adf-129">Example</span></span>
<span data-ttu-id="c3adf-130">Можно классифицировать контакты в соответствии с объемами продаж:</span><span class="sxs-lookup"><span data-stu-id="c3adf-130">You can classify your contacts according to how much they bought from you:</span></span>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="c3adf-131"><strong>Ответ</strong></span><span class="sxs-lookup"><span data-stu-id="c3adf-131"><strong>Answer</strong></span></span></th>
<th><span data-ttu-id="c3adf-132"><strong>Применяется к</strong></span><span class="sxs-lookup"><span data-stu-id="c3adf-132"><strong>Applies to</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="c3adf-133">А</span><span class="sxs-lookup"><span data-stu-id="c3adf-133">A</span></span></p></td>
<td><p><span data-ttu-id="c3adf-134">контактам, сделавшим покупки на сумму от 500 000 руб.</span><span class="sxs-lookup"><span data-stu-id="c3adf-134">contacts who bought for 500,000 LCY or more</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="c3adf-135">Б</span><span class="sxs-lookup"><span data-stu-id="c3adf-135">B</span></span></p></td>
<td><p><span data-ttu-id="c3adf-136">контактам, сделавшим покупки на сумму от 100 000 до 499 999 руб. включительно</span><span class="sxs-lookup"><span data-stu-id="c3adf-136">contacts who bought for 100,000 up to 499,999 LCY</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="c3adf-137">З</span><span class="sxs-lookup"><span data-stu-id="c3adf-137">C</span></span></p></td>
<td><p><span data-ttu-id="c3adf-138">контактам, сделавшим покупки на сумму 99 999 руб. или меньше</span><span class="sxs-lookup"><span data-stu-id="c3adf-138">contacts who bought for 99,999 LCY or less</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="c3adf-139">Чтобы это сделать, заполните на странице **Анкета профиля - настройка** следующим образом:</span><span class="sxs-lookup"><span data-stu-id="c3adf-139">To do this, fill on the **Profile Questionnaire Setup** page as follows:</span></span>


<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="c3adf-140"><strong>Тип</strong></span><span class="sxs-lookup"><span data-stu-id="c3adf-140"><strong>Type</strong></span></span></th>
<th><span data-ttu-id="c3adf-141"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="c3adf-141"><strong>Description</strong></span></span></th>
<th><span data-ttu-id="c3adf-142"><strong>Автоматическая классификация</strong></span><span class="sxs-lookup"><span data-stu-id="c3adf-142"><strong>Automatic Classification</strong></span></span></th>
<th><span data-ttu-id="c3adf-143"><strong>От значения</strong></span><span class="sxs-lookup"><span data-stu-id="c3adf-143"><strong>From Value</strong></span></span></th>
<th><span data-ttu-id="c3adf-144"><strong>До значения</strong></span><span class="sxs-lookup"><span data-stu-id="c3adf-144"><strong>To Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="c3adf-145">Вопрос</span><span class="sxs-lookup"><span data-stu-id="c3adf-145">Question</span></span></p></td>
<td><p><span data-ttu-id="c3adf-146">Классификация по алфавиту</span><span class="sxs-lookup"><span data-stu-id="c3adf-146">ABC Classification</span></span></p></td>
<td><p><span data-ttu-id="c3adf-147">Щелкните, чтобы установить флажок</span><span class="sxs-lookup"><span data-stu-id="c3adf-147">Click to insert a check mark</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="c3adf-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3adf-148">Answer</span></span></p></td>
<td><p><span data-ttu-id="c3adf-149">П</span><span class="sxs-lookup"><span data-stu-id="c3adf-149">A</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="c3adf-150">500,000</span><span class="sxs-lookup"><span data-stu-id="c3adf-150">500,000</span></span></p></td>
<td><p> </p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="c3adf-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3adf-151">Answer</span></span></p></td>
<td><p><span data-ttu-id="c3adf-152">Б</span><span class="sxs-lookup"><span data-stu-id="c3adf-152">B</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="c3adf-153">100,000</span><span class="sxs-lookup"><span data-stu-id="c3adf-153">100,000</span></span></p></td>
<td><p><span data-ttu-id="c3adf-154">499,999</span><span class="sxs-lookup"><span data-stu-id="c3adf-154">499,999</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="c3adf-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3adf-155">Answer</span></span></p></td>
<td><p><span data-ttu-id="c3adf-156">З</span><span class="sxs-lookup"><span data-stu-id="c3adf-156">C</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="c3adf-157">99 999</span><span class="sxs-lookup"><span data-stu-id="c3adf-157">99,999</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="c3adf-158">Потом заполните страницу **Вопрос профиля - подробности** следующим образом:</span><span class="sxs-lookup"><span data-stu-id="c3adf-158">Then fill on the **Profile Question Details** page as follows:</span></span>
<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="c3adf-159"><strong>Поле</strong></span><span class="sxs-lookup"><span data-stu-id="c3adf-159"><strong>Field</strong></span></span></th>
<th><span data-ttu-id="c3adf-160"><strong>Значение</strong></span><span class="sxs-lookup"><span data-stu-id="c3adf-160"><strong>Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="c3adf-161"><strong>Поле классификации клиентов</strong></span><span class="sxs-lookup"><span data-stu-id="c3adf-161"><strong>Customer Classification Field</strong></span></span></td>
<td><span data-ttu-id="c3adf-162"><emphasis>Продажи (руб.)</emphasis></span><span class="sxs-lookup"><span data-stu-id="c3adf-162"><emphasis>Sales (LCY)</emphasis></span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c3adf-163"><strong>Метод классификации</strong></span><span class="sxs-lookup"><span data-stu-id="c3adf-163"><strong>Classification Method</strong></span></span></td>
<td><span data-ttu-id="c3adf-164"><emphasis>Заданное значение</emphasis></span><span class="sxs-lookup"><span data-stu-id="c3adf-164"><emphasis>Defined Value</emphasis></span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="c3adf-165">При назначении контакту профиля анкеты, содержащей этот вопрос, программа автоматически вводит соответствующий ответ для этого контакта в строках профиля карточки контакта.</span><span class="sxs-lookup"><span data-stu-id="c3adf-165">When you assign the profile questionnaire containing this question to a contact, the program automatically enters the relevant answer for this contact on the profile lines of the contact card.</span></span>

## <a name="see-also"></a><span data-ttu-id="c3adf-166">См. также</span><span class="sxs-lookup"><span data-stu-id="c3adf-166">See Also</span></span>
[<span data-ttu-id="c3adf-167">Создание контактов</span><span class="sxs-lookup"><span data-stu-id="c3adf-167">Creating Contacts</span></span>](marketing-create-contact-companies.md)  
