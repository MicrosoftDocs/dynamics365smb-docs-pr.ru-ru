---
title: "Настройка отраслевых групп в контактных организациях | Документы Майкрософт"
description: "Описывается порядок определения отраслевой группы и ее назначения контактной организации, например в сфере розничной торговли или автомобильной промышленности."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: c7a8549a5c6528cafb5e2959a3391fb323fe92ca
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="set-up-industry-groups-for-contact-companies"></a><span data-ttu-id="d9d7f-103">Настройка отраслевых групп в контактных организациях</span><span class="sxs-lookup"><span data-stu-id="d9d7f-103">Set Up Industry Groups for Contact Companies</span></span>
<span data-ttu-id="d9d7f-104">Отраслевые группы используются для указания типа отрасли, к которой относится контакт, например розничная торговля или автомобильное производство.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-104">You use industry groups to indicate the type of industry to which your contacts belong, for example, the retail industry or the automobile industry.</span></span>

<span data-ttu-id="d9d7f-105">Использование отраслевых групп для контактов — это двухэтапный процесс.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-105">Using industry groups on contacts is a two-step process.</span></span> <span data-ttu-id="d9d7f-106">Сначала вы определяете код отраслевой группы.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-106">First, you define the industry group code.</span></span> <span data-ttu-id="d9d7f-107">Этот шаг нужно выполнить один раз для каждой отраслевой группы.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-107">You only have to perform this step one time for each industry group.</span></span> <span data-ttu-id="d9d7f-108">После настройки кода отраслевой группы можно начинать назначение кода контактным организациям.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-108">Once you have an industry group code, you can start to assign the code to contact companies.</span></span>

> [!NOTE]  
>   <span data-ttu-id="d9d7f-109">При планировании синхронизации контактов с поставщиками, клиентами или банковскими счетами в других частях приложения может понадобиться настроить для них деловое отношение.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-109">If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="to-define-an-industry-group-code"></a><span data-ttu-id="d9d7f-110">Определение кода отраслевой группы</span><span class="sxs-lookup"><span data-stu-id="d9d7f-110">To define an industry group code</span></span>
<span data-ttu-id="d9d7f-111">Код отраслевой группы определяет тип или категорию группы, например РЕКЛАМА для сферы рекламы или ПРЕССА для ТВ и радио.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-111">The industry group code defines the type or category of the group, such as ADVERT for advertising, or PRESS, for TV and radio.</span></span> <span data-ttu-id="d9d7f-112">Допускается наличие нескольких кодов отраслевых групп.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-112">You can have several industry group codes.</span></span> <span data-ttu-id="d9d7f-113">Для определения отраслевых групп используется окно **Отраслевые группы**.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-113">To define the industry groups, you use the **Industry Groups** window.</span></span>

1. <span data-ttu-id="d9d7f-114">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Отраслевые группы**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Industry Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="d9d7f-115">Выберите действие **Создать**, введите код и описание.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-115">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="d9d7f-116">Длина кода не должна превышать 11 знаков (допускается сочетание букв и цифр).</span><span class="sxs-lookup"><span data-stu-id="d9d7f-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="AssignIndustryGroupContact"></a> <span data-ttu-id="d9d7f-117">Присвоение отраслевых групп контакту</span><span class="sxs-lookup"><span data-stu-id="d9d7f-117">To assign industry groups to a contact</span></span>
<span data-ttu-id="d9d7f-118">Нельзя назначать отраслевые группы контактным лицам — только организациям.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-118">You cannot assign industry groups to a contact person - only companies.</span></span>

1. <span data-ttu-id="d9d7f-119">Откройте контакт.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-119">Open the contact.</span></span>
2. <span data-ttu-id="d9d7f-120">Выберите действие **Организация**, а затем действие **Отраслевые группы**.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-120">Choose the **Company** action, and then the **Industry Groups** action.</span></span> <span data-ttu-id="d9d7f-121">Откроется окно **Отраслевые группы контакта**.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-121">The **Contact Industry Groups** window opens.</span></span>
3. <span data-ttu-id="d9d7f-122">В поле **Код отраслевой группы** выберите отраслевую группу, которую нужно назначить.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-122">In the **Industry Groups Code** field, select the industry groups you want to assign.</span></span>

<span data-ttu-id="d9d7f-123">Повторите эти шаги для назначения желаемого количества отраслевых групп.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-123">Repeat these steps to assign as many industry groups as you want.</span></span> <span data-ttu-id="d9d7f-124">Также можно назначать отраслевые группы из списка контактов, следуя той же процедуре.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-124">You can also assign industry groups from the contact list by following the same procedure.</span></span>

<span data-ttu-id="d9d7f-125">Число отраслевых групп, назначенных контакту, отображается в окне **Контакт** в разделе **Сегментация** в поле **Число отраслевых групп**.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-125">The number of industry groups that you have assigned to the contact is displayed in the **No. of Industry Groups** field in the **Segmentation** section in the **Contact** window.</span></span>

<span data-ttu-id="d9d7f-126">После назначения контактам отраслевых групп эта информация может использоваться для выбора контактов для сегментов.</span><span class="sxs-lookup"><span data-stu-id="d9d7f-126">After you have assigned industry groups to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="d9d7f-127">Дополнительные сведения см. в разделе [Добавление контактов к сегментам](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="d9d7f-127">For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="d9d7f-128">См. также</span><span class="sxs-lookup"><span data-stu-id="d9d7f-128">See Also</span></span>
[<span data-ttu-id="d9d7f-129">Создание контактных организаций</span><span class="sxs-lookup"><span data-stu-id="d9d7f-129">Creating Contact Companies</span></span>](marketing-create-contact-companies.md)  
<span data-ttu-id="d9d7f-130">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d9d7f-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

