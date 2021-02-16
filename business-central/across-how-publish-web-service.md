---
title: Предоставление объектов как веб-службы
description: Публикуйте объекты как веб-службы, чтобы сделать их доступными сразу для вашего решения Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/08/2020
ms.author: edupont
ms.openlocfilehash: 2220b5227cfe0e99a53071829096a67b6aeb0521
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4754921"
---
# <a name="publish-a-web-service"></a><span data-ttu-id="bff86-103">Публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="bff86-103">Publish a Web Service</span></span>

<span data-ttu-id="bff86-104">Веб-службы представляют облегченный способ сделать доступными функции приложений для различных внешних систем и пользователей.</span><span class="sxs-lookup"><span data-stu-id="bff86-104">Web services are a lightweight way to make application functionality available to different kinds of external systems and users.</span></span> <span data-ttu-id="bff86-105">По умолчанию [!INCLUDE[prod_short](includes/prod_short.md)] предоставляет ряд объектов как веб-службы для лучшей интеграции с другими службами Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bff86-105">By default, [!INCLUDE[prod_short](includes/prod_short.md)] exposes a number of objects as web services for better integration with other Microsoft services.</span></span> <span data-ttu-id="bff86-106">Вы можете добавить другие веб-службы, если этого требует ваш бизнес.</span><span class="sxs-lookup"><span data-stu-id="bff86-106">You can add other web services as your business requires.</span></span>  

<span data-ttu-id="bff86-107">Настройте веб-службу в [!INCLUDE[prod_short](includes/prod_short.md)], а затем опубликуйте веб-службу, чтобы она была доступна пользователям, прошедшим аутентификацию.</span><span class="sxs-lookup"><span data-stu-id="bff86-107">Set up a web service in [!INCLUDE[prod_short](includes/prod_short.md)], and then publish the web service so that it is available to authenticated users.</span></span> <span data-ttu-id="bff86-108">Все авторизованные пользователи могут получить доступ к метаданным для веб-служб, но доступ к фактическим данным имеется только у пользователей с достаточными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="bff86-108">All authorized users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span></span>  

## <a name="creating-and-publishing-a-web-service"></a><span data-ttu-id="bff86-109">Создание и публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="bff86-109">Creating and Publishing a Web Service</span></span>

<span data-ttu-id="bff86-110">В следующих шагах объясняется порядок создания и публикации веб-службы.</span><span class="sxs-lookup"><span data-stu-id="bff86-110">The following steps explain how to create and publish a web service.</span></span>  

### <a name="to-create-and-publish-a-web-service"></a><span data-ttu-id="bff86-111">Создание и публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="bff86-111">To create and publish a web service</span></span>  

1. <span data-ttu-id="bff86-112">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Веб-службы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="bff86-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Web Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="bff86-113">На странице **Веб-службы** выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="bff86-113">On the **Web Services** page, choose **New**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    > <span data-ttu-id="bff86-114">**Модуль Codeunit** и **Страница** — допустимые типы для веб-служб SOAP.</span><span class="sxs-lookup"><span data-stu-id="bff86-114">**Codeunit** and **Page** are valid types for SOAP web services.</span></span> <span data-ttu-id="bff86-115">**Страница** и **Запрос** — допустимые типы веб-служб OData.</span><span class="sxs-lookup"><span data-stu-id="bff86-115">**Page** and **Query** are valid types for OData web services.</span></span> <span data-ttu-id="bff86-116">Начиная с версии 16.3 **Codeunit** — это также допустимый тип для веб-служб OData v4, но тогда в пользовательском интерфейсе URL-адрес не отображается.</span><span class="sxs-lookup"><span data-stu-id="bff86-116">Starting with version 16.3, **Codeunit** is also a valid type for OData v4 web services, but then no URL is shown in the user interface.</span></span> <span data-ttu-id="bff86-117">Кроме того, если база данных содержит несколько организаций, можно выбрать Идентификатор объекта, относящийся к одной из организаций.</span><span class="sxs-lookup"><span data-stu-id="bff86-117">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span></span>  
    > <span data-ttu-id="bff86-118">Наконец, имя службы видимо для клиентов вашей веб-службы и является основой для идентификации и различения веб-служб, поэтому следует применять осмысленное имя.</span><span class="sxs-lookup"><span data-stu-id="bff86-118">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span></span>

