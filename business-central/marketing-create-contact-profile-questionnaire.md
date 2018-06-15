---
title: "Использование профилей для классификации контактов"
description: "Настройка анкет профилей для облегчения классификации бизнес-контактов"
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: contacts, profiles
ms.author: edupont
ms.date: 05/09/2018
ms.translationtype: HT
ms.sourcegitcommit: 75501b9402bb1c14fcfeb2fc6e61f055a2247493
ms.openlocfilehash: 00cfce8b467040a4de419c1b59a258c0eacf0b9a
ms.contentlocale: ru-ru
ms.lasthandoff: 05/15/2018

---

# <a name="use-profile-questionnaires-to-classify-business-contacts"></a><span data-ttu-id="3cb0b-103">Использование анкет профилей для классификации бизнес-контактов</span><span class="sxs-lookup"><span data-stu-id="3cb0b-103">Use Profile Questionnaires to Classify Business Contacts</span></span>
<span data-ttu-id="3cb0b-104">Можно настроить анкеты профиля, которые будут использоваться при вводе информации о профиле контакта.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-104">You can set up profile questionnaires that you want to use when entering information about your contacts' profiles.</span></span> <span data-ttu-id="3cb0b-105">В каждой анкете можно настроить разные вопросы, которые планируется задавать контактам.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-105">Within each questionnaire, you can set up the different questions you intend to ask your contacts.</span></span>  

<span data-ttu-id="3cb0b-106">Также можно указать, чтобы ответы на некоторые из этих вопросов заполнялись автоматически на основе данных о контакте, заказчике или поставщике.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-106">You can also run the questionnaire to answer some of the questions based on contact, customer, or vendor data automatically.</span></span>  

## <a name="to-add-a-profile-questionnaire"></a><span data-ttu-id="3cb0b-107">Добавление анкеты профиля</span><span class="sxs-lookup"><span data-stu-id="3cb0b-107">To add a profile questionnaire</span></span>
1.  <span data-ttu-id="3cb0b-108">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Настройка анкеты**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Questionnaire Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="3cb0b-109">На вкладке **Главная** в группе **Создать** выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-109">On the **Home** tab, in the **New** group, choose **New**.</span></span>  
3.  <span data-ttu-id="3cb0b-110">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-110">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-add-questions-to-a-profile-questionnaire"></a><span data-ttu-id="3cb0b-111">Добавление вопросов в анкету профиля</span><span class="sxs-lookup"><span data-stu-id="3cb0b-111">To add questions to a profile questionnaire</span></span>
1.  <span data-ttu-id="3cb0b-112">Выберите соответствующую анкету профиля, после чего на вкладке **Главная** в группе **Процесс** выберите пункт **Изменение настройки анкеты**.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-112">Choose the relevant profile questionnaire, and then on the **Home** tab, in the **Process** group, choose **Edit Questionnaire Setup**.</span></span>  
2.  <span data-ttu-id="3cb0b-113">На первой пустой строке в поле **Тип** выберите **Вопрос** и введите вопрос в поле **Описание**.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-113">On the first empty line, in the **Type** field, choose **Question** and type your question in the **Description** field.</span></span> <span data-ttu-id="3cb0b-114">Заполните остальные поля в этой строке.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-114">Fill in the other fields on this line.</span></span>  
3.  <span data-ttu-id="3cb0b-115">Находясь на следующей пустой строке, в поле **Тип**, выберите **Ответ** и введите ответ в поле **Описание**.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-115">On the next empty line, in the **Type** field, choose **Answer** and type your answer in the **Description** field.</span></span>  
4.  <span data-ttu-id="3cb0b-116">В поле **Приоритет** выберите приоритет.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-116">In the **Priority** field, select the priority.</span></span> <span data-ttu-id="3cb0b-117">Введите диапазон значений полях **От значения** и **До значения**.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-117">In the **From Value** and **To Value** fields, define a point range.</span></span> <span data-ttu-id="3cb0b-118">Контакты, которые получат баллы в заданном диапазоне, получат ответ.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-118">Contacts that receive points within the defined range will get the answer.</span></span>  

<span data-ttu-id="3cb0b-119">Повторите эти шаги, чтобы ввести все вопросы и ответы в анкете профиля.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-119">Repeat these steps to enter all the questions and answers within the profile questionnaire.</span></span>

<span data-ttu-id="3cb0b-120">После создания анкеты необходимо создать рейтинги контактов для классификации ваших контактов.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-120">After you have created a questionnaire, you must create contact ratings to classify your contacts.</span></span> <span data-ttu-id="3cb0b-121">Можно также настроить вопросы, которые расклассифицированы автоматически в соответствии с информацией в карточке контакта.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-121">You can also set up questions that are rated automatically based on information in the contact card.</span></span>  

