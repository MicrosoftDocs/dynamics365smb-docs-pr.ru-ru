---
title: Настройка возможностей Copilot и ИИ
description: 'В этой статье объясняется, как включить Copilot в среде.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: how-to
ms.date: 02/27/2024
ms.custom: bap-template
ms.search.form: 7775
ms.collection:
  - bap-ai-copilot
---

# Настройка возможностей Copilot и ИИ 

<!--[!INCLUDE[ai-preview](includes/ai-preview.md)]-->

<!--This article explains how you can control the ability to create AI-powered item marketing text with Copilot for your organization. This task is done by an admin. There are two requirements that you must fulfill to make the feature available to users:-->

В этой статье рассматривается, как управлять Copilot и другими возможностями ИИ в Business Central. Эту задачу выполняет администратор. Copilot — это системная функция и неотъемлемая часть Business Central. Как и в случае с большинством системных функций, вы не предоставляете доступ отдельным пользователям и не можете включить или отключить Copilot. Однако в Copilot предусмотрены элементы управления данными и возможность деактивации отдельных возможностей Copilot и ИИ для каждой среды. Существуют разные уровни управления доступом к возможностям ИИ, в зависимости от функции:

- Разрешение на перемещение данных между географическими регионами.

  Эта задача требуется только в том случае, если ваша среда Business Central находится в другой географии, чем используемая ею служба Azure OpenAI. [Подробнее](#allow-data-movement-across-geographies)

- Активируйте эту функцию на странице **Возможности Copilot и ИИ**. [Подробнее](#activate-features)

<!-- For 2024 there are no AI features governed by **Feature Management**, so this section is not shown
- Enable the specific feature if it's governed by **Feature Management**.

  Check whether  of 2024 release wave 1, chat with Copilot, marketing text suggestions, and bank account reconciliation assist features are included under **Feature Management**. [Learn more](#enable-feature-in-feature-management)
<!-- 
- Enable the specific feature, if it's still governed by **Feature Management**.

  In 2023 release wave 2, both the marketing text suggestions and bank account reconciliation assist features are included under **Feature Management**. [Learn more](#enable-feature-in-feature-management)-->

Если какие-либо из этих требований не выполняются, функция недоступна для использования.-->

## Предварительные требования

- Вы используете Business Central Online <!--[preview version](ai-preview-getstarted.md) of Business Central that's enabled for Copilot.-->
- У вас есть права администратора или суперпользователя в Business Central.  <!--For more information, go to [Configure AI-powered item marketing text with Copilot](enable-ai.md).-->

## Разрешение перемещения данных между географическими регионами

Эта задача применима только в том случае, если переключатель **Разрешить перемещение данных** появляется в верхней части страницы **Возможности Copilot и ИИ**. Если вместо переключателя **Разрешить перемещение данных** отображается ссылка **Как управлять своими данными Copilot?**, пропустите этот шаг.

![Показан снимок экрана с переключателем «Разрешить перемещение данных» на странице «Возможности Copilot и ИИ».](media/allow-data-movement-v2.png)

Переключатель **Разрешить перемещение данных** указывает, что местоположение вашей среды Business Central &mdash; географический регион, в котором обрабатываются и хранятся данные &mdash; не соответствует региону службы Azure OpenAI, используемому Copilot. Если вы хотите включить Copilot, вам необходимо разрешить перемещение данных между географическими регионами. Чтобы узнать больше о перемещении данных, перейдите в раздел [Перемещение данных Copilot между регионами](ai-copilot-data-movement.md). 

Чтобы разрешить перемещение данных за пределы вашего географического региона, выполните следующие действия:

1. В Business Central найдите и откройте страницу **Возможности Copilot и ИИ**.
1. Включите переключатель **Разрешить перемещение данных**.

   Переключатель **Разрешить перемещение данных** включен по умолчанию для сред в регионах Azure «Западная Европа и «Северная Европа».

Вы можете отказаться от перемещения данных, выключив переключатель **Разрешить перемещение данных**. Как только служба Azure OpenAI станет доступна в регионе вашей среды Business Central, среда автоматически подключится к ней, и переключатель больше не будет доступен.

<!-- Don't review
| Australia, United Kingdom, United States | Within the respective geographical region |
| Europe, France, Germany, Norway, Switzerland  | Sweden or Switzerland |
| Asia Pacific, Brazil, Canada, India, Japan, Singapore, South Africa, South Korea, United Arab Emirates  | United States |-->



<!--Note

If your environment is hosted in North America, Copilot will use an Azure OpenAI endpoint in North America to process your data.
If your environment is hosted in Europe, Copilot will use an Azure OpenAI endpoint in Europe to process your data.
If your environment is hosted anywhere else, Copilot will use an Azure OpenAI endpoint outside of the region in which the environment is hosted.
To opt in 

Copilot and other AI capabilities use Azure OpenAI Service.  and are provided by default to only those customers with environments that have United States as their geography for data processing and storage. While the Azure OpenAI Service is available in multiple geographies including Australia, Canada, United States, France, Japan and UK, Copilot does not follow the same regional rollout schedule.

Meanwhile, customers with environments outside the United States can use Copilot AI features by opting in to share relevant data with the Azure OpenAI Service in United States or Switzerland.

The information in the following table outlines the Azure OpenAI service that's used by the Copilot services based on the geography of their Dynamics 365 environment when they opt-in to share data.-->

## Активирование функций

Все возможности Copilot и ИИ активны по умолчанию, когда предлагаются в качестве предварительной версии или становятся общедоступными. Используя страницу **Возможности Copilot и ИИ**, вы можете отключать и снова включать отдельные функции для всех пользователей.

1. В Business Central найдите и откройте страницу **Возможности Copilot и ИИ**.

1. На странице перечислены все доступные функции Copilot и ИИ, а также их текущий статус, который может быть активным или неактивным. Функции разделены на два раздела &mdash; один раздел для функций в предварительной версии, а другой для функций, которые общедоступны. 

   [![Показывает ролевой центр Business Central и контрольный список для Copilot](media/copilot-and-ai-capabilties-page.svg)](media/copilot-and-ai-capabilties-page.svg#lightbox)

   - Чтобы включить функцию, выберите ее в списке, а затем выберите действие **Активировать**.
   - Чтобы выключить функцию, выберите ее, а затем выберите действие **Деактивировать**. 

<!-- don't review 

<!-- For 2024 there are no AI features governed by **Feature Management**, so this section is not shown
## Enable feature in Feature Management

When individual Copilot capabilities are released in Business Central minor updates, these capabilities are optional until the next major update. **Feature Management** is used to turn on or off features that are in preview, like bank reconciliation, and some features that are generally available, like marketing text suggestions. [Learn more about feature management](/dynamics365/business-central/dev-itpro/administration/feature-management).

1. In Business Central, search for and open the **Feature Management** page.
2. To enable a feature, set the **Enabled for** column to **All users**. To disable a feature, set the **Enabled for** column to **None**. Use the following table to help you determine the switch that applies to the Copilot and AI capability you want to enable:

   - **Feature Preview: Bank account reconciliation with Copilot** enables the bank account reconciliation assist feature.
   - **Feature Preview: Chat with Copilot** enables the chat with Copilot feature.
   - **Feature preview: Create AI-powered product descriptions with Copilot** enables the marketing text suggestions feature.

   For more information about feature management in general, go to [Feature Management](/dynamics365/business-central/dev-itpro/administration/feature-management).-->

## Предоставление доступа пользователям

Возможности Copilot и ИИ могут содержать функциональность, предназначенную для любых пользователей в вашей организации или для пользователей с конкретными ролями. Большинство возможностей Copilot и ИИ предусматривают управление доступом с использованием разрешений и наборов разрешений в системе управления разрешениями Business Central. [Узнайте больше о разрешениях и наборах разрешений](ui-define-granular-permissions.md).

В следующей таблице перечислены разрешения, необходимые для использования функций Copilot, предоставляемых Business Central.

|Функции Copilot|Необходимые разрешения|
|-|-|
|Помощь при анализе|Набор разрешений **АНАЛИЗ ДАННЫХ — ВЫПОЛНИТЬ** или разрешение на выполнение системного объекта 9640 **Разрешить режим анализа данных**. Это те же разрешения, которые необходимы для доступа к режиму анализа.|
|Помощь при выверке банковских счетов|Разрешение на стр. 7250 **Предлож. ИИ при выверке банк. счета** и на стр. 7252 **Предложение ИИ по переводу на счет ГК**.|
|Чат |Не существует разрешений или наборов разрешений, которые бы управляли доступом к чату для каждого пользователя. Если чат активирован, он доступен всем пользователям.|
|Предлагаемые маркетинговые тексты |Разрешение на странице 5836 **Маркетинговый текст Copilot**|

Чтобы предоставить или запретить доступ к определенным возможностям помощника, не связанного с Microsoft, и ИИ, сверьтесь с документацией по этой функции или обратитесь к ее к издателю, чтобы узнать, какие разрешения необходимы.

## Дальнейшие шаги

После того как вы активируете функции и дадите согласие на их использование, вы готовы опробовать их. Переходите к разделам:

- [Добавление маркетингового текста для товаров](item-marketing-text.md)
- [Анализ данных в режиме анализа с Copilot](analysis-assist.md)  
- [Чат с Copilot](chat-with-copilot.md)
- [Выверка с использованием помощи в выверке банковских счетов](bank-reconciliation-with-copilot.md)

## См. также

[Устранение неполадок с возможностями Copilot и ИИ](ai-copilot-troubleshooting.md)  
[Вопросы и ответы о помощи при анализе](faqs-analysis-assist.md)  
[Вопросы и ответы о помощи в выверке банковского счета](faqs-bank-reconciliation.md)  
[Вопросы и ответы о чате с Copilot](faqs-chat-with-copilot.md)  
[Вопросы и ответы о предлагаемых маркетинговых текстах](faqs-marketing-text.md)  
[Обзор предлагаемых маркетинговых текстов](ai-overview.md)  