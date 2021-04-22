---
title: Конфигурирование шаблонов API | Документация Майкрософт
description: Описываются действия, которые необходимо выполнить для настройки шаблонов API для Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: API templates, configuring templates
ms.date: 04/01/2021
ms.author: solsen
ms.openlocfilehash: 7d39262993a173fec1eae68bcb44a85332a9866a
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5773108"
---
# <a name="configuring-api-templates"></a><span data-ttu-id="322eb-103">Конфигурирование шаблонов API</span><span class="sxs-lookup"><span data-stu-id="322eb-103">Configuring API Templates</span></span>
<span data-ttu-id="322eb-104">Библиотека API для [!INCLUDE[prod_short_md](includes/prod_short.md)] предоставляет разработчикам упрощенное представление лежащих в ее основе объектов.</span><span class="sxs-lookup"><span data-stu-id="322eb-104">The API library for [!INCLUDE[prod_short_md](includes/prod_short.md)] provides a simplified representation of the underlying entities.</span></span> <span data-ttu-id="322eb-105">Не все свойства в приложении предоставляются через связанный API.</span><span class="sxs-lookup"><span data-stu-id="322eb-105">All the properties in the application are not exposed through the associated API.</span></span> <span data-ttu-id="322eb-106">Страница **Настройка API** позволяет определить шаблоны, используемые для заполнения пустых свойств в объекте при создании действия POST через API.</span><span class="sxs-lookup"><span data-stu-id="322eb-106">The **API Setup** page allows you to define templates that are used to populate empty properties on an entity when you create a POST action through the API.</span></span> 

<span data-ttu-id="322eb-107">Например, если для объекта товара определен шаблон конфигурации, при создании новой записи товара через API товаров все свойства нового товара, не определенные в вызове API, будут заполняться из выбранного шаблона.</span><span class="sxs-lookup"><span data-stu-id="322eb-107">For example, if a configuration template is defined for the item entity, when a new item record is created through the items API, any properties for the new item that are not defined in the API call will be populated from the selected template.</span></span> <span data-ttu-id="322eb-108">Например, если для поля **Общая товарная группа** не задается значение через API, однако значение задано в выбранном шаблоне, то к новому товару будет применено значение товарной группы, определенное в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="322eb-108">If, for example, no value is defined for the **Gen. Prod. Posting Group** field through the API, but a value is defined in the selected template, then the posting group value defined in the template will be applied to the new item.</span></span> 

## <a name="setting-up-the-entity-template"></a><span data-ttu-id="322eb-109">Создание шаблона объекта</span><span class="sxs-lookup"><span data-stu-id="322eb-109">Setting up the Entity Template</span></span>
<span data-ttu-id="322eb-110">Чтобы использовать шаблоны с библиотекой API, необходимо сначала создать шаблоны и определить для них свойства.</span><span class="sxs-lookup"><span data-stu-id="322eb-110">To use templates with the API library, you must first set up and define properties for the templates.</span></span> <span data-ttu-id="322eb-111">Создать эти шаблоны можно на странице **Шаблоны конфигурации**.</span><span class="sxs-lookup"><span data-stu-id="322eb-111">You can set up these templates on the **Configuration Templates** page.</span></span> <span data-ttu-id="322eb-112">Дополнительные сведения см. в разделе [Подготовка к миграции данных клиента](admin-use-templates-to-prepare-customer-data-for-migration.md).</span><span class="sxs-lookup"><span data-stu-id="322eb-112">For more information, see [Prepare to Migrate Customer Data](admin-use-templates-to-prepare-customer-data-for-migration.md).</span></span> 

## <a name="assign-the-template-to-an-api"></a><span data-ttu-id="322eb-113">Назначение шаблона API-интерфейсу</span><span class="sxs-lookup"><span data-stu-id="322eb-113">Assign the template to an API</span></span>

<span data-ttu-id="322eb-114">Чтобы назначить шаблон API-интерфейсу, необходимо выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="322eb-114">To assign a template to an API, you must go through the following steps.</span></span>