> [!NOTE]
> <span data-ttu-id="3cb0b-122">При вводе вопроса, на который программа будет отвечать автоматически, щелкните <STRONG>Строка</STRONG> и выберите <STRONG>Вопрос - подробности</STRONG>, чтобы ввести критерии, которые будут использоваться для автоматического ответа на вопрос.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-122">If you enter a question that is automatically answered, choose <STRONG>Line</STRONG>, and then choose <STRONG>Question Details</STRONG>, to enter the criteria to automatically answer the question.</span></span>

## <a name="the-automatic-classification-of-contacts"></a><span data-ttu-id="3cb0b-123">Автоматическая классификация контактов</span><span class="sxs-lookup"><span data-stu-id="3cb0b-123">The Automatic Classification of Contacts</span></span>
<span data-ttu-id="3cb0b-124">Вы можете автоматически классифицировать свои контакты по клиенту, поставщику и контактной информации путем настройки профильных вопросов, на которые программа отвечает автоматически, в окне **Настройка анкеты профиля**.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-124">You can automatically classify your contacts according to customer, vendor, and contact information, by setting up automatically answered profile questions in the **Profile Questionnaire Setup** window.</span></span>  

> [!NOTE]
> <span data-ttu-id="3cb0b-125">Только зарегистрированным в качестве клиентов контактам может быть назначена классификация, основанная на данных клиентов, и только зарегистрированным в качестве поставщиков контактам может быть назначена классификация, основанная на данных поставщиков.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-125">Only contacts that are recorded as customers can be assigned a classification based on customer data and only contacts that are recorded as vendors can be assigned a classification based on vendor data.</span></span> <span data-ttu-id="3cb0b-126">Автоматическая классификация не обновляется автоматически.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-126">The automatic classification is not updated automatically.</span></span> <span data-ttu-id="3cb0b-127">Впоследствии может понадобиться обновить профиль анкет после обновления данных клиента, поставщика или контакта, на которых они основаны.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-127">Consequently, you may want to update the profile questionnaires, after you have updated the customer, vendor or contact data they are based on.</span></span>  

<span data-ttu-id="3cb0b-128">После настройки вопросов, на которые программа отвечает автоматически, при назначении профильной анкеты контакту [!INCLUDE[d365fin](includes/d365fin_md.md)] автоматически назначит контакту правильные ответы.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-128">After you have set up automatically answered profile questions, if you assign the profile questionnaire containing these questions to a contact, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically assign the right answers for the contact.</span></span>  

