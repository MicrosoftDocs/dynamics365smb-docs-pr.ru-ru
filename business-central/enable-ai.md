---
title: Настройка возможностей Copilot и ИИ
description: 'В этой статье объясняется, как включить Copilot в среде.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: how-to
ms.date: 06/28/2024
ms.custom: bap-template
ms.search.form: 7775
ms.collection:
  - bap-ai-copilot
---

# <a name="configure-copilot-and-ai-capabilities"></a>Настройка возможностей Copilot и ИИ

<!--[!INCLUDE[ai-preview](includes/ai-preview.md)]-->

<!--This article explains how you can control the ability to create AI-powered item marketing text with Copilot for your organization. This task is done by an admin. There are two requirements that you must fulfill to make the feature available to users:-->

В этой статье рассматривается, как управлять Microsoft Copilot и другими возможностями ИИ в Dynamics 365 Business Central. Эти задачи должен выполнять администратор.

Copilot — это функция системы и неотъемлемая часть Business Central. Как и в случае с большинством системных функций, вы не предоставляете доступ отдельным пользователям и не можете включить или отключить Copilot. Однако в Copilot предусмотрены элементы управления данными и возможность деактивации отдельных возможностей Copilot и ИИ для каждой среды. Существуют разные уровни управления доступом к возможностям ИИ, в зависимости от функции:

