---
title: Получение Business Central на настольном компьютере
description: В этой статье описывается, как установить приложение Business Central на настольный компьютер Windows или MACiOS.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: phone, tablet
ms.date: 10/01/2021
ms.author: jswymer
ms.openlocfilehash: babf20be3c22a3d4b7dd710e2486c59bc11351fe
ms.sourcegitcommit: 795f0298e32b4c0174aeeb9a7da64f1e5c8457d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/04/2021
ms.locfileid: "7596651"
---
# <a name="get-business-central-desktop-app"></a>Получение приложения Business Central на настольном компьютере

Если у вас есть компьютер с Windows (ПК) или macOS, вы можете установить приложение Business Central на свой настольный компьютер. 
> [!NOTE]
> Если вы используете Business Central выпуска 2021 волны 1 или более раннюю версию, загрузите приложение из [Магазина Windows](https://go.microsoft.com/fwlink/?LinkId=734848).

## <a name="why-use-the-app"></a>Почему нужно использовать это приложение?

Приложение Business Central похоже на веб-клиент, но имеет несколько преимуществ, например:

- Приложение доступно в меню **Пуск**, вы можете легко закрепить его на панели задач или запустить по умолчанию при запуске компьютера.
- В целом, приложение также быстрее и плавнее отображается на экране без разницы в производительности по сравнению с [!INCLUDE[prod_short](includes/prod_short.md)], запущенным в браузере.
- Приложение открывается в отдельном окне, независимо от окон браузера. Эта функция упрощает поиск при запуске большого количества приложений или вкладок браузера.
- Если у вас несколько сред Business Central (только в Интернете), вы можете установить приложение отдельно для каждой среды.

     Когда вы открываете приложение для определенной среды, имя среды включается в заголовок окна. При работе с несколькими средами [!INCLUDE[prod_short](includes/prod_short.md)] каждое окно приложения отображается отдельно. По названию вам будет легче увидеть, какое окно связано с каждой средой.

## <a name="install-the-app"></a>Установка приложения

1. Откройте веб-клиент [!INCLUDE[prod_short](includes/prod_short.md)] в Microsoft Edge или Google Chrome.

2. Если появится страница выбора среды, вы можете сделать одно из двух:

   - Выберите среду и перейдите к следующему шагу, чтобы установить приложение. В этом случае установленное приложение откроет выбранную вами среду.
   - Не выбирайте среду и просто перейдите к следующему шагу, чтобы установить приложение. В этом случае установленное приложение откроет страницу выбора среды, а не конкретную среду.

3. Чтобы установить приложение, в зависимости от вашего браузера выберите ![Значок для установки приложения в Microsoft Edge.](media/ui-edge-install-app-icon.png) **Приложение доступно. Установить Business Central** или ![Значок для установки приложения в Chrome.](media/ui-chrome-install-app-icon.png) **Установить Business Central**, затем **Установить**.

   | Microsoft Edge | Google Chrome |
   |--|--|
   | :::image type="content" source="media/ui-edge-install-app-v2.png" alt-text="иллюстрация кнопки для установки приложения в Microsoft Edge."::: | :::image type="content" source="media/ui-chrome-install-app-v2.png" alt-text="иллюстрация кнопки для установки приложения в Chrome."::: |

  > [!TIP]
  > С Microsoft Edge вы также можете установить приложение, перейдя в меню **Настройки и другое** в браузере, затем выбрав **Приложения** > **Установить этот сайт как приложение** > **Установить**.

После установки приложение появится в меню **Пуск**. Если вы выбрали определенную среду для приложения, имя среды добавляется к имени приложения в меню **Пуск**.

### <a name="for-business-central-on-premises"></a>Локальная версия Business Central

Установка приложения при использовании локальной версии Business Central в основном такая же, как описано выше. Если у вас только один клиент, просто откройте Business Central в своем браузере и выберите ![Значок для установки приложения в Microsoft Edge.](media/ui-edge-install-app-icon.png) **Приложение доступно. Установить Business Central** или ![Значок для установки приложения в Chrome.](media/ui-chrome-install-app-icon.png) **Установить Business Central**, как показано выше. 

Разница есть, если у вас несколько клиентов. В отличие от локальной версии [!INCLUDE[prod_short](includes/prod_short.md)], где вы можете установить приложение отдельно для разных сред, в локальной среде вы можете установить приложение только для одного клиента. Поэтому перед установкой приложения, если у вас несколько клиентов, обязательно переключитесь на правильный клиент. После установки, когда вы открываете приложение, оно сразу открывает клиента.

<!-- for FAQ or troubleshooting
> [!NOTE]
> To install the app, [!INCLUDE[prod_short](includes/prod_short.md)] must be configured for HTTPS. If it isn't, you won't see ![Icon for installing an app in Edge.](media/ui-edge-install-app-icon.png) **App available. Install Business Central** or ![Icon for installing an app in Chrome.](media/ui-chrome-install-app-icon.png) **Install Business Central** in the browser. If you're having problems, contact your administrator or see [Configuring SSL to Secure the Business Central Web Client Connection](/dynamics365/business-central/dev-itpro/deployment/configure-ssl-web-client-connection) about how to configure HTTPS.
-->

## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/alternative-interfaces-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Вопросы и ответы по мобильным приложениям](ui-mobile-faq.yml)  
[Подготовьтесь к ведению бизнеса](ui-get-ready-business.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]