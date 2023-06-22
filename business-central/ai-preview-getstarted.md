---
title: Начало работы с предварительной версией Business Central для Copilot
description: 'Объясняет, как получить среду Business Central с новой возможностью искусственного интеллекта для создания текстовых предложений для описаний товаров/продуктов.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: how-to
ms.date: 03/16/2023
ms.custom: bap-template
---

# <a name="get-started-with-a-business-central-preview-version-for-copilot" />Начало работы с предварительной версией Business Central для Copilot

[!INCLUDE[ai-preview](includes/ai-preview.md)]

Вы можете попробовать создать маркетинговый текст на основе ИИ с помощью Copilot, независимо от того, являетесь ли вы существующим клиентом Business Central или потенциальным клиентом. То есть у вас просто должен быть интерес в изучении Business Central и опробовании новых возможностей. Для начала работы вам потребуется получить доступ к версии Business Central Online, которая поддерживает новую возможность. Заполните раздел ниже, который применяется к вам.

## <a name="your-organization-already-uses-business-central" />Ваша организация уже использует Business Central

Как существующему клиенту или партнеру вам потребуется администратор с правом доступа к центру администрирования Business Central для настройки среды, в которой работает предварительная версия, включающая Copilot. Как только среда будет настроена и запущена, пользователи смогут опробовать новую функцию.

Если вы являетесь администратором среды, выполните следующие действия:

1. Войдите в центр администрирования Business Central.
2. Выберите **Среды** > **Создать**.
3. На панели **Создание среды** укажите имя новой среды в поле **Имя среды**.
4. Задайте для параметра **Тип среды** значение **Песочница** или **Производственная**.
5. Установите для параметра **Страна** любую страну/регион из списка, но примите во внимание, что в предварительной версии сгенерированный ИИ маркетинговый текст из Copilot предлагается только на английском языке.
6. В поле **Версия** выберите из списка версию 22 или более позднюю версию.

   <!--
   > [!IMPORTANT]
   > You must use **22.0.54157.54311 (Preview - Copilot edition)** to experience Copilot.
   -->
7. Выберите **Создать**.  

