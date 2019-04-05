---
title: Отслеживание сегментов и соответствующих взаимодействий | Документы Майкрософт
description: Узнайте о создании сегментов для определения групп контактов и определения взаимодействий для сегментов.
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
ms.openlocfilehash: 1fcec3051fdabae818528742fba5d9ca57a721c8
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "805277"
---
# <a name="managing-interactions-for-segments"></a><span data-ttu-id="ff360-103">Управление взаимодействиями для сегментов</span><span class="sxs-lookup"><span data-stu-id="ff360-103">Managing Interactions for Segments</span></span>
<span data-ttu-id="ff360-104">Страница **Сегмент** является своеобразным рабочим листом, где можно:</span><span class="sxs-lookup"><span data-stu-id="ff360-104">The **Segment** page is a type of worksheet where you can:</span></span>

* <span data-ttu-id="ff360-105">создавать сегменты;</span><span class="sxs-lookup"><span data-stu-id="ff360-105">Create segments.</span></span>
* <span data-ttu-id="ff360-106">сохранять критерии сегментации, использовавшиеся для выбора контактов;</span><span class="sxs-lookup"><span data-stu-id="ff360-106">Save the segmentation criteria you have used to select contacts.</span></span>
* <span data-ttu-id="ff360-107">записывать сегмент и регистрировать взаимодействия, содержащие контакты внутри этого сегмента.</span><span class="sxs-lookup"><span data-stu-id="ff360-107">Log the segment and record interactions involving the contacts within the segment.</span></span>

## <a name="segmenting"></a><span data-ttu-id="ff360-108">Сегментация</span><span class="sxs-lookup"><span data-stu-id="ff360-108">Segmenting</span></span>
<span data-ttu-id="ff360-109">Есть несколько способов создания сегментов:</span><span class="sxs-lookup"><span data-stu-id="ff360-109">There are several ways to create segments:</span></span>

* <span data-ttu-id="ff360-110">Можно вручную вводить контакты, которые надо включить в сегмент, в строках сегмента.</span><span class="sxs-lookup"><span data-stu-id="ff360-110">You can manually enter the contacts you want to include in the segment in the segment lines.</span></span>
* <span data-ttu-id="ff360-111">Можно выбрать контакты.</span><span class="sxs-lookup"><span data-stu-id="ff360-111">You can select contacts.</span></span>
* <span data-ttu-id="ff360-112">Можно повторно использовать зарегистрированный сегмент как базис для создания нового.</span><span class="sxs-lookup"><span data-stu-id="ff360-112">You can reuse a logged segment as the basis to create a new one.</span></span>
* <span data-ttu-id="ff360-113">Можно повторно использовать сохраненные критерии сегментации.</span><span class="sxs-lookup"><span data-stu-id="ff360-113">You can reuse saved segmentation criteria.</span></span>

## <a name="interactions"></a><span data-ttu-id="ff360-114">Взаимодействия</span><span class="sxs-lookup"><span data-stu-id="ff360-114">Interactions</span></span>
<span data-ttu-id="ff360-115">На странице **Сегмент** можно создавать взаимодействия для нескольких контактов одновременно.</span><span class="sxs-lookup"><span data-stu-id="ff360-115">On the **Segment** page, you can create interactions for several contacts simultaneously.</span></span> <span data-ttu-id="ff360-116">Например, можно связать сегмент с документом Microsoft Word, для того чтобы можно было отправить письмо всем контактам в сегменте.</span><span class="sxs-lookup"><span data-stu-id="ff360-116">For example, you can merge a segment with a Microsoft Word document, so that you can send a letter to all the contacts in the segment.</span></span>

