---
title: Управление доступом к Business Central
description: Администраторы используют многоуровневый подход к управлению доступом к Business Central и возможностям системы.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: jswymer
ms.topic: overview
ms.date: 04/04/2023
ms.custom: bap-template
---

# <a name="manage-access-to-business-central"></a>Управление доступом к Business Central

[!INCLUDE[azure-ad-to-microsoft-entra-id](~/../shared-content/shared/azure-ad-to-microsoft-entra-id.md)]

В этой статье содержится ориентированный на администраторов и разработчикам приложений общий обзор того, как управлять доступом к [!INCLUDE [prod_short](includes/prod_short.md)] и возможностям системы. Используйте ссылки для перехода к другим статьям, которые содержат более подробную информацию по конкретным темам.

## <a name="layered-access"></a>Многоуровневый доступ

В [!INCLUDE [prod_short](includes/prod_short.md)] используется многоуровневый подход к безопасности приложений, как показано на следующей схеме. Подробнее о каждом уровне см. в статье [Безопасность приложений в Business Central](/dynamics365/business-central/dev-itpro/security/security-application).

:::image type="content" source="media/security-overview.png" alt-text="Многоуровневая безопасность приложений в Business Central.":::

## <a name="licenses"></a>Лицензии

Пользователям [!INCLUDE [prod_short](includes/prod_short.md)] назначается лицензия на **Dynamics 365 Business Central**, чтобы они могли просматривать и изменять свои бизнес-данные, а также выполнять действия с ними из любого пользовательского интерфейса. Подробнее о каждом уровне см. в статье [Лицензирование в Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/deployment/licensing).

Тем не менее, люди, которым требуется эпизодический доступ только на чтение к информации в [!INCLUDE [prod_short](includes/prod_short.md)] , могут использовать лицензию на **Microsoft 365**. Подробнее о предоставлении временного доступа см. в статье [Доступ к Business Central Access с лицензиями на Microsoft 365](admin-access-with-m365-license.md).

Для получения исчерпывающих сведений о различных типах лицензий и о том, как работает лицензирование в [!INCLUDE[prod_short](includes/prod_short.md)], [загрузите Руководство по лицензированию Dynamics 365](https://go.microsoft.com/fwlink/?LinkId=866544).

## <a name="business-central-administrator-tasks"></a>Задачи администратора Business Central

В следующей таблице указано, как администраторы могут управлять доступом к [!INCLUDE [prod_short](includes/prod_short.md)] и функциям, которые будут использовать пользователи. Некоторые из задач также помогают поддерживать настройки доступа в актуальном состоянии.

|Задача| Узнать больше |
|--|--|--|
|У каждого человека должна быть учетная запись пользователя, прежде чем он сможет войти в [!INCLUDE [prod_short](includes/prod_short.md)]. Самый простой способ создания пользователей — добавлять их по одному в [центре администрирования Microsoft 365](https://go.microsoft.com/fwlink/p/?linkid=2024339). |[Одновременное добавление пользователей и назначение лицензий](/microsoft-365/admin/add-users/add-users)|
|Управление доступом для всех пользователей на уровне среды. Создайте группу безопасности Microsoft Entra и назначьте ее среде.<br><br> Вы также можете использовать группы безопасности для управления доступом для определенных групп пользователей. | [Управление доступом к средам ](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-manage-access)<br><br>[Управление доступом к Business Central с помощью групп безопасности](ui-security-groups.md) |
|Создайте пользователей в [!INCLUDE [prod_short](includes/prod_short.md)] и определите, кто может входить в систему. | [Создание пользователей в соответствии с лицензиями](ui-how-users-permissions.md) |
|В сочетании с лицензиями пользователей разрешения определяют, к каким объектам пользователь может получить доступ в каждой базе данных или среде. Укажите, могут ли пользователи читать, изменять или вводить данные в объекты базы данных. |[Назначение разрешений пользователям и группам](ui-define-granular-permissions.md)|
|Если вашу бухгалтерию и финансовую отчетность ведет внешний бухгалтер, пригласите его в [!INCLUDE [prod_short](includes/prod_short.md)]. Так он сможет эффективнее работать с вашими финансовыми данными.|[Работа бухгалтера в [!INCLUDE[prod_long](includes/prod_long.md)]](finance-accounting.md)|
|Если вы являетесь партнером-реселлером по [!INCLUDE [prod_short](includes/prod_short.md)] , вы можете отправить клиенту сообщение электронной почты с запросом на сотрудничество с вами в качестве реселлера. Вы можете включить в сообщение электронной почты делегированные административные права в отношении Microsoft Entra ID и Microsoft 365.| [Делегированный доступ администратора к Business Central Online](/dynamics365/business-central/dev-itpro/administration/delegated-admin)|
|Тег службы Azure представляет группу IP-адресов, с которых может поступать или на которые может уходить трафик для службы. Используйте теги службы, чтобы настроить брандмауэры так, чтобы они пропускали трафик только от определенных служб. Тег **Dynamics365BusinessCentral** позволяет использовать правила брандмауэра и группы безопасности сети для ограничения входящего и исходящего трафика [!INCLUDE [prod_short](includes/prod_short.md)].| [Теги безопасности служб Azure](/dynamics365/business-central/dev-itpro/security/security-service-tags)|
|При использовании проверки подлинности Microsoft Entra в сочетании с [!INCLUDE [prod_short](includes/prod_short.md)] рекомендуется использовать [многофакторную проверку подлинности (MFA) Microsoft Entra ID](/azure/active-directory/authentication/concept-mfa-howitworks). MFA обеспечивает дополнительный контроль доступа к приложению и данным.|[Многофакторная проверка подлинности для Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/security/multifactor-authentication)|

## <a name="business-central-developer-tasks"></a>Задачи разработчика Business Central

Иметь дело с управлением доступом к [!INCLUDE [prod_short](includes/prod_short.md)] приходится также разработчикам. Например, разработчики и администраторы могут создавать и подключать к приложения [!INCLUDE [prod_short](includes/prod_short.md)], которые приносят пользу бизнесу:  

* Упрощают бизнес-процессы
* Улучшают взаимодействие с клиентами
* Позволяют принимать решения быстрее и эффективнее

В следующей таблице приведены ссылки на информацию о том, как предоставлять приложениям и расширениям доступ к данным [!INCLUDE [prod_short](includes/prod_short.md)].

| Задача | Узнать больше |
|--|--|
|С определением доступа к функциям связаны два основных понятия: права и разрешения. Права дают широкий доступ к объектам в соответствии с лицензиями или ролями Microsoft Entra. Разрешения и наборы разрешений позволяют точно настраивать доступ к объектам. |[Обзор прав и наборов разрешений](/dynamics365/business-central/dev-itpro/developer/devenv-entitlements-and-permissionsets-overview)|

## <a name="see-also"></a>См. также

[Безопасность в Business Central](/dynamics365/business-central/dev-itpro/security/security-and-protection)
