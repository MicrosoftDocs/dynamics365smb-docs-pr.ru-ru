---
title: Оптимизация Outlook для входящего рабочего почтового ящика
description: Узнайте о том, что вы можете сделать, чтобы улучшить работу с "Входящие" для бизнеса в Microsoft Outlook.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Outlook, Microsoft 365, inbox, business inbox, WebView2, Edge, addin, add-in
ms.date: 05/12/2021
ms.author: jswymer
ms.openlocfilehash: 2fee1782057d0f45319e4d12d715c2e1e0d3d4a6
ms.sourcegitcommit: 61e279b253370cdf87b7bc1ee0f927e4f0521344
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "6064860"
---
# <a name="optimizing-outlook-for-your-business-inbox"></a>Оптимизация Outlook для входящего рабочего почтового ящика 

В этой статье рассказывается о том, что вы можете сделать, чтобы максимально использовать возможности "Входящие" для бизнеса в Microsoft Outlook. 

## <a name="update-outlook"></a>Обновить Outlook

Обновите Outlook до версии 2012 или новее.

> [!NOTE]
> Если вы не можете обновить Outlook до версии 2012 или более поздней, убедитесь, что вы обновили хотя бы до версии 1905. Это предотвращает запуск надстройки Outlook с использованием устаревших компонентов Internet Explorer

### <a name="how-to-check-your-version-of-outlook"></a>Как проверить свою версию Outlook

Независимо от того, используете ли вы Office 2019 или Microsoft 365, следуйте этому руководству службы поддержки Microsoft, чтобы узнать, какая у вас версия Outlook:  

[О Office: какую версию Office я использую?](https://support.microsoft.com/office/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19)

### <a name="how-to-update-outlook"></a>Как обновить Outlook

Чтобы обновить Outlook до последней версии, следуйте этому руководству службы поддержки Microsoft или обратитесь к администратору:

[Установить обновления Office](https://support.microsoft.com/office/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5)

## <a name="install-microsoft-edge-webview2"></a>Установите Microsoft Edge WebView2

Убедитесь, что Microsoft Edge WebView2 установлен на вашем устройстве.

### <a name="how-to-check-if-microsoft-edge-webview2-is-installed"></a>Как проверить, установлен ли Microsoft Edge WebView2 

Чтобы проверить, установлен ли Microsoft Edge WebView2 на компьютере, выполните следующие действия:

В меню «Пуск»:

1. Выберите **Пуск** ![Запуск Windows](media/windows-start-icon.png "Значок &quot;Пуск Windows&quot;") > **Параметры** ![Параметры Windows](media/windows-settings-icon.png "Значок настроек Windows") > **Приложения и функции**.
2. Введите **WebView2** в поле поиска. Если Microsoft Edge WebView2 установлен, вы увидите запись с названием **Среда выполнения Microsoft Edge WebView2**.

На панели управления:

1. В поле поиска рядом с **Пуск** ![Запуск Windows](media/windows-start-icon.png "Значок &quot;Пуск Windows&quot;") введите **Панель управления**, а затем выберите результат.
2. Выберите **Программ** > **Программы и компоненты**.
3. Введите **WebView2** в поле поиска. Если Microsoft Edge WebView2 установлен, вы увидите запись с названием **Среда выполнения Microsoft Edge WebView2**.

### <a name="how-to-install-microsoft-edge-webview2"></a>Как установить Microsoft Edge WebView2 

1. В браузере перейдите в [https://developer.microsoft.com/microsoft-edge/webview2/](https://developer.microsoft.com/microsoft-edge/webview2/).
2. Выберите **Загрузить**.
3. Задайте **Выбрать архитектуру**, чтобы соответствовать вашей системе.
4. Выберите **Загрузить**.

> [!NOTE]
> В вашей организации могут быть ограничения на то, какие компоненты могут быть установлены на вашем устройстве. Обратитесь за помощью к администратору.

## <a name="use-a-supported-browser"></a>Использование поддерживаемого браузера

Рассмотрите возможность использования Outlook для Интернета в одном из браузеров, поддерживаемых Business Central. Список поддерживаемых браузеров см. в [Минимальные требования для использования Business Central](product-requirements.md#browsers).

## <a name="see-also"></a>См. также

[Подготовьтесь к ведению бизнеса](ui-get-ready-business.md)  
[Получение Business Central на моем мобильном устройстве](install-mobile-app.md)  
[Отправка документов по электронной почте](ui-how-send-documents-email.md)  
[Финансы](finance.md)  
[Продажи](sales-manage-sales.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Минимальные требования для Outlook](product-requirements.md#outlook)  
[Использование надстроек в Outlook в Интернете](https://support.office.com/article/Using-Add-ins-in-Outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce?appver=OWB150)  


[!INCLUDE[footer-include](includes/footer-banner.md)]