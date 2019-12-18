---
title: Создание среды "песочницы" | Документация Майкрософт
description: Создайте среду для исследования, обучения, демонстрации, разработки и тестирования.
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sandbox, demo, develop
ms.date: 12/06/2019
ms.author: solsen
ms.openlocfilehash: 0f8f0f85df89c1d71fc3e114ebd902f2aa85f802
ms.sourcegitcommit: b6e506a45a1cd632294bafa1c959746cc3a144f6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/06/2019
ms.locfileid: "2896113"
---
# <a name="creating-a-sandbox-environment-in-include-prodshortincludesprodshortmd"></a>Создание среды "песочницы" в [!INCLUDE [prodshort](includes/prodshort.md)]

В [!INCLUDE [prodshort](includes/prodshort.md)] вы можете легко создать безопасную среду, в которой тестировать, обучать или устранять неполадки, не нарушая рабочие процессы вашей компании или бизнес-данные. Такая непроизводственная среда называется *песочницей*. В среде песочницы, изолированной от производственной среды, можно безопасно исследовать, обучать, демонстрировать, разрабатывать и тестировать сервисы без риска повлиять на данные или настройки производственной среды.  

Ваш администратор может создавать среду "песочницы" в [центре администрирования](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments?toc=/dynamics365/business-central/toc.json), но если вы хотите быстро протестировать что-нибудь, вы можете создать среду "песочницы" из [!INCLUDE [prodshort](includes/prodshort.md)].  

> [!NOTE]
> Формально среды "песочницы" сильно отличаются от производственных сред, даже если ваш администратор создает "песочницу", включающую производственные данные. Вы не можете использовать песочницу для сравнительного и не можете, например, запросить экспорт базы данных. Если вы хотите создать "песочницу" для сравнительного тестирования, ваш администратор может создать выделенную производственную среду в центре администрирования. Дополнительные сведения см. в разделе [Типы сред](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments#types-of-environments).

## <a name="to-create-a-sandbox-environment-in-your-include-prodshortincludesprodshortmd"></a>Создание среды "песочницы" в [!INCLUDE [prodshort](includes/prodshort.md)]

1. Выполните вход в производственный экземпляр [!INCLUDE[d365fin](includes/d365fin_md.md)].

2. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Среда "песочницы"**, затем выберите соответствующую ссылку.
    <!-- ![Sandbox Environment Setup](./media/across-sandbox/sandbox-environment-setup.png) -->
3. Нажмите кнопку **Создать**.  

    Откроется еще одна вкладка с [!INCLUDE[d365fin](includes/d365fin_md.md)], на которой вы можете завершить настройку среды песочницы.

    > [!NOTE]  
    >  Если в браузере включена блокировка всплывающих окон, измените ее, чтобы разрешить URL-адреса с адреса *.businesscentral.dynamics.com.

Когда среда песочницы будет готова, вы будете перенаправлены в приветственный мастер среды песочницы.
<!-- ![Sandbox Welcome Wizard](./media/across-sandbox/sandbox-wizard.png) -->

Нажмите кнопку **Подробнее**, чтобы прочитать о сценариях для разработчиков, которые вы можете попробовать в среде песочницы, или кнопку **Закрыть**, чтобы перейти к ролевому центру вашего экземпляр песочницы [!INCLUDE[d365fin](includes/d365fin_md.md)].

В верхней части ролевого центра появится уведомление о том, что это среда песочницы. Тип среды также отображается в строке заголовка клиента.
    <!-- ![Sandbox RoleCenter Notification](./media/across-sandbox/sandbox-rolecenter-notification.png) -->

> [!NOTE]
> Созданная таким образом среда песочницы содержит только демонстрационные данные по умолчанию для компании CRONUS. Никакие данные не копируются и не переносятся каким-либо другим образом из производственной среды.<br /><br />
> Вы также можете создать среду песочницы, содержащую производственные данные. Вы должны сделать это через центр администрирования. Дополнительные сведения см. в разделе [Управление средами](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments) в справке для разработчиков и ИТ-специалистов.

В любой момент можно вернуться на страницу **Среда "песочницы"** и сбросить среду "песочницы".

> [!NOTE]  
> При сбросе среды песочницы она полностью удаляется, а затем создается заново с демонстрационными данными по умолчанию.  

<!--To switch between your production and sandbox environments, you can use the Business Central app launcher.
    ![Sandbox Dynamics365 Menu](./media/across-sandbox/sandbox-dynamics365-menu.png) -->

Администратор может ограничить или даже блокировать доступ некоторых пользователей к среде "песочницы". Это можно сделать с помощью стандартных функций безопасности для продукта, таких как карта пользователя, группы пользователей и наборы разрешений. Дополнительные сведения см. в разделе [Назначение разрешений пользователям и группам](ui-define-granular-permissions.md).  

<!-- ![Sandbox Permission Sets](./media/across-sandbox/sandbox-permission-sets.png) -->

## <a name="advanced-functionality-in-the-sandbox-environment"></a>Расширенная функциональная возможность в среде песочницы

Среда "песочницы" не менее полезна, потому что она включает в себя несколько удобных функций.

### <a name="designer"></a>Конструктор

В среде "песочницы" включен **Конструктор**. Вы можете активировать конструктор, выбрав значок конструктора ![Конструктор](./media/across-sandbox/sandbox-inclient-design-icon.png) на странице или выбрав дизайн пункт меню **Конструктор** в меню настроек ![Настройки](media/ui-experience/settings_icon_small.png).

<!-- ![In-client Designer](./media/across-sandbox/sandbox-inclient-designer.png) -->

### <a name="to-enable-the-advanced-user-experience"></a>Включение расширенных возможностей пользователя
Можно включить и попробовать расширенные (полные) функциональные возможности [!INCLUDE[d365fin](includes/d365fin_md.md)] в среде арендатора песочницы, задав поле **Опыт** на странице **Информация о компании**.

<!-- ![Sandbox Environment Advanced](./media/across-sandbox/sandbox-advanced.png) -->

<!-- ![Sandbox Production](./media/across-sandbox/sandbox-production.png) -->

После включения расширенных функциональных возможностей в арендаторе песочницы вы получаете доступ ко всем стандартным профилям (ролям) и ролевым центрам. Можно также создать полностью настроенную пробную организацию, включая демонстрационные данные и доступ к расширенным возможностям продукта.

<!-- ![Sandbox New Company](./media/across-sandbox/sandbox-newcompany.png) -->

## <a name="see-also"></a>См. также

[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Пробные версии и подписки [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](across-preview.md)  
[Управление средами в центре администрирования Business Central](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments)  
