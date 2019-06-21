---
title: Использование данных для создания приложения | Microsoft Docs
description: Данные Business Central можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания бизнес-приложения с помощью PowerApps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Odata, Power App, SOAP
ms.date: 05/13/2019
ms.author: edupont
ms.openlocfilehash: 67d7129e32ccde3154a02dd12b806d712f470833
ms.sourcegitcommit: 92c7b6c5f0a5d8becbef106ab85258906765bc3e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "1540273"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-powerapps"></a>Подключение к данным Business Central для создания бизнес-приложения с помощью PowerApps
Данные [!INCLUDE[d365fin](includes/d365fin_md.md)] можно сделать доступными как источник данных в PowerApps.  

> [!NOTE]  
>   Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в PowerApps.  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-powerapps"></a>Добавление [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных в PowerApps
1. В браузере перейдите к [powerapps.microsoft.com](https://powerapps.microsoft.com/en-us/) и выполните вход.
2. На домашней странице выберите шаблон **Начать с данных** для создания нового приложения на основе холста. Это приложение будет разработано для использования на мобильных устройствах, но также можно выбрать для использования другой шаблон.

    Следующий шаг создания PowerApp — выбор данных. Щелкните значок стрелки, а затем выберите параметр **Новое подключение** в левом верхнем углу страницы.
3. В списке доступных соединений выберите **Business Central**, затем нажмите кнопку **Создать**.

    PowerApps подключится к вашему [!INCLUDE [prodshort](includes/prodshort.md)] с использованием учетных данных, с которыми вы выполнили вход. Если вы не являетесь администратором [!INCLUDE [prodshort](includes/prodshort.md)], может потребоваться выполнить вход с другой учетной записью.  

4. Если имеется несколько организаций в [!INCLUDE [prodshort](includes/prodshort.md)], необходимо выбрать организацию для подсоединения к ней. Затем PowerApps отобразит список *таблиц*, доступных из [!INCLUDE [prodshort](includes/prodshort.md)]. Эти так называемые таблицы являются частью API-интерфейса [!INCLUDE [prodshort](includes/prodshort.md)]. Можно не настаивать конечные точки самому, — соединитель [!INCLUDE [prodshort](includes/prodshort.md)] для PowerApps сделает это за вас.  

    Если требуется включение данных из других таблиц в [!INCLUDE [prodshort](includes/prodshort.md)] в ваше приложение, необходимо работать с разработчиком для определения пользовательского API-интерфейса в [!INCLUDE [prodshort](includes/prodshort.md)], затем использовать этот пользовательский API-интерфейс через пользовательский соединитель в PowerApps. Дополнительные сведения см. в разделе [Создание пользовательского соединителя с нуля](/connectors/custom-connectors/define-blank).  

На этом шаге вы успешно подключились с данным [!INCLUDE [prodshort](includes/prodshort.md)] и готовы начать создание PowerApp. Можно добавить дополнительные экраны и подключить дополнительные данные из [!INCLUDE [prodshort](includes/prodshort.md)]. Дополнительные сведения см. в разделе [Создание приложения на основе холста из шаблона в PowerApps](/powerapps/maker/canvas-apps/get-started-test-drive).  

После разработки и построения приложения можно поделиться им с коллегами. Дополнительные сведения см. в разделе [Сохранение и публикация приложения на основе холста в PowerApps](/powerapps/maker/canvas-apps/save-publish-app).  

> [!NOTE]
> Если требуется подключиться к [!INCLUDE [prodshort](includes/prodshort.md)] On-Premises, необходимо выбрать соединитель **Business Central (локальная версия)** на шаге 3.  

## <a name="see-also"></a>См. также

[Создание приложения на основе холста из шаблона в PowerApps](/powerapps/maker/canvas-apps/get-started-test-drive)  
[Приступая к работе](product-get-started.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Финансы](finance.md)  
[Начальные сведения по разработке соединительных приложений для Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  
