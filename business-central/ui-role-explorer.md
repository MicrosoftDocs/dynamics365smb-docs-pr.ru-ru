---
title: Изучение и навигация по страницам и отчетам по каждой роли
description: 'Вы можете получить обзор всех бизнес-функций, доступных для вашей роли, а также для других ролей, с помощью обозревателя ролей.'
author: jswymer
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'role explorer, find features, navigate'
ms.search.form: 'RoleExplorer, 9020, 9022, 9027, 9024'
ms.date: 07/15/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---

# <a name="finding-pages-and-reports-with-the-role-explorer"></a>Поиск страниц и отчетов с помощью обозревателя ролей

Вы можете получить обзор всех бизнес-функций, доступных для вашей роли, а также для других ролей. В данной статье этот обзор функций называется *обозреватель ролей*.

Каждый элемент в обозревателе ролей представляет собой действие, которое открывает страницу или отчет. Соответственно, вы также можете использовать обозреватель ролей в качестве средства навигации по [!INCLUDE[prod_short](includes/prod_short.md)].

[!INCLUDE [about-ui-learn](includes/about-ui-learn.md)]

## <a name="open-the-role-explorer"></a>Откройте обозреватель ролей

Открыть обозреватель ролей можно из ролевого центра и со всех страниц списка, а также из окна **Что вы хотите сделать**.

- В ролевом центре или на любой странице списка выберите ![Кнопка меню.](media/ui_menu_button.png "Кнопка меню") справа от панели навигации или нажмите <kbd>Shift</kbd>+<kbd>F12</kbd>.
- В окне **Что вы хотите сделать** выберите действие под ссылкой **обозревателем ролей** в нижней части окна.

Когда вы впервые открываете ролевой центр, он показывает ссылки на большинство функций, доступных для вашей роли.

## <a name="open-the-role-explorer-filtered-to-show-reports"></a>Открытие обозревателя ролей с фильтрацией для просмотра отчетов

Открыть обозреватель ролей можно из ролевого центра в представлении, отфильтрованном для отображения отчетов из ролевого центра, со всех страниц списка, а также из окна **Что вы хотите сделать**.

- В ролевом центре или на любой странице списка выберите ссылку **Все отчеты** справа от панели навигации.
- В окне **Что вы хотите сделать** выберите действие **обозреватель ролей** в нижней части окна.

## <a name="navigate-features"></a>Функции навигации

Действия, которые открывают страницы или отчеты, организованы в виде узлов, названных по названию функций или областей приложения. Каждый узел можно свернуть или развернуть по отдельности; также можно свернуть/развернуть все узлы вместе.

- Чтобы развернуть/свернуть отдельный узел, выберите узел. Это относится к узлам верхнего уровня и подузлам.
- Чтобы развернуть/свернуть все узлы верхнего уровня на странице, но оставить подузлы такими, какие они есть, выберите **...** вверху, затем выберите **Развернуть** или **Свернуть**.
- Чтобы развернуть/свернуть все узлы верхнего уровня и подузлы под ним, выберите **...** вверху, затем выберите действие **Развернуть все** или **Свернуть все**.

## <a name="search-for-features"></a>Поиск функций

Чтобы быстро найти объекты, выберите **Найти**, затем введите слово или фразу для объекта, который вы пытаетесь найти. Ролевой центр выделит совпадающий текст, если он будет найден. Если функция скрыта, потому что находится в свернутом узле, свернутый узел помечается точкой. 

## <a name="explore-other-roles"></a>Изучите другие роли

Чтобы изучить роли, отличные от вашей, выберите **Другие роли**. В ролевом центре каждая роль отображается под отдельным заголовком со ссылками на ее функции. Вы можете находить функции и переходить к ним так же, как при изучении своей роли.

> [!NOTE]
> У вас будет доступ только к ролям, настроенным для отображения в обозревателе ролей. Если роль недоступна, возможно, она для этого не настроена. Дополнительные сведения см. в разделе [Управление профилями](admin-users-profiles-roles.md). 

При изучении других ролей вы также можете сузить область исследования, используя действия **Отчет и анализ** и **Администрирование** в верхней части ролевого центра.

- **Отчет и анализ** показывает только те функции, которые классифицируются как функции отчетов и анализа.
- **Администрирование** показывает только те функции, которые отнесены к категории функций администрирования.

> [!TIP]
> Для разработчиков вы классифицируете страницы и отчеты, устанавливая [свойство UsageCategory](/dynamics365/business-central/dev-itpro/developer/properties/devenv-usagecategory-property) в AL-коде объекта.
<!--
 
## <a name="role-explorer-actions"></a>Role explorer actions

There a several actions along the top of the role explorer to help you locate features of your role and other roles.

|Action|Description|
|------|------|
|**All**|Shows all features that are related to the role.|
|**Find**|Lets you enter a word or phrase to quickly locate feature names that match.|
|**Explore more roles**|All business features that are available for all roles including your own. When exploring all roles, the other actions work the same way, except for all roles shown. **NOTE:** You can only access roles that are set up to show in role explorer. For more information, see [Manage Profiles](admin-users-profiles-roles.md).  |
|**Report & Analysis**|This action Shows only those features that are categorized as reports and analysis features.|
|**Administration**|Shows only those features that are categorized as administration features.|



<!--
Choose the **Find** action at the top of the role explorer to quickly locate feature names that contain a certain term.

Choose the **Explore more roles** action at the top of the role explorer to get an overview of all business features that are available for all roles including your own.

> [!NOTE]
> Only Role Center actions for profiles where the **Show in Role Explorer** check box is selected will appear on the extended version of the role explorer (shown with the **Explore more roles** action). For more information, see [Manage Profiles](admin-users-profiles-roles.md).
-->

## <a name="expand-and-collapse-nodes-on-the-role-explorer"></a>Развернуть и свернуть узлы в обозревателе ролей

Действия, которые открывают страницы, организованы под узлами, названными по названию функций или областей приложения. Каждый узел можно свернуть или развернуть по отдельности, и вы можете свернуть/развернуть все узлы вместе.

- Чтобы развернуть/свернуть узел, выберите узел. Это относится к узлам верхнего уровня и подузлам.
- Чтобы развернуть/свернуть все узлы верхнего уровня на странице, выберите действие **Развернуть** или **Свернуть** в правом верхнем углу.
- Чтобы развернуть/свернуть все узлы верхнего уровня и все вложенные узлы под ним, выполните одно из следующих действий:
  - Нажимайте клавиши <kbd>Ctrl</kbd>+<kbd>Shift</kbd>, выбирая действие **Развернуть** или **Свернуть** в правом верхнем углу.
  - Выберите **...** в правом верхнем углу, затем выберите действие **Развернуть все** или **Свернуть все**.

## <a name="see-also"></a>См. также

[Поиск страниц и информации с помощью функции "Что вы хотите сделать"](ui-search.md)  
[Управление профилями](admin-users-profiles-roles.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
