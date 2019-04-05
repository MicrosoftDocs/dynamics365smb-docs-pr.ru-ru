---
title: Настройка веб-источников в контактных организациях | Документы Майкрософт
description: Вы можете определить интернет- и веб-источники и назначить их контактной организации, чтобы вам было проще находить информацию о своих контактах.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: internet
ms.date: 10/01/2018
ms.author: jswymer
redirect_url: marketing-setup-contacts
ms.openlocfilehash: 22b9f0be189fa24f366c1ffa20934d2d8e7e8fc5
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "804688"
---
# <a name="set-up-web-sources-for-contact-companies"></a><span data-ttu-id="23470-103">Настройка веб-источников для контактных организаций</span><span class="sxs-lookup"><span data-stu-id="23470-103">Set Up Web Sources for Contact Companies</span></span>
<span data-ttu-id="23470-104">Можно присваивать веб-источники с контактными организациям, чтобы определять, например, поисковые системы и веб-сайты в Интернете, которые должны использоваться для поиска информации о контактах.</span><span class="sxs-lookup"><span data-stu-id="23470-104">You can use web sources with your contact companies to identify, for example, search engines and web sites, on the Internet that you want to use to search for information about the contacts.</span></span> <span data-ttu-id="23470-105">При присвоении веб-источников указывается, какую поисковую систему и какое слово поиска приложение использует для поиска требуемой информации.</span><span class="sxs-lookup"><span data-stu-id="23470-105">When assigning web sources, you specify which search engine and search word the application will use to find the requested information.</span></span>

<span data-ttu-id="23470-106">Использование веб-источников для контактов — это двухэтапный процесс.</span><span class="sxs-lookup"><span data-stu-id="23470-106">Using web sources on contacts is a two-step process.</span></span> <span data-ttu-id="23470-107">Сначала вы определяете код веб-источника.</span><span class="sxs-lookup"><span data-stu-id="23470-107">First, you define the web source code.</span></span> <span data-ttu-id="23470-108">Этот шаг нужно выполнить один раз для каждого веб-источника.</span><span class="sxs-lookup"><span data-stu-id="23470-108">You only have to perform this step one time for each web source.</span></span> <span data-ttu-id="23470-109">После настройки кода веб-источника можно начинать назначение кода контактным лицам.</span><span class="sxs-lookup"><span data-stu-id="23470-109">Once you have a web source code, you can start to assign the code to contact persons.</span></span>

## <a name="to-define-a-web-source-code"></a><span data-ttu-id="23470-110">Определение кода веб-источника</span><span class="sxs-lookup"><span data-stu-id="23470-110">To define a web source code</span></span>
1. <span data-ttu-id="23470-111">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Веб-источники**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="23470-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Web Sources**, and then choose the related link.</span></span>
2. <span data-ttu-id="23470-112">Выберите действия **Создать**.</span><span class="sxs-lookup"><span data-stu-id="23470-112">Choose the **New** actions.</span></span>
3. <span data-ttu-id="23470-113">Заполните поля **Код**, **Описание** и **URL-адрес**.</span><span class="sxs-lookup"><span data-stu-id="23470-113">Fill in the **Code**, **Description**, and **URL** fields.</span></span>

    <span data-ttu-id="23470-114">В поле **URL-адрес** введите %1 для вставки заполнителя для слова поиска в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="23470-114">Type %1 in the **URL** field to insert a placeholder for a search word in the URL.</span></span> <span data-ttu-id="23470-115">При запуске веб-источника из контакта %1 заменяется на слово поиска (например, на название организации), которое было введено на странице **Веб-источники контакта**.</span><span class="sxs-lookup"><span data-stu-id="23470-115">When you launch the web source from a contact, the %1 is replaced with the search word, for example, the name of the company that you have entered on the **Contact Web Sources** page.</span></span>

<span data-ttu-id="23470-116">Повторите эти шаги, чтобы настроить необходимое количество веб-источников.</span><span class="sxs-lookup"><span data-stu-id="23470-116">Repeat these steps to set up as many web sources as you want.</span></span>

## <a name="to-assign-web-sources-to-a-contact-company"></a><span data-ttu-id="23470-117">Назначение веб-источников контактной организации</span><span class="sxs-lookup"><span data-stu-id="23470-117">To assign web sources to a contact company</span></span>
<span data-ttu-id="23470-118">При назначении веб-источников вы указываете, какую поисковую систему и какое слово поиска приложение будет использовать для поиска требуемой информации.</span><span class="sxs-lookup"><span data-stu-id="23470-118">When assigning web sources, you specify which search engine and search word that the application will use to find the requested information.</span></span>

1. <span data-ttu-id="23470-119">Откройте контакт.</span><span class="sxs-lookup"><span data-stu-id="23470-119">Open the contact.</span></span>
2. <span data-ttu-id="23470-120">Выберите действие **Организация**, а затем — действие **Веб-источники**.</span><span class="sxs-lookup"><span data-stu-id="23470-120">Choose the **Company** action, and then choose the **Web Sources** action.</span></span> <span data-ttu-id="23470-121">Откроется страница **Веб-источники контакта**.</span><span class="sxs-lookup"><span data-stu-id="23470-121">The **Contact Web Sources** page opens.</span></span>
3. <span data-ttu-id="23470-122">В поле **Код веб-источника** выберите веб-источник, который нужно назначить.</span><span class="sxs-lookup"><span data-stu-id="23470-122">In the **Web Source Code** field, choose the web source you want to assign.</span></span>
4. <span data-ttu-id="23470-123">В поле **Поиск слова** введите искомое слово, используемое для поиска информации.</span><span class="sxs-lookup"><span data-stu-id="23470-123">In the **Search Word** field, enter the search word that you want to use to find the information.</span></span>

<span data-ttu-id="23470-124">Повторите эти шаги для назначения желаемого количества веб-источников.</span><span class="sxs-lookup"><span data-stu-id="23470-124">Repeat these steps to assign as many web sources as you want.</span></span>

<span data-ttu-id="23470-125">Также можно назначать веб-источники на странице **Список контактов**, следуя той же процедуре.</span><span class="sxs-lookup"><span data-stu-id="23470-125">You can also assign web sources from the **Contact List** page by following the same procedure.</span></span>

## <a name="see-also"></a><span data-ttu-id="23470-126">См. также</span><span class="sxs-lookup"><span data-stu-id="23470-126">See Also</span></span>
[<span data-ttu-id="23470-127">Создание контактов</span><span class="sxs-lookup"><span data-stu-id="23470-127">Creating Contacts</span></span>](marketing-create-contact-companies.md)  
<span data-ttu-id="23470-128">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="23470-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
