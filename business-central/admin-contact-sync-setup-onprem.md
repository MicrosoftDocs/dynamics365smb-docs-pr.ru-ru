---
title: Настройка синхронизации контактов с Outlook для локальной версии Business Central
description: 'Узнайте, как настроить локальную среду Business Central для синхронизации контактов в Business Central и Outlook.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.service: dynamics365-business-central
ms.topic: how-to
ms.date: 09/28/2023
ms.custom: bap-template
---

# <a name="set-up-contact-sync-with-outlook-for-business-central-on-premises"></a>Настройка синхронизации контактов с Outlook для локальной версии Business Central

[!INCLUDE[azure-ad-to-microsoft-entra-id](~/../shared-content/shared/azure-ad-to-microsoft-entra-id.md)]

В этой статье вы узнаете, как настроить [!INCLUDE[prod_short](includes/prod_short.md)] локальную синхронизацию контактов в [!INCLUDE[prod_short](includes/prod_short.md)] с контактами в Outlook. Дополнительную информацию об этой функции см. в разделе [Синхронизация контактов в Business Central с контактами в Microsoft Outlook](admin-synchronize-outlook-contacts.md).

## <a name="introduction"></a>Введение

Синхронизация контактов требует использования протокола OAuth 2.0 для аутентификации в Exchange Online. Ранее также поддерживалась обычная аутентификация, но она устарела и больше не поддерживается в Exchange Online. Вы можете узнать больше о прекращении поддержки в разделе [Прекращение поддержки обычной аутентификации в Exchange Online](/exchange/clients-and-mobile-in-exchange-online/deprecation-of-basic-authentication-exchange-online). Это изменение означает, что синхронизация контактов в Business Central могла перестать работать в вашей локальной среде. В этой статье объясняется, как сделать так, чтобы она стала снова работать.

## <a name="prerequisites"></a>Предварительные требования

- Exchange Online, в виде отдельной версии или в рамках плана Microsoft 365  
- Доступ к арендатору Microsoft Entra, используемому Exchange Online
- У пользователей [!INCLUDE[prod_short](includes/prod_short.md)] есть учетная запись электронной почты Microsoft 365 или Exchange Online, которая назначена их учетным записям в [!INCLUDE[prod_short](includes/prod_short.md)]. Проверить эту настройку можно в разделе **Проверка подлинности Microsoft 365** профиля пользователя в списке **Пользователи**. 

## <a name="set-up-contact-sync"></a>Настройка синхронизации контактов

Выполните следующие шаги, чтобы настроить синхронизацию контактов. Если вы используете [!INCLUDE[prod_short](includes/prod_short.md)] Spring 2019 (v.14), вам потребуется выполнить дополнительный шаг, который либо изменит код приложения, либо установит соединение с Power BI.

1. <a name="registerapp"></a>Регистрация приложения для Exchange Online API в вашем арендаторе Microsoft Entra.

   В рамках этого шага вам необходимо добавить зарегистрированное приложение в арендатор Microsoft Entra, соответствующий вашему плану Microsoft 365 или Exchange Online. Как и другим службам Azure, которые работают с Business Central, Exchange Online требуется приложение, зарегистрированное в Microsoft Entra ID. Зарегистрированное приложение предоставляет услуги аутентификации и авторизации между Business Central и Exchange Online.

   Подробные инструкции можно найти в справке для разработчиков и ИТ-специалистов, в статье [Регистрация приложения в Microsoft Entra ID](/dynamics365/business-central/dev-itpro/administration/register-app-azure#register-an-application-in-azure-active-directory). При выполнении инструкций помните о следующих аспектах:

   - Если вы уже зарегистрировали приложение в рамках интеграции с другим продуктом Майкрософт, например Power BI, то используйте это зарегистрированное приложение. В этом случае вам просто нужно настроить приложение с разрешениями Office 365 Exchange Online, описанными в следующем пункте.

   - Настройте зарегистрированное приложение со следующими делегированными разрешениями Office 365 Exchange Online для API:

     - Контакты.ReadWrite
     - EWS.AccessAsUser.All

2. Для [!INCLUDE[prod_short](includes/prod_short.md)] версии 14 выполните одну из следующих задач:

   - Измените страницу 6700, заменив `FALSE` на `TRUE` в следующей строке кода в триггере `OnPageOpen`:

     ```
     PasswordRequired := AzureADMgt.GetAccessToken(AzureADMgt.GetO365Resource,AzureADMgt.GetO365ResourceName,TRUE) = '';
     ```

   - Создайте новую страницу со следующим кодом в триггере OnPageOpen:

     ```
     PasswordRequired := AzureADMgt.GetAccessToken(AzureADMgt.GetO365Resource,AzureADMgt.GetO365ResourceName,TRUE) = '';
     ```

   - Настройте Power BI, следуя инструкциям в разделе [Настройка локальной версии Business Central для интеграции с Power BI](admin-powerbi-setup.md#setup).

   После того, как выбранное вами решение будет готово, попросите пользователей либо запустить новую/измененную страницу, либо [подключиться к Power BI](across-working-with-powerbi.md#connect). Им нужно будет выполнить этот шаг только один раз.

## <a name="next-steps"></a>Дальнейшие шаги

[Синхронизация контактов в Business Central с контактами в Microsoft Outlook](admin-synchronize-outlook-contacts.md)  
