---
title: Использование данных для создания приложения | Документация Майкрософт
description: Данные Business Central можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания бизнес-приложения с помощью Power Apps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: OData, Power App, SOAP
ms.date: 11/20/2019
ms.author: edupont
ms.openlocfilehash: 9cf587dca8224e742ecbde30bcabc35697bb6f2a
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881004"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-power-apps"></a>Подключение к данным Business Central для создания бизнес-приложения с помощью Power Apps

Данные [!INCLUDE[prodshort](includes/prodshort.md)] можно сделать доступными как источник данных в Power Apps.  

> [!NOTE]  
> Вы должны иметь допустимую учетную запись в [!INCLUDE[prodshort](includes/prodshort.md)] и в Power Apps.  

## <a name="to-add-includeprodshortincludesprodshortmd-as-a-data-source-in-power-apps"></a>Добавление [!INCLUDE[prodshort](includes/prodshort.md)] как источника данных в Power Apps

1. В браузере перейдите к [powerapps.microsoft.com](https://powerapps.microsoft.com/) и выполните вход.
2. На домашней странице выберите **Приложения**, **Создать приложение** и **Холст**, чтобы создать новое приложение на основе холста. Это приложение будет разработано для использования на мобильных устройствах, но также можно выбрать для использования другой шаблон.

    Следующий шаг создания Power App — выбор данных. Щелкните значок стрелки, а затем выберите параметр **Новое подключение** в левом верхнем углу страницы.
3. В списке доступных соединений выберите **Business Central**, затем нажмите кнопку **Создать**.

    Power Apps подключится к вашему [!INCLUDE [prodshort](includes/prodshort.md)] с использованием учетных данных, с которыми вы выполнили вход. Если вы не являетесь администратором [!INCLUDE [prodshort](includes/prodshort.md)], может потребоваться выполнить вход с другой учетной записью.  

4. Power Apps отобразит список *сред и организаций*, доступных в [!INCLUDE [prodshort](includes/prodshort.md)]. Выберите среду и организацию, содержащую данные, к которым вы хотите подключиться. Далее вы увидите список API. Выберите **API**, к которому вы ходите подключиться.

Эти так называемые таблицы являются частью API-интерфейса [!INCLUDE [prodshort](includes/prodshort.md)]. Можно не настаивать конечные точки самому — соединитель [!INCLUDE [prodshort](includes/prodshort.md)] для Power Apps сделает это за вас.  

> [!NOTE]
> Если требуется включение данных из других таблиц в [!INCLUDE [prodshort](includes/prodshort.md)] в ваше приложение, необходимо совместно с разработчиком определить пользовательский API в [!INCLUDE [prodshort](includes/prodshort.md)], а затем использовать этот пользовательский API через пользовательский соединитель в Power Apps. Дополнительные сведения см. в разделе [Создание пользовательского соединителя с нуля](/connectors/custom-connectors/define-blank).  

На этом шаге вы успешно подключились с данным [!INCLUDE [prodshort](includes/prodshort.md)] и готовы начать создание PowerApp. Можно добавить дополнительные экраны и подключить дополнительные данные из [!INCLUDE [prodshort](includes/prodshort.md)]. Дополнительные сведения см. в разделе [Создание приложения на основе холста из шаблона в Power Apps](/powerapps/maker/canvas-apps/get-started-test-drive).  

После разработки и построения приложения можно поделиться им с коллегами. Дополнительные сведения см. в разделе [Сохранение и публикация приложения на основе холста в Power Apps](/powerapps/maker/canvas-apps/save-publish-app).  

> [!NOTE]
> Если требуется подключиться к [!INCLUDE [prodshort](includes/prodshort.md)] On-Premises, необходимо выбрать соединитель **Business Central (локальная версия)** на шаге 3.  

## <a name="see-also"></a>См. также

[Создание приложения на основе холста из шаблона в Power Apps](/powerapps/maker/canvas-apps/get-started-test-drive)  
[Приступая к работе](product-get-started.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Финансы](finance.md)  
[Начальные сведения по разработке соединительных приложений для Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  