- Разрешение на перемещение данных между географическими регионами.

    Эта задача требуется только в том случае, если ваша среда Business Central и используемая ею служба Azure OpenAI находятся в разных географических регионах. [Узнайте больше о этой задаче](#allow-data-movement-across-geographies).

- Активация функции на странице **Возможности Copilot и ИИ**. [Узнайте больше о этой задаче](#activate-features).

<!-- For 2024 there are no AI features governed by **Feature Management**, so this section is not shown
- Enable the specific feature if it's governed by **Feature Management**.

  Check whether  of 2024 release wave 1, chat with Copilot, marketing text suggestions, and bank account reconciliation assist features are included under **Feature Management**. [Learn more](#enable-feature-in-feature-management)
<!-- 
- Enable the specific feature, if it's still governed by **Feature Management**.

  In 2023 release wave 2, both the marketing text suggestions and bank account reconciliation assist features are included under **Feature Management**. [Learn more](#enable-feature-in-feature-management)-->

Если какие-либо из этих требований не выполнены, функция недоступна для использования.

## <a name="prerequisites"></a>Предварительные требования

- Вы используете Business Central Online.
- Вы являетесь [администратором](#requirements-for-being-an-administrator) в Business Central.

## <a name="allow-data-movement-across-geographies"></a>Разрешение перемещения данных между географическими регионами

Эта задача применима только в том случае, если в верхней части страницы **Возможности Copilot и ИИ** присутствует переключатель **Разрешить перемещение данных**. Если вместо переключателя **Разрешить перемещение данных** отображается ссылка **Как управлять своими данными помощника?**, пропустите эту задачу.

![Снимок экрана с переключателем «Разрешить перемещение данных» на странице «Возможности Copilot и ИИ».](media/allow-data-movement-v2.png)

Присутствие переключателя **Разрешить перемещение данных** указывает, что местоположение вашей среды Business Central (географический регион, в котором обрабатываются и хранятся данные) отличается от региона службы Azure OpenAI, используемому Copilot. Чтобы включить Copilot, вам необходимо разрешить перемещение данных между географическими регионами. [Узнайте больше о перемещении данных](ai-copilot-data-movement.md).

Чтобы разрешить перемещение данных за пределы вашего географического региона, выполните следующие действия:

1. В Business Central найдите и откройте страницу **Возможности Copilot и ИИ**.
1. Включите переключатель **Разрешить перемещение данных**.

    > [!NOTE]
    > Переключатель **Разрешить перемещение данных** включен по умолчанию для сред в регионах Azure «Западная Европа и «Северная Европа».

Чтобы отказаться от перемещения данных, выключите переключатель **Разрешить перемещение данных**.

Как только служба Azure OpenAI станет доступна в регионе вашей среды Business Central, среда автоматически подключится к ней. После этого переключатель **Разрешить перемещение данных** исчезнет со страницы **Возможности Copilot и ИИ**.

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

## <a name="activate-features"></a>Активирование функций

Все возможности Copilot и ИИ активны по умолчанию, когда предлагаются в качестве предварительной версии или становятся общедоступными. На странице **Возможности Copilot и ИИ** вы можете отключать и снова включать отдельные функции для всех пользователей.

1. В Business Central найдите и откройте страницу **Возможности Copilot и ИИ**.
1. На странице перечислены все доступные функции Copilot и ИИ, а также их текущий статус. (Статус может быть *Активно* или *Неактивно*.) Функции разделены на два раздела: один для функций на этапе предварительной версии, а другой для функций на этапе общей доступности.

    - Чтобы включить функцию, выберите ее в списке, а затем выберите **Активировать**.
    - Чтобы выключить функцию, выберите ее в списке, а затем выберите **Деактивировать**.

    [![Снимок экрана, на котором показаны кнопки «Активировать» и «Деактивировать» для списков функций на странице возможностей Copilot и ИИ.](media/copilot-and-ai-capabilties-page.svg)](media/copilot-and-ai-capabilties-page.svg#lightbox)

<!-- don't review 

<!-- For 2024 there are no AI features governed by **Feature Management**, so this section is not shown
## <a name="enable-feature-in-feature-management"></a>Enable feature in Feature Management

When individual Copilot capabilities are released in Business Central minor updates, these capabilities are optional until the next major update. **Feature Management** is used to turn on or off features that are in preview, like bank reconciliation, and some features that are generally available, like marketing text suggestions. [Learn more about feature management](/dynamics365/business-central/dev-itpro/administration/feature-management).

1. In Business Central, search for and open the **Feature Management** page.
2. To enable a feature, set the **Enabled for** column to **All users**. To disable a feature, set the **Enabled for** column to **None**. Use the following table to help you determine the switch that applies to the Copilot and AI capability you want to enable:

   - **Feature Preview: Bank account reconciliation with Copilot** enables the bank account reconciliation assist feature.
   - **Feature Preview: Chat with Copilot** enables the chat with Copilot feature.
   - **Feature preview: Create AI-powered product descriptions with Copilot** enables the marketing text suggestions feature.

   For more information about feature management in general, go to [Feature Management](/dynamics365/business-central/dev-itpro/administration/feature-management).-->

## <a name="granting-user-access"></a>Предоставление доступа пользователям

Возможности Copilot и ИИ могут содержать функциональность, предназначенную для любых пользователей в вашей организации или для пользователей с конкретными ролями. Большинство возможностей Copilot и ИИ предусматривают управление доступом с использованием разрешений и наборов разрешений в системе управления разрешениями Business Central. [Узнайте больше о разрешениях и наборах разрешений](ui-define-granular-permissions.md).

В следующей таблице перечислены разрешения, необходимые для использования функций Copilot, предоставляемых Business Central.

| Функция Copilot | Необходимые разрешения |
|---|---|
| Помощь при анализе | Набор разрешений **DATA ANALYSIS - EXEC** или разрешение на выполнение системного объекта 9640 **Разрешить режим анализа данных**. Это те же разрешения, которые необходимы для доступа к режиму анализа. |
| Помощь при выверке банковских счетов | Разрешение на стр. 7250 **Предлож. ИИ при выверке банк. счета** и на стр. 7252 **Предложение ИИ по переводу на счет ГК**. |
| Чат | Не существует разрешений или наборов разрешений, которые управляли бы доступом к чату для каждого пользователя. Если чат активирован, он доступен всем пользователям. |
| Сопоставление электронных документов | Разрешение на странице 6166 **Предл. Copilot по эл. док. и заказам**. |
| Предлагаемые маркетинговые тексты | Разрешение на странице 5836 **Маркетинговый текст Copilot**. |
| Предложения строк продаж | Разрешение на странице 7275 **Предлагаемые ИИ строки продаж** и страница 7276 **Предлагаемые ИИ строки продаж суб.**. |

Чтобы предоставить или запретить доступ к конкретным помощникам и возможностям ИИ, предлагаемым не Майкрософт, сверьтесь с документацией по соответствующему компоненту или обратитесь к его издателю, чтобы узнать, какие разрешения необходимы.

## <a name="requirements-for-being-an-administrator"></a>Требования к администратору

У вас должны быть либо разрешения SUPER в учетной записи пользователя Business Central, либо одна из следующих лицензий Business Central:

- Делегированный административный агент - партнер
- Делегированный агент службы поддержки - партнер
- Внутренний администратор
- Внутренний администратор BC
- Администратор Dynamics 365

В Business Central пока не предусмотрено детальных разрешений на уровне объекта, чтобы только определенные администраторы могли настраивать Copilot.

## <a name="next-steps"></a>Дальнейшие шаги

После того как вы активируете функции и дадите согласие на их использование, вы готовы опробовать их. В этом вам помогут следующие статьи:

- [Добавление маркетингового текста к товарам с помощью Copilot](item-marketing-text.md)
- [Анализ данных в списках с помощью Copilot](analysis-assist.md)
- [Чат с Copilot](chat-with-copilot.md)
- [Сопоставление электронных документов со строками заказов на покупку с помощью Copilot](map-edocuments-with-copilot.md)
- [Выверка банковских счетов с помощью Copilot](bank-reconciliation-with-copilot.md)
- [Предложение строк в заказах на продажу с помощью Copilot](sales-suggest-sales-lines-with-copilot.md)

## <a name="see-also"></a>См. также

[Устранение неполадок с возможностями Copilot и ИИ](ai-copilot-troubleshooting.md)  
[Вопросы и ответы о помощи при анализе](faqs-analysis-assist.md)  
[Вопросы и ответы о помощи при выверке банковских счетов](faqs-bank-reconciliation.md)  
[Вопросы и ответы о чате с Copilot](faqs-chat-with-copilot.md)  
[Вопросы и ответы о сопоставлении электронных документов с заказами на покупку](faqs-map-edocuments.md)  
[Вопросы и ответы о предлагаемых маркетинговых текстах](faqs-marketing-text.md)  
[Вопросы и ответы о предлагаемых строках продаж](faq-sales-suggest-sales-lines-with-copilot.md)  
[Обзор предлагаемых маркетинговых текстов](ai-overview.md)
