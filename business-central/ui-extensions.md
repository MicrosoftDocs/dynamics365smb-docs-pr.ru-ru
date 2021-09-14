---
title: Установка расширений для настройки Business Central
description: Узнайте все о добавлении функций и настройке Business Central путем установки расширений здесь.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: app, add-in, manifest, customize
ms.date: 08/25/2021
ms.author: edupont
ms.openlocfilehash: b408afe65f2063ab77dca4e4e87fcfc4715f1204
ms.sourcegitcommit: e891484daad25f41c37b269f7ff0b97df9e6dbb0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2021
ms.locfileid: "7440507"
---
# <a name="customizing-business-central-online-using-extensions"></a>Настройка Business Central Online с помощью расширений

Вы можете изменить [!INCLUDE[prod_short](includes/prod_short.md)] интернет-версии за счет установки расширений, которые добавляют функциональность, изменяют поведение или, например, предоставляют доступ к новым интернет-службам.

> [!NOTE]
> Чтобы установить или удалить расширения из AppSource или добавить расширения для каждого арендатора, у вас должны быть соответствующие разрешения. Вы должны либо быть участником группы пользователей РАСШИР. УПР. - АДМИН. или у вас должен быть набор расширений РАСШИР. УПР. - АДМИН. Если вы являетесь администратором, вы можете назначать группы пользователей и разрешения другим пользователям в вашей компании.
>
> Чтобы использовать функциональную возможность, предоставляемую расширением, такую как открытие страниц, запуск отчетов, выбор действий и т. п., необходимо назначить наборы разрешений, которые устанавливаются как часть расширения.

> [!NOTE]  
> Набор разрешений **РАСШИР. УПР. — АДМИН** был представлен в волне выпуска 1 Business Central 2021 в качестве замены набора разрешений **УПР. РАСШИР. D365** в более ранних версиях.

> [!IMPORTANT]  
> Загрузка расширений для каждого арендатора и установка расширения AppSource не поддерживаются через страницу **Управление расширениями** для локальных установок. Вы не можете установить расширения AppSource локальной версии, в том числе в развертываниях на основе Docker.

При первом запуске [!INCLUDE[prod_short](includes/prod_short.md)] некоторые расширения уже установлены. Со временем вам станут доступны дополнительные расширения, и вы сможете выбрать, хотите ли вы использовать эти расширения.

Например, корпорация Майкрософт предлагает расширение, которое обеспечивает интеграцию с PayPal Payments Standard. Это расширение установлено по умолчанию.
Но если появится другое расширение, предлагающее интеграцию с другой службой платежей, вы можете установить его и выбрать службу платежей для использования.  

Управление расширениями осуществляется на странице **Управление расширениями**. Эта страница доступна с начальной страницы. Также можно выбрать значок **Поиск страницы или отчета** ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать") в правом верхнем углу, ввести **Расширение**, а затем выбрать соответствующую ссылку. Дополнительные сведения см. в разделе [Установка и удаление расширений](ui-extensions-install-uninstall.md).

> [!NOTE]  
> Если вы считаете, что у вас должен быть доступ к расширению, но вы не можете найти его функциональные возможности, проверьте страницу **Управление расширениями**. Если расширение не указано в списке, вы можете установить его, как описано в следующем разделе.  