Для получения дополнительной информации о том, как создавать среды, перейдите к разделу [Создание среды](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments#create-a-new-environment).

> [!IMPORTANT]
> Если у вас имеются песочницы предварительной версии, в которых используется версия **22.0.54157.54311 (предварительная версия — выпуск Copilot)**, обратите внимание, что эти среды будут доступны только до 1 мая 2023 года. После этой даты вам нужно будет подготовить новую среду или обновить любую из других сред до версии 22.0 или более поздней, чтобы продолжить пользоваться предварительной версией функции создания маркетингового текста на базе ИИ.

## <a name="your-organization-doesnt-use-business-central" />Ваша организация не использует Business Central

Если вы не являетесь клиентом Business Central, зарегистрируйте бесплатную пробную версию, чтобы испытать новые возможности ИИ. Зарегистрировать пробную версию очень просто. Вам будет предложено выполнить несколько шагов, где вам нужно будет предоставить определенную информацию, включая адрес электронной почты, номер телефона и имя. Чтобы получить пробную версию, выполните следующие действия:

1. Перейдите на [этот сайт пробной версии](https://go.microsoft.com/fwlink/?linkid=2227167) , чтобы начать процесс регистрации.
2. Следуйте инструкциям на экране.

   Вас попросят предоставить информацию, включая адрес электронной почты, имя и номер телефона. Точные сведения запроса могут варьироваться в зависимости от предоставленной вами информации. <!--But here are a couple important points to be aware of as you run through the sign-up process:--> В качестве адреса электронной почты используете рабочий или учебный адрес электронной почты. Мы установим вашу пробную версию в учетной записи вашей организации. Вы не можете использовать адреса электронной почты, предоставленные потребительскими службами электронной почты или поставщиками телекоммуникационных услуг, такими как outlook.com, hotmail.com, gmail.com и другими.
   
   <!-- When you get to the option for **Country or region** be sure to set this **United States**.

      > [!IMPORTANT]
      > You must set **Country or region** to **United States**; otherwise the AI-powered item marketing text with Copilot won't be available in Business Central.  -->
3. Когда вы дойдете до шага **Сведения подтверждения**, вы будете готовы начать пробную версию.

   - Чтобы перейти непосредственно в Business Central, выберите **Пропустить и перейти в Dynamics 365 Business Central** > **Начало работы**.
   - У вас также есть возможность пригласить других сотрудников вашей организации на бесплатную пробную версию. Просто введите адреса электронной почты каждого человека, а затем выберите **Отправить приглашения**. Выберите **Начать**, чтобы перейти в Business Central.  

   Вы будете перенаправлены в пробную версию в [https://businesscentral.dynamics.com/](https://businesscentral.dynamics.com/). При первом входе в систему подготовка пробной версии может занять несколько минут.

<!--
1. On the **Let's get you started** step, enter your work or school email address, then select **Next**.

   Use your work or school email address. We'll establish your trial on your organization's account. You can't use email addresses provided by consumer email services or telecommunication providers, such as outlook.com, hotmail.com, gmail.com, and others.
3. When asked what kind of email you have, select **I got it from my organization** > **Next**.
4. On the **Create your account** step, you provide information that will help use set up a trial version of Business Central that you can sign in to.

   1. Provide a telephone number that we can use to send you a verification code. Enter a country code and number that isn't VoIP or toll free.
   2. Choose how you want us to send the verification code:
      - Select **Text me** to get the verification code in a text message.
      - Select **Call me** to get the code in a voice message.
   3. Select **Send verification code**. 
   4. When you get the code, type it in the **Enter your verification code** box, then select **Verify**.

      Once you're verified, we'll send you an email with another verification code that you'll use in the next step to complete creating your account.
   5. Fill in your first and last name.
   6. Set **Country or region** to **United States**.

      > [!IMPORTANT]
      > You must set **Country or region** to **United States**; otherwise the AI-powered item marketing text with Copilot won't be available in Business Central.  

   7. Enter a valid phone umber in the **Business telephone number** box.
   8. In the **Create password** and **Confirm password** boxes, enter a password that you want to use to sign in to Business Central. The password must at least eight characters and include at least one number, an uppercase letter, and a lower case letter.
   9. In the **Verification code** box, enter the verification code we sent you in an email, then select **Next**.
   10. When you get a prompt that your account is successfully created, select **Sign in**.
-->

4. После входа в систему вы увидите домашнюю страницу Business Central, называемую ролевым центром, которая выглядит примерно так, как показано на следующем рисунке:

   [![Показывает ролевой центр Business Central и контрольный список для Copilot](media/copilot-checklist.png)](media/copilot-checklist.png#lightbox)

5. Чтобы получить пошаговое руководство по созданию маркетингового текста на базе ИИ с помощью Copilot, в разделе **Ваш контрольный список** в верхней части страницы выберите **Создать с помощью Copilot** > **Начать обзор**. Затем следуйте инструкциям на экране.

   > [!TIP]
   > Если вы не видите **Ваш контрольный список**, сначала нажмите кнопку **Показать демонстрационные обзоры** .

## <a name="next-steps" />Дальнейшие шаги

Чтобы использовать Copilot, нужно включить возможности искусственного интеллекта, предоставляемые Copilot. Чтобы включить возможности искусственного интеллекта, администратор должен согласиться с условиями [предварительной версии](https://dynamics.microsoft.com/legaldocs/supp-dynamics365-preview/) и [Заявлением о конфиденциальности Microsoft](https://go.microsoft.com/fwlink/?LinkId=521839) от имени организации.

> [!NOTE]
> Если вы используете пробную версию, вы являетесь администратором. Если вы пригласили других людей в вашей организации на пробную версию во время регистрации, они не смогут использовать Copilot, пока вы не согласитесь с условиями.

Есть два способа дать согласие в качестве администратора:

- Самый простой способ — использовать Copilot. При первом использовании Copilot в качестве администратора вам будет предложено ознакомиться с условиями, а затем согласиться или не согласиться. Чтобы узнать, как использовать Copilot, перейдите в раздел [Добавление маркетингового текста для товаров](item-marketing-text.md).  

- Другой способ — использовать страницу **Статус уведомлений о конфиденциальности** в Business Central и согласиться с **интеграцией Azure OpenAI** для всех пользователей. Чтобы узнать больше, перейдите на страницу [Согласие с условиями](enable-ai.md#consent-to-or-reject-the-preview-and-privacy-terms-and-conditions-for-all-users).

## <a name="see-also" />См. также

[Обзор функции создания маркетинговых текстов для товаров на базе ИИ с помощью Copilot](ai-overview.md)  
[Настройка создания маркетинговых текстов для товаров на базе ИИ с помощью Copilot в качестве администратора](enable-ai.md)  
[Создание маркетингового текста для товаров с помощью Copilot](item-marketing-text.md)  
[Создание маркетинговых текстов для товаров на базе ИИ с помощью Copilot: вопросы и ответы](ai-faq.md)  
