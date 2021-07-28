---
title: Создание среды "песочницы"
description: Создайте среду песочницу "тест" для безопасного изучения, обучения, демонстрирования, устранения сбоев и тестирования в Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sandbox, demo, develop
ms.date: 06/08/2021
ms.author: solsen
ms.openlocfilehash: 2f4ca6a98aac49fa5fea7d8658ef51a9510c97d7
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "6437681"
---
# <a name="creating-a-sandbox-environment-in-prod_short"></a>Создание среды "песочницы" в [!INCLUDE[prod_short](includes/prod_short.md)]

В [!INCLUDE[prod_short](includes/prod_short.md)] вы можете легко создать безопасную среду, в которой тестировать, обучать или устранять неполадки, не нарушая рабочие процессы вашей компании или бизнес-данные. Такая непроизводственная среда называется *песочницей*. В среде песочницы, изолированной от производственной среды, можно безопасно исследовать, обучать, демонстрировать, разрабатывать и тестировать сервисы без риска повлиять на данные или настройки производственной среды.  

Ваш администратор может управлять средами "песочницы" в [центре администрирования](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments?toc=/dynamics365/business-central/toc.json), но если вы хотите быстро протестировать что-нибудь, вы можете создать среду "песочницы" из [!INCLUDE[prod_short](includes/prod_short.md)]. Когда вы закончите, вы можете удалить песочницу с помощью центра администрирования.  

> [!NOTE]
> Формально среды "песочницы" сильно отличаются от производственных сред, даже если ваш администратор создает "песочницу", включающую производственные данные. Вы не можете использовать песочницу для сравнительного и не можете, например, запросить экспорт базы данных. Если вы хотите создать "песочницу" для сравнительного тестирования, ваш администратор может создать выделенную среду в центре администрирования. Для получения дополнительной информации см. [Рабочая среда и среда песочницы](/dynamics365/business-central/dev-itpro/administration/environment-types).

## <a name="to-create-a-sandbox-environment-in-your-prod_short"></a>Создание среды "песочницы" в [!INCLUDE[prod_short](includes/prod_short.md)]

1. Выполните вход в производственный экземпляр [!INCLUDE[prod_short](includes/prod_short.md)].

2. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Среда-песочница**, а затем выберите связанную ссылку.
    <!-- ![Sandbox Environment Setup.](./media/across-sandbox/sandbox-environment-setup.png) -->
3. Нажмите кнопку **Создать**.  

    Откроется еще одна вкладка с [!INCLUDE[prod_short](includes/prod_short.md)], на которой вы можете завершить настройку среды песочницы.

    > [!NOTE]  
    >  Если в браузере включена блокировка всплывающих окон, измените ее, чтобы разрешить URL-адреса с адреса *.businesscentral.dynamics.com.

Когда среда песочницы будет готова, вы будете перенаправлены в приветственный мастер среды песочницы.
<!-- ![Sandbox Welcome Wizard.](./media/across-sandbox/sandbox-wizard.png) -->

Нажмите кнопку **Подробнее**, чтобы прочитать о сценариях для разработчиков, которые вы можете попробовать в среде песочницы, или кнопку **Закрыть**, чтобы перейти к ролевому центру вашего экземпляр песочницы [!INCLUDE[prod_short](includes/prod_short.md)].

В верхней части ролевого центра появится уведомление о том, что это среда песочницы. Тип среды также отображается в строке заголовка клиента.
    <!-- ![Sandbox RoleCenter Notification.](./media/across-sandbox/sandbox-rolecenter-notification.png) -->

> [!NOTE]
> Созданная таким образом среда песочницы содержит только демонстрационные данные по умолчанию для компании CRONUS. Никакие данные не копируются и не переносятся каким-либо другим образом из производственной среды.
>
> В качестве альтернативы можно создать среду песочницы на основе производственных данных. Вы должны сделать это через центр администрирования. Дополнительные сведения см. в разделе [Управление средами](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments) в документации для разработчиков и администраторов.  

<!--To switch between your production and sandbox environments, you can use the Business Central app launcher.
    ![Sandbox Dynamics365 Menu.](./media/across-sandbox/sandbox-dynamics365-menu.png) -->

