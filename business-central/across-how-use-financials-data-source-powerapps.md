---
title: Использование данных для создания приложения | Документация Майкрософт
description: Данные Business Central можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания бизнес-приложения с помощью Power Apps.
author: jswymer
ms.topic: conceptual
ms.service: dynamics365-business-central
ms.search.keywords: 'OData, Power App, SOAP'
ms.date: 05/15/2023
ms.author: jswymer
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-power-apps"></a>Подключение к данным Business Central для создания бизнес-приложения с помощью Power Apps

Данные [!INCLUDE[prod_short](includes/prod_short.md)] можно сделать доступными в качестве источника данных в Power Apps.  

> [!TIP]  
> Теперь Business Central поддерживает разработку и использование решений Power Platform на языке AL-Go, а также содержит образцы, с помощью которых вы сможете начать создавать свои собственные приложения в Power Apps. Эти функции в настоящее время находятся на этапе предварительной версии. Чтобы узнать больше, прочитайте статью [Business Central и Power Apps](/dynamics365/business-central/dev-itpro/powerplatform/power-apps-overview) в справке для разработчиков и ИТ-специалистов.

## <a name="prerequisites"></a>Предварительные требования

Вы должны иметь допустимую учетную запись в [!INCLUDE[prod_short](includes/prod_short.md)] и в Power Apps.  

## <a name="add--as-a-data-source-in-power-apps"></a>Добавление [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных в Power Apps

Эти шаги позволяют добавить таблицу Business Central, такую как «Клиенты» или «Товары», в качестве источника данных приложения Power Apps .

1. В браузере перейдите на [powerapps.microsoft.com](https://powerapps.microsoft.com/) и выполните вход.
2. На панели навигации слева выберите **+ Создать**, а затем выберите **Другие источники данных** на странице **Создание приложения** .
  
   <!-- This step opens Power Apps canavs. On first sign-in, you must specify the country/region.  -->
3. В списке **Подключения** отображаются все существующие у вас подключения к данным.

   - Если подключение **Business Central** уже есть, выберите его, а затем выберите **Создать**.

   - Если вы не видите подключения к Business Central, выберите **+ Новое подключение**, найдите и выберите **Business Central**, а затем выберите **Создать**.

   > [!NOTE]
   > Если вы хотите подключаться к локальному экземпляру [!INCLUDE[prod_short](includes/prod_short.md)], вы должны выбрать соединитель **Business Central (локальный)**.  
  
4. Power Apps подключается к вашему экземпляру [!INCLUDE[prod_short](includes/prod_short.md)]. Войдите в систему, используя учетную запись и пароль Business Central. Если вы не являетесь администратором [!INCLUDE[prod_short](includes/prod_short.md)], может потребоваться выполнить вход с другой учетной записью.  
5. После входа в систему Power Apps отобразит список *сред и организаций*, доступных в [!INCLUDE[prod_short](includes/prod_short.md)]. Выберите среду и организацию, содержащую данные, к которым вы хотите подключиться, такие как *РАБОЧАЯ — Моя компания*.  
6. Далее вы увидите список таблиц, которые предоставляются в составе API для вашей среды. Выберите таблицу, к которой вы хотите подключиться, а затем выберите **Подключить**.

Эти так называемые таблицы отображаются как конечные точки соединителем [!INCLUDE[prod_short](includes/prod_short.md)] для Power Apps.  

> [!NOTE]
> Если вы хотите включить в свое приложение данные из других таблиц в [!INCLUDE[prod_short](includes/prod_short.md)], вы должны совместно с разработчиком определить пользовательский API-интерфейс в [!INCLUDE[prod_short](includes/prod_short.md)].  

На данный момент вы успешно подключились с данным [!INCLUDE[prod_short](includes/prod_short.md)] и готовы приступать к созданию приложения Power Apps. Вы можете в любой момент добавить дополнительные экраны и подключить дополнительные данные. Подробнее см. в статье [Создание приложения на основе холста из примера в Power Apps](/powerapps/maker/canvas-apps/open-and-run-a-sample-app).  

После разработки и построения приложения можно поделиться им с коллегами. Дополнительные сведения см. в разделе [Сохранение и публикация приложения на основе холста в Power Apps](/powerapps/maker/canvas-apps/save-publish-app).  

<!--
## <a name="sample-apps-to-get-started"></a>Sample apps to get started

As a preview version, Business Central offers several sample apps that you can use as a starting point for building your own apps that use Business Central data. These sample apps are available in the [Business Central Demos](https://github.com/BusinessCentralDemos) repo on GitHub. For a quick overview on the apps, go to [Power Apps samples for Business Central](/dynamics365/business-central/dev-itpro/powerplatform/power-apps-samples).

## <a name="develop-and-maintain-apps-application-lifecycle-management"></a>Develop and maintain apps application lifecycle management

As an app developer, you may already be familiar with Business Central AL-Go. AL-Go is set of tools on GiHub that enables you to maintain professional DevOps processes for your Business Central AL projects. AL-Go supports source control and activities, like building, testing, and deploying. As a preview, Business Central now offers an Al-Go version that supports for Power Platform solutions. The preview, for example, includes workflows that let you push and pull Power Platfrom changes to and from enviroments. You can access the tools at [https://github.com/BusinessCentralDemos/AL-Go-PTE](https://github.com/BusinessCentralDemos/AL-Go-PTE). For more information, see [Application lifecycle management for Power Apps in Business Central](/dynamics365/business-central/dev-itpro/powerplatform/power-apps-alm).-->

## <a name="see-also"></a>См. также

[Создание приложения на основе холста из шаблона в Power Apps](/powerapps/maker/canvas-apps/get-started-test-drive)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Начальные сведения по разработке соединительных приложений для Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
