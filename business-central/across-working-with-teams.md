---
title: Совместное использование записей Business Central в Microsoft Teams
description: Узнайте, как использовать приложение Business Central для Microsoft Teams.
author: jswymer
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork, share records
ms.date: 05/19/2021
ms.author: jswymer
ms.openlocfilehash: 4d8ca98d4e13d50bcf58f4a66956c33b1d0996f3
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "8147116"
---
# <a name="sharing-business-central-records-and-page-links-in-microsoft-teams"></a>Совместное использование записей Business Central и ссылок на страницы в Microsoft Teams

[!INCLUDE [online_only](includes/online_only.md)]

[!INCLUDE [prod_short](includes/prod_short.md)] дает несколько способов обмена данными из Business Central непосредственно в беседе Microsoft Teams:

<!-- 
## Overview
In this article, you'll learn how to use the app to share [!INCLUDE [prod_short](includes/prod_short.md)] records, like a customer, sales order, or invoice, with coworkers in a Teams conversation.
The [!INCLUDE [prod_short](includes/prod_short.md)] app lets you:
[!INCLUDE [prod_short](includes/prod_short.md)] offers an app that connects Microsoft Teams to your business data in [!INCLUDE [prod_short](includes/prod_short.md)], so you can quickly share details across team members and respond faster to inquiries. In this article, you'll learn how to use the app to share [!INCLUDE [prod_short](includes/prod_short.md)] records, like a customer, sales order, or invoice, with coworkers in a Teams conversation.

-->
- С помощью приложения [!INCLUDE [prod_short](includes/prod_short.md)], установленного в Teams, вы можете включить интерактивную карточку записи Business Central в беседу Teams.

