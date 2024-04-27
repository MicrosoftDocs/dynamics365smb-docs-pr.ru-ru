---
title: Вопросы и ответы по чату с Copilot
description: В этой статье приводятся ответы на распространенные вопросы о чате с Copilot в Business Central.
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: conceptual
ms.collection:
  - bap-ai-copilot
ms.date: 02/27/2024
ms.custom: bap-template jswymer
---
# <a name="chat-with-copilot-faq"></a>Вопросы и ответы по чату с Copilot

[!INCLUDE[preview-banner](includes/preview-banner.md)]

В этой статье приводятся ответы на распространенные вопросы о чате с Copilot в [!INCLUDE[prod_short](includes/prod_short.md)]. По вопросам, связанным с ИИ и чатом, обратитесь к разделу [Часто задаваемые вопросы об ответственном использовании ИИ для чата с Copilot](faqs-chat-with-copilot.md).

[!INCLUDE[production-ready-preview-dynamics365](includes/production-ready-preview-dynamics365.md)]

## <a name="can-admins-grant-or-deny-permission-to-individual-users-to-get-access-to-chat"></a>Могут ли администраторы предоставлять или запрещать отдельным пользователям доступ к чату?

Нет, для чата не существует разрешения или набора разрешений. Если чат активирован на странице [Возможности Copilot и искусственного интеллекта](enable-ai.md), каждый пользователь в среде имеет доступ к чату.
 
## <a name="is-chat-available-on-tablet-phone-or-other-form-factors"></a>Доступен ли чат на планшете, телефоне или в другом форм-факторе?

Нет, панель чата доступна только в веб-клиенте [!INCLUDE[web_client](includes/web_client.md)].

## <a name="i-dont-use-business-central-in-english-what-are-my-options"></a>Я не использую Business Central на английском языке. Какие есть варианты?

В настоящее время чат доступен только на английском языке. Вы можете изменить язык пользователя на английский в разделе [Мои настройки](ui-change-basic-settings.md#language).

## <a name="which-business-central-version-do-i-need-to-experience-chat"></a>Какая версия Business Central мне нужна для работы с чатом?

Чат доступен в общедоступной предварительной версии начиная с версии 24.0 (2024, выпуск волны 1).

## <a name="does-chat-work-with-my-customizations"></a>Работает ли чат с моими настройками?

Это зависит от типа вопроса, который вы задаете Copilot. Например.

- Когда вы задаете вопросы для поиска записей, Copilot может находить записи в ваших настраиваемых таблицах, которые идентифицируются с помощью настраиваемых полей.
- Когда вы запрашиваете объяснения или рекомендации, Copilot не имеет доступа к какой-либо информации о ваших настройках или документации для ваших надстроек.

## <a name="copilot-never-seems-to-open-the-record-or-page-i-asked-for-what-am-i-doing-wrong"></a>Кажется, что Copilot так и не открыл запись или страницу, которую я просил. Что я делаю не так?

Когда вы просите Copilot найти записи в [!INCLUDE[prod_short](includes/prod_short.md)], он отображает все найденные записи в виде выбираемых плиток или ссылок на панели чата. На этапе предварительной версии Copilot не переходит автоматически ни на одну страницу.

## <a name="the-answers-i-get-from-copilot-vary-even-though-i-ask-the-same-question-is-it-a-bug"></a>Ответы, которые я получаю от Copilot, различаются, хотя я задаю один и тот же вопрос. Это ошибка?

Copilot иногда может отвечать по-разному. Ответы не обязательно идентичны.

## <a name="when-should-i-use-the-copy-function-on-chat-messages"></a>Когда мне следует использовать функцию копирования в сообщениях чата?

Вы можете использовать кнопку «Копировать», чтобы скопировать сообщение из предыдущего разговора с Copilot, вставить его в поле ввода и повторить попытку, или попробовать вариант своего сообщения для Copilot.

## <a name="how-do-i-customize-or-extend-chat"></a>Как настроить или расширить чат?

На этапе предварительной версии панель чата и ответы Copilot нельзя каким-либо образом изменить с помощью настройки, надстроек или персонализации.

## <a name="does-copilot-find-data-in-other-companies-or-environments"></a>Находит ли Copilot данные в других компаниях или средах?

Даже если ваша организация использует несколько сред или компаний для разделения данных, Copilot ищет записи только в той компании, в которую вы в данный момент вошли.

## <a name="the-copilot-chat-pane-doesnt-show-what-can-i-do"></a>Панель чата Copilot не отображается. Что можно сделать?

Убедитесь, что в разделе «Мои настройки» для вашего языка пользователя выбран английский и что ваша среда имеет версию 24.0 или более позднюю. На странице «Возможности Copilot и ИИ» убедитесь, что администраторы включили согласие на передачу данных между географическими регионами и активировали чат. Убедитесь, что ваша локализация среды не Канада.

Если вы по-прежнему не видите функцию чата с Copilot, возможно, Microsoft все еще внедряет ее в вашем регионе. Copilot будет доступен для клиентов в США сначала в апреле 2024 года, а затем в течение нескольких недель будет доступен для локализаций в других странах.

## <a name="next-steps"></a>Дальнейшие шаги

[Чат с Copilot (предварительная версия)](chat-with-copilot.md)