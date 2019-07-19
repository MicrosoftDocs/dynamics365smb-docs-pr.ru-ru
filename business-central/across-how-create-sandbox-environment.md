---
title: Создание среды "песочницы" | Документы Майкрософт
description: Создайте среду для исследования, обучения, демонстрации, разработки и тестирования.
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sandbox, demo, develop
ms.date: 06/26/2019
ms.author: solsen
ms.openlocfilehash: 217310522d7e54eeaa9dbd50df4ff89b0d68517d
ms.sourcegitcommit: 5b6dd8d881c0eb65ece6936a94dfda3185574335
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "1711087"
---
[!INCLUDE[d365fin_early_release](includes/d365fin_early_release.md.md)]

# <a name="creating-a-sandbox-environment"></a>Создание среды "песочницы"
Среда песочницы (функция для предварительного ознакомления) представляет собой непроизводственный экземпляр [!INCLUDE[d365fin](includes/d365fin_md.md)]. В среде песочницы, изолированной от производственной среды, можно безопасно исследовать, обучать, демонстрировать, разрабатывать и тестировать сервисы без риска повлиять на данные или настройки производственной среды.

## <a name="to-create-a-sandbox-environment"></a>Создание среды "песочницы"
Чтобы можно было создать среду песочницы, необходима подписка на [!INCLUDE[d365fin](includes/d365fin_md.md)]. В каждой подписке может быть только одна среда песочницы.

1. Выполните вход в производственный экземпляр службы [!INCLUDE[d365fin](includes/d365fin_md.md)].

2. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Среда "песочницы"**, затем выберите связанную ссылку.
<!-- ![Sandbox Environment Setup](./media/across-sandbox/sandbox-environment-setup.png) -->
3. Нажмите кнопку **Создать**.  

    Откроется еще одна вкладка с [!INCLUDE[d365fin](includes/d365fin_md.md)], на которой вы можете завершить настройку среды песочницы.

    > [!NOTE]  
    >  Если в браузере включена блокировка всплывающих окон, измените ее, чтобы разрешить URL-адреса с адреса *.businesscentral.dynamics.com.

4. Когда среда песочницы будет готова, вы будете перенаправлены в приветственный мастер среды песочницы.
<!-- ![Sandbox Welcome Wizard](./media/across-sandbox/sandbox-wizard.png) -->

5. Нажмите кнопку **Подробнее**, чтобы прочитать о сценариях, которые вы можете попробовать в среде песочницы, или кнопку **Закрыть**, чтобы перейти к ролевому центру вашего экземпляр песочницы [!INCLUDE[d365fin](includes/d365fin_md.md)].

    В верхней части ролевого центра появится уведомление о том, что это среда песочницы. Тип среды также отображается в строке заголовка клиента.
    <!-- ![Sandbox RoleCenter Notification](./media/across-sandbox/sandbox-rolecenter-notification.png) -->

    > [!NOTE]
    > Созданная таким образом среда песочницы содержит только демонстрационные данные по умолчанию для компании CRONUS. Никакие данные не копируются и не переносятся каким-либо другим образом из производственной среды.<br /><br />
    > Вы также можете создать среду песочницы, содержащую производственные данные. Вы должны сделать это через центр администрирования. Дополнительные сведения см. в разделе [Управление средами](/business-central/dev-itpro/administration/tenant-admin-center-environments) в справке для разработчиков и ИТ-специалистов.

6. В любой момент можно вернуться на страницу **Среда "песочницы"** и сбросить среду "песочницы".
    > [!NOTE]  
    >  При сбросе среды песочницы она полностью удаляется, а затем создается заново с демонстрационными данными по умолчанию.  

7. Для переключения между производственной средой и средой песочницы можно использовать средства запуска приложений Business Central.
<!-- ![Sandbox Dynamics365 Menu](./media/across-sandbox/sandbox-dynamics365-menu.png) -->

8. Администратор или другой пользователь может ограничить или даже блокировать доступ некоторых пользователей к среде песочницы. Это можно сделать с помощью стандартных функций безопасности для продукта, таких как карта пользователя, группы пользователей и наборы разрешений.

<!-- ![Sandbox Permission Sets](./media/across-sandbox/sandbox-permission-sets.png) -->

## <a name="advanced-functionality-in-the-sandbox-environment"></a>Расширенная функциональная возможность в среде песочницы
### <a name="designer"></a>Дизайнер
В среде песочницы имеется включенная функция **Конструктор**, которую можно активировать, выбрав значок конструктора ![Конструктор](./media/across-sandbox/sandbox-inclient-design-icon.png) на странице.

<!-- ![In-client Designer](./media/across-sandbox/sandbox-inclient-designer.png) -->

### <a name="to-enable-the-advanced-user-experience"></a>Включение расширенных возможностей пользователя
Можно включить и попробовать расширенные (полные) функциональные возможности [!INCLUDE[d365fin](includes/d365fin_md.md)] в среде арендатора песочницы, задав поле **Опыт** на странице **Информация о компании**.

<!-- ![Sandbox Environment Advanced](./media/across-sandbox/sandbox-advanced.png) -->

<!-- ![Sandbox Production](./media/across-sandbox/sandbox-production.png) -->

После включения расширенных функциональных возможностей в арендаторе песочницы вы получаете доступ ко всем стандартным профилям и ролевым центрам. Можно также создать полностью настроенную пробную организацию, включая демонстрационные данные и доступ к расширенным возможностям продукта.

<!-- ![Sandbox New Company](./media/across-sandbox/sandbox-newcompany.png) -->


## <a name="see-also"></a>См. также
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
