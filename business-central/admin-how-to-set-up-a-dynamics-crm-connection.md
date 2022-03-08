---
title: Подключение к Dynamics 365 for Sales | Документы Майкрософт
description: Можно выполнить интеграцию с Dynamics 365 for Sales.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/06/2019
ms.author: bholtorf
ms.openlocfilehash: dfcb664d352683566df233d6b9b95900f2d76a5a
ms.sourcegitcommit: f2e3b571eab6e01d9f5aa8ef47056b6bd313dcbd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/13/2019
ms.locfileid: "1629646"
---
# <a name="set-up-a-connection-to-dynamics-365-for-sales"></a>Настройка подключения к Dynamics 365 for Sales
Для интеграции с [!INCLUDE[crm_md](includes/crm_md.md)] необходимо настроить подключение между [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)].

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2085501]

## <a name="before-you-start"></a>Перед началом работы
Прежде чем начинать подключать приложения, полезно подготовить определенные сведения:  

* URL-адрес для вашего приложения [!INCLUDE[crm_md](includes/crm_md.md)]. Быстрый способ получить URL-адрес — открыть [!INCLUDE[crm_md](includes/crm_md.md)] и скопировать URL-адрес, затем вставить его в поле **URL-адрес Dynamics 365 for Sales** в [!INCLUDE[d365fin](includes/d365fin_md.md)]. [!INCLUDE[d365fin](includes/d365fin_md.md)] скорректирует форматирование для вас.  
* Имя пользователя и пароль учетной записи пользователя, которая используется для интеграции.  
* Имя пользователя и пароль учетной записи с разрешениями администратора.  

