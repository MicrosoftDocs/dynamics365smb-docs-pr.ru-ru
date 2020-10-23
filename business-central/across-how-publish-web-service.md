---
title: Предоставление объектов как веб-службы
description: Публикуйте объекты как веб-службы, чтобы сделать их доступными сразу для вашего решения Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/08/2020
ms.author: edupont
ms.openlocfilehash: 658816cfb65580404bc8ef10472a5b62c6815c9e
ms.sourcegitcommit: 4bca699d2a5ce182eb5572d72fac4fb478c4f293
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/12/2020
ms.locfileid: "3989492"
---
# <a name="publish-a-web-service"></a><span data-ttu-id="95ea7-103">Публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="95ea7-103">Publish a Web Service</span></span>

<span data-ttu-id="95ea7-104">Веб-службы представляют облегченный способ сделать доступными функции приложений для различных внешних систем и пользователей.</span><span class="sxs-lookup"><span data-stu-id="95ea7-104">Web services are a lightweight way to make application functionality available to different kinds of external systems and users.</span></span> <span data-ttu-id="95ea7-105">По умолчанию [!INCLUDE[d365fin](includes/d365fin_md.md)] предоставляет ряд объектов как веб-службы для лучшей интеграции с другими службами Microsoft.</span><span class="sxs-lookup"><span data-stu-id="95ea7-105">By default, [!INCLUDE[d365fin](includes/d365fin_md.md)] exposes a number of objects as web services for better integration with other Microsoft services.</span></span> <span data-ttu-id="95ea7-106">Вы можете добавить другие веб-службы, если этого требует ваш бизнес.</span><span class="sxs-lookup"><span data-stu-id="95ea7-106">You can add other web services as your business requires.</span></span>  

<span data-ttu-id="95ea7-107">Настройте веб-службу в [!INCLUDE[d365fin](includes/d365fin_md.md)], а затем опубликуйте веб-службу, чтобы она была доступна пользователям, прошедшим аутентификацию.</span><span class="sxs-lookup"><span data-stu-id="95ea7-107">Set up a web service in [!INCLUDE[d365fin](includes/d365fin_md.md)], and then publish the web service so that it is available to authenticated users.</span></span> <span data-ttu-id="95ea7-108">Все авторизованные пользователи могут получить доступ к метаданным для веб-служб, но доступ к фактическим данным имеется только у пользователей с достаточными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="95ea7-108">All authorized users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span></span>  

## <a name="creating-and-publishing-a-web-service"></a><span data-ttu-id="95ea7-109">Создание и публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="95ea7-109">Creating and Publishing a Web Service</span></span>

<span data-ttu-id="95ea7-110">В следующих шагах объясняется порядок создания и публикации веб-службы.</span><span class="sxs-lookup"><span data-stu-id="95ea7-110">The following steps explain how to create and publish a web service.</span></span>  

### <a name="to-create-and-publish-a-web-service"></a><span data-ttu-id="95ea7-111">Создание и публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="95ea7-111">To create and publish a web service</span></span>  

1. <span data-ttu-id="95ea7-112">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Веб-службы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="95ea7-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Web Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="95ea7-113">На странице **Веб-службы** выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="95ea7-113">On the **Web Services** page, choose **New**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    > <span data-ttu-id="95ea7-114">**Модуль Codeunit** и **Страница** — допустимые типы для веб-служб SOAP.</span><span class="sxs-lookup"><span data-stu-id="95ea7-114">**Codeunit** and **Page** are valid types for SOAP web services.</span></span> <span data-ttu-id="95ea7-115">**Страница** и **Запрос** — допустимые типы веб-служб OData.</span><span class="sxs-lookup"><span data-stu-id="95ea7-115">**Page** and **Query** are valid types for OData web services.</span></span> <span data-ttu-id="95ea7-116">Начиная с версии 16.3 **Codeunit** — это также допустимый тип для веб-служб OData v4, но тогда в пользовательском интерфейсе URL-адрес не отображается.</span><span class="sxs-lookup"><span data-stu-id="95ea7-116">Starting with version 16.3, **Codeunit** is also a valid type for OData v4 web services, but then no URL is shown in the user interface.</span></span> <span data-ttu-id="95ea7-117">Кроме того, если база данных содержит несколько организаций, можно выбрать Идентификатор объекта, относящийся к одной из организаций.</span><span class="sxs-lookup"><span data-stu-id="95ea7-117">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span></span>  
    > <span data-ttu-id="95ea7-118">Наконец, имя службы видимо для клиентов вашей веб-службы и является основой для идентификации и различения веб-служб, поэтому следует применять осмысленное имя.</span><span class="sxs-lookup"><span data-stu-id="95ea7-118">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span></span>

