---
title: Предоставление объектов как веб-службы | Документация Майкрософт
description: Публикуйте объекты как веб-службы, чтобы сделать их доступными сразу для вашего решения Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 05/19/2020
ms.author: edupont
ms.openlocfilehash: 230f3a7fc11e19813d77da2ff15388433642c744
ms.sourcegitcommit: aeaa0dc64e54432a70c4b0e1faf325cd17d01389
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2020
ms.locfileid: "3697651"
---
# <a name="publish-a-web-service"></a><span data-ttu-id="ea094-103">Публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="ea094-103">Publish a Web Service</span></span>

<span data-ttu-id="ea094-104">Веб-службы представляют облегченный способ сделать доступными функции приложений для различных внешних систем и пользователей.</span><span class="sxs-lookup"><span data-stu-id="ea094-104">Web services are a lightweight way to make application functionality available to a variety of external systems and users.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="ea094-105">содержит ряд объект, которые по умолчанию предоставляются как веб-службы в связи с интеграцией с другими службами Microsoft, но можно также добавить другие веб-службы.</span><span class="sxs-lookup"><span data-stu-id="ea094-105">includes an number of objects that are exposed as web services by default due to integration with other Microsoft services, but you can also add other web services.</span></span>  

<span data-ttu-id="ea094-106">Настройка веб-службы производится в клиенте [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="ea094-106">You set up a web service in the [!INCLUDE[d365fin](includes/d365fin_md.md)] client.</span></span> <span data-ttu-id="ea094-107">Затем следует опубликовать веб-службу так, чтобы она была доступна для служебных запросов по сети.</span><span class="sxs-lookup"><span data-stu-id="ea094-107">You must then publish the web service so that it is available to service requests over the network.</span></span> <span data-ttu-id="ea094-108">Пользователи могут обнаружить веб-службы, указав в браузере расположение сервера и запросив список существующих служб.</span><span class="sxs-lookup"><span data-stu-id="ea094-108">Users can discover web services by pointing a browser at the server location and requesting a list of available services.</span></span> <span data-ttu-id="ea094-109">При публикации веб-службы она немедленно становится доступной в сети для пользователей, прошедших проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="ea094-109">When you publish a web service, it is immediately available over the network for authenticated users.</span></span> <span data-ttu-id="ea094-110">Все авторизованные пользователи могут получить доступ к метаданным для веб-служб, но доступ к фактическим данным имеется только у пользователей с достаточными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="ea094-110">All authorized users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span></span>

## <a name="creating-and-publishing-a-web-service"></a><span data-ttu-id="ea094-111">Создание и публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="ea094-111">Creating and Publishing a Web Service</span></span>

<span data-ttu-id="ea094-112">В следующих шагах объясняется порядок создания и публикации веб-службы.</span><span class="sxs-lookup"><span data-stu-id="ea094-112">The following steps explain how to create and publish a web service.</span></span>  

<!--
    You can also create a new web service URL in [!INCLUDE [prodshort](includes/prodshort.md)] instead. Choose one of the following methods:

      - Use the **Create Data Set** action on the **Web Services** page
      - Use the **Set Up Reporting** Assisted Setup guide
      - Choose the **Edit in Excel** action in any lists
    -->

### <a name="to-create-and-publish-a-web-service"></a><span data-ttu-id="ea094-113">Создание и публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="ea094-113">To create and publish a web service</span></span>  

1. <span data-ttu-id="ea094-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Веб-службы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="ea094-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Web Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ea094-115">На странице **Веб-службы** выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="ea094-115">On the **Web Services** page, choose **New**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    > <span data-ttu-id="ea094-116">**Модуль Codeunit** и **Страница** — допустимые типы для веб-служб SOAP.</span><span class="sxs-lookup"><span data-stu-id="ea094-116">**Codeunit** and **Page** are valid types for SOAP web services.</span></span> <span data-ttu-id="ea094-117">**Страница** и **Запрос** — допустимые типы веб-служб OData.</span><span class="sxs-lookup"><span data-stu-id="ea094-117">**Page** and **Query** are valid types for OData web services.</span></span>  
    > <span data-ttu-id="ea094-118">Кроме того, если база данных содержит несколько организаций, можно выбрать Идентификатор объекта, относящийся к одной из организаций.</span><span class="sxs-lookup"><span data-stu-id="ea094-118">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span></span>  
    > <span data-ttu-id="ea094-119">Наконец, имя службы видимо для клиентов вашей веб-службы и является основой для идентификации и различения веб-служб, поэтому следует применять осмысленное имя.</span><span class="sxs-lookup"><span data-stu-id="ea094-119">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span></span>

3. <span data-ttu-id="ea094-120">Установите флажок в столбце **Опубликовано**.</span><span class="sxs-lookup"><span data-stu-id="ea094-120">Select the check box in the **Published** column.</span></span>  

<span data-ttu-id="ea094-121">При публикации веб-службы в полях **URL-адрес OData** и **URL SOAP** можно увидеть URL-адреса, сгенерированные для веб-службы.</span><span class="sxs-lookup"><span data-stu-id="ea094-121">When you publish the web service, in the **OData URL** and **SOAP URL** fields, you can see the URLs that are generated for the web service.</span></span> <span data-ttu-id="ea094-122">Веб-службу можно немедленно проверить, выбрав ссылки в полях **URL-адрес OData** и **URL SOAP**.</span><span class="sxs-lookup"><span data-stu-id="ea094-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span></span> <span data-ttu-id="ea094-123">При необходимости можно скопировать значение поля и сохранить его для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="ea094-123">Optionally, you can copy the value of the field and save it for later use.</span></span>  

> [!NOTE]
> <span data-ttu-id="ea094-124">Если объекты, которые вы предоставляете в качестве веб-служб, не должны быть доступны из [!INCLUDE[prodshort](includes/prodshort.md)] Online, вы должны пометить предоставляемые в коде методы как `[Scope('OnPrem')]`.</span><span class="sxs-lookup"><span data-stu-id="ea094-124">If the objects that you expose as web services must not be accessible from [!INCLUDE[prodshort](includes/prodshort.md)] online, you must mark the methods exposed in the code as `[Scope('OnPrem')]`.</span></span> <span data-ttu-id="ea094-125">Дополнительные сведения см. в разделе [Атрибут Scope](/dynamics365/business-central/dev-itpro/developer/methods/devenv-scope-attribute).</span><span class="sxs-lookup"><span data-stu-id="ea094-125">For more information, see [Scope Attribute](/dynamics365/business-central/dev-itpro/developer/methods/devenv-scope-attribute).</span></span>

<span data-ttu-id="ea094-126">После публикации веб-службы она становится доступна для внешних сторон.</span><span class="sxs-lookup"><span data-stu-id="ea094-126">After you publish a web service, it is available to external parties.</span></span> <span data-ttu-id="ea094-127">Можно проверить доступность веб-службы с помощью браузера или выбрать ссылку в полях **URL-адрес OData** и **URL SOAP** на странице **Веб-службы**.</span><span class="sxs-lookup"><span data-stu-id="ea094-127">You can verify the availability of that web service by using a browser, or you can choose the link in the **OData URL** and **SOAP URL** fields on the **Web Services** page.</span></span> <span data-ttu-id="ea094-128">В следующей процедуре показано, как можно проверить наличие веб-службы для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="ea094-128">The following procedure illustrates how you can verify the availability of the web service for later use.</span></span>  

### <a name="to-verify-the-availability-of-a-web-service"></a><span data-ttu-id="ea094-129">Проверка наличия веб-службы</span><span class="sxs-lookup"><span data-stu-id="ea094-129">To verify the availability of a web service</span></span>  

1. <span data-ttu-id="ea094-130">В браузере введите соответствующий URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="ea094-130">In your browser, enter the relevant URL.</span></span> <span data-ttu-id="ea094-131">В таблице ниже показаны типы URL-адресов, которые можно ввести для различных типов веб-служб.</span><span class="sxs-lookup"><span data-stu-id="ea094-131">The following table illustrates the types of URLs that you can enter for different web service types.</span></span>  

    > [!div class="mx-tdBreakAll"]
    > |<span data-ttu-id="ea094-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ea094-132">Type</span></span>|<span data-ttu-id="ea094-133">Синтаксис</span><span class="sxs-lookup"><span data-stu-id="ea094-133">Syntax</span></span>|<span data-ttu-id="ea094-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ea094-134">Example</span></span>|
    > |----------------|------|-------|
    > |<span data-ttu-id="ea094-135">SOAP</span><span class="sxs-lookup"><span data-stu-id="ea094-135">SOAP</span></span>|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/WS/*CompanyName*/*entity*/` |`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/WS/CRONUS%20USA%2C%20Inc./Page/InvoiceDocument`|
    > |<span data-ttu-id="ea094-136">OData V4</span><span class="sxs-lookup"><span data-stu-id="ea094-136">OData V4</span></span>|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/ODataV4/Company('*CompanyName*')/*entity*`|`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/ODataV4/Company('CRONUS%20USA%2C%20Inc.')/InvoiceDocument`<br/>    <span data-ttu-id="ea094-137">Название организации учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="ea094-137">The company name is case-sensitive.</span></span>|

2. <span data-ttu-id="ea094-138">Просмотрите сведения, которые отражаются в браузере.</span><span class="sxs-lookup"><span data-stu-id="ea094-138">Review the information that is displayed in the browser.</span></span> <span data-ttu-id="ea094-139">Удостоверьтесь, что созданное вами имя веб-службы отображается правильно.</span><span class="sxs-lookup"><span data-stu-id="ea094-139">Verify that you can see the name of the web service that you have created.</span></span>  

<span data-ttu-id="ea094-140">При доступе к веб-службе и необходимости внести данные в [!INCLUDE[d365fin](includes/d365fin_md.md)] следует указать название организации.</span><span class="sxs-lookup"><span data-stu-id="ea094-140">When you access a web service, and you want to write data back to [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the company name.</span></span> <span data-ttu-id="ea094-141">Можно указать организацию при URI, как показано в примерах, или указать организацию при настройке параметров запроса.</span><span class="sxs-lookup"><span data-stu-id="ea094-141">You can specify the company as part of the URI as shown in the examples, or you can specify the company as part of the query parameters.</span></span> <span data-ttu-id="ea094-142">Например, следующие URI указывают на одну и ту же веб-службу OData, и оба URI действительны.</span><span class="sxs-lookup"><span data-stu-id="ea094-142">For example, the following URIs point to the same OData web service and are both valid URIs.</span></span>  

```
https://api.businesscentral.dynamics.com/v1.0/OData/Company('CRONUS International Ltd.')/Customer  
```

```
https://api.businesscentral.dynamics.com/v1.0/OData/Customer?company='CRONUS International Ltd.'  
```

## <a name="see-also"></a><span data-ttu-id="ea094-143">См. также</span><span class="sxs-lookup"><span data-stu-id="ea094-143">See Also</span></span>

[<span data-ttu-id="ea094-144">Администрация</span><span class="sxs-lookup"><span data-stu-id="ea094-144">Administration</span></span>](admin-setup-and-administration.md)  
[<span data-ttu-id="ea094-145">Веб-службы Business Central для разработчиков</span><span class="sxs-lookup"><span data-stu-id="ea094-145">Business Central Web Services for developers</span></span>](/dynamics365/business-central/dev-itpro/webservices/web-services)  
[<span data-ttu-id="ea094-146">Лимиты запросов OData</span><span class="sxs-lookup"><span data-stu-id="ea094-146">OData request limits</span></span>](/dynamics365/business-central/dev-itpro/administration/operational-limits-online#ODataServices)  
