---
title: Вопросы и ответы по ответственному использованию ИИ для чата с Copilot (предварительная версия)
description: 'В этом разделе часто задаваемых вопросов представлена информация о технологии искусственного интеллекта, используемой для чата с Copilot в Business Central. В нем также содержатся ключевые соображения и сведения о том, как используется ИИ, как он тестировался и оценивался, а также о любых конкретных ограничениях.'
ms.date: 03/18/2024
ms.custom:
  - responsible-ai-faqs
ms.topic: article
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.search.keywords: 'copilot, AI, chat'
---
# <a name="responsible-ai-faq-for-chat-with-copilot-preview"></a>Вопросы и ответы по ответственному использованию ИИ для чата с Copilot (предварительная версия)

[!INCLUDE[production-ready-preview-dynamics365](includes/production-ready-preview-dynamics365.md)]

Эти часто задаваемые вопросы (вопросы и ответы) описывают влияние ИИ функции чата с Copilot в [!INCLUDE[prod_short](includes/prod_short.md)]. Если вас интересуют общие вопросы об использовании этой функции, перейдите в раздел [Часто задаваемые вопросы для чата с Copilot](chat-with-copilot-faq.md).

## <a name="what-is-chat-with-copilot"></a>Что представляет собой Чат с Copilot?

Microsoft Copilot — это помощник на базе искусственного интеллекта, который помогает пробудить творческий подход, повысить производительность и избавиться от утомительных задач. Вы можете общаться с Copilot в Business Central, чтобы отвечать на вопросы и находить бизнес-данные, выражая то, что вы ищете, на естественном языке.

Чат с Copilot, также называемый чатом, — это интерактивная функция, которая отвечает на вопросы и находит бизнес-данные, связанные с [!INCLUDE[prod_short](includes/prod_short.md)], без необходимости пользователям перемещаться по пользовательскому интерфейсу или документации по продукту. Панель Copilot доступна из любой точки клиента [!INCLUDE[prod_short](includes/prod_short.md)].

Пользователи задают вопросы на естественном языке, например: «Как мне доставлять товары моим клиентам напрямую от моих поставщиков?» или «Есть ли у нас в наличии офисные стулья на сумму до 600 долларов США?» В ответ Copilot предоставляет ответы на естественном языке. В зависимости от вопросов ответы могут включать в себя обычный текст, ссылки на записи или страницы в [!INCLUDE[prod_short](includes/prod_short.md)] и ссылки на статьи справки [!INCLUDE[prod_short](includes/prod_short.md)] в Microsoft Learn.

## <a name="what-are-capabilities-of-chat-with-copilot"></a>Каковы возможности чата с Copilot?

Вы можете пообщаться с Copilot, чтобы получить ответы на следующие классы вопросов:

### <a name="explain-and-guide"></a>Объяснить и направить

Пользователи могут попросить Copilot объяснить конкретную концепцию, связанную с [!INCLUDE[prod_short](includes/prod_short.md)], например, что такое измерения, или дать рекомендации о том, как выполнить задачу, например, как разнести заказ на продажу. Copilot ищет в официальный документации [!INCLUDE[prod_short](includes/prod_short.md)], опубликованной Microsoft, и дает ответ на основе документации.

- Copilot использует знания о Microsoft Learn (не широкий поиск в Интернете) для семантического поиска только в документации по Dynamics 365 [!INCLUDE[prod_short](includes/prod_short.md)] в Microsoft Learn.

- Copilot не предпринимает никаких действий, не создает новые данные и не изменяет какие-либо конфигурации. Он просто обобщает все абзацы, найденные в Microsoft Learn, которые соответствуют вопросу или запросу в чате.

### <a name="find-business-data-and-related-pages"></a>Поиск бизнес-данных и связанных страниц

Пользователи могут попросить Copilot найти страницы по названию или запросить записи на основе их полей и ограничений. Если Copilot находит совпадение, он отправляет ссылку на соответствующую запись или страницу, которую пользователь затем может открыть.

- Copilot преобразует входные данные на естественном языке в запрос, состоящий из поиска по таблице, сортировки и критериев фильтрации.

  Эта возможность использует встроенные в [!INCLUDE[prod_short](includes/prod_short.md)] возможности поиска данных для поиска совпадающих данных в таблицах базы данных компании. В целях безопасности и соответствия требованиям поиск выполняется под собственным именем пользователя. Он не ищет за пределами базы данных [!INCLUDE[prod_short](includes/prod_short.md)].

- Copilot не предпринимает никаких действий, не создает новые данные и не изменяет какие-либо конфигурации. Он лишь обобщает записи, полученные от собственного поиска данных [!INCLUDE[prod_short](includes/prod_short.md)]. 

## <a name="what-is-the-intended-use-of-chat-with-copilot"></a>Каково предполагаемое использование чата с Copilot?

Чат предназначен для корпоративного использования и позволяет отвечать на вопросы, касающиеся [!INCLUDE[prod_short](includes/prod_short.md)] и бизнес-данных, которые он содержит. Эта функция позволяет людям решать общие задачи, такие как поиск записей или получение рекомендаций, выражая свои мысли своими словами, что делает работу с [!INCLUDE[prod_short](includes/prod_short.md)] проще и доступнее.

## <a name="how-was-chat-with-copilot-evaluated-what-metrics-are-used-to-measure-performance"></a>Как оценивалась функция чата с Copilot? Какие метрики используются для измерения ее производительности?

