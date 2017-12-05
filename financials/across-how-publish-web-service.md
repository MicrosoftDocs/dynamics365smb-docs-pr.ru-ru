---
title: "Предоставление объектов как веб-службы | Microsoft Docs"
description: "При публикации объектов [!INCLUDE[d365fin](includes/d365fin_md.md)] в виде веб-служб они сразу же становятся доступными по сети."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: af1aef6ec730083c49b17ae8c0c9e39c7f663244
ms.contentlocale: ru-ru
ms.lasthandoff: 11/10/2017

---
# <a name="how-to-publish-a-web-service"></a><span data-ttu-id="fcdfb-103">Практическое руководство. Публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="fcdfb-103">How to: Publish a Web Service</span></span>
<span data-ttu-id="fcdfb-104">Веб-службы представляют облегченный способ сделать доступными функции приложений для различных внешних систем и пользователей.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-104">Web services are a lightweight way to make application functionality available to a variety of external systems and users.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="fcdfb-105"> содержит ряд объект, которые по умолчанию предоставляются как веб-службы в связи с интеграцией с другими службами Microsoft, но можно также добавить другие веб-службы.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-105"> includes an number of objects that are exposed as web services by default due to integration with other Microsoft services, but you can also add other web services.</span></span>  

<span data-ttu-id="fcdfb-106">Можно настроить веб-службу в клиенте Windows или в веб-клиенте.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-106">You can set up a web service in the Windows client or in the Web client.</span></span> <span data-ttu-id="fcdfb-107">Затем следует опубликовать веб-службу так, чтобы она была доступна для служебных запросов по сети.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-107">You must then publish the web service so that it is available to service requests over the network.</span></span> <span data-ttu-id="fcdfb-108">Пользователи могут обнаружить веб-службы, указав в браузере расположение сервера и запросив список существующих служб.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-108">Users can discover web services by pointing a browser at the server location and requesting a list of available services.</span></span> <span data-ttu-id="fcdfb-109">При публикации веб-службы она немедленно становится доступной в сети для пользователей, прошедших проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-109">When you publish a web service, it is immediately available over the network for authenticated users.</span></span> <span data-ttu-id="fcdfb-110">Все авторизованные пользователи могут получить доступ к метаданным для веб-служб, но доступ к фактическим данным имеется только у пользователей с достаточными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-110">All authorized users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span></span>

## <a name="creating-and-publishing-a-web-service"></a><span data-ttu-id="fcdfb-111">Создание и публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="fcdfb-111">Creating and Publishing a Web Service</span></span>  
 <span data-ttu-id="fcdfb-112">В следующих шагах объясняется порядок создания и публикации веб-службы.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-112">The following steps explain how to create and publish a web service.</span></span>  

#### <a name="to-create-and-publish-a-web-service"></a><span data-ttu-id="fcdfb-113">Создание и публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="fcdfb-113">To create and publish a web service</span></span>  

1.  <span data-ttu-id="fcdfb-114">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Веб-службы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Web Services**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="fcdfb-115">На странице **Веб-службы** выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-115">In the **Web Services** page, choose **New**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    >  <span data-ttu-id="fcdfb-116">**Модуль Codeunit** и **Страница** — допустимые типы для веб-служб SOAP.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-116">**Codeunit** and **Page** are valid types for SOAP web services.</span></span> <span data-ttu-id="fcdfb-117">**Страница** и **Запрос** — допустимые типы веб-служб OData.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-117">**Page** and **Query** are valid types for OData web services.</span></span>  
    <span data-ttu-id="fcdfb-118">Кроме того, если база данных содержит несколько организаций, можно выбрать Идентификатор объекта, относящийся к одной из организаций.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-118">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span></span>  
    <span data-ttu-id="fcdfb-119">Наконец, имя службы видимо для клиентов вашей веб-службы и является основой для идентификации и различения веб-служб, поэтому следует применять осмысленное имя.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-119">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span></span>

3.  <span data-ttu-id="fcdfb-120">Установите флажок в столбце **Опубликовано**.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-120">Select the check box in the **Published** column.</span></span>  

     <span data-ttu-id="fcdfb-121">При публикации веб-службы в полях **URL-адрес OData** и **URL SOAP** можно увидеть URL-адреса, сгенерированные для веб-службы.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-121">When you publish the web service, in the **OData URL** and **SOAP URL** fields, you can see the URLs that are generated for the web service.</span></span> <span data-ttu-id="fcdfb-122">Веб-службу можно немедленно проверить, выбрав ссылки в полях **URL-адрес OData** и **URL SOAP**.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span></span> <span data-ttu-id="fcdfb-123">При необходимости можно скопировать значение поля и сохранить его для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-123">Optionally, you can copy the value of the field and save it for later use.</span></span>  