> [!Note]
> Эти шаги описывают процедуру для интернет-версии [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="set-up-test-and-enable-a-connection-to-crm_md"></a>Настройка, тестирование и активизация подключения к [!INCLUDE[crm_md](includes/crm_md.md)]  
Для всех типов проверки подлинности, отличных от проверки подлинности Office 365, вы настраиваете подключение к Dynamics 365 for Sales на странице **Настройка подключения к Microsoft Dynamics 365 for Sales**. Для проверки подлинности Office 365 также можно использовать мастер настройки **Настройка подключения к Dynamics 365 for Sales**, который поможет предоставить необходимую информацию.

### <a name="to-use-an-assisted-setup-guide"></a>Использование мастера настройки
Мастер настройки **Настройка подключения к Dynamics 365 for Sales** может помочь настроить подключение и указать, требуется ли включать расширенные функции, такие как связи между записями.

1. Выберите **Настройка и расширения**, затем выберите **Мастер настройки**.
2. Выберите пункт **Настройка подключения к Dynamics 365 for Sales**, чтобы запустить мастер настройки.
3. Заполните соответствующим образом поля.
4. При необходимости, имеются расширенные настройки, которые могут улучшить безопасность и включить дополнительные возможности [!INCLUDE[crm_md](includes/crm_md.md)], такие как обработка заказов на продажу и просмотр уровней запасов. Расширенные параметры рассматриваются в таблице ниже.  

|Поле|Описанием|
|-----|-----|
|**Импорт решения Dynamics 365 for Sales**|Разрешить это, чтобы установить и настроить решение интеграции в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [О решении интеграции Business Central](admin-prepare-dynamics-365-for-sales-for-integration.md#about-the-business-central-integration-solution).|
|**Публикация веб-службы наличия товаров**|Разрешите пользователям, которые используют [!INCLUDE[crm_md](includes/crm_md.md)], просматривать наличие товаров (продуктов) в запасах в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Для этого необходима учетная запись пользователя [!INCLUDE[d365fin](includes/d365fin_md.md)] с ключом доступа к веб-службам. Назначение ключа выполняется в два этапа. В учетной записи пользователя в [!INCLUDE[d365fin](includes/d365fin_md.md)] необходимо выбрать действие **Изменить ключ веб-службы**. В мастере настройки "Настройка подключения к Dynamics 365 for Sales" необходимо указать URL-адрес веб-службы Dynamics 365 Business Central OData и предоставить учетные данные пользователя [!INCLUDE[d365fin](includes/d365fin_md.md)] для получения доступа к сервису. Дополнительные сведения см. в разделе [Веб-службы OData](/dynamics365/business-central/dev-itpro/webservices/odata-web-services.md).|
|**URL-адрес веб-службы OData Dynamics 365 Business Central**|Если включена веб-служба наличия товаров, URL-адрес веб-службы OData предоставляется для вас.|
|**Имя пользователя веб-службы OData Dynamics 365 Business Central**|Имя пользователя учетной записи [!INCLUDE[d365fin](includes/d365fin_md.md)], которую [!INCLUDE[crm_md](includes/crm_md.md)] использует для извлечения сведений о наличии товаров в [!INCLUDE[d365fin](includes/d365fin_md.md)] через веб-службу OData.|
|**Ключ доступа веб-службы OData Dynamics 365 Business Central**|Ключ доступа учетной записи пользователя, которую [!INCLUDE[crm_md](includes/crm_md.md)] использует для получения сведений о наличии товаров из [!INCLUDE[d365fin](includes/d365fin_md.md)] через веб-службу OData. Ключ назначается пользователю, выбранному в поле **Имя пользователя веб-службы OData Dynamics 365 Business Central**. Чтобы получить ключ, выберите кнопку **Найти значение** рядом с именем пользователя, выберите пользователя, выберите **Управление**, затем выберите **Правка**. В карточке пользователя выберите **Действия**, **Проверка подлинности**, затем выберите **Изменить ключ веб-службы**.|
|**Включить интеграцию с заказом на продажу**|Когда люди создают заказы на продажу в [!INCLUDE[crm_md](includes/crm_md.md)], заказы копируются в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Для этого требуется, чтобы вы предоставили учетные данные для учетной записи пользователя-администратора в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Обработка данных в заказах на продажу](marketing-integrate-dynamicscrm.md#handling-sales-order-data).|
|**Включить подключение к Dynamics 365 for Sales**|Включите подключение к [!INCLUDE[crm_md](includes/crm_md.md)].|
|**Версия SDK Dynamics 365**|Это необходимо только в том случае, если выполняется интеграция с локальной версией [!INCLUDE[crm_md](includes/crm_md.md)]. Это комплект разработки программного обеспечения Dynamics 365 (также называемый Xrm), который используется для подключения [!INCLUDE[d365fin](includes/d365fin_md.md)] к [!INCLUDE[crm_md](includes/crm_md.md)]. Версия должна быть совместима с версией пакета SDK, которая используется [!INCLUDE[crm_md](includes/crm_md.md)], и равна или новее версии, используемой [!INCLUDE[crm_md](includes/crm_md.md)].|

> [!Note]
> Мастер настройки **Настройка подключения к Dynamics 365 for Sales** автоматически назначает роли безопасности **Администратор интеграции** и **Пользователь интеграции** учетной записи пользователя, используемой для интеграции. 

### <a name="to-create-or-maintain-the-connection-manually"></a>Создание или ведение подключения вручную
Далее описан порядок заполнения полей вручную на странице **Настройка подключения к Microsoft Dynamics 365 for Sales**. Это также страница, на которой можно управлять настройками для интеграции.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка подключения Microsoft Dynamics 365**, затем выберите связанную ссылку.
2. Введите следующие сведения для подключения из [!INCLUDE[crm_md](includes/crm_md.md)] к [!INCLUDE[d365fin](includes/d365fin_md.md)].

|Поле|Описанием|
|-----|-----|
|**URL-адрес Dynamics 365 for Sales**|URL-адрес вашего экземпляра [!INCLUDE[crm_md](includes/crm_md.md)]. Чтобы получить этот URL-адрес, откройте [!INCLUDE[crm_md](includes/crm_md.md)], скопируйте URL-адрес из адресной строки браузера, затем вставьте URL-адрес в это поле. [!INCLUDE[d365fin](includes/d365fin_md.md)] обеспечит правильный формат.|
|**Имя пользователя** и **Пароль**|Эти учетные данные учетной записи пользователя предназначены для интеграции. Дополнительные сведения см. в разделе [Настройка учетных записей пользователей для интеграции с Dynamics 365 for Sales](admin-setting-up-integration-with-dynamics-sales.md).|
|**Включено**|Начните использовать интеграцию. Если выполнять подключение в данный момент не требуется, можно сохранить настройки подключения, однако пользователи не получат доступа к данным [!INCLUDE[crm_md](includes/crm_md.md)] из [!INCLUDE[d365fin](includes/d365fin_md.md)]. Позднее следует вернуться на эту страницу и выполнить подключение.  |
|**Версия SDK Dynamics 365**|Если выполняется интеграция с локальной версией [!INCLUDE[crm_md](includes/crm_md.md)], следует использовать набор разработки программного обеспечения Dynamics 365 (также называемый Xrm) для подключения [!INCLUDE[d365fin](includes/d365fin_md.md)] к [!INCLUDE[crm_md](includes/crm_md.md)]. Выбранная версия должна быть совместима с версией SDK, которая используется приложением [!INCLUDE[crm_md](includes/crm_md.md)]. Эта версия равна или новее версии, используемой приложением [!INCLUDE[crm_md](includes/crm_md.md)].|

> [!Note]
> Если вы подключаете локальную версию [!INCLUDE[d365fin](includes/d365fin_md.md)] к [!INCLUDE[crm_md](includes/crm_md.md)] и хотите настроить подключение к экземпляру [!INCLUDE[crm_md](includes/crm_md.md)] с определенным типом проверки подлинности, заполните поля на экспресс-вкладке **Сведения о типе проверки подлинности**. Дополнительные сведения см. в разделе [Использование строк подключения в средстве XRM для подключения к Dynamics 365](https://go.microsoft.com/fwlink/?linkid=843055). Этот шаг не требуется при подключении к сетевой версии [!INCLUDE[d365fin](includes/d365fin_md.md)].

3. Введите следующие сведения для подключения из [!INCLUDE[d365fin](includes/d365fin_md.md)] к [!INCLUDE[crm_md](includes/crm_md.md)].

|Поле|Описанием|
|-----|-----|
|**URL-адрес Dynamics 365 Business Central Web Client**|URL-адрес вашего экземпляра [!INCLUDE[d365fin](includes/d365fin_md.md)]. Это позволяет пользователям в [!INCLUDE[crm_md](includes/crm_md.md)] открывать соответствующие записи в [!INCLUDE[d365fin](includes/d365fin_md.md)] из записей в [!INCLUDE[crm_md](includes/crm_md.md)], например счет или продукт. Записи [!INCLUDE[d365fin](includes/d365fin_md.md)] открываются в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Для использования задайте в этом поле URL-адрес экземпляра [!INCLUDE[d365fin](includes/d365fin_md.md)].<br /><br /> Для возврата в поле URL-адреса по умолчанию для [!INCLUDE[d365fin](includes/d365fin_md.md)], выберите действие **Сбросить URL-адрес веб-клиента**.<br /><br /> Это поле используется только в случае установки решения интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)].|
|**Веб-служба наличия товаров включена**|Разрешите пользователям, которые используют [!INCLUDE[crm_md](includes/crm_md.md)], просматривать наличие товаров (продуктов) в запасах в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Если она включена, также необходимо указать имя пользователя и ключ доступа для [!INCLUDE[crm_md](includes/crm_md.md)], чтобы использовать веб-службу OData для наличия товаров (продуктов). Дополнительные сведения см. в разделе [Веб-службы OData](/dynamics365/business-central/dev-itpro/webservices/odata-web-services.md).|
|**URL-адрес веб-службы OData Dynamics 365 Business Central**|Если включена веб-служба наличия товаров, URL-адрес веб-службы OData предоставляется для вас.|
|**Имя пользователя веб-службы OData Dynamics 365 Business Central**|Имя пользователя учетной записи, которую [!INCLUDE[crm_md](includes/crm_md.md)] использует для получения сведений о наличии товаров из [!INCLUDE[d365fin](includes/d365fin_md.md)] через веб-службу OData.|
|**Ключ доступа веб-службы OData Dynamics 365 Business Central**|Ключ доступа учетной записи пользователя, которую [!INCLUDE[crm_md](includes/crm_md.md)] использует для получения сведений о наличии товаров из [!INCLUDE[d365fin](includes/d365fin_md.md)] через веб-службу OData. Ключ назначается пользователю, выбранному в поле **Имя пользователя веб-службы OData Dynamics 365 Business Central**. Чтобы получить ключ, выберите кнопку **Найти значение** рядом с именем пользователя, выберите пользователя, выберите **Управление**, затем выберите **Правка**. В карточке пользователя выберите **Действия**, **Проверка подлинности**, затем выберите **Изменить ключ веб-службы**.|

4. Введите следующие настройки для [!INCLUDE[crm_md](includes/crm_md.md)].

|Поле|Описанием|
|-----|-----|
|**Интеграция заказов на продажу разрешена**|Разрешите пользователям отправлять заказы на продажу и активированные предложения в [!INCLUDE[crm_md](includes/crm_md.md)] и затем просматривать и обрабатывать их в [!INCLUDE[d365fin](includes/d365fin_md.md)].|
|**Автоматически создавать заказы на продажу**|Создание заказов на продажу в [!INCLUDE[d365fin](includes/d365fin_md.md)], когда пользователь создает и отправляет заказ на продажу в [!INCLUDE[crm_md](includes/crm_md.md)].|
|**Автоматически обрабатывать предложения по продаже**|Обработка предложения по продаже в [!INCLUDE[d365fin](includes/d365fin_md.md)], когда пользователь создает и активирует его в [!INCLUDE[crm_md](includes/crm_md.md)].|

5. Введите следующие дополнительные настройки.

|Поле|Описанием|
|-----|-----|
|**Пользователи [!INCLUDE[d365fin](includes/d365fin_md.md)] должны сопоставляться пользователям Dynamics 365 for Sales**|Укажите, должны ли учетные записи пользователей [!INCLUDE[d365fin](includes/d365fin_md.md)] иметь соответствующие учетные записи пользователей в [!INCLUDE[crm_md](includes/crm_md.md)]. **Адрес проверки подлинности Office 365** пользователя [!INCLUDE[d365fin](includes/d365fin_md.md)] должен быть тем же, что и **Основной адрес электронной почты** пользователя [!INCLUDE[crm_md](includes/crm_md.md)].<br /><br /> Если задано **Да**,пользователи [!INCLUDE[d365fin](includes/d365fin_md.md)] без совпадающей учетной записи пользователя [!INCLUDE[crm_md](includes/crm_md.md)] не будут обладать возможностями интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)] в пользовательском интерфейсе. Доступ к данным [!INCLUDE[crm_md](includes/crm_md.md)] непосредственно из [!INCLUDE[d365fin](includes/d365fin_md.md)] выполняется от имени учетной записи пользователя [!INCLUDE[crm_md](includes/crm_md.md)].<br /><br /> Если задано **Нет**, все пользователи [!INCLUDE[d365fin](includes/d365fin_md.md)] будут обладать возможностями интеграции [!INCLUDE[crm_md](includes/crm_md.md)] в пользовательском интерфейсе. Доступ к данным [!INCLUDE[crm_md](includes/crm_md.md)] выполняется от имени пользователя подключения (интеграции) [!INCLUDE[crm_md](includes/crm_md.md)].|
|**Текущий пользователь Business Central сопоставлен с пользователем Dynamics 365 for Sales**|Указывает, сопоставлена ли учетная запись пользователя учетной записи в [!INCLUDE[crm_md](includes/crm_md.md)]|

