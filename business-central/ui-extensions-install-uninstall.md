---
title: Установка и удаление расширений в Business Central | Документация Майкрософт
description: Узнайте об установке и удалении расширений в Business Central.
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: app, add-in, manifest, customize, install, uninstall
ms.date: 10/01/2020
ms.author: solsen
ms.openlocfilehash: a0e62b60f9624cad44efa7fd42c5840a2ecd07b5
ms.sourcegitcommit: aea079b66e35c447bf31a11ffc2069cfdaf2ef38
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2020
ms.locfileid: "3970364"
---
# <a name="installing-and-uninstalling-extensions-in-business-central"></a>Установка и удаление расширений в Business Central

Вы можете изменить [!INCLUDE[d365fin](includes/d365fin_md.md)] за счет установки расширений, которые, например, добавляют функциональность, изменяют поведение или предоставляют доступ к новым интернет-службам. Дополнительные сведения см. в разделе [Настройка Business Central с помощью расширений](ui-extensions.md).

> [!NOTE]
> Чтобы установить расширения из AppSource или добавить расширения для каждого арендатора, у вас должны быть соответствующие разрешения. Вы должны быть либо участником группы пользователей D365 EXTENSION MGMT, либо у вас должен быть установлен набор разрешений D365 EXTENSION MGMT. Если вы являетесь администратором, вы можете назначать группы пользователей и разрешения другим пользователям в вашей компании.<br /><br />
Чтобы использовать функциональную возможность, предоставляемую расширением, такую как открытие страниц, запуск отчетов, выбор действий и т. п., необходимо назначить наборы разрешений, которые устанавливаются как часть расширения.

## <a name="installing-an-extension"></a>Установка расширения

Управление расширениями осуществляется на странице **Управление расширениями**. Эта страница доступна с начальной страницы. Также можно выбрать значок **Поиск страницы или отчета** ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать") в правом верхнем углу, ввести **Расширение**, а затем выбрать соответствующую ссылку.  

Новые расширения можно получить из магазина по адресу [AppSource.microsoft.com](https://go.microsoft.com/fwlink/?linkid=2081646). Здесь отображаются все доступные расширения для [!INCLUDE[d365fin](includes/d365fin_md.md)], и можно получить приложения, расширения и пакеты содержимого для других продуктов Майкрософт. Установите соответствующие фильтры, просмотрите информацию для каждого расширения и получите расширение для [!INCLUDE[d365fin](includes/d365fin_md.md)].  

> [!NOTE]  
> Войдите на сайт [AppSource.microsoft.com](https://appsource.microsoft.com/), используя учетную запись электронной почты, которая используется для [!INCLUDE[d365fin](includes/d365fin_md.md)]. Для удобства используйте эту же учетную запись для других служб и продуктов.  

Можно также перейти в магазин из [!INCLUDE[d365fin](includes/d365fin_md.md)]. На странице **Управление расширениями** отображаются все текущие установленные расширения, и можно открыть страницу **Магазин расширений**, на которой отображаются расширения для [!INCLUDE[d365fin](includes/d365fin_md.md)], доступные на данный момент на сайте AppSource. Если выбрать ссылку *Еще приложения*, производится переход на сайт [AppSource.microsoft.com](https://go.microsoft.com/fwlink/?linkid=2081646).  

Если вы выберите расширение, вы можете прочитать о его возможностях и открыть справку по расширению для получения более подробной информации. Если вы хотите получить расширение, необходимо согласиться с условиями использования. Если вы получили расширение с веб-сайта AppSource, для завершения установки выполняется вход в [!INCLUDE[d365fin](includes/d365fin_md.md)].  

При установке расширения может потребоваться настроить его, например указать учетную запись для использования расширения **PayPal Payments Standard для [!INCLUDE[d365fin](includes/d365fin_md.md)]**.
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
* [UK — Почтовые индексы Великобритании GetAddress.io](ui-extensions-getaddressio.md)
* [US/CA/UK/AU/NZ/ZA — Отправить авизо](ui-extensions-send-remittance-advice.md)

## <a name="uninstalling-an-extension"></a>Удаление расширения

Вы удаляете расширение с помощью страницы **Управление расширениями**. Если вы удалили расширение, а потом передумали, вы можете снова установить его. При удалении расширения, которое вы использовали, данные по умолчанию сохраняются, чтобы вы могли установить его снова. Вместо этого вы можете удалить данные с расширением. Это контролируется флажком **Удалить данные расширения**. По умолчанию этот флажок *не установлен*.

> [!IMPORTANT]  
> Если вы установите флажок **Удалить данные расширения**, вы получите диалоговое окно подтверждения, и вы должны выбрать **ОК**. С установленным флажком **Удалить данные расширения** теперь вы можете удалить расширение, и вам будет предложено еще раз подтвердить, что вы хотите удалить расширение и удалить данные. Отменить это действие невозможно.
Некоторые расширения являются обязательными. Удалить эти расширения со страницы **Управление расширениями** нельзя. Если вы попытаетесь это сделать, появится сообщение об ошибке.  

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
