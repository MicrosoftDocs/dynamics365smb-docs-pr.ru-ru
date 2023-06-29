---
title: Часто задаваемые вопросы по техническим сведениям
description: 'Детали реализации, связанные с соединителем Shopify.'
ms.date: 03/27/2023
ms.topic: article
ms.service: dynamics365-business-central
author: AndreiPanko
ms.author: andreipa
---

# <a name="faq-for-technical-details"></a><a name="faq-for-technical-details"></a>Часто задаваемые вопросы по техническим сведениям

Эта статья содержит ответы на вопросы о соединителе Shopify.

## <a name="what-is-shopify"></a><a name="what-is-shopify"></a>Что такое Shopify?

Shopify — это приложение на основе подписки, которое позволяет любому настроить интернет-магазин и продавать свою продукцию. Платформа Shopify предлагает интернет-магазинам пакет услуг для платежей, маркетинга, доставки и взаимодействия с клиентами.

## <a name="what-is-the-microsoft-dynamics-365-business-central-shopify-connector"></a><a name="what-is-the-microsoft-dynamics-365-business-central-shopify-connector"></a>Что такое соединитель Microsoft Dynamics 365 Business Central Shopify?

С помощью соединителя Shopify компании могут подключать свой магазин (или магазины) Shopify к [!INCLUDE[prod_short](../includes/prod_short.md)], чтобы максимально повысить эффективность бизнеса. Используя соединитель Shopify, они могут получать доступ к ценной информации о своем бизнесе и интернет-магазине Shopify и управлять всеми этими данными как единым блоком.

### <a name="capabilities"></a><a name="capabilities"></a>Возможности

- Поддержка нескольких магазинов Shopify
  - Каждый магазин имеет свою собственную настройку, включая набор продуктов, местоположения, используемые для расчета запасов, и прайс-листы.  
- Двунаправленная синхронизация товаров или продуктов
  - Соединитель синхронизирует изображения, варианты товаров, штрих-коды, номера товаров поставщиков, расширенные тексты и теги.  
  - Экспортируйте атрибуты товаров в Shopify.  
  - Используйте выбранные ценовые группы и скидки клиентов для определения цен, экспортируемых в Shopify.  
  - Решите, могут ли товары создаваться автоматически, или разрешите только обновления существующих продуктов.  
- Синхронизация уровней запасов
  - Выберите некоторые или все доступные местоположения в [!INCLUDE [prod_short](../includes/prod_short.md)].  
  - Обновите уровни запасов в нескольких местах в Shopify.  
- Двунаправленная синхронизация клиентов
  - Выполняйте умное сопоставление клиентов по телефону и электронной почте.  
  - Используйте шаблоны для конкретной страны при создании клиентов, что поможет обеспечить правильность налоговых настроек.  
- Импорт заказов из Shopify
  - Включите заказы, созданные в разных каналах продаж, таких как интернет-магазин или **POS-терминал Shopify**.
  - Стоимость доставки, подарочные карты, советы, способы доставки и оплаты, транзакции и риск мошенничества.  
  - Во время импорта вы можете автоматически создавать клиентов в [!INCLUDE [prod_short](../includes/prod_short.md)] или по своему усмотрению управлять клиентами в Shopify.  
  - Получайте информацию о платежах из Shopify Payments.
- Отслеживание информации о выполнении заказов
  - При желании можно передавать информацию о трассировке товаров из [!INCLUDE [prod_short](../includes/prod_short.md)] в Shopify.  

## <a name="why-did-microsoft-and-shopify-form-this-partnership"></a><a name="why-did-microsoft-and-shopify-form-this-partnership"></a>Почему Microsoft и Shopify создали это партнерство?

[!INCLUDE[prod_short](../includes/prod_long.md)] кооперируется с Shopify, чтобы помочь нашим клиентам создать лучший интерфейс покупок. Shopify предоставляет торговым организациям простое в использовании решение для коммерции, а [!INCLUDE[prod_short](../includes/prod_short.md)] предлагает комплексное решение для бизнес-управления финансами, продажами, сервисом и операциями. Вы можете использовать бесшовное соединение между приложениями для синхронизации заказов, запасов и информации о клиентах, что позволит вам быстрее выполнять заказы и лучше обслуживать клиентов.