<!--   Copy a link from any Business Central record, like a customer or sales order, then paste the link into a Teams conversation. The app connects Microsoft Teams to your business data in [!INCLUDE [prod_short](includes/prod_short.md)]. It then expands the link into a compact, interactive card that displays information about the record. Once in the conversation, you and coworkers can view more details about the record, edit data, and take action&mdash;without leaving Teams.

  [![Teams integration with Business Central.](media/teams-intro-v3.png)](media/teams-intro-v3.png#lightbox)-->

- С установленным приложением или без него [!INCLUDE [prod_short](includes/prod_short.md)] вы можете поделиться ссылкой со страниц в Business Central в беседе в Teams.

  <!-- ![!The Share menu displayed on a card.](media/teams-share-link.png "The Share menu displayed on a card.")-->

В следующих разделах подробно описано, как использовать различные способы.

## <a name="include-and-view-a-business-central-card-in-a-teams-conversation"></a>Включите и просмотрите карточку Business Central в беседу в Teams

С помощью приложения Business Central для Teams вы можете скопировать ссылку из любой записи Business Central, например клиента или заказа на продажу, и вставить ссылку в беседу Teams. Приложение подключает Microsoft Teams к вашим бизнес-данным в [!INCLUDE [prod_short](includes/prod_short.md)]\. Затем оно разворачивает ссылку превратится в компактную интерактивную карточку, отображающую информацию о записи. После разговора вы и ваши коллеги можете просматривать дополнительные сведения о записи, редактировать данные и принимать меры &mdash; не выходя из Teams.

[![Интеграция Teams с Business Central.](media/teams-intro-v3.png)](media/teams-intro-v3.png#lightbox)

### <a name="prerequisites"></a>Предварительные требования

- У вас есть доступ к Microsoft Teams.
- Вы установили приложение [!INCLUDE [prod_short](includes/prod_short.md)] в Teams. Для получения дополнительной информации см.[ Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)

> [!NOTE]
> Все участники беседы Teams смогут просматривать карточки для записей Business Central, которые вы отправляете в беседу. Но чтобы просмотреть более подробную информацию о записях, используя кнопки **Подробнее** или **Открыть на новой вкладке**, им потребуется доступ [!INCLUDE [prod_short](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Управление интеграцией Microsoft Teams](admin-teams-integration.md#minimum-requirements-1).

### <a name="include-a-business-central-card-in-a-teams-conversation"></a>Включите карточку Business Central в беседу в Teams

1. Водите в [!INCLUDE [prod_short](includes/prod_short.md)], используя ваш браузер.
2. Откройте запись, которое требуется поделиться.

    Приложение предназначено для отображения страниц типа карточек из [!INCLUDE [prod_short](includes/prod_short.md)]\. Итак, откройте страницу, которая отображает одну запись, например товар, клиента или заказ на продажу. Вы не можете использовать его для центров ролей или страниц, отображающих несколько записей в списке.

3. Скопируйте весь URL-адрес из адресной строки браузера.

   ![Скопируйте URL-адрес Business Central из браузера.](media/teams-url-v2.png)
4. Перейдите в Teams и начните разговор, который может быть чатом с человеком, группой людей или групповым каналом.

    <!--Teams imposes a few limitations here eg. you cannot unfurl a link during a Voice/Video call :/ We should probably only mention this in a Troubleshooting section (and i hope it will also be fixed soon)-->
5. Вставьте URL-адрес в поле сообщение, в которое вы составляете сообщение.

   ![Вставьте URL-адрес Business Central в Teams.](media/teams-paste-url-v2.png)
6. Когда вы впервые вставите ссылку в беседу, вам будет предложено войти в [!INCLUDE [prod_short](includes/prod_short.md)] и дать согласие на получение данных приложением. Просто следуйте инструкциям на экране.

    > [!NOTE]
    > Вам нужно выполнить этот шаг только один раз.

7. Подождите, пока в окне сообщения появится карточка.

8. Когда карточка появится, внимательно проверьте содержимое карточки на наличие конфиденциальной информации перед отправкой сообщения. Этот шаг важен, потому что как только вы отправите сообщение, все участники беседы смогут увидеть карточку.

9. Если карточка выглядит хорошо, выберите **Отправить**, чтобы отправить ее в беседу.

    > [!TIP]
    > После появления карточки и до того, как вы выберете **Отправить**, вы можете удалить вставленный URL-адрес, если хотите.

10. Чтобы просмотреть дополнительные сведения или внести изменения в запись, отображаемую на карточке, выберите **Подробнее**. Дополнительные сведения см. в следующем разделе.

### <a name="view-card-details"></a>Просмотр сведений карточки

После отправки карточки в беседу все участники с [надлежащими разрешениями](admin-teams-integration.md#permissions) могут выбрать **Детали**, чтобы открыть окно, в котором отображается дополнительная информация о записи &mdash; и, возможно, внести изменения в запись. Неважно, отправляете ли вы карточку или получаете ее. Функция **Детали** особенно полезна для получателей, поскольку она быстро предоставляет им краткую и целевую информацию о записи, в отличие от необходимости сканировать всю запись.

Окно сведений похоже на то, что вы бы видели в записи [!INCLUDE [prod_short](includes/prod_short.md)]. Но для Teams версия немного урезана. Когда вы закончите просмотр и внесите изменения, закройте окно, чтобы вернуться к беседе Teams.

При работе с данными карточки следует помнить о нескольких вещах:

- Чтобы открыть сведения о карточке, пользователи должны иметь разрешение на странице и ее данных в [!INCLUDE [prod_short](includes/prod_short.md)]\.
- Карточки в чатах Teams не обновляются автоматически при внесении изменений. Любые изменения, которые вы сохраняете в записи в окне сведений, сохраняются в [!INCLUDE [prod_short](includes/prod_short.md)]\. Но карточка в Teams не будет отображать изменения в преобразовании, пока вы снова не вставите ссылку.

Подробнее о работе с карточками и сведениях о карточках см. в разделе [Вопросы и ответы по Teams](teams-faq.md).

## <a name="share-a-link-to-page-from-business-central-to-teams"></a><a name="share-link"></a>Делитесь ссылкой на страницу в Business Central в Teams

Непосредственно с большинства страниц коллекций, таких как страница **Товары**, и страниц сведений, например карточка **Товары**, вы можете отправить ссылку на страницу определенным получателям в беседе Teams. Например, вы можете поделиться ссылкой на отфильтрованный просмотр ваших записей. Затем получатели могут выбрать ссылку, чтобы открыть страницу в [!INCLUDE [prod_short](includes/prod_short.md)]\.

 ![!Меню Поделиться отображается на карточке.](media/teams-share-link.png "Меню Поделиться отображается на карточке.")

### <a name="prerequisites"></a>Предварительные требования
У вас есть доступ к Microsoft Teams.

### <a name="share-a-link"></a>Поделитесь ссылкой

1. В [!INCLUDE [prod_short](includes/prod_short.md)]\, откройте страницу, которой требуется поделиться.
2. Вверху страницы выберите ![!Действие Поделиться с другими приложениями на страницах.](media/share-icon.png) затем **Поделиться в Teams**.
3. Если вас попросят, войдите в Teams со своим именем пользователя и паролем.
4. На странице **Отправка данных в Teams** введите имя человека, группы или канала, куда вы хотите отправить сообщение. 
5. В окне сообщения будет ссылка на страницу. Добавьте дополнительную информацию, если хотите, затем выберите **Поделиться**.
6. Ссылка отправлена. Если вы хотите перейти к беседе, выберите **Перейти в Teams**.

## <a name="see-also"></a>См. также

[Обзор интеграции Business Central и Microsoft Teams](across-teams-overview.md)  
[Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)  
[Вопросы и ответы по Teams](teams-faq.md)  
[Поиск клиентов, поставщиков и других контактов из Microsoft Teams](across-search-contacts-teams.md)  
[Изменение компании и других параметров в Teams](across-teams-settings.md)  
[Устранение неполадок Teams](admin-teams-troubleshooting.md)  
[Разработка для интеграции Teams](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]