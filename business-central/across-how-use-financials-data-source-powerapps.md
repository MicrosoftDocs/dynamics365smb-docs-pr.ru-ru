---
title: Использование данных для создания приложения | Документация Майкрософт
description: Данные Business Central можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания бизнес-приложения с помощью PowerApps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Odata, Power App, SOAP
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: 4b8005154afb988cf25c6a04b7beeaafd199afca
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2305031"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-powerapps"></a>Подключение к данным Business Central для создания бизнес-приложения с помощью PowerApps
Данные [!INCLUDE[d365fin](includes/d365fin_md.md)] можно сделать доступными в качестве источника данных в PowerApps.  

> [!NOTE]  
>   Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в PowerApps.  

## <a name="to-add-included365finincludesd365fin_mdmd-as-a-data-source-in-powerapps"></a>Добавление [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных в PowerApps
1. В браузере перейдите к [powerapps.microsoft.com](https://powerapps.microsoft.com/en-us/) и выполните вход.
2. На домашней странице выберите **Приложения**, **Создать приложение** и **Холст**, чтобы создать новое приложение на основе холста. Это приложение будет разработано для использования на мобильных устройствах, но также можно выбрать для использования другой шаблон.

    Следующий шаг создания PowerApp — выбор данных. Щелкните значок стрелки, а затем выберите параметр **Новое подключение** в левом верхнем углу страницы.
3. В списке доступных соединений выберите **Business Central**, затем нажмите кнопку **Создать**.

    PowerApps подключится к вашему экземпляру [!INCLUDE [prodshort](includes/prodshort.md)] с использованием учетных данных, с которыми вы выполнили вход. Если вы не являетесь администратором [!INCLUDE [prodshort](includes/prodshort.md)], может потребоваться выполнить вход с другой учетной записью.  

4.  PowerApps отобразит список *сред и организаций*, доступных в [!INCLUDE [prodshort](includes/prodshort.md)]. Выберите среду и организацию, содержащую данные, к которым вы хотите подключиться. Далее вы увидите список API. Выберите **API**, к которому вы ходите подключиться.

Эти так называемые таблицы являются частью API-интерфейса [!INCLUDE [prodshort](includes/prodshort.md)]. Настраивать конечные точки вам не нужно — соединитель [!INCLUDE [prodshort](includes/prodshort.md)] для PowerApps делает это автоматически.  

    If you want to include data from other tables in [!INCLUDE [prodshort](includes/prodshort.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE [prodshort](includes/prodshort.md)] and then consume that custom API through a custom connector in PowerApps. For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).  

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
