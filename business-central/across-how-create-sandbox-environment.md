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
ms.date: 04/01/2019
ms.author: solsen
ms.openlocfilehash: 113c081e60b825c48cfb85ae3475a713a1a1e215
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "937950"
---
[!INCLUDE[d365fin_early_release](includes/d365fin_early_release.md.md)]

# <a name="creating-a-sandbox-environment"></a>Создание среды "песочницы"
Среда песочницы (функция для предварительного ознакомления) представляет собой непроизводственный экземпляр [!INCLUDE[d365fin](includes/d365fin_md.md)]. В среде песочницы, изолированной от производственной среды, можно безопасно исследовать, обучать, демонстрировать, разрабатывать и тестировать сервисы без риска повлиять на данные или настройки производственной среды.

## <a name="to-create-a-sandbox-environment"></a>Создание среды "песочницы"
Чтобы можно было создать среду песочницы, необходима подписка на [!INCLUDE[d365fin](includes/d365fin_md.md)]. В каждой подписке может быть только одна среда песочницы.

1. Выполните вход в производственный экземпляр службы [!INCLUDE[d365fin](includes/d365fin_md.md)].
2. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Среда "песочницы"**, затем выберите связанную ссылку.
<!-- ![Sandbox Environment Setup](./media/across-sandbox/sandbox-environment-setup.png) -->
3. Выберите **Создать**.  
  В браузере откроется другая вкладка для завершения настройки среды песочницы.
> [!NOTE]  
>  Если в браузере включена блокировка всплывающих окон, измените ее, чтобы разрешить URL-адреса с адреса *.businesscentral.dynamics.com.   

4. Когда среда песочницы будет готова, вы будете перенаправлены в приветственный мастер среды песочницы.
<!-- ![Sandbox Welcome Wizard](./media/across-sandbox/sandbox-wizard.png) -->

5. Выберите **Узнать больше**, чтобы ознакомиться с сценариями, которые можно попробовать в среде песочницы. Или выберите **Закрыть**, чтобы перейти в ролевой центр экземпляра "песочницы" [!INCLUDE[d365fin](includes/d365fin_md.md)].
6. В верхней части ролевого центра появится уведомление о том, что это среда песочницы. Тип среды также отображается в строке заголовка клиента.
<!-- ![Sandbox RoleCenter Notification](./media/across-sandbox/sandbox-rolecenter-notification.png) --> В среде песочницы создан новый арендатор. Для этого арендатора загружены демонстрационные данные по умолчанию компании CRONUS. При создании песочницы никакие данные не копируются и не переносятся каким-либо другим образом из производственной среды.

7. В любой момент можно вернуться на страницу **Среда "песочницы"** и сбросить среду "песочницы".
> [!NOTE]  
>  При сбросе среды песочницы она полностью удаляется, а затем создается заново с демонстрационными данными по умолчанию.  

8. Для переключения между производственной средой и средой песочницы можно использовать средства запуска приложений Business Central.
<!-- ![Sandbox Dynamics365 Menu](./media/across-sandbox/sandbox-dynamics365-menu.png) -->

9. Администратор или другой пользователь может ограничить или даже блокировать доступ некоторых пользователей к среде песочницы. Это можно сделать с помощью стандартных функций безопасности для продукта, таких как карта пользователя, группы пользователей и наборы разрешений.

<!-- ![Sandbox Permission Sets](./media/across-sandbox/sandbox-permission-sets.png) -->

## <a name="advanced-functionality-in-the-sandbox-environment"></a>Расширенная функциональная возможность в среде песочницы
### <a name="designer"></a>Дизайнер
В среде песочницы имеется включенная функция **Конструктор**, которую можно активировать, выбрав значок конструктора ![Конструктор](./media/across-sandbox/sandbox-inclient-design-icon.png) на странице.

<!-- ![In-client Designer](./media/across-sandbox/sandbox-inclient-designer.png) -->

### <a name="enable-the-advanced-user-experience"></a>Включение расширенных возможностей пользователя
Можно включить и попробовать расширенные (полные) функциональные возможности [!INCLUDE[d365fin](includes/d365fin_md.md)] в среде арендатора песочницы, задав поле **Опыт** на странице **Информация о компании**.

<!-- ![Sandbox Environment Advanced](./media/across-sandbox/sandbox-advanced.png) -->

<!-- ![Sandbox Production](./media/across-sandbox/sandbox-production.png) -->

После включения расширенных функциональных возможностей в арендаторе песочницы вы получаете доступ ко всем стандартным профилям и ролевым центрам. Можно также создать полностью настроенную пробную организацию, включая демонстрационные данные и доступ к расширенным возможностям продукта.

<!-- ![Sandbox New Company](./media/across-sandbox/sandbox-newcompany.png) -->


## <a name="see-also"></a>См. также
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
