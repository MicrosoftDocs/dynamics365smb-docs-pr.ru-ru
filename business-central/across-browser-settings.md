---
title: Настройка браузера
description: 'Описывается, как настроить браузеры для работы с решением Business Central и продуктами, которые с ним интегрируются.'
author: jswymer
ms.topic: get-started
ms.devlang: al
ms.search.keywords: 'Teams, web client, troubleshooting, errors'
ms.date: 12/04/2023
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---
# <a name="setting-up-and-troubleshooting-your-browser-to-work-with-business-central-web-client"></a>Настройка и устранение неполадок браузера для работы с веб-клиентом Business Central

В этой статье объясняется, как настроить браузер так, чтобы [!INCLUDE[web_client](includes/web_client.md)] и все его функции работали правильно. Прочтите эту статью, если у вас возникли проблемы с открытием [!INCLUDE[web_client](includes/web_client.md)], потому что некоторые проблемы могут быть вызваны настройками вашего браузера.

В статье подробно рассказывается о настройке Microsoft Edge, но требования для JavaScript, файлов cookie и всплывающих окон одинаковы для всех поддерживаемых браузеров. Для других браузеров обратитесь к инструкциям производителя.  

## <a name="use-a-supported-browser"></a>Использование поддерживаемого браузера

Убедитесь, что вы используете один из поддерживаемых браузеров. См. раздел [Минимальные требования для использования Business Central](product-requirements.md#browsers).

Мы рекомендуем использовать версию браузера из стабильного канала, поскольку это самая надежная и стабильная версия, прошедшая тщательное тестирование и исправление ошибок. Это гарантирует вам комфортную работу и минимальную вероятность возникновения проблем при использовании веб-клиента.  

## <a name="allow-javascript-from-business-central"></a>Разрешение JavaScript из Business Central

*Проблема:*

Если браузер не поддерживает JavaScript, вы увидите сообщение **NotSupported/DisabledJavaScript** в адресной строке и сообщение **Ошибка HTTP 404.0 — не найдено** при попытке открыть [!INCLUDE[prod_short](includes/prod_short.md)], и 

<!-- http://localhost:8080/NotSupported/DisabledJavaScript HTTP Error 404.0 - Not Found
The resource you are looking for has been removed, had its name changed, or is temporarily unavailable. -->

*Исправление:*

1. В Microsoft Edge перейдите к пункту **Настройки** > **Файлы cookie и разрешения сайтов** > **JavaScript**.
2. Выполните один из следующих шагов. Выберите шаг, рекомендуемый вашей организацией:

    - Переместите выключатель **Разрешено** влево (Выкл.). Затем выберите **Добавить** и введите адрес (URL) для [!INCLUDE[prod_short](includes/prod_short.md)] в поле **Сайт**. Выберите **Добавить**, когда будете готовы.
    - Переместите выключатель **Разрешено** вправо (Вкл.).

## <a name="allow-cookies-from-business-central"></a>Разрешение файлов cookie из Business Central

*Проблема:*

Если в браузере не разрешены файлы cookie, вы увидите следующую ошибку:

**К сожалению, страница не найдена. Пожалуйста, проверьте адрес и попробуйте снова.** 

*Исправление:*

1. В Microsoft Edge перейдите к пункту **Настройки** > **Файлы cookie и разрешения сайтов** > **Файлы cookie и данные сайта**.
2. Переместите выключатель **Разрешить сайтам сохранять и читать данные файлов cookie** вправо (Вкл.).  

## <a name="allow-pop-ups-from-business-central"></a><a name="popup"></a>Разрешение всплывающих окон из Business Central

[!INCLUDE[prod_short](includes/prod_short.md)] интегрируется с несколькими продуктами. В некоторых случаях, например при использовании Microsoft Teams, [!INCLUDE[prod_short](includes/prod_short.md)] открывается во всплывающем окне внутри продукта. Эта возможность требует, чтобы ваш браузер разрешал всплывающие окна из [!INCLUDE[prod_short](includes/prod_short.md)].

*Проблема:*

Если всплывающие окна для [!INCLUDE[prod_short](includes/prod_short.md)] блокируются, вы получите сообщение, подобное следующему:

**Что-то пошло не так. Ваш браузер может блокировать всплывающие окна, необходимые Business Central.**

<!--
Something went wrong
Your browser may be blocking pop-ups needed by Business Central.

Change your browser settings to allow pop-ups or allow this for trusted domains, then try again.
If these settings are managed for your organization, you should contact your administrator for assistance.

Try again
-->
*Исправление:*

1. В Microsoft Edge перейдите к пункту **Настройки** > **Файлы cookie и разрешения сайтов** > **Всплывающие окна и перенаправления**.
2. Переместите выключатель **Блокировать** вправо (Вкл.).
3. Выберите **Добавить**. В поле **Сайт** введите `https://businesscentral.dynamics.com`, затем выберите **Добавить**.

## <a name="see-also"></a>См. также

[Устранение неполадок Teams](admin-teams-troubleshooting.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
