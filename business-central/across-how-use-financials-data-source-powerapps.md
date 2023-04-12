---
title: Использование данных для создания приложения | Документация Майкрософт
description: Данные Business Central можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания бизнес-приложения с помощью Power Apps.
author: jswymer
ms.topic: conceptual
ms.service: dynamics365-business-central
ms.search.keywords: 'OData, Power App, SOAP'
ms.date: 04/01/2023
ms.author: jswymer
---
# Подключение к данным Business Central для создания бизнес-приложения с помощью Power Apps

Данные [!INCLUDE[prod_short](includes/prod_short.md)] можно сделать доступными в качестве источника данных в Power Apps.  

> [!NOTE]  
> Вы должны иметь допустимую учетную запись в [!INCLUDE[prod_short](includes/prod_short.md)] и в Power Apps.  

## Добавление [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных в Power Apps

1. В браузере перейдите к [powerapps.microsoft.com](https://powerapps.microsoft.com/) и выполните вход.
2. На домашней странице, в разделе **Начать с данных**, выберите плитка **Другие источники данных**.  

    Это открывает Power Apps Studio. При первом входе в систему необходимо указать страну/регион.  
3. В списке доступных соединений выберите **Business Central**, затем нажмите кнопку **Создать**.

    Power Apps подключится к вашему экземпляру [!INCLUDE[prod_short](includes/prod_short.md)] с использованием учетных данных, с которыми вы выполнили вход. Если вы не являетесь администратором [!INCLUDE[prod_short](includes/prod_short.md)], может потребоваться выполнить вход с другой учетной записью.  

4. Power Apps отобразит список *сред и организаций*, доступных в [!INCLUDE[prod_short](includes/prod_short.md)]. Выберите среду и организацию, содержащую данные, к которым вы хотите подключиться, такие как *РАБОЧАЯ — Моя компания*.  

5. Далее вам будет представлен список таблиц, которые предоставляются как часть API для вашей среды. Выберите таблицу, к которой вы хотите подключиться, а затем выберите **Подключить**.

Эти так называемые таблицы отображаются как конечные точки соединителем [!INCLUDE[prod_short](includes/prod_short.md)] для Power Apps.  

> [!NOTE]
> Если вы хотите включить в свое приложение данные из других таблиц в [!INCLUDE[prod_short](includes/prod_short.md)], вы должны совместно с разработчиком определить пользовательский API-интерфейс в [!INCLUDE[prod_short](includes/prod_short.md)].  

На этом шаге вы успешно подключились с данным [!INCLUDE[prod_short](includes/prod_short.md)] и готовы начать создание PowerApp. Можно добавить дополнительные экраны и подключить дополнительные данные из [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Создание приложения на основе холста из примера в Power Apps](/powerapps/maker/canvas-apps/open-and-run-a-sample-app).  

После разработки и построения приложения можно поделиться им с коллегами. Дополнительные сведения см. в разделе [Сохранение и публикация приложения на основе холста в Power Apps](/powerapps/maker/canvas-apps/save-publish-app).  

> [!NOTE]
> Если требуется подключиться к [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises, необходимо выбрать соединитель **Business Central (локальная версия)** на шаге 3.  

## См. соответствующее [обучение Microsoft](/training/paths/power-apps-power-automate-business-central/)

## См. также

[Создание приложения на основе холста из шаблона в Power Apps](/powerapps/maker/canvas-apps/get-started-test-drive)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Начальные сведения по разработке соединительных приложений для Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
