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
# <a name="publish-a-web-service"></a>Публикация веб-службы

Веб-службы представляют облегченный способ сделать доступными функции приложений для различных внешних систем и пользователей. По умолчанию [!INCLUDE[d365fin](includes/d365fin_md.md)] предоставляет ряд объектов как веб-службы для лучшей интеграции с другими службами Microsoft. Вы можете добавить другие веб-службы, если этого требует ваш бизнес.  

Настройте веб-службу в [!INCLUDE[d365fin](includes/d365fin_md.md)], а затем опубликуйте веб-службу, чтобы она была доступна пользователям, прошедшим аутентификацию. Все авторизованные пользователи могут получить доступ к метаданным для веб-служб, но доступ к фактическим данным имеется только у пользователей с достаточными разрешениями.  

## <a name="creating-and-publishing-a-web-service"></a>Создание и публикация веб-службы

В следующих шагах объясняется порядок создания и публикации веб-службы.  

### <a name="to-create-and-publish-a-web-service"></a>Создание и публикация веб-службы  

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Веб-службы**, затем выберите соответствующую ссылку.  
2. На странице **Веб-службы** выберите **Создать**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    > **Модуль Codeunit** и **Страница** — допустимые типы для веб-служб SOAP. **Страница** и **Запрос** — допустимые типы веб-служб OData. Начиная с версии 16.3 **Codeunit** — это также допустимый тип для веб-служб OData v4, но тогда в пользовательском интерфейсе URL-адрес не отображается. Кроме того, если база данных содержит несколько организаций, можно выбрать Идентификатор объекта, относящийся к одной из организаций.  
    > Наконец, имя службы видимо для клиентов вашей веб-службы и является основой для идентификации и различения веб-служб, поэтому следует применять осмысленное имя.

3. Установите флажок в столбце **Опубликовано**.  

Когда вы публикуете веб-службу, поля **URL-адрес OData** и **URL-адрес SOAP** содержат новые URL-адреса. Однако для кодовых модулей, которые представлены как несвязанные действия OData v4, поля URL-адреса не отображаются.  

Веб-службу можно немедленно проверить, выбрав ссылки в полях **URL-адрес OData** и **URL SOAP**. При необходимости скопируйте значение поля и сохраните его для последующего использования. Чтобы протестировать модули кода, которые представлены как несвязанные действия OData v4, следуйте инструкциям в разделе [Проверка доступности веб-службы](/dynamics365/business-central/dev-itpro/developer/devenv-creating-and-interacting-with-odatav4-unbound-action#verifying-web-service-availability) в материалах разработчика.

> [!NOTE]
> Если объекты, которые вы предоставляете в качестве веб-служб, не должны быть доступны из [!INCLUDE[prodshort](includes/prodshort.md)] Online, вы должны пометить предоставляемые в коде методы как `[Scope('OnPrem')]`. Дополнительные сведения см. в разделе [Атрибут Scope](/dynamics365/business-central/dev-itpro/developer/methods/devenv-scope-attribute).

После публикации веб-службы она становится доступна для внешних сторон. Можно проверить доступность веб-службы с помощью браузера или можно выбрать ссылку в полях **URL-адрес OData** и **URL SOAP** на странице **Веб-службы**. В следующей процедуре показано, как можно проверить наличие веб-службы для последующего использования.  

### <a name="to-verify-the-availability-of-a-web-service"></a>Проверка наличия веб-службы  

1. В браузере введите соответствующий URL-адрес. В таблице ниже показаны типы URL-адресов, которые можно ввести для различных типов веб-служб.  

    > [!div class="mx-tdBreakAll"]
    > |Тип|Синтаксис|Пример|
    > |----------------|------|-------|
    > |SOAP|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/WS/*CompanyName*/*entity*/` |`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/WS/CRONUS%20USA%2C%20Inc./Page/InvoiceDocument`|
    > |OData V4|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/ODataV4/Company('*CompanyName*')/*entity*`|`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/ODataV4/Company('CRONUS%20USA%2C%20Inc.')/InvoiceDocument`<br/>    Название организации учитывает регистр.|

2. Просмотрите сведения, которые отражаются в браузере. Удостоверьтесь, что созданное вами имя веб-службы отображается правильно.  

При доступе к веб-службе и необходимости внести данные в [!INCLUDE[d365fin](includes/d365fin_md.md)] следует указать название организации. Можно указать организацию при URI, как показано в примерах, или же указать организацию при настройке параметров запроса. Например, следующие URI указывают на одну и ту же веб-службу OData, и оба URI действительны.  

```
https://api.businesscentral.dynamics.com/v1.0/OData/Company('CRONUS International Ltd.')/Customer  
```

```
https://api.businesscentral.dynamics.com/v1.0/OData/Customer?company='CRONUS International Ltd.'  
```

## <a name="see-also"></a>См. также

[Администрация](admin-setup-and-administration.md)  
[Веб-службы Business Central для разработчиков](/dynamics365/business-central/dev-itpro/webservices/web-services)  
[Лимиты запросов OData](/dynamics365/business-central/dev-itpro/administration/operational-limits-online#ODataServices)  
