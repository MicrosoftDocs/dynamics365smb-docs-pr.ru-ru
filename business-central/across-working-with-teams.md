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
ms.date: 10/08/2020
ms.author: jswymer
ms.openlocfilehash: fbe024f724f018aae6d3aeb5251281bf4c3bfbde
ms.sourcegitcommit: 4bca699d2a5ce182eb5572d72fac4fb478c4f293
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/12/2020
ms.locfileid: "3989429"
---
# <a name="working-with-business-central-data-in-microsoft-teams"></a>Работа с данными Business Central в Microsoft Teams

[!INCLUDE [teams_preview.md](includes/teams_preview.md)]

[!INCLUDE [prodshort](includes/prodshort.md)] предлагает приложение, которое соединяет Microsoft Teams с вашими бизнес-данным в [!INCLUDE [prodshort](includes/prodshort.md)], чтобы вы могли быстро обмениваться данными между участниками команды и быстрее отвечать на запросы. В этой статье вы узнаете, как использовать приложение для обмена данными [!INCLUDE [prodshort](includes/prodshort.md)] с коллегами в беседе в Teams.

## <a name="overview"></a>Обзор

Приложение позволяет [!INCLUDE [prodshort](includes/prodshort.md)]:

- Скопируйте ссылку на любую запись Business Central и вставьте ее в беседу Teams, чтобы поделиться ею с коллегами. Ссылка превратится в компактную интерактивную карточку, отображающую информацию о записи.
- После разговора вы и ваши коллеги можете просматривать дополнительные сведения о записи, редактировать данные и принимать меры — не выходя из Teams.

[![Интеграция Teams с Business Central](media/teams-intro-v3.png)](media/teams-intro-v3.png#lightbox)

## <a name="prerequisites"></a>Предварительные требования

- У вас есть доступ к Microsoft Teams.
- Вы установили приложение [!INCLUDE [prodshort](includes/prodshort.md)] в Teams. Для получения дополнительной информации см.[ Установка приложения [!INCLUDE [prodshort](includes/prodshort.md)] для Microsoft Teams](across-install-app-for-teams.md)

> [!NOTE]
> Все участники беседы Teams смогут просматривать карточки для записей Business Central, которые вы отправляете в беседу. Но чтобы просмотреть более подробную информацию о записях, используя кнопки **Подробнее** или **Открыть на новой вкладке**, им потребуется доступ [!INCLUDE [prodshort](includes/prodshort.md)]. Дополнительные сведения см. в разделе [Управление интеграцией Microsoft Teams](admin-teams-integration.md#minimum-requirements-1).
<!--
- People You and your coworkers have the following permissions in [!INCLUDE [prodshort](includes/prodshort.md)]
  - To paste a [!INCLUDE [prodshort](includes/prodshort.md)] link into a Teams conversation and have it expand into a card, you have to have at least permission to view the page and its data.
  - Once a card is submitted into a conversation, any user in that conversation can view that card without having permission to Business Central.
  - For other users to view more details from card, they must also have view permission, as a minimum, to the page and its data. If they want to change data, they'll need modify permissions.

  Setting up permissions is typically done by an administrator. For more information, see [Managing Microsoft Teams Integration](admin-teams-integration.md).-->

## <a name="include-a-business-central-card-in-a-teams-conversation"></a>Включите карточку Business Central в беседу в Teams

1. Водите в [!INCLUDE [prodshort](includes/prodshort.md)], используя ваш браузер.
2. Откройте запись, которое требуется поделиться.

    Приложение предназначено для отображения страниц типа карточек из [!INCLUDE [prodshort](includes/prodshort.md)]. Итак, откройте страницу, которая отображает одну запись, например товар, клиента или заказ на продажу. Вы не можете использовать его для центров ролей или страниц, отображающих несколько записей в списке.

3. Скопируйте весь URL-адрес из адресной строки браузера.

   ![Скопируйте URL-адрес Business Central из браузера](media/teams-url.png)
4. Перейдите в Teams и начните разговор, который может быть чатом с человеком, группой людей или групповым каналом.

    <!--Teams imposes a few limitations here eg. you cannot unfurl a link during a Voice/Video call :/ We should probably only mention this in a Troubleshooting section (and i hope it will also be fixed soon)-->
5. Вставьте URL-адрес в поле, в которое вы добавляете сообщение.

   ![Вставьте URL-адрес Business Central в Teams](media/teams-paste-url.png)
6. Когда вы впервые вставите ссылку в беседу, вам будет предложено войти в [!INCLUDE [prodshort](includes/prodshort.md)] и дать согласие на получение данных приложением. Просто следуйте инструкциям на экране.

    > [!NOTE]
    > Вам нужно выполнить этот шаг только один раз.

7. Подождите, пока в окне сообщения появится карточка.

8. Когда карточка появится, внимательно проверьте содержимое карточки на наличие конфиденциальной информации перед отправкой сообщения. Этот шаг важен, потому что как только вы отправите сообщение, все участники беседы смогут увидеть карточку.

9. Если карточка выглядит хорошо, выберите **Отправить**, чтобы отправить ее в беседу.

    > [!TIP]
    > После появления карточки и до того, как вы выберете **Отправить**, вы можете удалить вставленный URL-адрес, если хотите.

10. Чтобы просмотреть дополнительные сведения или внести изменения в запись, выберите **Подробнее**.

    Страница сведений похожа на то, что вы бы видели в [!INCLUDE [prodshort](includes/prodshort.md)]. Но для Teams версия немного урезана. Когда вы закончите просмотр и внесите изменения, закройте окно, чтобы вернуться к беседе Teams.

    > [!NOTE]
    > Любые внесенные вами изменения не будут отражены в карточке до тех пор, пока вы в следующий раз не вставите ссылку на нее в беседу.

## <a name="see-also"></a>См. также

[Обзор интеграции Business Central и Microsoft Teams](across-teams-overview.md)  
[Установите приложение [!INCLUDE [prodshort](includes/prodshort.md)] для Microsoft Teams](across-install-app-for-teams.md)  
[Разработка для интеграции Teams](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  
[Приступая к работе](product-get-started.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
