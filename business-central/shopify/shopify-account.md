---
title: Создание и настройка учетной записи Shopify
description: 'Узнайте, как получить учетную запись Shopify, чтобы продемонстрировать рабочий процесс интеграции Shopify и Business Central.'
ms.date: 03/04/2024
ms.topic: article
ms.service: dynamics-365-business-central
ms.search.form: '30101, 30102'
ms.reviewer: bholtorf
author: brentholtorf
ms.author: bholtorf
---

# <a name="create-and-set-up-a-shopify-account"></a>Создание и настройка учетной записи Shopify



Если вы рассматриваете возможность использования Shopify в качестве решения для электронной коммерции и вам нужна учетная запись Shopify для проверки интегрированного рабочего процесса, вы можете поступить следующим образом:

- Получить пробную версию. Это типичная отправная точка для конечных пользователей.  
- Создать магазины разработки. Этот подход предназначен для партнеров, которые регулярно проводят демонстрации, тренинги и оказывают поддержку.

## <a name="trial-end-user"></a>Пробная версия (конечный пользователь)

Перейдите на [веб-сайт Shopify](https://www.shopify.com) и используйте свою учетную запись электронной почты в качестве учетной записи администратора, чтобы подписаться на бесплатную пробную версию. Подробнее о том, как создать и персонализировать свой интернет-магазин, см. в [справочном центре Shopify](https://help.shopify.com/).

В разделе **Администрирование Shopify** созданного магазина примените следующие **Настройки**:

- Выберите план в параметрах [**План**](https://www.shopify.com/admin/settings/plan), чтобы протестировать процесс оплаты.

- Рекомендуем включить функцию *Show login link in the header of onilne store and checkout* в разделе **Accounts in online store and checkout** в параметрах [**учетных записей клиентов**](https://www.shopify.com/admin/settings/customer_accounts) на **портале администрирования Shopify**.
- Рекомендуем выбрать параметр *New customer account* в разделе **Accounts in online store and checkout** параметров учетных записей клиентов.
- Рекомендуем включить функцию *Self-serve returns* в разделе **New customer accounts** параметров учетных записей клиентов.

- Активировать тестовые платежи. В этом случае у вас есть два варианта. Для начала перейдите в параметры [**Платежей**](https://www.shopify.com/admin/settings/payments):  
  1. *(для тестирования) Bogus Gateway*. Дополнительные сведения см. в разделе [Активация Bogus Gateway для тестирования](https://help.shopify.com/en/manual/checkout-settings/test-orders#place-a-test-order-by-simulating-a-transaction).
  2. *Shopify Payments* в режиме тестирования. Дополнительные сведения см. в разделе [Тестирование Shopify Payments](https://help.shopify.com/en/manual/payments/shopify-payments/testing-shopify-payments).

- Деактивируйте параметр **Автоматически архивировать заказ** в разделе **Обработка заказов** в настройках [**Оформление заказа**](https://www.shopify.com/admin/settings/checkout) в **центре администрирования Shopify**.
- Рекомендуем выбрать параметр *Название компании — необязательно* в разделе **Информация о клиенте** в настройках оформления заказа.
- Включите параметр **Показывать варианты чаевых при оформлении заказа** в разделе **Чаевые** в параметрах оформления заказа, если вы планируете демонстрировать чаевые.

> [!Important]  
> Чтобы избежать платежей, не забудьте отменить пробную версию Shopify.

## <a name="development-store"></a>Магазин разработки

Начните с присоединения к [Партнерской программе Shopify](https://help.shopify.com/partners/about). После этого используйте **Панель мониторинга партнера**, чтобы создать магазин разработки. Подробнее см. в статье [Создание магазинов разработки](https://help.shopify.com/partners/dashboard/managing-stores/development-stores).

После создания магазина в разделе **Администрирование Shopify** созданного магазина примените следующие **Настройки**:

- Рекомендуем включить функцию *Show login link in the header of onilne store and checkout* в разделе **Accounts in online store and checkout** в параметрах [**учетных записей клиентов**](https://www.shopify.com/admin/settings/customer_accounts) на **портале администрирования Shopify**.
- Рекомендуем выбрать параметр *New customer account* в разделе **Accounts in online store and checkout** параметров учетных записей клиентов.
- Рекомендуем включить функцию *Self-serve returns* в разделе **New customer accounts** параметров учетных записей клиентов.
  
- Активировать тестовые платежи. У вас есть два варианта. Для начала перейдите в параметры [**Платежей**](https://www.shopify.com/admin/settings/payments):  
  1. *(для тестирования) Bogus Gateway*. Дополнительные сведения см. в разделе [Активация Bogus Gateway для тестирования](https://help.shopify.com/en/manual/checkout-settings/test-orders#place-a-test-order-by-simulating-a-transaction).
  2. *Shopify Payments* в режиме тестирования. Подробнее см. в разделе [Тестирование Shopify Payments](https://help.shopify.com/en/manual/payments/shopify-payments/testing-shopify-payments).
     
- Деактивируйте параметр **Automatically archive the order** в разделе **Order Processing** параметров [**оформления заказа**](https://www.shopify.com/admin/settings/checkout) на **портале администрирования Shopify**.
- Рекомендуем выбрать параметр *Company name - Optional* в разделе **Customer information** в параметрах оформления заказа.
- Включите параметр **Показывать варианты чаевых при оформлении заказа** в разделе **Чаевые** в параметрах оформления заказа, если вы планируете демонстрировать чаевые.


> [!Note]  
> Используемые для разработки магазины обычно защищены паролем. Когда вы пытаетесь открыть определенную страницу в своем интернет-магазине из [!INCLUDE [prod_short](../includes/prod_short.md)] — например, чтобы перейти к определенному продукту или заказу — вам потребуется ввести свой пароль. Во время тестирования, чтобы не вводить пароль, войдите в систему на портале администрирования Shopify и откройте свой магазин оттуда. Вам не нужно будет вводить пароль магазина, пока вы не закроете браузер или пока не истечет время вашего сеанса.  

## <a name="see-also"></a>См. также

[Начало работы с соединителем Shopify](get-started.md)  
[Пошаговое руководство: настройка и использование соединителя Shopify](walkthrough-setting-up-and-using-shopify.md)
