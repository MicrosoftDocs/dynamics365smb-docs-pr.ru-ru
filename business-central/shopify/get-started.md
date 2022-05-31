---
title: Начало работы с соединителем для Shopify
description: Первые шаги при настройке соединения между Business Central и Shopify
ms.date: 05/16/2022
ms.topic: article
ms.service: dynamics365-business-central
ms.reviewer: solsen
author: AndreiPanko
ms.author: andreipa
ms.openlocfilehash: 2b88995cad8cfe0c3688ca062643f2d339fed9bf
ms.sourcegitcommit: f071aef3660cc3202006e00f2f790faff849a240
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "8768155"
---
# <a name="get-started-with-the-shopify-connector"></a>Начало работы с соединителем Shopify

[!INCLUDE [prod_short](../includes/prod_short.md)] обеспечивает гибкость для подключения к нему вашего магазина (магазинов) Shopify, чтобы максимально повысить эффективность вашего бизнеса. Вы можете просматривать информацию о своем бизнесе и интернет-магазине Shopify и управлять всеми этими данными с помощью соединителя Shopify. Чтобы использовать Shopify с [!INCLUDE [prod_short](../includes/prod_short.md)], вам нужно выполнить несколько шагов. Эта страница служит руководством для завершения интеграции вашего магазина Shopify с [!INCLUDE [prod_short](../includes/prod_short.md)].

## <a name="prerequisites-for-shopify"></a>Предварительные требования для Shopify

У вас должны быть:

- учетная запись Shopify
- интернет-магазин Shopify

Чтобы создать новую учетную запись Shopify или зарегистрироваться для получения бесплатной 14-дневной пробной версии, перейдите на страницу [Shopify](https://www.shopify.com/). Для получения дополнительной информации о том, как создать и персонализировать свой интернет-магазин, см. [Центр справки Shopify](https://help.shopify.com/).
  
- Поддерживаются и другие каналы продаж, например POS-терминалы Shopify.

### <a name="recommended-settings"></a>Рекомендуемые параметры

- Деактивируйте параметр **Автоматически архивировать заказ** в разделе **Обработка заказов** в настройках [**Оформление заказа**](https://www.shopify.com/admin/settings/checkout) в **центре администрирования Shopify**.

Чтобы узнать больше о настройках Shopify для демонстрационных и пробных сценариев, см. раздел [Тестовые и обучающие сценарии](/dynamics365/business-central/dev-itpro/administration/admin-shopify-connector#preparation).

## <a name="prerequisites-for-business-central"></a>Предварительные требования для Business Central

- Убедитесь, что у вас установлено расширение **Подключение к Shopify для [!INCLUDE[prod_short](../includes/prod_short.md)]**.

Расширение предварительно устанавливается для всех новых учетных записей и пробных версий. Если вам нужно установить расширения из Marketplace, посетите страницу [Установка и удаление расширений](../ui-extensions-install-uninstall.md#install). Выполните шаги, перечисленные ниже, если у вас нет [!INCLUDE[prod_short](../includes/prod_short.md)].
<!--
## Installing the **Dynamics 365 Business Central** app to your Shopify online store

For existing [!INCLUDE[prod_short](../includes/prod_short.md)], this step is optional and can be skipped.

1. Locate the [Dynamics 365 Business Central](https://apps.shopify.com/dynamics-365-business-central) app on the [Shopify AppStore](https://apps.shopify.com/)
2. Choose the **Add App** button. Sign-in into your Shopify account if prompted. Select the required online shop if you've more than one.
3. After reviewing privacy and permissions, choose the **Install App** button.
  You can find and open the installed **Dynamics 365 Business Central** app in the **Apps** section on the sidebar of **Shopify admin**.
4. Choose **Sign up now** to start [!INCLUDE[prod_short](../includes/prod_short.md)] trial or **Sign in** if you already have [!INCLUDE[prod_short](../includes/prod_short.md)]. You'll be redirected to your [!INCLUDE[prod_short](../includes/prod_short.md)] at [Business Central](https://businesscentral.dynamics.com).
5. The next steps should be done in [!INCLUDE[prod_short](../includes/prod_short.md)].
-->
## <a name="connecting-business-central-to-the-shopify-online-store"></a>Подключение Business Central к интернет-магазину Shopify

1. Нажмите на значок поиска ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../media/ui-search/search_small.png "Что вы хотите сделать"), значок, введите **магазин Shopify** и выберите связанную ссылку.
2. Выберите действие **Создать**.  
3. В поле **Код** укажите нужный код.  
4. В поле **URL-адрес Shopify** введите адрес вашего интернет-магазина, который необходимо подключить.
5. Установите переключатель в положение **Включено**, а затем посмотрите и примите условия использования.
6. При появлении запроса войдите в свою учетную запись Shopify, проверьте конфиденциальность и разрешения, а затем нажмите кнопку **Установить приложение**.

Повторите шаги 2–6 для всех интернет-магазинов, которые хотите подключить.

### <a name="next-steps"></a>Дальнейшие шаги

Теперь ваш интернет-магазин подключен к [!INCLUDE[prod_short](../includes/prod_short.md)]. На следующих этапах вы определите, как и что синхронизировать.

- [Синхронизация товаров](synchronize-items.md)
- [Синхронизация клиентов](synchronize-customers.md)
- [Синхронизация заказов](synchronize-orders.md)

## <a name="see-also"></a>См. также

[Тестовые и обучающие сценарии](/dynamics365/business-central/dev-itpro/administration/admin-shopify-connector).

