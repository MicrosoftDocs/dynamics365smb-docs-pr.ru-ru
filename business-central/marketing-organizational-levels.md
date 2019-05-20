---
title: Настройка организационных уровней для контактных лиц | Документы Майкрософт
description: В можете определить организационный уровень и назначить его контакту, чтобы указать положение, которое они занимают в организации, например относятся к высшему руководству.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, client, prospect
ms.date: 04/01/2019
ms.author: jswymer
redirect_url: marketing-setup-contacts
ms.openlocfilehash: 68f20af84652f684eaa0d69c98e0dc3cb722ee91
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1242932"
---
# <a name="set-up-organizational-levels-for-contact-persons"></a><span data-ttu-id="2dc62-103">Настройка организационных уровней для контактных лиц</span><span class="sxs-lookup"><span data-stu-id="2dc62-103">Set Up Organizational Levels for Contact Persons</span></span>
<span data-ttu-id="2dc62-104">Вы можете использовать организационные уровни для контактов, чтобы задавать положение, которое они занимают в организации, например относятся к высшему руководству.</span><span class="sxs-lookup"><span data-stu-id="2dc62-104">You can use organizational levels on your contacts to specify which position they have in the company, for example, top management.</span></span> <span data-ttu-id="2dc62-105">Эту информацию можно использовать при вводе информации о контактах.</span><span class="sxs-lookup"><span data-stu-id="2dc62-105">You can use this information when entering information about your contacts.</span></span>

<span data-ttu-id="2dc62-106">Использование организационных уровней для контактов — это двухэтапный процесс.</span><span class="sxs-lookup"><span data-stu-id="2dc62-106">Using organizational levels on contacts is a two-step process.</span></span> <span data-ttu-id="2dc62-107">Сначала вы определяете код организационного уровня.</span><span class="sxs-lookup"><span data-stu-id="2dc62-107">First, you define the organizational level code.</span></span> <span data-ttu-id="2dc62-108">Этот шаг нужно выполнить один раз для каждого организационного уровня.</span><span class="sxs-lookup"><span data-stu-id="2dc62-108">You only have to perform this step one time for each organizational level.</span></span> <span data-ttu-id="2dc62-109">После настройки кода организационного уровня можно начинать назначение кода контактным лицам.</span><span class="sxs-lookup"><span data-stu-id="2dc62-109">Once you have an organizational level code, you can start to assign the code to contact persons.</span></span>

## <a name="to-define-an-organizational-level-code"></a><span data-ttu-id="2dc62-110">Определение кода организационного уровня</span><span class="sxs-lookup"><span data-stu-id="2dc62-110">To define an organizational level code</span></span>
<span data-ttu-id="2dc62-111">Код организационного уровня определяет тип или категорию организационного уровня, например ГЕД или ФИД.</span><span class="sxs-lookup"><span data-stu-id="2dc62-111">The organizational level code defines the type or category of the organizational level, such a CEO  or CFO.</span></span> <span data-ttu-id="2dc62-112">Допускается наличие нескольких кодов организационных уровней.</span><span class="sxs-lookup"><span data-stu-id="2dc62-112">You can have several organizational level codes.</span></span> <span data-ttu-id="2dc62-113">Для определения организационного уровня используется страница **Организационные уровни**.</span><span class="sxs-lookup"><span data-stu-id="2dc62-113">To define the organizational level, you use the **Organizational Levels** page.</span></span>

1. <span data-ttu-id="2dc62-114">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Организационные уровни**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2dc62-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Organizational Levels**, and then choose the related link.</span></span>
2. <span data-ttu-id="2dc62-115">Выберите действие **Создать**, введите код и описание.</span><span class="sxs-lookup"><span data-stu-id="2dc62-115">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="2dc62-116">Длина кода не должна превышать 11 знаков (допускается сочетание букв и цифр).</span><span class="sxs-lookup"><span data-stu-id="2dc62-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="to-assign-organizational-levels-to-a-contact-person"></a><span data-ttu-id="2dc62-117">Назначение организационных уровней контактному лицу</span><span class="sxs-lookup"><span data-stu-id="2dc62-117">To assign organizational levels to a contact person</span></span>
<span data-ttu-id="2dc62-118">Организационные уровни можно назначать только контактным лицам, а не контактным организациям.</span><span class="sxs-lookup"><span data-stu-id="2dc62-118">You can assign organizational levels to contact persons only, not contact companies.</span></span> <span data-ttu-id="2dc62-119">Каждому контакту можно назначить только один организационный уровень.</span><span class="sxs-lookup"><span data-stu-id="2dc62-119">You can only assign one organizational level to each contact.</span></span>

1. <span data-ttu-id="2dc62-120">Откройте контакт.</span><span class="sxs-lookup"><span data-stu-id="2dc62-120">Open the contact.</span></span>
2. <span data-ttu-id="2dc62-121">В поле **Организационные уровни** выберите код, который нужно назначить.</span><span class="sxs-lookup"><span data-stu-id="2dc62-121">In the **Organizational Levels** field, select the code you want to assign.</span></span>

<span data-ttu-id="2dc62-122">После назначения организационных уровней контактам можно использовать эту информацию для создания сегментов.</span><span class="sxs-lookup"><span data-stu-id="2dc62-122">After you have assigned organizational levels to your contacts, you can use this information to create segments.</span></span>

<span data-ttu-id="2dc62-123">После назначения контактам должностных обязанностей можно использовать эту информацию для выбора контактов для сегмента.</span><span class="sxs-lookup"><span data-stu-id="2dc62-123">After you have assigned job responsibilities to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="2dc62-124">Дополнительные сведения см. в разделе [Добавление контактов к сегментам](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="2dc62-124">For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="2dc62-125">См. также</span><span class="sxs-lookup"><span data-stu-id="2dc62-125">See Also</span></span>
[<span data-ttu-id="2dc62-126">Создание контактов</span><span class="sxs-lookup"><span data-stu-id="2dc62-126">Creating Contacts</span></span>](marketing-create-contact-companies.md)  
<span data-ttu-id="2dc62-127">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2dc62-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
