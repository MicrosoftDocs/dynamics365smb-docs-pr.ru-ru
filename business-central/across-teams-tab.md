---
title: Добавление вкладки Business Central в Microsoft Teams
description: 'Узнайте, как добавлять в Teams вкладки, на которых будут отображаться страницы Business Central.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.service: dynamics365-business-central
ms.topic: how-to
ms.date: 12/12/2023
ms.custom: bap-template
ms.search.keywords: 'Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork, share records, tab'
---

# <a name="add-business-central-tab-in-microsoft-teams"></a>Добавление вкладки Business Central в Microsoft Teams

[!INCLUDE [online_only](includes/online_only.md)]

В Teams вкладки находятся вверху каналов и чатов, что позволяет участникам быстро получать доступ к соответствующей информации. В этой статье рассматриваются различные способы добавления вкладки, на которой будут отображаться данные из [!INCLUDE [prod_short](includes/prod_short.md)].

![Вкладки в Teams](media/teams-tabs-border.png)

## <a name="about-business-central-tabs"></a>О вкладках Business Central

На вкладке [!INCLUDE [prod_short](includes/prod_short.md)] содержится компактное представление страниц-списков и страниц-карточек [!INCLUDE [prod_short](includes/prod_short.md)]. На вкладке не отображается весь веб-клиент [!INCLUDE [prod_short](includes/prod_short.md)]. На ней нет границы браузера, баннера [!INCLUDE [prod_short](includes/prod_short.md)] (например, с функцией "Что вы хотите сделать", поиском и справкой) или верхнего меню навигации &mdash; только содержимое страницы и связанные с ним действия. Содержимое интерактивно, то есть вы можете выбирать действия и ссылки, изменять данные и многое другое. То, что вы видите и то, что вы можете делать, ограничивается разрешениями, назначенными вашей учетной записи в [!INCLUDE [prod_short](includes/prod_short.md)].