3. <span data-ttu-id="95ea7-119">Установите флажок в столбце **Опубликовано**.</span><span class="sxs-lookup"><span data-stu-id="95ea7-119">Select the check box in the **Published** column.</span></span>  

<span data-ttu-id="95ea7-120">Когда вы публикуете веб-службу, поля **URL-адрес OData** и **URL-адрес SOAP** содержат новые URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="95ea7-120">When you publish the web service, the **OData URL** and **SOAP URL** fields show the new URLs.</span></span> <span data-ttu-id="95ea7-121">Однако для кодовых модулей, которые представлены как несвязанные действия OData v4, поля URL-адреса не отображаются.</span><span class="sxs-lookup"><span data-stu-id="95ea7-121">However, for codeunits that are exposed as OData v4 unbound actions, the URL fields are not shown.</span></span>  

<span data-ttu-id="95ea7-122">Веб-службу можно немедленно проверить, выбрав ссылки в полях **URL-адрес OData** и **URL SOAP**.</span><span class="sxs-lookup"><span data-stu-id="95ea7-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span></span> <span data-ttu-id="95ea7-123">При необходимости скопируйте значение поля и сохраните его для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="95ea7-123">Optionally, copy the value of the field and save it for later use.</span></span> <span data-ttu-id="95ea7-124">Чтобы протестировать модули кода, которые представлены как несвязанные действия OData v4, следуйте инструкциям в разделе [Проверка доступности веб-службы](/dynamics365/business-central/dev-itpro/developer/devenv-creating-and-interacting-with-odatav4-unbound-action#verifying-web-service-availability) в материалах разработчика.</span><span class="sxs-lookup"><span data-stu-id="95ea7-124">To test codeunits that are exposed as OData v4 unbound actions, follow the instructions in the [Verifying web service availability](/dynamics365/business-central/dev-itpro/developer/devenv-creating-and-interacting-with-odatav4-unbound-action#verifying-web-service-availability) section in the developer content.</span></span>

> [!NOTE]
> <span data-ttu-id="95ea7-125">Если объекты, которые вы предоставляете в качестве веб-служб, не должны быть доступны из [!INCLUDE[prodshort](includes/prodshort.md)] Online, вы должны пометить предоставляемые в коде методы как `[Scope('OnPrem')]`.</span><span class="sxs-lookup"><span data-stu-id="95ea7-125">If the objects that you expose as web services must not be accessible from [!INCLUDE[prodshort](includes/prodshort.md)] online, you must mark the methods exposed in the code as `[Scope('OnPrem')]`.</span></span> <span data-ttu-id="95ea7-126">Дополнительные сведения см. в разделе [Атрибут Scope](/dynamics365/business-central/dev-itpro/developer/methods/devenv-scope-attribute).</span><span class="sxs-lookup"><span data-stu-id="95ea7-126">For more information, see [Scope Attribute](/dynamics365/business-central/dev-itpro/developer/methods/devenv-scope-attribute).</span></span>

<span data-ttu-id="95ea7-127">После публикации веб-службы она становится доступна для внешних сторон.</span><span class="sxs-lookup"><span data-stu-id="95ea7-127">After you publish a web service, it is available to external parties.</span></span> <span data-ttu-id="95ea7-128">Можно проверить доступность веб-службы с помощью браузера или можно выбрать ссылку в полях **URL-адрес OData** и **URL SOAP** на странице **Веб-службы**.</span><span class="sxs-lookup"><span data-stu-id="95ea7-128">You can verify the availability of that web service by using a browser, or choose the link in the **OData URL** and **SOAP URL** fields on the **Web Services** page.</span></span> <span data-ttu-id="95ea7-129">В следующей процедуре показано, как можно проверить наличие веб-службы для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="95ea7-129">The following procedure illustrates how you can verify the availability of the web service for later use.</span></span>  

### <a name="to-verify-the-availability-of-a-web-service"></a><span data-ttu-id="95ea7-130">Проверка наличия веб-службы</span><span class="sxs-lookup"><span data-stu-id="95ea7-130">To verify the availability of a web service</span></span>  

