---
title: "Создание взаимодействий для контактов и сегментов | Microsoft Docs"
description: "Описывается, как создавать взаимодействия для ваших коммуникаций с контактами и сегментами в Dynamics 365, например прямых почтовых рассылок."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/15/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 57cbc08ab2e05777fae54018fe714d44b64d14e0
ms.contentlocale: ru-ru
ms.lasthandoff: 11/10/2017

---
# <a name="how-to-create-interactions-on-contacts-and-segments"></a><span data-ttu-id="0a467-103">Практическое руководство. Создание взаимодействий для контактов и сегментов</span><span class="sxs-lookup"><span data-stu-id="0a467-103">How to: Create Interactions on Contacts and Segments</span></span>
<span data-ttu-id="0a467-104">Можно создавать взаимодействия для того, чтобы регистрировать все взаимодействия и коммуникации с контактами и сегментами, например, прямые почтовые рассылки.</span><span class="sxs-lookup"><span data-stu-id="0a467-104">You can create interactions to record all the interactions and communications you have with your contacts and segments, for example, direct mail.</span></span>

<span data-ttu-id="0a467-105">Перед созданием взаимодействий следует настроить шаблоны взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="0a467-105">Before you create interactions, you must set up interaction templates.</span></span> <span data-ttu-id="0a467-106">Дополнительные сведения см. в разделе [Настройка шаблона взаимодействий](marketing-interactions.md).</span><span class="sxs-lookup"><span data-stu-id="0a467-106">For more information, see  [Set Up Interaction Templates](marketing-interactions.md).</span></span>

## <a name="to-create-an-interaction"></a><span data-ttu-id="0a467-107">Создание взаимодействия</span><span class="sxs-lookup"><span data-stu-id="0a467-107">To create an interaction</span></span>
1. <span data-ttu-id="0a467-108">Откройте контакт, менеджера по продажам или операцию журнала взаимодействий.</span><span class="sxs-lookup"><span data-stu-id="0a467-108">Open the contact, salesperson, or interaction log entry.</span></span>
2. <span data-ttu-id="0a467-109">Выберите действие **Создать взаимодействие**.</span><span class="sxs-lookup"><span data-stu-id="0a467-109">Choose the **Create Interaction** action.</span></span>
3. <span data-ttu-id="0a467-110">Заполните поля и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="0a467-110">Fill in the fields, and then choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="0a467-111">Если необходимо выполнить другую задачу до завершения взаимодействия, можно нажать **Отмена** и завершить взаимодействие позднее.</span><span class="sxs-lookup"><span data-stu-id="0a467-111">If you need to perform another task before finishing the interaction, you can choose **Cancel** and then finish the interaction at a later time.</span></span> <span data-ttu-id="0a467-112">Взаимодействие будет отложено.</span><span class="sxs-lookup"><span data-stu-id="0a467-112">This postpones the interaction.</span></span>

## <a name="to-finish-and-delete-postponed-interactions"></a><span data-ttu-id="0a467-113">Завершение и удаление отложенных взаимодействий</span><span class="sxs-lookup"><span data-stu-id="0a467-113">To finish and delete postponed interactions</span></span>
1. <span data-ttu-id="0a467-114">Откройте контакт, менеджера по продажам или операцию журнала взаимодействий.</span><span class="sxs-lookup"><span data-stu-id="0a467-114">Open the contact, salesperson, or interaction log entry.</span></span>
2. <span data-ttu-id="0a467-115">Выберите **Отложенные взаимодействия**.</span><span class="sxs-lookup"><span data-stu-id="0a467-115">Choose **Postponed Interactions**.</span></span>
3. <span data-ttu-id="0a467-116">Выберите взаимодействие, которое требуется завершить, а затем выберите действие **Возобновить**.</span><span class="sxs-lookup"><span data-stu-id="0a467-116">Select the interaction you want to finish, and then choose the **Resume** action.</span></span>