- Эта функция прошла тщательное тестирование, в ходе которого Copilot было передано множество текстов на английском языке, охватывающих широкий спектр тем и стилей выражения намерений. Результаты оценивались по точности, актуальности и безопасности.
- Эта функция создана в соответствии со стандартом ответственного ИИ Microsoft. [Узнайте больше об ответственном использовании ИИ от Microsoft](https://aka.ms/RAI).

## <a name="how-does-microsoft-monitor-the-quality-of-generated-content"></a>Как Microsoft контролирует качество создаваемого контента?

В Microsoft имеются различные системы, обеспечивающие высочайшее качество контента, создаваемого Copilot, обнаружение злоупотреблений и обеспечение безопасности наших клиентов и их данных.

Пользователи имеют возможность оставить отзыв на каждый ответ Copilot и сообщить о неточном или неприемлемом содержимом, чтобы помочь Microsoft улучшить эту функцию. 

- Вы оставляете отзыв, используя значок «Нравится» (палец вверх) или «Не нравится» (палец вниз) в области **Copilot** в [!INCLUDE[prod_short](includes/prod_short.md)].
- Мы анализируем и используем отзывы пользователей об этой функции, чтобы улучшить качество ответов.
- Если вы столкнулись с неприемлемым содержимым, сообщите об этом в Microsoft, используя эту форму обратной связи: [Сообщить о нарушении](https://go.microsoft.com/fwlink/?linkid=2249810).
- Microsoft может отключить функции Copilot для выбранных клиентов, если будет обнаружено злоупотребление этой функциональностью.

## <a name="what-are-the-limitations-of-chat-with-copilot-how-can-users-minimize-the-impact-of-the-chat-with-copilot-limitations-when-using-the-system"></a>Каковы ограничения чата с Copilot? Как пользователи могут свести к минимуму влияние ограничений чата с Copilot при использовании системы?

- Общие ограничения ИИ

  Системы искусственного интеллекта — ценные инструменты, но они недетерминированы. Создаваемый ими контент может быть не совсем точным. Поэтому важно использовать свое суждение для просмотра и проверки ответов Copilot, прежде чем принимать решения, которые могут повлиять на заинтересованные стороны, такие как клиенты и партнеры. Для большинства ответов Copilot также будет включать цитаты или справочные ссылки, которые вы можете использовать, чтобы быстро проверить, пришел ли Copilot к правильному ответу. Например, когда его спрашивают, как выполнить какую-то задачу, Copilot включает ссылку на исходную статью. Когда его просят найти запись по определенным критериям, Copilot включает ссылки, описывающие страницу списка, которую он определил как тему разговора, а также любые фильтры или сортировку, которые были применены для получения ответа.

- Языковые ограничения

  - Чат поддерживается только на английском языке для следующих языковых стандартов: en-AU, en-CA, en-GB, en-IE, en-IN, en-NZ, en-PH, en-SG, en-US, en-ZA.

    Если язык интерфейса в [!INCLUDE[prod_short](includes/prod_short.md)] не входит в число этих языков, чат недоступен.

  - Качество ответов может быть ниже при следующих условиях:
    - Языковой стандарт отличается от en-US.
    - Когда языковая настройка пользователя в [!INCLUDE[prod_short](includes/prod_short.md)] отличается от основного языка данных в базе данных [!INCLUDE[prod_short](includes/prod_short.md)].

- Ограничения по конкретной отрасли, продукту и теме

   Чат включает в себя встроенные механизмы безопасности, которые предотвращают нежелательное создание вредного контента, например контента откровенно сексуального характера или подстрекательства к насилию. Иногда клиенты работают в отраслях, продают продукты и услуги или работают с процессами, которые естественным образом пересекаются с тем, что может считаться неуместным в других контекстах, или работают с данными, которые могут активировать эти меры безопасности. В таких случаях чат может работать неэффективно.

<!--## What operational factors and settings allow for effective and responsible use of the feature?-->

## <a name="what-data-does-chat-with-copilot-collect-and-how-is-it-used"></a>Какие данные собирает чат с Copilot и как они используются

Microsoft не использует данные вашей компании, включая текст, который вы отправляете в Copilot, для обучения базовых моделей ИИ на благо других. Администраторы компании имеют полный контроль над управлением этими данными, которые являются частью их подписки Azure. Поскольку администраторы или другие сотрудники вашей компании могут иметь доступ к этим данным по решению вашего работодателя, мы рекомендуем пользователям не вводить конфиденциальные данные, такие как пароли или другие секретные данные.

## <a name="what-does-chat-with-copilot-offer-for-security"></a>Что чат с Copilot предлагает для обеспечения безопасности

Чат спроектирован безопасным и работает от имени пользователя, наследуя все разрешения безопасности и другие ограничения и никогда не работая за пределами безопасности платформы [!INCLUDE[prod_short](includes/prod_short.md)]. Это означает, что Copilot может получить доступ только к тем данным, к которым имеет доступ пользователь.

Пользователям с разрешением SUPER чат может легче находить незащищенные данные, к которым обычно сложнее получить доступ другим пользователям. Организации, которые не применяют модель безопасности [!INCLUDE[prod_short](includes/prod_short.md)] для ограничения доступа к таблицам и объектам каждого пользователя или роли пользователя, могут подвергаться повышенному риску при использовании чата. Поэтому мы рекомендуем вашей организации либо внедрить модель безопасности [!INCLUDE[prod_short](includes/prod_short.md)], либо деактивировать чат.

## <a name="see-also"></a>См. также

[Чат с Copilot (предварительная версия)](chat-with-copilot.md)
