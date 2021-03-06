---
title: Использование данных для создания приложения | Документация Майкрософт
description: Данные Business Central можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания бизнес-приложения с помощью Power Apps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: OData, Power App, SOAP
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 25607473e20bca8cec8cd65e2e808e12dda47869
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5774540"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-power-apps"></a>Подключение к данным Business Central для создания бизнес-приложения с помощью Power Apps

Данные [!INCLUDE[prod_short](includes/prod_short.md)] можно сделать доступными в качестве источника данных в Power Apps.  

> [!NOTE]  
> Вы должны иметь допустимую учетную запись в [!INCLUDE[prod_short](includes/prod_short.md)] и в Power Apps.  

## <a name="to-add-prod_short-as-a-data-source-in-power-apps"></a>Добавление [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных в Power Apps

1. В браузере перейдите к [powerapps.microsoft.com](https://powerapps.microsoft.com/) и выполните вход.
2. На домашней странице, в разделе **Начать с данных**, выберите плитка **Другие источники данных**.  

    Это открывает Power Apps Studio. При первом входе в систему необходимо указать страну/регион.  
3. В списке доступных соединений выберите **Business Central**, затем нажмите кнопку **Создать**.

    Power Apps подключится к вашему экземпляру [!INCLUDE[prod_short](includes/prod_short.md)] с использованием учетных данных, с которыми вы выполнили вход. Если вы не являетесь администратором [!INCLUDE[prod_short](includes/prod_short.md)], может потребоваться выполнить вход с другой учетной записью.  

4. Power Apps отобразит список *сред и организаций*, доступных в [!INCLUDE[prod_short](includes/prod_short.md)]. Выберите среду и организацию, содержащую данные, к которым вы хотите подключиться, такие как *РАБОЧАЯ — Моя компания*.  

5. Далее вам будет представлен список таблиц, которые предоставляются как часть API для вашей среды. Выберите таблицу, к которой вы хотите подключиться, а затем выберите **Подключить**.

Эти так называемые таблицы отображаются как конечные точки соединителем [!INCLUDE[prod_short](includes/prod_short.md)] для Power Apps.  

> [!NOTE]
> Если требуется включение данных из других таблиц в [!INCLUDE[prod_short](includes/prod_short.md)] в ваше приложение, необходимо работать с разработчиком для определения пользовательского API-интерфейса в [!INCLUDE[prod_short](includes/prod_short.md)], затем использовать этот пользовательский API-интерфейс через пользовательский соединитель в Power Apps. Дополнительные сведения см. в разделе [Создание пользовательского соединителя с нуля](/connectors/custom-connectors/define-blank).  

На этом шаге вы успешно подключились с данным [!INCLUDE[prod_short](includes/prod_short.md)] и готовы начать создание PowerApp. Можно добавить дополнительные экраны и подключить дополнительные данные из [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Создание приложения на основе холста из примера в Power Apps](/powerapps/maker/canvas-apps/open-and-run-a-sample-app).  

После разработки и построения приложения можно поделиться им с коллегами. Дополнительные сведения см. в разделе [Сохранение и публикация приложения на основе холста в Power Apps](/powerapps/maker/canvas-apps/save-publish-app).  

> [!NOTE]
> Если требуется подключиться к [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises, необходимо выбрать соединитель **Business Central (локальная версия)** на шаге 3.  

## <a name="see-also"></a>См. также

[Создание приложения на основе холста из шаблона в Power Apps](/powerapps/maker/canvas-apps/get-started-test-drive)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Начальные сведения по разработке соединительных приложений для Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  


[!INCLUDE[footer-include](includes/footer-banner.md)]