<span data-ttu-id="ff360-117">Можно указать информацию о взаимодействии для сегмента в заголовке **Сегмент**.</span><span class="sxs-lookup"><span data-stu-id="ff360-117">You can specify information about the interaction for the segment on the **Segment** header.</span></span> <span data-ttu-id="ff360-118">Например, можно выбрать, какой шаблон взаимодействия следует использовать для всех контактов, задать описание, тип корреспонденции и т. д.</span><span class="sxs-lookup"><span data-stu-id="ff360-118">For example, you can decide which interaction template you want to use for all the contacts, specify a description, a correspondence type, and so on.</span></span> <span data-ttu-id="ff360-119">Однако вы можете изменять эту информацию в строках сегмента для каждого отдельного контакта, например задавая другое описание для одного контакта.</span><span class="sxs-lookup"><span data-stu-id="ff360-119">However, you can modify this information in the segment line for each particular contact, for example, by specifying another description for one contact.</span></span> <span data-ttu-id="ff360-120">При слиянии сегмента с документом Microsoft Word можно персонализировать документ для отправки нескольким контактам внутри сегмента, например добавляя индивидуализированные комментарии к документу.</span><span class="sxs-lookup"><span data-stu-id="ff360-120">If you are merging a segment with a Microsoft Word document, you can personalize the document to be sent for one or several of the contacts within the segment, for example, by adding individualized comments to the document.</span></span>

## <a name="logging"></a><span data-ttu-id="ff360-121">Регистрация</span><span class="sxs-lookup"><span data-stu-id="ff360-121">Logging</span></span>
<span data-ttu-id="ff360-122">Если щелкнуть **Журнал** на странице **Сегмент**, приложение зарегистрирует взаимодействия на странице **Журнал взаимодействия** и зафиксирует сегмент.</span><span class="sxs-lookup"><span data-stu-id="ff360-122">On the **Segment** page, when you choose **Log**, the application records the interactions on the **Interaction Log Entry** page, and logs the segment.</span></span> <span data-ttu-id="ff360-123">После того, как сегмент зарегистрирован, его можно найти только на странице **Зарегистрированные сегменты**.</span><span class="sxs-lookup"><span data-stu-id="ff360-123">After you have logged the segment, you can only find it on the **Logged Segments** page.</span></span>

<span data-ttu-id="ff360-124">На странице **Зарегистрированные сегменты** вы можете создать контрольный сегмент, содержащий те же контакты, что и в зарегистрированном сегменте.</span><span class="sxs-lookup"><span data-stu-id="ff360-124">On the **Logged Segments** page, you can decide to create a follow-up segment containing the same contacts as the segment you have logged.</span></span>

## <a name="see-also"></a><span data-ttu-id="ff360-125">См. также</span><span class="sxs-lookup"><span data-stu-id="ff360-125">See Also</span></span>
[<span data-ttu-id="ff360-126">Создание сегментов</span><span class="sxs-lookup"><span data-stu-id="ff360-126">Create Segments</span></span>](marketing-how-create-segment.md)  
[<span data-ttu-id="ff360-127">Создание взаимодействий для сегментов</span><span class="sxs-lookup"><span data-stu-id="ff360-127">Create Interactions for Segments</span></span>](marketing-how-create-interactions.md)  
[<span data-ttu-id="ff360-128">Управление сегментами</span><span class="sxs-lookup"><span data-stu-id="ff360-128">Managing Segments</span></span>](marketing-segments.md)  
[<span data-ttu-id="ff360-129">Регистрация взаимодействий с контактами</span><span class="sxs-lookup"><span data-stu-id="ff360-129">Recording Interactions With Contacts</span></span>](marketing-interactions.md)  
[<span data-ttu-id="ff360-130">Управление возможностями продаж</span><span class="sxs-lookup"><span data-stu-id="ff360-130">Managing Sales Opportunities</span></span>](marketing-manage-sales-opportunities.md)  
[<span data-ttu-id="ff360-131">Создание контактов и управление ими</span><span class="sxs-lookup"><span data-stu-id="ff360-131">Creating and Managing Contacts</span></span>](marketing-contacts.md)  
[<span data-ttu-id="ff360-132">Работа с Business Central</span><span class="sxs-lookup"><span data-stu-id="ff360-132">Working with Business Central</span></span>](ui-work-product.md)
