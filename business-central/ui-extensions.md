---
title: Установка расширений для настройки Business Central | Документы Майкрософт
description: Узнайте о добавлении функций и настройке Business Central путем установки расширений.
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: app, add-in, manifest, customize
ms.date: 04/01/2019
ms.author: edupont
ms.openlocfilehash: d03d1aa3910dc73dc61c61bdd66725e8e8af3c66
ms.sourcegitcommit: 04581558f6c5488c705a7ac392cf297be10b5f4f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2019
ms.locfileid: "1621118"
---
# <a name="customizing-business-central-using-extensions"></a>Настройка Business Central с помощью расширений
Вы можете изменить [!INCLUDE[d365fin](includes/d365fin_md.md)] за счет установки расширений, которые добавляют функциональность, изменяют поведение или, например, предоставляют доступ к новым интернет-службам.
При первом запуске [!INCLUDE[d365fin](includes/d365fin_md.md)] некоторые расширения уже установлены. Со временем вам станут доступны дополнительные расширения, и вы сможете выбрать, хотите ли вы использовать эти расширения.

Например, корпорация Майкрософт предлагает расширение, которое обеспечивает интеграцию с PayPal Payments Standard. Это расширение установлено по умолчанию.
Но если появится другое расширение, предлагающее интеграцию с другой службой платежей, вы можете установить его и выбрать службу платежей для использования.  

Управление расширениями осуществляется на странице **Управление расширениями**. Эта страница доступна с начальной страницы. Также можно выбрать значок **Поиск страницы или отчета** ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать") в правом верхнем углу, ввести **Расширение**, затем выбрать связанную ссылку.  

> [!NOTE]  
>   Если вы считаете, что у вас должен быть доступ к расширению, но вы не можете найти его функциональные возможности, проверьте страницу **Управление расширениями**. Если расширение не указано в списке, вы можете установить его, как описано в следующем разделе.  

## <a name="installing-an-extension"></a>Установка расширения
Новые расширения можно получить из магазина по адресу [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?src=dynamics365website&product=dynamics-365-business-central). Здесь отображаются все доступные расширения для [!INCLUDE[d365fin](includes/d365fin_md.md)], и можно получить приложения, расширения и пакеты содержимого для других продуктов Майкрософт. Установите соответствующие фильтры, просмотрите информацию для каждого расширения и получите расширение для [!INCLUDE[d365fin](includes/d365fin_md.md)].  
> [!NOTE]  
>   Войдите на сайт [AppSource.microsoft.com](https://appsource.microsoft.com/), используя учетную запись электронной почты, которая используется для [!INCLUDE[d365fin](includes/d365fin_md.md)]. Для удобства используйте эту же учетную запись для других служб и продуктов.  

Можно также перейти в магазин из [!INCLUDE[d365fin](includes/d365fin_md.md)]. На странице **Управление расширениями** отображаются все текущие установленные расширения, и можно открыть страницу **Магазин расширений**, на которой отображаются расширения для [!INCLUDE[d365fin](includes/d365fin_md.md)], доступные на данный момент на сайте AppSource. Если выбрать ссылку *Еще приложения*, производится переход на сайт [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).  

Если вы выберите расширение, вы можете прочитать о его возможностях и открыть справку по расширению для получения более подробной информации. Если вы хотите получить расширение, необходимо согласиться с условиями использования. Если вы получили расширение с веб-сайта AppSource, для завершения установки выполняется вход в [!INCLUDE[d365fin](includes/d365fin_md.md)].  

При установке расширения может потребоваться настроить его, например указать учетную запись для использования расширения **PayPal Payments Standard для [!INCLUDE[d365fin](includes/d365fin_md.md)]**.
Другие расширения просто добавляют поля на существующую страницу или добавляют новую страницу.   

Если вы удалили расширение, а потом передумали, вы можете снова установить его. При удалении расширения, которое вы использовали, данные сохраняются, чтобы вы могли установить его снова и данные были по-прежнему доступны.  

Некоторые расширения разработаны Майкрософт, а другие — [другими организациями](ui-extensions-other.md). Расширения тестируются, прежде чем они становятся доступными для вас, но мы рекомендуем перейти по ссылкам, доступным для каждого расширения, чтобы узнать больше информации о расширении перед его установкой.  

Корпорация Майкрософт предоставляет следующие расширения:  

* [Миграция данных Dynamics GP](ui-extensions-dynamicsgp-data-migration.md)  
* [Envestnet Yodlee Bank Feeds](ui-extensions-yodlee-bank-feeds.md)  
* [Microsoft Pay](ui-extensions-microsoft-pay-payments.md)  
* [PayPal Payments Standard](ui-extensions-paypal-payments-standard.md)  
* [Миграция данных QuickBooks](ui-extensions-quickbooks-data-migration.md)  
* [Прогноз продаж и запасов](ui-extensions-sales-forecast.md)  
* [Зарплата Ceridian](ui-extensions-ceridian-payroll.md)  
* [Импорт файла зарплаты Quickbooks](ui-extensions-quickbooks-payroll.md)  
* [WorldPay Payments Standard](ui-extensions-worldpay-payments-standard.md)  
* [Почтовые индексы Великобритании GetAddress.io](ui-extensions-getaddressio.md)  
* [Миграция данных QuickBooks Online](ui-extensions-quickbooks-online-data-migration.md)  
* [Портал бухгалтера](ui-extensions-accountant-portal.md)  
* [Анализатор изображений](ui-extensions-image-analyzer.md)  
* [Платежи и выверки (DK)](ui-extensions-payments-reconciliation-formats-dk.md)  
* [Миграция данных C5](ui-extensions-c5-data-migration.md)  
* [Важная бизнес-аналитика](ui-extensions-essential-business-insights.md)  
* [Прогнозы просрочки оплаты](ui-extensions-late-payment-prediction.md  )
* [Отправить авизо](ui-extensions-send-remittance-advice.md)

> [!NOTE]  
>  Новые расширения не становятся доступными в AppSource сразу после объявления об обновлении. Следить за выходом новых расширений можно на сайте [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).

## <a name="see-also"></a>См. также
[Расширение Dynamics 365 Business Central](about-develop-extensions.md)  
[Расширения для Business Central от других поставщиков](ui-extensions-other.md)  
[Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md)  
[Включение платежей клиентов через PayPal](sales-how-enable-payment-service-extensions.md)  
[Миграция бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка расширения "Почтовые индексы Великобритании GetAddress.io"](LocalFunctionality/UnitedKingdom/uk-setup-postal-code-service.md)  
[Расширения [!INCLUDE[d365fin](includes/d365fin_md.md)] от других поставщиков](ui-extensions-other.md)  
[Приступая к работе](product-get-started.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