## <a name="example"></a><span data-ttu-id="3cb0b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3cb0b-129">Example</span></span>
<span data-ttu-id="3cb0b-130">Можно классифицировать контакты в соответствии с объемами продаж:</span><span class="sxs-lookup"><span data-stu-id="3cb0b-130">You can classify your contacts according to how much they bought from you:</span></span>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="3cb0b-131"><strong>Ответ</strong></span><span class="sxs-lookup"><span data-stu-id="3cb0b-131"><strong>Answer</strong></span></span></th>
<th><span data-ttu-id="3cb0b-132"><strong>Применяется к</strong></span><span class="sxs-lookup"><span data-stu-id="3cb0b-132"><strong>Applies to</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="3cb0b-133">А</span><span class="sxs-lookup"><span data-stu-id="3cb0b-133">A</span></span></p></td>
<td><p><span data-ttu-id="3cb0b-134">контактам, сделавшим покупки на сумму от 500 000 руб.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-134">contacts who bought for 500,000 LCY or more</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="3cb0b-135">Б</span><span class="sxs-lookup"><span data-stu-id="3cb0b-135">B</span></span></p></td>
<td><p><span data-ttu-id="3cb0b-136">контактам, сделавшим покупки на сумму от 100 000 до 499 999 руб. включительно</span><span class="sxs-lookup"><span data-stu-id="3cb0b-136">contacts who bought for 100,000 up to 499,999 LCY</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="3cb0b-137">C</span><span class="sxs-lookup"><span data-stu-id="3cb0b-137">C</span></span></p></td>
<td><p><span data-ttu-id="3cb0b-138">контактам, сделавшим покупки на сумму 99 999 руб. или меньше</span><span class="sxs-lookup"><span data-stu-id="3cb0b-138">contacts who bought for 99,999 LCY or less</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="3cb0b-139">Чтобы это сделать, заполните окно **Настройка анкеты профиля** следующим образом:</span><span class="sxs-lookup"><span data-stu-id="3cb0b-139">To do this, fill in the **Profile Questionnaire Setup** window as follows:</span></span>


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
<th><span data-ttu-id="3cb0b-140"><strong>Тип</strong></span><span class="sxs-lookup"><span data-stu-id="3cb0b-140"><strong>Type</strong></span></span></th>
<th><span data-ttu-id="3cb0b-141"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="3cb0b-141"><strong>Description</strong></span></span></th>
<th><span data-ttu-id="3cb0b-142"><strong>Автоматическая классификация</strong></span><span class="sxs-lookup"><span data-stu-id="3cb0b-142"><strong>Automatic Classification</strong></span></span></th>
<th><span data-ttu-id="3cb0b-143"><strong>От значения</strong></span><span class="sxs-lookup"><span data-stu-id="3cb0b-143"><strong>From Value</strong></span></span></th>
<th><span data-ttu-id="3cb0b-144"><strong>До значения</strong></span><span class="sxs-lookup"><span data-stu-id="3cb0b-144"><strong>To Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="3cb0b-145">Вопрос</span><span class="sxs-lookup"><span data-stu-id="3cb0b-145">Question</span></span></p></td>
<td><p><span data-ttu-id="3cb0b-146">Классификация по алфавиту</span><span class="sxs-lookup"><span data-stu-id="3cb0b-146">ABC Classification</span></span></p></td>
<td><p><span data-ttu-id="3cb0b-147">Щелкните, чтобы установить флажок</span><span class="sxs-lookup"><span data-stu-id="3cb0b-147">Click to insert a check mark</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="3cb0b-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="3cb0b-148">Answer</span></span></p></td>
<td><p><span data-ttu-id="3cb0b-149">А</span><span class="sxs-lookup"><span data-stu-id="3cb0b-149">A</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="3cb0b-150">500 000</span><span class="sxs-lookup"><span data-stu-id="3cb0b-150">500,000</span></span></p></td>
<td><p> </p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="3cb0b-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="3cb0b-151">Answer</span></span></p></td>
<td><p><span data-ttu-id="3cb0b-152">Б</span><span class="sxs-lookup"><span data-stu-id="3cb0b-152">B</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="3cb0b-153">100 000</span><span class="sxs-lookup"><span data-stu-id="3cb0b-153">100,000</span></span></p></td>
<td><p><span data-ttu-id="3cb0b-154">499 999</span><span class="sxs-lookup"><span data-stu-id="3cb0b-154">499,999</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="3cb0b-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="3cb0b-155">Answer</span></span></p></td>
<td><p><span data-ttu-id="3cb0b-156">C</span><span class="sxs-lookup"><span data-stu-id="3cb0b-156">C</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="3cb0b-157">99 999</span><span class="sxs-lookup"><span data-stu-id="3cb0b-157">99,999</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="3cb0b-158">Затем заполните окно **Вопрос профиля - подробности** следующим образом:</span><span class="sxs-lookup"><span data-stu-id="3cb0b-158">Then fill in the **Profile Question Details** window as follows:</span></span>
<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="3cb0b-159"><strong>Поле</strong></span><span class="sxs-lookup"><span data-stu-id="3cb0b-159"><strong>Field</strong></span></span></th>
<th><span data-ttu-id="3cb0b-160"><strong>Значение</strong></span><span class="sxs-lookup"><span data-stu-id="3cb0b-160"><strong>Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="3cb0b-161"><strong>Поле классификации клиентов</strong></span><span class="sxs-lookup"><span data-stu-id="3cb0b-161"><strong>Customer Classification Field</strong></span></span></td>
<td><span data-ttu-id="3cb0b-162"><emphasis>Продажи (руб.)</emphasis></span><span class="sxs-lookup"><span data-stu-id="3cb0b-162"><emphasis>Sales (LCY)</emphasis></span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3cb0b-163"><strong>Метод классификации</strong></span><span class="sxs-lookup"><span data-stu-id="3cb0b-163"><strong>Classification Method</strong></span></span></td>
<td><span data-ttu-id="3cb0b-164"><emphasis>Заданное значение</emphasis></span><span class="sxs-lookup"><span data-stu-id="3cb0b-164"><emphasis>Defined Value</emphasis></span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="3cb0b-165">При назначении контакту профиля анкеты, содержащей этот вопрос, программа автоматически вводит соответствующий ответ для этого контакта в строках профиля карточки контакта.</span><span class="sxs-lookup"><span data-stu-id="3cb0b-165">When you assign the profile questionnaire containing this question to a contact, the program automatically enters the relevant answer for this contact on the profile lines of the contact card.</span></span>

## <a name="see-also"></a><span data-ttu-id="3cb0b-166">См. также</span><span class="sxs-lookup"><span data-stu-id="3cb0b-166">See Also</span></span>
[<span data-ttu-id="3cb0b-167">Создание контактных лиц</span><span class="sxs-lookup"><span data-stu-id="3cb0b-167">Creating Contact Persons</span></span>](marketing-create-contact-persons.md)  
[<span data-ttu-id="3cb0b-168">Создание контактных лиц</span><span class="sxs-lookup"><span data-stu-id="3cb0b-168">Create Contact Persons</span></span>](marketing-how-create-contact-persons.md)  
[<span data-ttu-id="3cb0b-169">Создание контактных организаций</span><span class="sxs-lookup"><span data-stu-id="3cb0b-169">Creating Contact Companies</span></span>](marketing-create-contact-companies.md)  

