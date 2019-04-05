---
title: Настройка отраслевых групп в контактных организациях | Документы Майкрософт
description: Описывается порядок определения отраслевой группы и ее назначения контактной организации, например в сфере розничной торговли или автомобильной промышленности.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 10/01/2018
ms.author: jswymer
redirect_url: marketing-setup-contacts
ms.openlocfilehash: 61d1385691a0ed2bdc11745e98b14fa57e50475a
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "805026"
---
# <a name="set-up-industry-groups-for-contact-companies"></a><span data-ttu-id="97fef-103">Настройка отраслевых групп в контактных организациях</span><span class="sxs-lookup"><span data-stu-id="97fef-103">Set Up Industry Groups for Contact Companies</span></span>
<span data-ttu-id="97fef-104">Отраслевые группы используются для указания типа отрасли, к которой относится контакт, например розничная торговля или автомобильное производство.</span><span class="sxs-lookup"><span data-stu-id="97fef-104">You use industry groups to indicate the type of industry to which your contacts belong, for example, the retail industry or the automobile industry.</span></span>

<span data-ttu-id="97fef-105">Использование отраслевых групп для контактов — это двухэтапный процесс.</span><span class="sxs-lookup"><span data-stu-id="97fef-105">Using industry groups on contacts is a two-step process.</span></span> <span data-ttu-id="97fef-106">Сначала вы определяете код отраслевой группы.</span><span class="sxs-lookup"><span data-stu-id="97fef-106">First, you define the industry group code.</span></span> <span data-ttu-id="97fef-107">Этот шаг нужно выполнить один раз для каждой отраслевой группы.</span><span class="sxs-lookup"><span data-stu-id="97fef-107">You only have to perform this step one time for each industry group.</span></span> <span data-ttu-id="97fef-108">После настройки кода отраслевой группы можно начинать назначение кода контактным организациям.</span><span class="sxs-lookup"><span data-stu-id="97fef-108">Once you have an industry group code, you can start to assign the code to contact companies.</span></span>

> [!NOTE]  
>   <span data-ttu-id="97fef-109">При планировании синхронизации контактов с поставщиками, клиентами или банковскими счетами в других частях приложения может понадобиться настроить для них деловое отношение.</span><span class="sxs-lookup"><span data-stu-id="97fef-109">If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="to-define-an-industry-group-code"></a><span data-ttu-id="97fef-110">Определение кода отраслевой группы</span><span class="sxs-lookup"><span data-stu-id="97fef-110">To define an industry group code</span></span>
<span data-ttu-id="97fef-111">Код отраслевой группы определяет тип или категорию группы, например РЕКЛАМА для сферы рекламы или ПРЕССА для ТВ и радио.</span><span class="sxs-lookup"><span data-stu-id="97fef-111">The industry group code defines the type or category of the group, such as ADVERT for advertising, or PRESS, for TV and radio.</span></span> <span data-ttu-id="97fef-112">Допускается наличие нескольких кодов отраслевых групп.</span><span class="sxs-lookup"><span data-stu-id="97fef-112">You can have several industry group codes.</span></span> <span data-ttu-id="97fef-113">Для определения отраслевых групп используется страница **Отраслевые группы**.</span><span class="sxs-lookup"><span data-stu-id="97fef-113">To define the industry groups, you use the **Industry Groups** page.</span></span>

1. <span data-ttu-id="97fef-114">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Отраслевые группы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="97fef-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Industry Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="97fef-115">Выберите действие **Создать**, введите код и описание.</span><span class="sxs-lookup"><span data-stu-id="97fef-115">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="97fef-116">Длина кода не должна превышать 11 знаков (допускается сочетание букв и цифр).</span><span class="sxs-lookup"><span data-stu-id="97fef-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="AssignIndustryGroupContact"></a> <span data-ttu-id="97fef-117">Присвоение отраслевых групп контакту</span><span class="sxs-lookup"><span data-stu-id="97fef-117">To assign industry groups to a contact</span></span>
<span data-ttu-id="97fef-118">Нельзя назначать отраслевые группы контактным лицам — только организациям.</span><span class="sxs-lookup"><span data-stu-id="97fef-118">You cannot assign industry groups to a contact person - only companies.</span></span>

1. <span data-ttu-id="97fef-119">Откройте контакт.</span><span class="sxs-lookup"><span data-stu-id="97fef-119">Open the contact.</span></span>
2. <span data-ttu-id="97fef-120">Выберите действие **Организация**, а затем действие **Отраслевые группы**.</span><span class="sxs-lookup"><span data-stu-id="97fef-120">Choose the **Company** action, and then the **Industry Groups** action.</span></span> <span data-ttu-id="97fef-121">Откроется страница **Отраслевые группы контакта**.</span><span class="sxs-lookup"><span data-stu-id="97fef-121">The **Contact Industry Groups** page opens.</span></span>
3. <span data-ttu-id="97fef-122">В поле **Код отраслевой группы** выберите отраслевую группу, которую нужно назначить.</span><span class="sxs-lookup"><span data-stu-id="97fef-122">In the **Industry Groups Code** field, select the industry groups you want to assign.</span></span>

<span data-ttu-id="97fef-123">Повторите эти шаги для назначения желаемого количества отраслевых групп.</span><span class="sxs-lookup"><span data-stu-id="97fef-123">Repeat these steps to assign as many industry groups as you want.</span></span> <span data-ttu-id="97fef-124">Также можно назначать отраслевые группы из списка контактов, следуя той же процедуре.</span><span class="sxs-lookup"><span data-stu-id="97fef-124">You can also assign industry groups from the contact list by following the same procedure.</span></span>

<span data-ttu-id="97fef-125">Число отраслевых групп, назначенных контакту, отображается в окне **Контакт** в разделе **Сегментация** на странице **Число отраслевых групп**.</span><span class="sxs-lookup"><span data-stu-id="97fef-125">The number of industry groups that you have assigned to the contact is displayed in the **No. of Industry Groups** field in the **Segmentation** section on the **Contact** page.</span></span>

<span data-ttu-id="97fef-126">После назначения контактам отраслевых групп эта информация может использоваться для выбора контактов для сегментов.</span><span class="sxs-lookup"><span data-stu-id="97fef-126">After you have assigned industry groups to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="97fef-127">Дополнительные сведения см. в разделе [Добавление контактов к сегментам](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="97fef-127">For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="97fef-128">См. также</span><span class="sxs-lookup"><span data-stu-id="97fef-128">See Also</span></span>
[<span data-ttu-id="97fef-129">Создание контактов</span><span class="sxs-lookup"><span data-stu-id="97fef-129">Creating Contacts</span></span>](marketing-create-contact-companies.md)  
<span data-ttu-id="97fef-130">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="97fef-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