Узнать, кто может просматривать содержимое в [!INCLUDE [prod_short](includes/prod_short.md)], можно в разделе [Кто может видеть содержимое вкладки?](/dynamics365/business-central/teams-faq?tabs=tabs#who-can-view).

> [!TIP]
> Вы разработчик? Вы также можете добавлять вкладки программно с помощью API Microsoft Graph. Дополнительные сведения см. в статье [Добавление вкладок Business Central в Teams](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams-tabs).  

## <a name="prerequisites"></a>Предварительные требования

Для добавления вкладки [!INCLUDE [prod_short](includes/prod_short.md)] должны быть соблюдены следующие требования:

- У вас есть доступ к Microsoft Teams.
- У вас есть лицензия [!INCLUDE [prod_short](includes/prod_short.md)].
- Вы установили приложение [!INCLUDE [prod_short](includes/prod_short.md)] в Teams. Дополнительные сведения см. в статье [ Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md).

Для просмотра вкладки [!INCLUDE [prod_short](includes/prod_short.md)], которую добавил другой участник канала или чата, должны быть соблюдены следующие требования:

- У вас есть доступ к Microsoft Teams.
- У вас есть лицензия [!INCLUDE [prod_short](includes/prod_short.md)] или ограниченный доступ к Business Central с лицензией только на Microsoft 365. Дополнительные сведения см. в статье [Доступ к Business Central с лицензиями на Microsoft 365](admin-access-with-m365-license.md).
- Вы установили приложение [!INCLUDE [prod_short](includes/prod_short.md)] в Teams.

## <a name="add-tab-using-recommended-content"></a>Добавление вкладки с рекомендуемым содержимым

Следуя инструкциям ниже, вы можете добавить вкладку, выбрав, что должно на ней отображаться, из готового списка рекомендуемого содержимого на основе вашего ролевого центра &mdash; не выходя из Teams. Подробнее о предлагаемом на выбор содержимом см. в статье [Откуда берется рекомендуемое содержимое?](/dynamics365/business-central/teams-faq?tabs=tabs#where-does-the-recommended-content-come-from).

1. В верхней части канала или чата в Teams выберите **+ Добавить вкладку**.
2. В поле **Поиск** введите *business central*, затем выберите значок **[!INCLUDE [prod_short](includes/prod_short.md)]** и дождитесь появления окна настройки вкладки [!INCLUDE [prod_short](includes/prod_short.md)].

   ![Показано окно настройки вкладки Business Central в Teams](media/teams-bc-tab-config-window.png)

3. Рядом с пунктом **Выберите что-либо содержимого, рекомендуемого для** показана организация [!INCLUDE [prod_short](includes/prod_short.md)], с которой вы работаете. Если вы хотите показать содержимое из другой организации, выберите текущую организацию, а затем с помощью параметров **Среда** и **Организация** укажите организацию, с которой вы хотите работать.
4. Выберите стрелку вниз в пункте **Содержимое вкладки** и выберите содержимое, которое вы хотите отобразить.

   <!-- The list shows all pages that are bookmarked on your role center in [!INCLUDE [prod_short](includes/prod_short.md)]. To learn more about the content that you can choose from, see [Where does the recommended content come from?](teams-faq.md#recommended-content).-->
5. Некоторые страницы могут включать разные представления — варианты страницы, отфильтрованные для отображения конкретных данных. Чтобы изменить представление содержимого, выберите стрелку вниз в пункте **Предпочтительное представление** и выберите представление из списка.

   Дополнительные сведения о представлениях см. в статье [Сохранение и персонализация представлений](ui-views.md).
6. Выберите **Опубликовать в канале объявление об этой вкладке**, чтобы автоматически опубликовать в канале или чате Teams объявление для его участников о том, что вы добавили эту вкладку.
7. Нажмите **Сохранить**.

## <a name="add-tab-using-a-page-link"></a>Добавление вкладки с использованием ссылки на страницу

Другой способ добавить вкладку — это использовать ссылку (URL-адрес) на страницу, которую вы хотите отображать. Этим способом удобно пользоваться, когда вы хотите отобразить определенную запись [!INCLUDE [prod_short](includes/prod_short.md)] или страницу-список, которая не отмечена закладкой в вашем ролевом центре.

1. В верхней части канала или чата в Teams выберите **+ Добавить вкладку**.
2. В поле **Поиск** введите *business central*, затем выберите значок  **[!INCLUDE [prod_short](includes/prod_short.md)]**.
3. Дождитесь появления окна настройки вкладки [!INCLUDE [prod_short](includes/prod_short.md)], затем выберите вариант **Вставить ссылку на [!INCLUDE [prod_short](includes/prod_short.md)]**.

   ![Показано окно настройки вкладки Business Central в Teams с выделенным вариантом со ссылкой](media/teams-bc-tab-config-window-page-link.png)
4. Перейдите в [!INCLUDE [prod_short](includes/prod_short.md)] и откройте страницу, которую вы хотите отобразить на вкладке.
5. Скопируйте ссылку на страницу.

   Существуют два способа копирования ссылки. Самый простой и предпочтительный способ — выбрать **Поделиться** ![Значок Поделиться в Business Central](media/share-icon.png) > **Копировать ссылку**. Другой способ — скопировать весь URL-адрес из адресной строки браузера. Подробнее о том, как это сделать, см. в статье [Совместное использование записей Business Central и ссылок на страницы](across-working-with-teams.md).

6. Вернитесь в Teams и вставьте ссылку в поле **URL-адрес**.
7. В поле **Имя вкладки** введите название, которое будет отображаться на вкладке.
8. Выберите **Опубликовать в канале объявление об этой вкладке**, чтобы автоматически опубликовать в канале или чате Teams объявление для его участников о том, что вы добавили эту вкладку.
9. Нажмите **Сохранить**.

## <a name="add-tab-by-pinning-card-details"></a>Добавление вкладки путем закрепления подробностей карточки

Следуя этим инструкциям, вы сможете добавить вкладку для записи, которая была опубликована или вставлена в канал или чат Teams. Чтобы узнать, как делиться записями и ссылками на страницы в Teams, см. статью [Совместное использование записей Business Central и ссылок на страницы в Teams](across-working-with-teams.md).

1. В Teams выберите кнопку **Подробности** на карточке.
2. В правом верхнем углу подробностей карточки выберите значок **Закрепить наверху чата** ![Значок булавки для добавления вкладки Teams в Business Central](media/pin-teams.png).

## <a name="change-a-tab-and-its-content"></a>Изменение вкладки и ее содержимого

После добавления вкладки вы можете внести в нее определенные изменения. Например, вы можете переименовать вкладку, переместить ее и удалить. Вы найдете эти действия в параметрах вкладки, которые доступны, если выбрать стрелку вниз на вкладке.

![Показано окно настройки вкладки Business Central в Teams и меню параметров вкладки](media/teams-bc-tab-config-window-options.png)

Что касается содержимого вкладки, вы можете изменить данные, если у вас есть разрешение. Если вы измените данные, другие пользователи не увидят изменений, пока не уйдут с вкладки и не вернутся на нее. Это справедливо и в вашем отношении, если кто-то другой внесет изменения в данные. Изменить отображаемую на вкладке страницу нельзя, поэтому просто удалите вкладку и добавьте новую.

Вы также можете изменять представление страницы и данных на ней, например сортировать данные и переключаться между представлениями списка и плиток. Такие изменения не влияют на то, что видят другие пользователи. Они будут видеть то, что вы изначально опубликовали, пока сами не внесут аналогичные изменения.

## <a name="see-also"></a>См. также

[Обзор интеграции Business Central и Microsoft Teams](across-teams-overview.md)  
[Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)  
[Совместное использование записей Business Central и ссылок на страницы в Microsoft Teams](across-working-with-teams.md).
[Вопросы и ответы по Teams](teams-faq.md)  
[Поиск клиентов, поставщиков и других контактов из Microsoft Teams](across-search-contacts-teams.md)  
[Изменение компании и других параметров в Teams](across-teams-settings.md)  
[Устранение неполадок Teams](admin-teams-troubleshooting.md)  
[Разработка для интеграции Teams](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