Администратор может ограничить или даже блокировать доступ некоторых пользователей к среде "песочницы". Это можно сделать с помощью стандартных функций безопасности для продукта, таких как карта пользователя, группы пользователей и наборы разрешений. Дополнительные сведения см. в разделе [Назначение разрешений пользователям и группам](ui-define-granular-permissions.md).  

<!-- ![Sandbox Permission Sets.](./media/across-sandbox/sandbox-permission-sets.png) -->

## <a name="advanced-functionality-in-the-sandbox-environment"></a>Расширенная функциональная возможность в среде песочницы

Среда "песочницы" не менее полезна, потому что она включает в себя несколько удобных функций:

* [Повышенное удобство работы пользователей](#advanced-user-experience)  
* [Полные демонстрационные данные](#complete-sample-data)  
* [Конструктор](#designer)  

### <a name="advanced-user-experience"></a>Повышенное удобство работы пользователей

Можно включить и попробовать полные функциональные возможности стандартной версии [!INCLUDE[prod_short](includes/prod_short.md)] в среде арендатора песочницы, задав поле **Опыт** на странице **Информация о компании** на *Premium*. Найдите страницу **Информация о компании** в :::image type="content" source="media/ui-experience/settings_icon_small.png" alt-text="Значок настроек."::: меню.  

После того как вы включили вариант настройки *Premium*, вы получаете доступ ко всем стандартным профилям (ролям) и ролевым центрам стандартной версии. Можно также создать полностью настроенную пробную организацию, включая демонстрационные данные и доступ к расширенным возможностям продукта. Кроме того, вы можете связаться с партнером по перепродаже для демонстрации возможностей. Для получения дополнительной информации прочитайте раздел [Как найти партнера по перепродаже?](across-faq.yml#how-do-i-find-a-reselling-partner).  

### <a name="complete-sample-data"></a>Полные демонстрационные данные

В ситуациях, когда вам нужны дополнительные примеры данных, обратитесь к своему партнеру по перепродаже.
<!-- In the sandbox environment, you can also create a new company with the **Advanced Evaluation - Complete Sample Data** option so that you can take training or step through walkthroughs that require additional sample data, such as [Walkthrough: Receiving and Putting Away in Basic Warehouse Configurations](walkthrough-receiving-and-putting-away-in-basic-warehousing.md).   -->

#### <a name="to-create-a-company-with-complete-sample-data-in-a-sandbox"></a>Создать компанию с полными демонстрационными данными в песочнице

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Компании**, а затем выберите связанную ссылку.  
2. Выберите действие **Создать**, а затем выберите **Создать новую компанию**.  
3. На странице **Мастер настройки по созданию компании** выберите страницу **Далее**.  
4. Укажите имя для новой компании, а затем в поле **Выбор данных и выполнение настройки для начала работы**, выберите **Расширенный ознакомительный выпуск — полные демонстрационные данные**.  
5. Выполните остальные шаги мастера настройки.  

Когда мастер настройки будет завершен, вы можете начать изучать новую компанию с полными демонстрационными данными. Дополнительную информацию см. в разделе [Создание новой организации в [!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md).  

### <a name="designer"></a>Конструктор

В среде "песочницы" включен **Конструктор**. Вы можете активировать конструктора, выбрав значок дизайна ![Конструктор.](./media/across-sandbox/sandbox-inclient-design-icon.png) на странице или выбрав пункт меню **Дизайн** в ![Параметры](media/ui-experience/settings_icon_small.png) Меню параметров.  

Для получения дополнительной информации см. [Использование конструктора](/dynamics365/business-central/dev-itpro/developer/devenv-inclient-designer) в документации разработчика и администратора (только на английском языке).  

<!-- ![In-client Designer.](./media/across-sandbox/sandbox-inclient-designer.png) -->

## <a name="see-also"></a>См. также

[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Пробные версии и подписки [!INCLUDE[prod_long](includes/prod_long.md)]](across-preview.md)  
[Управление средами в центре администрирования Business Central](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
