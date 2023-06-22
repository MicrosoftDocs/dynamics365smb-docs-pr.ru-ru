---
title: Почему заблокирована персонализация страницы?
description: 'Вам может быть заблокирована возможность персонализировать страницу. Прочтите здесь о том, что вы можете сделать, чтобы разблокировать ее, чтобы вы могли персонализировать.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'customize, personalize, personalization, hide columns, remove fields, move fields'
ms.search.form: null
ms.date: 04/01/2021
ms.author: edupont
---
# <a name="why-a-page-is-locked-from-personalization" />Почему заблокирована персонализация страницы?

Существует два условия, которые не позволяют персонализировать страницу. Страница может быть заперта (о чем свидетельствует значок ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации")) или заблокирована (о чем свидетельствует ![Персонализация заблокирована.](media/personalization-blocked-icon.png "Персонализация заблокирована") значок).

## <a name="locked-from-personalizing" />Замок персонализации

Если есть значок ![Персонализация заблокирована.](media/personalization-lock-icon.png "Замок персонализации") на панели **Персонализация** при открытой странице, это означает, что вы в настоящее время не можете делать никаких дополнительных изменений персонализации на странице.

<!-- This is because we changed the way personalization works behind the scenes since the last time that you personalized the page. Unfortunately, the old way and new of doing things do not work together.

The page currently includes the last personalization changes that you made. If you want to continue personalizing the page, then you can choose the lock icon and then **Unlock**. Just be aware that if you choose to unlock the page, the current personalization of the page will be cleared, and you will have to start from scratch.
-->

Для этого может быть две причины:

1. Вы персонализировали страницу ранее, но это делалось с помощью ранней версии продукта. Мы изменили то, как работает персонализация в фоновом режиме, с момента последней персонализации страницы. К сожалению, старый и новый способы персонализации несовместимы.

2. До настоящего времени вы использовали устаревший [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] для персонализации страницы.

### <a name="unlocking-the-page" />Снятие замка со страницы

Если вы хотите снять замок со страницы и продолжить персонализировать ее, выберите значок ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации"), затем выберите действие **Разблокировать**.  

> [!CAUTION]
> Текущая персонализация страницы будет сброшена. Страница вернется назад к исходному макеты, и вам придется начинать с начала.  

## <a name="blocked-from-personalizing" />Персонализация заблокирована

Если в баннере **Персонализация** имеется значок ![Персонализация заблокирована](media/personalization-blocked-icon.png "Персонализация заблокирована"), вам запрещена любая персонализация на этой странице.

<!-- Only text is translated, so removing this image for non-English UX reasons.  ![Personalize blocked.](media/personalization-blocked.png "Personalize lock") -->

Причина заключается в том, что ролевой центр или роль, которая в настоящее время связана с вашей учетной записью пользователя, изменяет эту страницу специально для вашей роли. Обратитесь за помощью к администратору. В качестве альтернативы попробуйте перейти к ролевому центру, который предусматривает ролевую настройку этой страницы. Дополнительные сведения см. в разделе [Изменение базовых настроек](ui-change-basic-settings.md).

## <a name="see-also" />См. также

[Персонализация рабочей области](ui-personalization-user.md)  
[Настройка страниц для профилей](ui-personalization-manage.md)  
[Изменение базовых настроек](ui-change-basic-settings.md)  
[Изменение набора отображаемых функций](ui-experiences.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