1. <span data-ttu-id="322eb-115">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка API**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="322eb-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **API Setup**, and choose the related link.</span></span>
2. <span data-ttu-id="322eb-116">Выберите **Создать**, а затем выберите значение поля **Порядок** для записи.</span><span class="sxs-lookup"><span data-stu-id="322eb-116">Choose **New**, and then choose the **Order** value for the record.</span></span>  
<span data-ttu-id="322eb-117">Если для API (ИД страницы) выбрано несколько шаблонов, шаблоны применяются в порядке, определенном в поле **Порядок**.</span><span class="sxs-lookup"><span data-stu-id="322eb-117">If there is more than one template selected for an API (Page ID), the templates are applied in the order defined in the **Order** column.</span></span>   
<span data-ttu-id="322eb-118">При применении каждого шаблона значения полей, определенные в шаблоне, применяются только к полям, для которых еще не задано значение — либо явно в API, либо в ранее примененном согласно порядку шаблоне.</span><span class="sxs-lookup"><span data-stu-id="322eb-118">When each template is applied, field values defined in the template are only applied to fields that have not already had a value defined, either explicitly in the API, or in a previously applied template in the order.</span></span> 
3. <span data-ttu-id="322eb-119">Выберите значение в поле **ИД страницы**.</span><span class="sxs-lookup"><span data-stu-id="322eb-119">Select a **Page ID** value.</span></span>  
<span data-ttu-id="322eb-120">Это страница для API, к которому будет применяться шаблон.</span><span class="sxs-lookup"><span data-stu-id="322eb-120">This is the page for the API to which the template will be applied.</span></span> <span data-ttu-id="322eb-121">Поиск в поле **ИД страницы** выводит список всех API-интерфейсов, имеющихся в библиотеке.</span><span class="sxs-lookup"><span data-stu-id="322eb-121">The **Page ID** lookup provides a list of all APIs available in the library.</span></span>
4. <span data-ttu-id="322eb-122">Выберите значение в поле **Код шаблона**.</span><span class="sxs-lookup"><span data-stu-id="322eb-122">Select a value in the **Template Code** field.</span></span>  
<span data-ttu-id="322eb-123">Код шаблона — это код для шаблона, который был определен на странице **Шаблоны конфигураций**.</span><span class="sxs-lookup"><span data-stu-id="322eb-123">The template code is the code for the template that was defined on the **Configuration Templates** page.</span></span> <span data-ttu-id="322eb-124">Определенные в шаблоне значения применяются к API.</span><span class="sxs-lookup"><span data-stu-id="322eb-124">The template values defined are applied to the API.</span></span> 
5. <span data-ttu-id="322eb-125">В поле **Условия** укажите, какой шаблон должен быть применен.</span><span class="sxs-lookup"><span data-stu-id="322eb-125">In the **Conditions** field, specify which template should be applied.</span></span>  
<span data-ttu-id="322eb-126">Заданный шаблон применяется к новой записи, создаваемой через API, если и только если значения, уже определенные для нового экземпляра записи, соответствуют условиям, определенным в поле **Условия**.</span><span class="sxs-lookup"><span data-stu-id="322eb-126">The defined template is applied to a new record created through the API if, and only if, the conditions defined in the **Conditions** field are met by the values already defined for the new instance of the entity.</span></span>

## <a name="see-also"></a><span data-ttu-id="322eb-127">См. также</span><span class="sxs-lookup"><span data-stu-id="322eb-127">See Also</span></span>
[<span data-ttu-id="322eb-128">Документация по API</span><span class="sxs-lookup"><span data-stu-id="322eb-128">API Documentation</span></span>](/dynamics-nav/fin-graph)  
<span data-ttu-id="322eb-129">[Разработка приложений-связей [!INCLUDE[prod_short_md](includes/prod_short.md)]](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)</span><span class="sxs-lookup"><span data-stu-id="322eb-129">[Developing Connect Apps for [!INCLUDE[prod_short_md](includes/prod_short.md)]](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)</span></span>  
[<span data-ttu-id="322eb-130">Включение API</span><span class="sxs-lookup"><span data-stu-id="322eb-130">Enabling the APIs</span></span>](/dynamics-nav/enabling-apis-for-dynamics-nav)  
[<span data-ttu-id="322eb-131">Конечные точки для API</span><span class="sxs-lookup"><span data-stu-id="322eb-131">Endpoints for the APIs</span></span>](/dynamics-nav/endpoints-apis-for-dynamics)  
[<span data-ttu-id="322eb-132">Настройка организации со службами RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="322eb-132">Setting Up a Company with RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="322eb-133">Администрация</span><span class="sxs-lookup"><span data-stu-id="322eb-133">Administration</span></span>](admin-setup-and-administration.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]