## <a name="to-create-an-interaction-on-a-segment"></a><span data-ttu-id="0a467-117">Создание взаимодействия для сегмента</span><span class="sxs-lookup"><span data-stu-id="0a467-117">To create an interaction on a segment</span></span>
1. <span data-ttu-id="0a467-118">На начальной странице выберите **Активные сегменты** или выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Сегменты**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="0a467-118">On the Home page, choose **Active Segments**, or choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Segments**, and then choose the related link.</span></span>
2. <span data-ttu-id="0a467-119">В окне **Сегмент** в разделе **Взаимодействие** заполните поля, чтобы указать, какое взаимодействие следует назначить сегменту.</span><span class="sxs-lookup"><span data-stu-id="0a467-119">In the **Segment window**, in the **Interaction** section, fill in the fields to specify which interaction you want to assign to the segment.</span></span>

    <span data-ttu-id="0a467-120">После назначения взаимодействия сегменту можно персонализировать взаимодействие для каждого отдельного контакта внутри сегмента, например, выбрав другой шаблон взаимодействия в строках окна **Сегмент**.</span><span class="sxs-lookup"><span data-stu-id="0a467-120">After you have assigned an interaction to the segment, you can personalize the interaction for each particular contact within the segment, for example, by selecting another interaction template on the lines in the **Segment** window.</span></span>  
3. <span data-ttu-id="0a467-121">Чтобы зарегистрировать сегмент и взаимодействия, выберите действие **Журнал**.</span><span class="sxs-lookup"><span data-stu-id="0a467-121">To log the segment and interactions, choose the **Log** action.</span></span> <span data-ttu-id="0a467-122">Откроется окно **Регистрировать сегмент**.</span><span class="sxs-lookup"><span data-stu-id="0a467-122">The **Log Segment** window opens.</span></span>
4. <span data-ttu-id="0a467-123">Если необходимо создать новый сегмент с такими же контактами, установите флажок **Создать контрольный сегмент**.</span><span class="sxs-lookup"><span data-stu-id="0a467-123">If you want to create a new segment containing the same contacts, select the **Create Follow-up Segment** check box.</span></span> <span data-ttu-id="0a467-124">Чтобы создать контрольный сегмент, необходимо указать серии номеров для сегментов в окне **Маркетинг - настройка**.</span><span class="sxs-lookup"><span data-stu-id="0a467-124">To create a follow-up segment, you must have specified number series for segments in the **Marketing Setup** window.</span></span>

<span data-ttu-id="0a467-125">Взаимодействие записывается для каждого контакта внутри сегмента в таблице **Журнал взаимодействия**, а сегмент регистрируется.</span><span class="sxs-lookup"><span data-stu-id="0a467-125">An interaction is recorded for each contact within the segment in the **Interaction Log Entry** table, and the segment is logged.</span></span> <span data-ttu-id="0a467-126">Фиксированные сегменты могут быть найдены в окне **Зарегистрированный cегмент**.</span><span class="sxs-lookup"><span data-stu-id="0a467-126">Logged segments can be found in the **Logged Segment** window.</span></span>

<span data-ttu-id="0a467-127">Если установлен флажок в поле **Создать контрольный сегмент**, программа автоматически создает новый сегмент, содержащий те же контакты, что и только что зарегистрированный.</span><span class="sxs-lookup"><span data-stu-id="0a467-127">If you have selected the **Create Follow-up Segment** check box, a new segment is created that contains the same contacts as the segment you have just logged.</span></span>

## <a name="see-also"></a><span data-ttu-id="0a467-128">См. также</span><span class="sxs-lookup"><span data-stu-id="0a467-128">See Also</span></span>
[<span data-ttu-id="0a467-129">Регистрация взаимодействий</span><span class="sxs-lookup"><span data-stu-id="0a467-129">Recording Interactions</span></span>](marketing-interactions.md)  
[<span data-ttu-id="0a467-130">Управление контактами</span><span class="sxs-lookup"><span data-stu-id="0a467-130">Managing Contacts</span></span>](marketing-contacts.md)  
[<span data-ttu-id="0a467-131">Управление возможностями продаж</span><span class="sxs-lookup"><span data-stu-id="0a467-131">Managing Sales Opportunities</span></span>](marketing-manage-sales-opportunities.md)  
[<span data-ttu-id="0a467-132">Настройка управления отношениями</span><span class="sxs-lookup"><span data-stu-id="0a467-132">Setting Up Relationship Management</span></span>](marketing-setup-marketing.md)  
[<span data-ttu-id="0a467-133">Работа с Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="0a467-133">Working with Dynamics 365</span></span>](ui-work-product.md)