6. Для тестирования настроек подключения выберите **Проверить подключение**.  

    > [!NOTE]  
    >  Если шифрование данных не включено в [!INCLUDE[d365fin](includes/d365fin_md.md)], вы получите запрос, требуется ли его включить. Чтобы включить шифрование данных, выберите **Да** и предоставьте требуемую информацию. В противном случае выберите **Нет**. Шифрование данных можно включить позднее. Дополнительные сведения см. в разделе [Шифрование данных в Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-encrypting-data) в справке для разработчиков и ИТ-специалистов.  

7. Если синхронизация [!INCLUDE[crm_md](includes/crm_md.md)] еще не настроена, вы получите запрос, следует ли использовать настройки синхронизации по умолчанию. В зависимости от того, требуется ли соответствие записей в [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)], выберите **Да** или **Нет**.

> [!Note]
> При подключении к Dynamics 365 for Sales с помощью страницы **Настройка подключения к Microsoft Dynamics 365 for Sales** может потребоваться назначить роли безопасности Администратор интеграции и Пользователь интеграции учетной записи пользователя, используемой для интеграции. Для получения дополнительной информации см. [Назначение роли безопасности пользователю](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles#assign-a-security-role-to-a-user).


> [!Note]
> При подключении к Dynamics 365 for Sales с помощью страницы **Настройка подключения к Microsoft Dynamics 365 for Sales** может потребоваться [назначить роли безопасности **Администратор интеграции** и **Пользователь интеграции**](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles#assign-a-security-role-to-a-user) учетной записи пользователя, используемой для интеграции.


### <a name="to-disconnect-from-crm_md"></a>Отключение от [!INCLUDE[crm_md](includes/crm_md.md)]  
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка подключения Microsoft Dynamics 365 for Sales**, затем выберите связанную ссылку.
2. На странице **Настройка подключения Microsoft Dynamics 365 for Sales** снимите флажок **Включено**.  

<!--## Install the [!INCLUDE[d365fin](includes/d365fin_md.md) Integration Solution
[!INCLUDE[d365fin](includes/d365fin_md.md)] includes a solution that enables users to access coupled records, such as customers and items, from records in [!INCLUDE[crm_md](includes/crm_md.md)], such as accounts and products. The solution adds a link to the pages in [!INCLUDE[crm_md](includes/crm_md.md)] to open the coupled [!INCLUDE[d365fin](includes/d365fin_md.md)] record. The solution also displays information from [!INCLUDE[d365fin](includes/d365fin_md.md)]on certain entities in [!INCLUDE[crm_md](includes/crm_md.md)], such as accounts. Installing this solution is optional. <!--"Solution" sounds old school. Is it an app, or an add-in, or an extension?


1.  From [!INCLUDE[d365fin](includes/d365fin_md.md)] installation media \(DVD\), copy the DynamicsNAVIntegrationSolution.zip file to your computer.  

     The DynamicsNAVIntegrationSolution.zip file is located in the **CrmCustomization** folder. This file is the solution package.   

2.  In [!INCLUDE[crm_md](includes/crm_md.md)], import the DynamicsNAVIntegrationSolution.zip as a solution.  

     This step adds the **[!INCLUDE[d365fin](includes/d365fin_md.md) Connection** entity and **[!INCLUDE[d365fin](includes/d365fin_md.md) Account Statistics** entity in the system and additional items such as [!INCLUDE[d365fin](includes/d365fin_md.md)] integration security roles.  

     For more information about how to manage solutions in [!INCLUDE[crm_md](includes/crm_md.md)], [http://go.microsoft.com/fwlink/?LinkID=616519](http://go.microsoft.com/fwlink/?LinkID=616519).  

3.  Optional: Set up the **[!INCLUDE[d365fin](includes/d365fin_md.md) Connection** entity to display in the **Settings** area of [!INCLUDE[crm_md](includes/crm_md.md)].  

     This enables [!INCLUDE[crm_md](includes/crm_md.md)] users who are assigned the **[!INCLUDE[d365fin](includes/d365fin_md.md) Admin** role to modify the entity in [!INCLUDE[crm_md](includes/crm_md.md)]. For more information about how to modify entities in [!INCLUDE[crm_md](includes/crm_md.md)], see [View or edit entity information](http://go.microsoft.com/fwlink/?LinkID=616521).  

4.  Assign the **[!INCLUDE[d365fin](includes/d365fin_md.md) Integration Administrator** role to the user account for the connection to [!INCLUDE[d365fin](includes/d365fin_md.md)].  

5.  Assign the **Business Central Integration User** role to all users who will use the [!INCLUDE[d365fin](includes/d365fin_md.md)] integration solution.  

If you install the [!INCLUDE[d365fin](includes/d365fin_md.md)] integration solution after you have set up the connection to [!INCLUDE[crm_md](includes/crm_md.md)] in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must modify the connection setup to point to the URL.-->

<!--of the [!INCLUDE[nav_web_md](../developer/includes/nav_web_md.md)]. For more information, see [How to: Set Up a Microsoft Dynamics 365 for Sales Connection]() -->

<!--
# View Item Availability - Support Matrix
For most versions of [!INCLUDE[d365fin](includes/d365fin_md.md) and Dynamics 365 for Sales, you can view availability figures for items across the integrated products. The following table shows which version combinations support viewing item availability.

| |Dynamics 365 for Sales version|2015/Update 1/Online|2016/Update 1/Online|Dynamics 365 for Sales|
|-|---------------------|---------------------|--------------------------|-----------------|
|**Dynamics NAV version**|
|**2016**||Not supported|Not supported|Not supported|
|**2017**||Not supported - Install from 2016|Supported|Supported|
|**Dynamics 365 for Financials**||Not supported - Install from 2016|Supported|Supported|


> [Note]
> You can obtain item availability support for combinations of Dynamics CRM 2015 and Business Central by running the DynamicsNAVIntegrationSolution.zip file on the Business Central product DVD.

For more information, see [System Requirements for Business Central](../deployment/system-requirement-business-central.md).

-->

## <a name="see-also"></a>См. также  
[Просмотр статуса синхронизации](admin-how-to-view-synchronization-status.md)  