3. <span data-ttu-id="bff86-119">Установите флажок в столбце **Опубликовано**.</span><span class="sxs-lookup"><span data-stu-id="bff86-119">Select the check box in the **Published** column.</span></span>  

<span data-ttu-id="bff86-120">Когда вы публикуете веб-службу, поля **URL-адрес OData** и **URL-адрес SOAP** содержат новые URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="bff86-120">When you publish the web service, the **OData URL** and **SOAP URL** fields show the new URLs.</span></span> <span data-ttu-id="bff86-121">Однако для кодовых модулей, которые представлены как несвязанные действия OData v4, поля URL-адреса не отображаются.</span><span class="sxs-lookup"><span data-stu-id="bff86-121">However, for codeunits that are exposed as OData v4 unbound actions, the URL fields are not shown.</span></span>  

<span data-ttu-id="bff86-122">Веб-службу можно немедленно проверить, выбрав ссылки в полях **URL-адрес OData** и **URL SOAP**.</span><span class="sxs-lookup"><span data-stu-id="bff86-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span></span> <span data-ttu-id="bff86-123">При необходимости скопируйте значение поля и сохраните его для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="bff86-123">Optionally, copy the value of the field and save it for later use.</span></span> <span data-ttu-id="bff86-124">Чтобы протестировать модули кода, которые представлены как несвязанные действия OData v4, следуйте инструкциям в разделе [Проверка доступности веб-службы](/dynamics365/business-central/dev-itpro/developer/devenv-creating-and-interacting-with-odatav4-unbound-action#verifying-web-service-availability) в материалах разработчика.</span><span class="sxs-lookup"><span data-stu-id="bff86-124">To test codeunits that are exposed as OData v4 unbound actions, follow the instructions in the [Verifying web service availability](/dynamics365/business-central/dev-itpro/developer/devenv-creating-and-interacting-with-odatav4-unbound-action#verifying-web-service-availability) section in the developer content.</span></span>

> [!NOTE]
> <span data-ttu-id="bff86-125">Если объекты, которые вы предоставляете в качестве веб-служб, не должны быть доступны из [!INCLUDE[prod_short](includes/prod_short.md)] Online, вы должны пометить предоставляемые в коде методы как `[Scope('OnPrem')]`.</span><span class="sxs-lookup"><span data-stu-id="bff86-125">If the objects that you expose as web services must not be accessible from [!INCLUDE[prod_short](includes/prod_short.md)] online, you must mark the methods exposed in the code as `[Scope('OnPrem')]`.</span></span> <span data-ttu-id="bff86-126">Дополнительные сведения см. в разделе [Атрибут Scope](/dynamics365/business-central/dev-itpro/developer/methods/devenv-scope-attribute).</span><span class="sxs-lookup"><span data-stu-id="bff86-126">For more information, see [Scope Attribute](/dynamics365/business-central/dev-itpro/developer/methods/devenv-scope-attribute).</span></span>

<span data-ttu-id="bff86-127">После публикации веб-службы она становится доступна для внешних сторон.</span><span class="sxs-lookup"><span data-stu-id="bff86-127">After you publish a web service, it is available to external parties.</span></span> <span data-ttu-id="bff86-128">Можно проверить доступность веб-службы с помощью браузера или можно выбрать ссылку в полях **URL-адрес OData** и **URL SOAP** на странице **Веб-службы**.</span><span class="sxs-lookup"><span data-stu-id="bff86-128">You can verify the availability of that web service by using a browser, or choose the link in the **OData URL** and **SOAP URL** fields on the **Web Services** page.</span></span> <span data-ttu-id="bff86-129">В следующей процедуре показано, как можно проверить наличие веб-службы для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="bff86-129">The following procedure illustrates how you can verify the availability of the web service for later use.</span></span>  

### <a name="to-verify-the-availability-of-a-web-service"></a><span data-ttu-id="bff86-130">Проверка наличия веб-службы</span><span class="sxs-lookup"><span data-stu-id="bff86-130">To verify the availability of a web service</span></span>  