<span data-ttu-id="fcdfb-124">После публикации веб-службы она становится доступна для внешних сторон.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-124">After you publish a web service, it is available to external parties.</span></span> <span data-ttu-id="fcdfb-125">Можно проверить доступность веб-службы с помощью браузера или выбрать ссылку в полях **URL-адрес OData** и **URL SOAP** в окне **Веб-службы**.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-125">You can verify the availability of that web service by using a browser, or you can choose the link in the **OData URL** and **SOAP URL** fields in the **Web Services** window.</span></span> <span data-ttu-id="fcdfb-126">В следующей процедуре показано, как можно проверить наличие веб-службы для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-126">The following procedure illustrates how you can verify the availability of the web service for later use.</span></span>  

#### <a name="to-verify-the-availability-of-a-web-service"></a><span data-ttu-id="fcdfb-127">Проверка наличия веб-службы</span><span class="sxs-lookup"><span data-stu-id="fcdfb-127">To verify the availability of a web service</span></span>  

1.  <span data-ttu-id="fcdfb-128">В браузере введите соответствующий URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-128">In your browser, enter the relevant URL.</span></span> <span data-ttu-id="fcdfb-129">Следующая таблица описывает типы URL-адресов, которые можно ввести.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-129">The following table illustrates the types of URLs that you can enter.</span></span>  

    >    [!div class="mx-tdBreakAll"]
    >    |<span data-ttu-id="fcdfb-130">Тип веб-службы</span><span class="sxs-lookup"><span data-stu-id="fcdfb-130">Web service type</span></span>|<span data-ttu-id="fcdfb-131">Синтаксис</span><span class="sxs-lookup"><span data-stu-id="fcdfb-131">Syntax</span></span>|<span data-ttu-id="fcdfb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fcdfb-132">Example</span></span>|  
    >    |----------------|------|-------|
    >    |<span data-ttu-id="fcdfb-133">SOAP</span><span class="sxs-lookup"><span data-stu-id="fcdfb-133">SOAP</span></span> |<span data-ttu-id="fcdfb-134">https://*Server*:*SOAPWebServicePort*/*ServerInstance*/WS/*CompanyName*/salesDocuments/</span><span class="sxs-lookup"><span data-stu-id="fcdfb-134">https://*Server*:*SOAPWebServicePort*/*ServerInstance*/WS/*CompanyName*/salesDocuments/</span></span> |<span data-ttu-id="fcdfb-135">https://mycompany.financials.dynamics.com:7047/MS/WS/MyCompany/Page/salesDocuments?tenant=mycompany.financials.dynamics.com</span><span class="sxs-lookup"><span data-stu-id="fcdfb-135">https://mycompany.financials.dynamics.com:7047/MS/WS/MyCompany/Page/salesDocuments?tenant=mycompany.financials.dynamics.com</span></span> |  
    >    |<span data-ttu-id="fcdfb-136">OData</span><span class="sxs-lookup"><span data-stu-id="fcdfb-136">OData</span></span> |<span data-ttu-id="fcdfb-137">https://*Server*:*ODataWebServicePort*/*ServerInstance*/OData/Company('*CompanyName*')</span><span class="sxs-lookup"><span data-stu-id="fcdfb-137">https://*Server*:*ODataWebServicePort*/*ServerInstance*/OData/Company('*CompanyName*')</span></span>|<span data-ttu-id="fcdfb-138">[https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com](https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com)</span><span class="sxs-lookup"><span data-stu-id="fcdfb-138">[https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com](https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com)</span></span> <br />    <span data-ttu-id="fcdfb-139">Название организации учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-139">The company name is case-sensitive.</span></span>|

2.  <span data-ttu-id="fcdfb-140">Просмотрите сведения, которые отражаются в браузере.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-140">Review the information that is displayed in the browser.</span></span> <span data-ttu-id="fcdfb-141">Удостоверьтесь, что созданное вами имя веб-службы отображается правильно.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-141">Verify that you can see the name of the web service that you have created.</span></span>  

 <span data-ttu-id="fcdfb-142">При доступе к веб-службе и необходимости внести данные в [!INCLUDE[d365fin](includes/d365fin_md.md)] следует указать название организации.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-142">When you access a web service, and you want to write data back to [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the company name.</span></span> <span data-ttu-id="fcdfb-143">Можно указать организацию при URI, как показано в примерах, или указать организацию при настройке параметров запроса.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-143">You can specify the company as part of the URI as shown in the examples, or you can specify the company as part of the query parameters.</span></span> <span data-ttu-id="fcdfb-144">Например, следующие URI указывают на одну и ту же веб-службу OData, и оба URI действительны.</span><span class="sxs-lookup"><span data-stu-id="fcdfb-144">For example, the following URIs point to the same OData web service and are both valid URIs.</span></span>  

```  
https://localhost:7048/server/OData/Company('CRONUS International Ltd.')/Customer  
```  

```  
https://localhost:7048/server/OData/Customer?company='CRONUS International Ltd.'  
```  

## <a name="see-also"></a><span data-ttu-id="fcdfb-145">См. также</span><span class="sxs-lookup"><span data-stu-id="fcdfb-145">See Also</span></span>  
[<span data-ttu-id="fcdfb-146">Настройка и администрирование в Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="fcdfb-146">Setup and Administration in Dynamics 365 for Financials</span></span>](admin-setup-and-administration.md)  