## <a name="which-microsoft-products-are-the-shopify-connector-available-for"></a><a name="which-microsoft-products-are-the-shopify-connector-available-for"></a>Для каких продуктов Microsoft доступен соединитель Shopify?

Эта функция доступна только для [!INCLUDE[prod_short](../includes/prod_short.md)] Online, начиная с версии 20.1. Она не доступна для локальных развертываний. Соединитель предварительно устанавливается для новых сред. Организации с существующими средами могут скачать и установить соединитель из AppSource. Организация должна иметь как лицензию [!INCLUDE [prod_short](../includes/prod_short.md)], так и лицензию Shopify для использования соединителя. Чтобы узнать больше о поддерживаемых странах, языках и выпусках [!INCLUDE[prod_short](../includes/prod_short.md)], перейдите к разделу [Соединитель Shopify в AppSource](https://go.microsoft.com/fwlink/?linkid=2196238).

Соединитель Shopify не работает с [внедренными приложениями](/dynamics365/business-central/dev-itpro/deployment/embed-app-overview), где URL-адрес клиента имеет формат: `https://[application name].bc.dynamics.com`.

## <a name="what-support-is-offered-for-the-shopify-connector"></a><a name="what-support-is-offered-for-the-shopify-connector"></a>Какая поддержка предлагается для соединителя Shopify?

### [!INCLUDE[prod_short](../includes/prod_short.md)]

Соединитель Shopify покрывается текущей моделью поддержки. Дополнительные сведения см. в разделе [Техническая поддержка](/dynamics365/business-central/dev-itpro/administration//manage-technical-support) (только на английском языке).

Получите помощь от консультанта, который знаком с соединителем Shopify для [!INCLUDE[prod_short](../includes/prod_short.md)], чтобы удовлетворить ваши уникальные бизнес-требования. Выполните поиск в разделе [Консультационные услуги](https://aka.ms/BCShopifyConsultant).

### <a name="shopify"></a><a name="shopify"></a>Shopify

Получите помощь с Shopify на сайте [Общий центр справки Shopify](https://help.shopify.com/) или [Круглосуточная ежедневная поддержка вашего магазина как торгового предприятия Shopify](https://help.shopify.com/questions#/).

Вы также можете изучить [Площадку экспертов](https://experts.shopify.com/), чтобы найти нужных экспертов, которые предлагают услуги продавцам Shopify.

## <a name="currently-unsupported-features-however-were-tracking-them-and-may-consider-adding-them"></a><a name="currently-unsupported-features-however-were-tracking-them-and-may-consider-adding-them"></a>Не поддерживаемые в настоящее время функции, которые мы отслеживаем и можем рассмотреть возможность их добавления:

- Функции B2B, включая компании, прайс-листы компаний и условия оплаты
- Рынки
  - Разные переводы основных данных. Вы можете выбрать один язык, который будет использоваться для экспорта информации о продукте.
  - Цены для страны или региона. Для выбранной валюты доступен один прайс-лист. Shopify осуществляет конвертацию в другие валюты.

## <a name="is-the-shopify-connector-extensible"></a><a name="is-the-shopify-connector-extensible"></a>Является ли соединитель Shopify расширяемым?

Да, соединитель Shopify является расширяемым. Посетите GitHub, чтобы получить доступ к [списку точек расширяемости](https://github.com/microsoft/ALAppExtensions/tree/main/Apps/W1/Shopify) и изучить некоторые [примеры](https://github.com/microsoft/ALAppExtensions/blob/main/Apps/W1/Shopify/extensibility_examples.md).

## <a name="is-the-shopify-connector-open-for-contribution"></a><a name="is-the-shopify-connector-open-for-contribution"></a>Может ли сообщество вносить свои изменения в соединитель Shopify?

Да, это расширение открыто для внесения улучшений нашим сообществом. Вы можете найти [исходный код](https://github.com/microsoft/ALAppExtensions/tree/main/Apps/W1/Shopify) в репозитории надстроек приложения Microsoft AL.

## <a name="see-also"></a><a name="see-also"></a>См. также

[Начало работы с соединителем для Shopify](get-started.md)  
