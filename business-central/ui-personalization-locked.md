---
title: Я не могу персонализировать страницу | Microsoft Docs
description: Объяснение причин, почему невозможно персонализировать страницу и как разблокировать страницу, чтобы ее можно было персонализировать.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: 64995372f68ed2804bc165823dacc34ad6a3194d
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1251289"
---
# <a name="why-a-page-is-locked-from-personalization"></a>Почему заблокирована персонализация страницы?

Существует два условия, которые не позволяют персонализировать страницу. Либо страница заперта (как показано значком ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации")), либо она заблокирована как показано значком ![Персонализация заблокирована](media/personalization-blocked-icon.png "Персонализация заблокирована")).

## <a name="locked-from-personalizing"></a>Замок персонализации

Если в баннере **Персонализация** открытой страницы имеется значок ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации") (как показано), это означает, что вы в настоящее время не можете делать никаких дополнительных изменений персонализации на этой странице.

![Замок персонализации](media/personalization-locked.png "Замок персонализации")


<!-- This is because we changed the way personalization works behind the scenes since the last time that you personalized the page. Unfortunately, the old way and new of doing things do not work together.

The page currently includes the last personalization changes that you made. If you want to continue personalizing the page, then you can choose the lock icon and then **Unlock**. Just be aware that if you choose to unlock the page, the current personalization of the page will be cleared, and you will have to start from scratch.
-->

Для этого может быть две причины.

1. Вы персонализировали страницу ранее, но это делалось с помощью ранней версии подукта. Мы изменили то, как работает персонализация в фоновом режиме, с момента последней персонализации страницы. К сожалению, старый и новый способы персонализации несовместимы.

2. До настоящего времени вы использовали только [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] для персонализации страницы.

### <a name="unlocking-the-page"></a>Снятие замка со страницы

Если нужно разблокировать страницу и продолжить персонализировать ее, выберите ![Замок персонализации](media/personalization-lock-icon.png "Замок персонализации"), затем **Разблокировать**.  

Перед тем как разблокировать страницу, учтите следующее:

- Текущая персонализация страницы будет сброшена. Страница вернется назад к исходному макеты, и вам придется начинать с начала.

- В [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] страница останется без изменений, и на нее не будут влиять новые изменения персонализации, сделанные в клиенте Business Central. В будущем персонализация в [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] и клиенте Business Central будут полностью независимыми друг от друга.

## <a name="blocked-from-personalizing"></a>Персонализация заблокирована

Если в баннере персонализации имеется значок ![Персонализация заблокирована](media/personalization-blocked-icon.png "Персонализация заблокирована"), это означает, что вам запрещена любая персонализация на этой странице.

![Персонализация заблокирована](media/personalization-blocked.png "Замок персонализации")

Причина этого заключается в том, что ролевой центр или профиль, который в настоящее время связан с вашей учетной записью пользователя, изменяет эту страницу специально для вашей роли. Обратитесь к администратору за помощью или, если это имеет смысл, попробуйте переключиться на ролевой центр (из [**Мои настройки**](https://businesscentral.dynamics.com?page=9176 "Прямой переход на вашу страницу пользовательских настроек в Business Central")), который действительно включает настройку для ролей для этой страницы.

## <a name="see-also"></a>См. также
[Персонализация рабочей области](ui-personalization-manage.md)  
[Управление персонализацией](ui-personalization-manage.md)  
[Изменение базовых настроек](ui-change-basic-settings.md)  
[Изменение набора отображаемых функций](ui-experiences.md)  