1. <span data-ttu-id="bff86-131">В браузере введите соответствующий URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="bff86-131">In your browser, enter the relevant URL.</span></span> <span data-ttu-id="bff86-132">В таблице ниже показаны типы URL-адресов, которые можно ввести для различных типов веб-служб.</span><span class="sxs-lookup"><span data-stu-id="bff86-132">The following table illustrates the types of URLs that you can enter for different web service types.</span></span>  

    > [!div class="mx-tdBreakAll"]
    > |<span data-ttu-id="bff86-133">Тип</span><span class="sxs-lookup"><span data-stu-id="bff86-133">Type</span></span>|<span data-ttu-id="bff86-134">Синтаксис</span><span class="sxs-lookup"><span data-stu-id="bff86-134">Syntax</span></span>|<span data-ttu-id="bff86-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bff86-135">Example</span></span>|
    > |----------------|------|-------|
    > |<span data-ttu-id="bff86-136">SOAP</span><span class="sxs-lookup"><span data-stu-id="bff86-136">SOAP</span></span>|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/WS/*CompanyName*/*entity*/` |`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/WS/CRONUS%20USA%2C%20Inc./Page/InvoiceDocument`|
    > |<span data-ttu-id="bff86-137">OData V4</span><span class="sxs-lookup"><span data-stu-id="bff86-137">OData V4</span></span>|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/ODataV4/Company('*CompanyName*')/*entity*`|`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/ODataV4/Company('CRONUS%20USA%2C%20Inc.')/InvoiceDocument`<br/>    <span data-ttu-id="bff86-138">Название организации учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="bff86-138">The company name is case-sensitive.</span></span>|

2. <span data-ttu-id="bff86-139">Просмотрите сведения, которые отражаются в браузере.</span><span class="sxs-lookup"><span data-stu-id="bff86-139">Review the information that is displayed in the browser.</span></span> <span data-ttu-id="bff86-140">Удостоверьтесь, что созданное вами имя веб-службы отображается правильно.</span><span class="sxs-lookup"><span data-stu-id="bff86-140">Verify that you can see the name of the web service that you have created.</span></span>  

<span data-ttu-id="bff86-141">При доступе к веб-службе и необходимости внести данные в [!INCLUDE[prod_short](includes/prod_short.md)] следует указать название организации.</span><span class="sxs-lookup"><span data-stu-id="bff86-141">When you access a web service, and you want to write data back to [!INCLUDE[prod_short](includes/prod_short.md)], you must specify the company name.</span></span> <span data-ttu-id="bff86-142">Можно указать организацию при URI, как показано в примерах, или же указать организацию при настройке параметров запроса.</span><span class="sxs-lookup"><span data-stu-id="bff86-142">You can specify the company as part of the URI as shown in the examples; alternatively, specify the company as part of the query parameters.</span></span> <span data-ttu-id="bff86-143">Например, следующие URI указывают на одну и ту же веб-службу OData, и оба URI действительны.</span><span class="sxs-lookup"><span data-stu-id="bff86-143">For example, the following URIs point to the same OData web service and are both valid URIs.</span></span>  

```
https://api.businesscentral.dynamics.com/v1.0/OData/Company('CRONUS International Ltd.')/Customer  
```

```
https://api.businesscentral.dynamics.com/v1.0/OData/Customer?company='CRONUS International Ltd.'  
```

## <a name="see-also"></a><span data-ttu-id="bff86-144">См. также</span><span class="sxs-lookup"><span data-stu-id="bff86-144">See Also</span></span>

[<span data-ttu-id="bff86-145">Администрация</span><span class="sxs-lookup"><span data-stu-id="bff86-145">Administration</span></span>](admin-setup-and-administration.md)  
[<span data-ttu-id="bff86-146">Веб-службы Business Central для разработчиков</span><span class="sxs-lookup"><span data-stu-id="bff86-146">Business Central Web Services for developers</span></span>](/dynamics365/business-central/dev-itpro/webservices/web-services)  
[<span data-ttu-id="bff86-147">Лимиты запросов OData</span><span class="sxs-lookup"><span data-stu-id="bff86-147">OData request limits</span></span>](/dynamics365/business-central/dev-itpro/administration/operational-limits-online#ODataServices)  