1. <span data-ttu-id="95ea7-131">В браузере введите соответствующий URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="95ea7-131">In your browser, enter the relevant URL.</span></span> <span data-ttu-id="95ea7-132">В таблице ниже показаны типы URL-адресов, которые можно ввести для различных типов веб-служб.</span><span class="sxs-lookup"><span data-stu-id="95ea7-132">The following table illustrates the types of URLs that you can enter for different web service types.</span></span>  

    > [!div class="mx-tdBreakAll"]
    > |<span data-ttu-id="95ea7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="95ea7-133">Type</span></span>|<span data-ttu-id="95ea7-134">Синтаксис</span><span class="sxs-lookup"><span data-stu-id="95ea7-134">Syntax</span></span>|<span data-ttu-id="95ea7-135">Пример</span><span class="sxs-lookup"><span data-stu-id="95ea7-135">Example</span></span>|
    > |----------------|------|-------|
    > |<span data-ttu-id="95ea7-136">SOAP</span><span class="sxs-lookup"><span data-stu-id="95ea7-136">SOAP</span></span>|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/WS/*CompanyName*/*entity*/` |`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/WS/CRONUS%20USA%2C%20Inc./Page/InvoiceDocument`|
    > |<span data-ttu-id="95ea7-137">OData V4</span><span class="sxs-lookup"><span data-stu-id="95ea7-137">OData V4</span></span>|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/ODataV4/Company('*CompanyName*')/*entity*`|`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/ODataV4/Company('CRONUS%20USA%2C%20Inc.')/InvoiceDocument`<br/>    <span data-ttu-id="95ea7-138">Название организации учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="95ea7-138">The company name is case-sensitive.</span></span>|

2. <span data-ttu-id="95ea7-139">Просмотрите сведения, которые отражаются в браузере.</span><span class="sxs-lookup"><span data-stu-id="95ea7-139">Review the information that is displayed in the browser.</span></span> <span data-ttu-id="95ea7-140">Удостоверьтесь, что созданное вами имя веб-службы отображается правильно.</span><span class="sxs-lookup"><span data-stu-id="95ea7-140">Verify that you can see the name of the web service that you have created.</span></span>  

<span data-ttu-id="95ea7-141">При доступе к веб-службе и необходимости внести данные в [!INCLUDE[d365fin](includes/d365fin_md.md)] следует указать название организации.</span><span class="sxs-lookup"><span data-stu-id="95ea7-141">When you access a web service, and you want to write data back to [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the company name.</span></span> <span data-ttu-id="95ea7-142">Можно указать организацию при URI, как показано в примерах, или же указать организацию при настройке параметров запроса.</span><span class="sxs-lookup"><span data-stu-id="95ea7-142">You can specify the company as part of the URI as shown in the examples; alternatively, specify the company as part of the query parameters.</span></span> <span data-ttu-id="95ea7-143">Например, следующие URI указывают на одну и ту же веб-службу OData, и оба URI действительны.</span><span class="sxs-lookup"><span data-stu-id="95ea7-143">For example, the following URIs point to the same OData web service and are both valid URIs.</span></span>  

```
https://api.businesscentral.dynamics.com/v1.0/OData/Company('CRONUS International Ltd.')/Customer  
```

```
https://api.businesscentral.dynamics.com/v1.0/OData/Customer?company='CRONUS International Ltd.'  
```

## <a name="see-also"></a><span data-ttu-id="95ea7-144">См. также</span><span class="sxs-lookup"><span data-stu-id="95ea7-144">See Also</span></span>

[<span data-ttu-id="95ea7-145">Администрация</span><span class="sxs-lookup"><span data-stu-id="95ea7-145">Administration</span></span>](admin-setup-and-administration.md)  
[<span data-ttu-id="95ea7-146">Веб-службы Business Central для разработчиков</span><span class="sxs-lookup"><span data-stu-id="95ea7-146">Business Central Web Services for developers</span></span>](/dynamics365/business-central/dev-itpro/webservices/web-services)  
[<span data-ttu-id="95ea7-147">Лимиты запросов OData</span><span class="sxs-lookup"><span data-stu-id="95ea7-147">OData request limits</span></span>](/dynamics365/business-central/dev-itpro/administration/operational-limits-online#ODataServices)  
