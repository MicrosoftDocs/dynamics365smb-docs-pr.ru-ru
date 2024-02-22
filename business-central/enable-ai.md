---
title: Настройка возможностей Copilot и ИИ
description: 'В этой статье объясняется, как включить Copilot в среде.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: how-to
ms.date: 10/29/2023
ms.custom: bap-template
ms.search.form: 7775
ms.collection:
  - bap-ai-copilot
---

# <a name="configure-copilot-and-ai-capabilities"></a>Настройка возможностей Copilot и ИИ

<!--[!INCLUDE[ai-preview](includes/ai-preview.md)]-->

<!--This article explains how you can control the ability to create AI-powered item marketing text with Copilot for your organization. This task is done by an admin. There are two requirements that you must fulfill to make the feature available to users:-->

В этой статье рассматривается, как управлять Copilot и другими возможностями ИИ в Business Central. Эту задачу выполняет администратор. Copilot — это системная функция и неотъемлемая часть Business Central. Как и в случае с большинством системных функций, вы не предоставляете доступ отдельным пользователям и не можете включить или отключить Copilot. Однако в Copilot предусмотрены элементы управления данными и возможность деактивации отдельных возможностей Copilot и ИИ для каждой среды. Существуют разные уровни управления доступом к возможностям ИИ, в зависимости от функции:

- Разрешение на перемещение данных между географическими регионами

  Эта задача требуется только в том случае, если ваша среда Business Central находится в другой географии, чем используемая ею служба Azure OpenAI. [Подробнее](#allow-data-movement-across-geographies)

- Активируйте эту функцию на странице **Возможности Copilot и ИИ**. [Подробнее](#activate-features)

- Включите конкретную функцию, если она все еще управляется разделом **Управление функциями**.

  В волне 2 выпуска 2023 года в разделе **Управление функциями** включены как предложения маркетингового текста, так и функции помощи в выверке банковских счетов. [Подробнее](#enable-feature-in-feature-management)

Если какие-либо из этих требований не выполняются, функция не доступна для использования.

## <a name="prerequisites"></a>Предварительные требования

- Вы используете Business Central Online версии 23.1 или более поздней. <!--[preview version](ai-preview-getstarted.md) of Business Central that's enabled for Copilot.-->
- У вас есть права администратора или суперпользователя в Business Central.  <!--For more information, go to [Configure AI-powered item marketing text with Copilot](enable-ai.md).-->

## <a name="allow-data-movement-across-geographies"></a>Разрешение перемещения данных между географическими регионами

Эта задача применима только в том случае, если переключатель **Разрешить перемещение данных** появляется в верхней части страницы **Возможности Copilot и ИИ**. Если вместо переключателя **Разрешить перемещение данных** отображается ссылка **Как управлять своими данными Copilot?**, пропустите этот шаг.

![Показан снимок экрана с переключателем «Разрешить перемещение данных» на странице «Возможности Copilot и ИИ».](media/allow-data-movement-v2.png)

Переключатель **Разрешить перемещение данных** указывает, что местоположение вашей среды Business Central &mdash; географический регион, в котором обрабатываются и хранятся данные &mdash; не соответствует региону службы Azure OpenAI, используемому Copilot. Если вы хотите включить Copilot, вам необходимо разрешить перемещение данных между географическими регионами. Чтобы узнать больше о перемещении данных, перейдите в раздел [Перемещение данных Copilot между регионами](ai-copilot-data-movement.md). 

Чтобы разрешить перемещение данных за пределы вашего географического региона, выполните следующие действия:

1. В Business Central найдите и откройте страницу **Возможности Copilot и ИИ**.
1. Включите переключатель **Разрешить перемещение данных**.

Вы можете отказаться, выключив переключатель **Разрешить перемещение данных**. Как только служба Azure OpenAI станет доступна в регионе вашей среды Business Central, среда автоматически подключится к ней, и переключатель больше не будет доступен. 


<!--
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

Все возможности Copilot и ИИ активны по умолчанию, когда предлагаются в качестве предварительной версии или становятся общедоступными. Используя страницу **Возможности Copilot и ИИ**, вы можете отключать и снова включать отдельные функции для всех пользователей.

1. В Business Central найдите и откройте страницу **Возможности Copilot и ИИ**.

1. На странице перечислены все доступные функции Copilot и ИИ, а также их текущий статус, который может быть активным или неактивным. Функции разделены на два раздела &mdash; один раздел для функций в предварительной версии, а другой для функций, которые общедоступны. 

   [![Показывает ролевой центр Business Central и контрольный список для Copilot](media/copilot-and-ai-capabilties-page.svg)](media/copilot-and-ai-capabilties-page.svg#lightbox)

   - Чтобы включить функцию, выберите ее в списке, а затем выберите действие **Активировать**.
   - Чтобы выключить функцию, выберите ее, а затем выберите действие **Деактивировать**. 


## <a name="enable-feature-in-feature-management"></a>Включение функции в разделе «Управление функциями»

Когда отдельные возможности Copilot выпускаются в рамках незначительных обновлений Business Central, эти возможности являются необязательными до следующего обновления с основным номером версии. **Управление функциями** используется для включения или отключения функций, находящихся на этапе предварительной версии, таких как выверка банковских счетов, а также некоторых общедоступных функций, таких как предлагаемые маркетинговые тексты. [Узнайте больше об управлении функциями](/dynamics365/business-central/dev-itpro/administration/feature-management).

1. В Business Central найдите и откройте страницу **Управление функциями**.
2. Чтобы включить функцию, установите для столбца **Включено для** значение **Все пользователи**. Чтобы отключить функцию, установите для столбца **Включено для** значение **Нет**. Используйте следующую таблицу, чтобы определить переключатель, относящийся к возможности Copilot и ИИ, которую вы хотите включить:

   - **Предварительная версия функции: выверка банковских счетов с помощью Copilot** относится к функции помощи в выверке банковских счетов.
   - **Предварительная версия функции: создание описаний продуктов на основе ИИ с помощью Copilot** относится к функции предложений маркетингового текста.

   Дополнительные сведения об управлении функциями в целом см. в разделе [Управление функциями](/dynamics365/business-central/dev-itpro/administration/feature-management).

## <a name="granting-user-access"></a>Предоставление доступа пользователям

Возможности Copilot и ИИ могут содержать функциональность, предназначенную для любых пользователей в вашей организации или для пользователей с конкретными ролями. Большинство возможностей Copilot и ИИ предусматривают управление доступом с использованием разрешений и наборов разрешений в системе управления разрешениями Business Central. [Узнайте больше о разрешениях и наборах разрешений](ui-define-granular-permissions.md).

Чтобы предоставить или запретить доступ к определенным возможностям Copilot и ИИ, сверьтесь с документацией по этой функции или обратитесь к ее к издателю, чтобы узнать, какие разрешения необходимы. 

## <a name="next-steps"></a>Дальнейшие шаги

После того как вы активируете функции и дадите согласие на их использование, вы готовы опробовать их. Переходите к разделам:

- [Добавление маркетингового текста для товаров](item-marketing-text.md) 
- [Выверка с использованием помощи в выверке банковских счетов](bank-reconciliation-with-copilot.md) 

## <a name="see-also"></a>См. также

[Устранение неполадок с возможностями Copilot и ИИ](ai-copilot-troubleshooting.md)  
[Обзор предлагаемых маркетинговых текстов](ai-overview.md)   
[Вопросы и ответы о предлагаемых маркетинговых текстах](faqs-marketing-text.md)  