> [!NOTE]  
> Войдите на сайт [AppSource.microsoft.com](https://appsource.microsoft.com/), используя учетную запись электронной почты, которая используется для [!INCLUDE[prod_short](includes/prod_short.md)] интернет-версии. Для удобства используйте эту же учетную запись для других служб и продуктов.  

Можно также перейти в магазин из [!INCLUDE[prod_short](includes/prod_short.md)]. На странице **Управление расширениями** отображаются все текущие установленные расширения, и можно открыть страницу **Магазин расширений**, на которой отображаются расширения для [!INCLUDE[prod_short](includes/prod_short.md)], доступные на данный момент на сайте AppSource. Если выбрать ссылку *Еще приложения*, производится переход на сайт [AppSource.microsoft.com](https://appsource.microsoft.com/marketplace/apps?product=dynamics-365%3Bdynamics-365-business-central&page=1).  

Если вы выберите расширение, вы можете прочитать о его возможностях и открыть справку по расширению для получения более подробной информации. Если вы хотите получить расширение, необходимо согласиться с условиями использования. Если вы получили расширение с веб-сайта AppSource, для завершения установки выполняется вход в [!INCLUDE[prod_short](includes/prod_short.md)].  

При установке расширения может потребоваться настроить его, например указать учетную запись для использования расширения **PayPal Payments Standard для [!INCLUDE[prod_short](includes/prod_short.md)]**.
Другие расширения просто добавляют поля на существующую страницу или добавляют новую страницу.   

Если вы удалили расширение, а потом передумали, вы можете снова установить его. При удалении расширения, которое вы использовали, данные сохраняются, чтобы вы могли установить его снова и данные были по-прежнему доступны. Некоторые расширения являются обязательными. Удалить эти расширения со страницы **Управление расширениями** нельзя. Если вы попытаетесь это сделать, появится сообщение об ошибке.  

Некоторые расширения разработаны Майкрософт, а другие — [другими организациями](ui-extensions-other.md). Расширения тестируются, прежде чем они становятся доступными для вас, но мы рекомендуем перейти по ссылкам, доступным для каждого расширения, чтобы узнать больше информации о расширении перед его установкой.  

Корпорация Майкрософт предоставляет следующие расширения:  

* [Расширение AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md)
* [Зарплата Ceridian](ui-extensions-ceridian-payroll.md)
* [Раздел организации](ui-extensions-company-hub.md)  
* [Миграция данных Dynamics GP](ui-extensions-dynamicsgp-data-migration.md)
* [Envestnet Yodlee Bank Feeds](ui-extensions-yodlee-bank-feeds.md)
* [Важная бизнес-аналитика](ui-extensions-essential-business-insights.md)
* [Анализатор изображений](ui-extensions-image-analyzer.md)
* [Интеллектуальное облако](ui-extensions-data-replication.md)
* [База интеллектуального облака](ui-extensions-intelligent-cloud.md)  
* [Прогнозы просрочки оплаты](ui-extensions-late-payment-prediction.md)
* [Microsoft Pay](ui-extensions-microsoft-pay-payments.md)
* [PayPal Payments Standard](ui-extensions-paypal-payments-standard.md)
* [Миграция данных QuickBooks](ui-extensions-quickbooks-data-migration.md)
* [Миграция данных QuickBooks Online](ui-extensions-quickbooks-online-data-migration.md)
* [Импорт файла зарплаты Quickbooks](ui-extensions-quickbooks-payroll.md)
* [Прогноз продаж и запасов](ui-extensions-sales-forecast.md)
* [Группа НДС](ui-extensions-vat-group.md)
* [WorldPay Payments Standard](ui-extensions-worldpay-payments-standard.md)
* [DK — Миграция данных C5](ui-extensions-c5-data-migration.md)
* [DK — Платежи и выверки](ui-extensions-payments-reconciliation-formats-dk.md)
* [DK — Форматы налоговой документации](ui-extensions-tax-file-formats-dk.md)
* [Расширение "Почтовые индексы Великобритании GetAddress.io"](LocalFunctionality/UnitedKingdom/ui-extensions-getaddressio.md)  
* [US/CA/UK/AU/NZ/ZA — Отправить авизо](ui-extensions-send-remittance-advice.md)

> [!NOTE]  
> Узнавать о новых расширениях от Майкрософт и других поставщиков можно по адресу [AppSource.microsoft.com](https://appsource.microsoft.com/marketplace/apps?product=dynamics-365%3Bdynamics-365-business-central&page=1).


## <a name="extensions-and-data-transfer"></a>Расширения и передача данных

Поскольку следующие расширения взаимодействуют с другими службами, они могут передавать данные за пределы географии среды [!INCLUDE[prod_short](includes/prod_short.md)]:

* Расширение AMC Banking 365 Fundamentals
* Анализатор изображений
* Прогнозирование просрочек оплаты
* PayPal Payments Standard
* Прогноз продаж и запасов
* WorldPay Payments Standard

Это также относится к некоторым функциям базового приложения, таким как следующие возможности:

* Прогноз движения денежных средств
* Служба обмена документами
* Подключения к Dataverse
* Сервис OCR
* Online Map
* Служба проверки ИНН в ЕС Сервис

## <a name="see-also"></a>См. также

[Настройка Business Central](ui-customizing-overview.md)  
[Расширения для Business Central от других поставщиков](ui-extensions-other.md)  
[Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md)  
[Включение платежей клиентов через PayPal](sales-how-enable-payment-service-extensions.md)  
[Миграция бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка расширения "Почтовые индексы Великобритании GetAddress.io"](LocalFunctionality/UnitedKingdom/uk-setup-postal-code-service.md)  
[Расширения [!INCLUDE[prod_short](includes/prod_short.md)] от других поставщиков](ui-extensions-other.md)  
[Подготовьтесь к ведению бизнеса](ui-get-ready-business.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]
