---
title: Работа с данными Business Central в Microsoft Teams | Документация Майкрософт
description: Узнайте, как использовать приложение Business Central для Microsoft Teams.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork
ms.date: 01/20/2021
ms.author: jswymer
ms.openlocfilehash: cbb505865e061bfa8017699a2127206bb25f91b4
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5381985"
---
# <a name="working-with-business-central-data-in-microsoft-teams"></a>Работа с данными Business Central в Microsoft Teams

[!INCLUDE [online_only](includes/online_only.md)]

[!INCLUDE [prod_short](includes/prod_short.md)] предлагает приложение, которое соединяет Microsoft Teams с вашими бизнес-данным в [!INCLUDE [prod_short](includes/prod_short.md)], чтобы вы могли быстро обмениваться данными между участниками команды и быстрее отвечать на запросы. В этой статье вы узнаете, как использовать приложение для обмена данными [!INCLUDE [prod_short](includes/prod_short.md)] с коллегами в беседе в Teams.

## <a name="overview"></a>Обзор

Приложение позволяет [!INCLUDE [prod_short](includes/prod_short.md)]:

- Скопируйте ссылку на любую запись Business Central и вставьте ее в беседу Teams, чтобы поделиться ею с коллегами. Приложение затем развернет ссылку в компактную интерактивную карточку, отображающую информацию о записи.
- После разговора вы и ваши коллеги можете просматривать дополнительные сведения о записи, редактировать данные и принимать меры &mdash; не выходя из Teams.

[![Интеграция Teams с Business Central](media/teams-intro-v3.png)](media/teams-intro-v3.png#lightbox)

## <a name="prerequisites"></a>Предварительные требования

- У вас есть доступ к Microsoft Teams.
- Вы установили приложение [!INCLUDE [prod_short](includes/prod_short.md)] в Teams. Для получения дополнительной информации см.[ Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)

> [!NOTE]
> Все участники беседы Teams смогут просматривать карточки для записей Business Central, которые вы отправляете в беседу. Но чтобы просмотреть более подробную информацию о записях, используя кнопки **Подробнее** или **Открыть на новой вкладке**, им потребуется доступ [!INCLUDE [prod_short](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Управление интеграцией Microsoft Teams](admin-teams-integration.md#minimum-requirements-1).

## <a name="include-a-business-central-card-in-a-teams-conversation"></a>Включите карточку Business Central в беседу в Teams

1. Водите в [!INCLUDE [prod_short](includes/prod_short.md)], используя ваш браузер.
2. Откройте запись, которое требуется поделиться.

    Приложение предназначено для отображения страниц типа карточек из [!INCLUDE [prod_short](includes/prod_short.md)]. Итак, откройте страницу, которая отображает одну запись, например товар, клиента или заказ на продажу. Вы не можете использовать его для центров ролей или страниц, отображающих несколько записей в списке.

3. Скопируйте весь URL-адрес из адресной строки браузера.

   ![Скопируйте URL-адрес Business Central из браузера](media/teams-url-v2.png)
4. Перейдите в Teams и начните разговор, который может быть чатом с человеком, группой людей или групповым каналом.

    <!--Teams imposes a few limitations here eg. you cannot unfurl a link during a Voice/Video call :/ We should probably only mention this in a Troubleshooting section (and i hope it will also be fixed soon)-->
5. Вставьте URL-адрес в поле сообщение, в которое вы составляете сообщение.

   ![Вставьте URL-адрес Business Central в Teams](media/teams-paste-url-v2.png)
6. Когда вы впервые вставите ссылку в беседу, вам будет предложено войти в [!INCLUDE [prod_short](includes/prod_short.md)] и дать согласие на получение данных приложением. Просто следуйте инструкциям на экране.

    > [!NOTE]
    > Вам нужно выполнить этот шаг только один раз.

7. Подождите, пока в окне сообщения появится карточка.

8. Когда карточка появится, внимательно проверьте содержимое карточки на наличие конфиденциальной информации перед отправкой сообщения. Этот шаг важен, потому что как только вы отправите сообщение, все участники беседы смогут увидеть карточку.

9. Если карточка выглядит хорошо, выберите **Отправить**, чтобы отправить ее в беседу.

    > [!TIP]
    > После появления карточки и до того, как вы выберете **Отправить**, вы можете удалить вставленный URL-адрес, если хотите.

10. Чтобы просмотреть дополнительные сведения или внести изменения в запись, отображаемую на карточке, выберите **Подробнее**. Дополнительные сведения см. в следующем разделе.

## <a name="view-card-details"></a>Просмотр сведений карточки

После отправки карточки в беседу все участники с [надлежащими разрешениями](admin-teams-integration.md#permissions) могут выбрать **Детали**, чтобы открыть окно, в котором отображается дополнительная информация о записи &mdash; и, возможно, внести изменения в запись. Неважно, отправляете ли вы карточку или получаете ее. Функция **Детали** особенно полезна для получателей, поскольку она быстро предоставляет им краткую и целевую информацию о записи, в отличие от необходимости сканировать всю запись.

Окно сведений похоже на то, что вы бы видели в записи [!INCLUDE [prod_short](includes/prod_short.md)]. Но для Teams версия немного урезана. Когда вы закончите просмотр и внесите изменения, закройте окно, чтобы вернуться к беседе Teams.

При работе с данными карточки следует помнить о нескольких вещах:

- Чтобы открыть сведения о карточке, пользователи должны иметь разрешение на странице и ее данных в [!INCLUDE [prod_short](includes/prod_short.md)].
- Карточки в чатах Teams не обновляются автоматически при внесении изменений. Любые изменения, которые вы сохраняете в записи в окне сведений, сохраняются в [!INCLUDE [prod_short](includes/prod_short.md)]. Но карточка в Teams не будет отображать изменения в преобразовании, пока вы снова не вставите ссылку.

Подробнее о работе с карточками и сведениях о карточках см. в разделе [Вопросы и ответы по Teams](teams-faq.md).

## <a name="see-also"></a>См. также

[Обзор интеграции Business Central и Microsoft Teams](across-teams-overview.md)  
[Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)  
[Вопросы и ответы по Teams](teams-faq.md)  
[Устранение неполадок Teams](admin-teams-troubleshooting.md)  
[Разработка для интеграции Teams](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]