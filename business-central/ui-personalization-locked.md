---
title: Я не могу персонализировать страницу | Документация Майкрософт
description: Объяснение причин, почему невозможно персонализировать страницу и как разблокировать страницу, чтобы ее можно было персонализировать.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 0bd24833f37fe70f8e642685be4d28dbb593a16d
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3923399"
---
# <a name="why-a-page-is-locked-from-personalization"></a>Почему заблокирована персонализация страницы?

Существует два условия, которые не позволяют персонализировать страницу. Страница может быть заперта (о чем свидетельствует значок ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации")) или заблокирована (о чем свидетельствует значок ![Персонализация заблокирована](media/personalization-blocked-icon.png "Персонализация заблокирована")).

## <a name="locked-from-personalizing"></a>Замок персонализации

Если в баннере **Персонализация** открытой страницы имеется значок ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации"), это означает, что вы в настоящее время не можете вносить в эту страницу никакие дополнительные изменения, связанные с персонализацией.

<!-- This is because we changed the way personalization works behind the scenes since the last time that you personalized the page. Unfortunately, the old way and new of doing things do not work together.

The page currently includes the last personalization changes that you made. If you want to continue personalizing the page, then you can choose the lock icon and then **Unlock**. Just be aware that if you choose to unlock the page, the current personalization of the page will be cleared, and you will have to start from scratch.
-->

Для этого может быть две причины.

1. Вы персонализировали страницу ранее, но это делалось с помощью ранней версии подукта. Мы изменили то, как работает персонализация в фоновом режиме, с момента последней персонализации страницы. К сожалению, старый и новый способы персонализации несовместимы.

2. До настоящего времени вы использовали только [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] для персонализации страницы.

### <a name="unlocking-the-page"></a>Снятие замка со страницы

Если вы хотите снять замок со страницы и продолжить персонализировать ее, выберите значок ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации"), затем выберите действие **Разблокировать**.  

Перед тем как разблокировать страницу, учтите следующее:

- Текущая персонализация страницы будет сброшена. Страница вернется назад к исходному макеты, и вам придется начинать с начала.

- В [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] страница останется без изменений, и на нее не будут влиять новые изменения персонализации, сделанные в клиенте Business Central. В будущем персонализация в [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] и клиенте Business Central будут полностью независимыми друг от друга.

## <a name="blocked-from-personalizing"></a>Персонализация заблокирована

Если в баннере **Персонализация** имеется значок ![Персонализация заблокирована](media/personalization-blocked-icon.png "Персонализация заблокирована"), это означает, что вам запрещена любая персонализация на этой странице.

<!-- Only text is translated, so removing this image for non-English UX reasons.  ![Personalize blocked](media/personalization-blocked.png "Personalize lock") -->

Причина этого заключается в том, что ролевой центр или роль, которая в настоящее время связана с вашей учетной записью пользователя, изменяет эту страницу специально для вашей роли. Обратитесь за помощью к администратору. В качестве альтернативы попробуйте перейти к ролевому центру, который предусматривает ролевую настройку этой страницы. Дополнительные сведения см. в разделе [Изменение базовых настроек](ui-change-basic-settings.md).

## <a name="see-also"></a>См. также
[Персонализация рабочей области](ui-personalization-user.md)  
[Настройка страниц для профилей](ui-personalization-manage.md)  
[Изменение базовых настроек](ui-change-basic-settings.md)  
[Изменение набора отображаемых функций](ui-experiences.md)  
