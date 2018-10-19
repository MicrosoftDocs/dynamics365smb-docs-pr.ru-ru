---
title: "Управление пользователями и ролями | Документы Майкрософт"
description: "Узнайте, как управлять пользователями и ролевыми центрами в Business Central."
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: profiles, users
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 1a94d023424c6eceb93af6e9ca89a90a3a94e996
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="understanding-users-profiles-and-role-centers"></a>Знакомство с пользователями, профилями и ролевыми центрами

В [!INCLUDE[d365fin](includes/d365fin_md.md)] пользователи добавляются администратором, который также предоставляет доступ к зонам [!INCLUDE[d365fin](includes/d365fin_md.md)], которые требуются им в процессе работы.  

Доступ к функции управляется с помощью *групп пользователей* и *профилей*. Как администратор вы можете добавлять и удалять пользователей в рамках своей подписки на [!INCLUDE[d365fin](includes/d365fin_md.md)], а также назначать разрешения для пользователей через группы.  

## <a name="adding-users"></a>Добавление пользователей

Для добавления пользователей в [!INCLUDE[d365fin](includes/d365fin_md.md)] Online администратор Office 365 организации сначала должен создать пользователей в центре администрирования Office 365. Дополнительные сведения см. в разделе [Добавление пользователей в Office 365 для бизнеса](https://aka.ms/CreateOffice365Users).

После этого администратор сможет назначить права доступа каждому пользователю и группе пользователей. Дополнительные сведения см. в разделе [Управление пользователями и разрешениями](ui-how-users-permissions.md).  

### <a name="users-of-on-premises-deployments"></a>Пользователи локальных развертываний

Для локальных развертываний [!INCLUDE[d365fin](includes/d365fin_md.md)] администратор может выбрать между различными механизмами авторизации учетной информации для пользователей. Затем при создании пользователя необходимо предоставить различную информацию в зависимости от используемого типа учетных данных в конкретном экземпляре [!INCLUDE[server](includes/server.md)]. Дополнительные сведения, см. в разделе [Проверка подлинности и типы учетных сведений](/dynamics365/business-central/dev-itpro/administration/users-credential-types) в разделе администрирование для разработчиков и содержимом ITPro для [!INCLUDE[d365fin](includes/d365fin_md.md)].  

## <a name="profiles"></a>Профили

Всем пользователям в организации, которые имеют доступ к [!INCLUDE[d365fin](includes/d365fin_md.md)], назначается *профиль*, открывающий им доступ к центру *Ролевой центр*.

Профили — это коллекции пользователей [!INCLUDE[d365fin](includes/d365fin_md.md)], которые относятся к одному ролевому центру. Ролевой центр является начальной страницей [!INCLUDE[d365fin](includes/d365fin_md.md)], с которой можно быстро запустить наиболее важные задачи и увидеть аналитику и КПЭ.  

> [!NOTE]  
>  В текущей версии [!INCLUDE[d365fin](includes/d365fin_md.md)] Online невозможно добавлять, изменять или удалять профили.  

## <a name="configuration-and-personalization"></a>Конфигурация и персонализация
<!--The concept of UI customization in [!INCLUDE[d365fin](includes/d365fin_md.md)] is divided in two:  

-   Configuration, performed by the administrator  

-   Personalization, performed by users  

The administrator configures the user interface for multiple users by customizing the user interface for a profile that the users are assigned to.  -->
Пользователи персонализируют пользовательский интерфейс персональной версии, настраивая ИП после входа со своими учетными данными. Эта персонализация может быть удалена администратором. Дополнительные сведения см. в разделе [Персонализация рабочей области](ui-personalization-user.md).  

## <a name="see-also"></a>См. также  
[Управление пользователями и разрешениями](ui-how-users-permissions.md)  
[Управление персонализацией в качестве администратора](ui-personalization-manage.md)  
[Персонализация рабочей области](ui-personalization-user.md)  

