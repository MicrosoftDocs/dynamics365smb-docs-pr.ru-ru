---
title: Настройка создания маркетинговых текстов для товаров на базе ИИ (предварительная версия) с помощью Copilot
description: 'В этой статье рассматривается, как получить пробную версию Business Central с Copilot и включить Copilot в среде.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: how-to
ms.date: 03/22/2023
ms.custom: bap-template
---

# <a name="configure-ai-powered-item-marketing-text-preview-with-copilot"></a><a name="configure-ai-powered-item-marketing-text-preview-with-copilot"></a><a name="configure-ai-powered-item-marketing-text-preview-with-copilot"></a>Настройка создания маркетинговых текстов для товаров на базе ИИ (предварительная версия) с помощью Copilot

[!INCLUDE[ai-preview](includes/ai-preview.md)]

В этой статье объясняется, как вы можете управлять возможностью создания маркетингового текста на базе ИИ с помощью Copilot для вашей организации. Эту задачу выполняет администратор. Чтобы сделать эту функцию доступной для пользователей, необходимо выполнить два требования:

- Включите функцию **Создание описаний товаров на базе ИИ с помощью Copilot**.
- Согласитесь с условиями [предварительной версии](https://dynamics.microsoft.com/legaldocs/supp-dynamics365-preview/) и [Заявлением о конфиденциальности Microsoft](https://go.microsoft.com/fwlink/?LinkId=521839) от имени организации.

Если какое-либо из этих требований не выполняется, функция не будет доступна для использования.

## <a name="prerequisites"></a><a name="prerequisites"></a><a name="prerequisites"></a>Предварительные требования

Вы используете [предварительную версию](ai-preview-getstarted.md) Business Central, в которой включен Copilot. Включение Copilot выполняется администратором. Для получения дополнительной информации перейдите к разделу [Настройка создания маркетингового текста для товаров на базе ИИ с помощью Copilot](enable-ai.md).

## <a name="enable-or-disable-create-ai-powered-product-descriptions-with-copilot"></a><a name="enable-or-disable-create-ai-powered-product-descriptions-with-copilot"></a><a name="enable-or-disable-create-ai-powered-product-descriptions-with-copilot"></a>Включение или выключение создания описаний товаров на базе ИИ с помощью Copilot

1. В Business Central найдите и откройте страницу **Управление функциями**.
2. Установите в столбце **Включено для** функции **Предварительная версии функции: создание описаний товаров на базе ИИ с помощью Copilot** значение **Все пользователи**, чтобы включить функцию, или **Нет**, чтобы ее отключить.

   Дополнительные сведения об управлении функциями в целом см. в разделе [Управление функциями](/dynamics365/business-central/dev-itpro/administration/feature-management).

## <a name="consent-to-or-reject-preview-and-privacy-terms-and-conditions-for-all-users"></a><a name="consent-to-or-reject-preview-and-privacy-terms-and-conditions-for-all-users"></a><a name="consent-to-or-reject-preview-and-privacy-terms-and-conditions-for-all-users"></a>Согласие на условия использования предварительной версии и условия конфиденциальности или отказ от них для всех пользователей

1. В Business Central найдите и откройте страницу **Статус уведомлений о конфиденциальности**.
2. В столбце **Имя интеграции** выберите **Azure OpenAI**, затем прочитайте условия.
3. В строке **Azure OpenAI** установите флажок **Принять для всех** для согласия или флажок **Отклонить для всех** для отказа.

## <a name="next-steps"></a><a name="next-steps"></a><a name="next-steps"></a>Дальнейшие шаги

После того как вы включите эту функцию и дадите на нее свое согласие, вы сможете опробовать Copilot на товарах в Business Central. Перейдите в раздел [Добавление маркетингового текста для товаров](item-marketing-text.md).  

## <a name="see-also"></a><a name="see-also"></a><a name="see-also"></a>См. также

[Обзор функции создания маркетинговых текстов для товаров на базе ИИ с помощью Copilot](ai-overview.md)  
[Создание маркетингового текста для товаров с помощью Copilot](item-marketing-text.md)  
[Вопросы и ответы по созданию маркетинговых текстов для товаров на базе ИИ с помощью Copilot](ai-faq.md)  
