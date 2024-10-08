---
title: Ad-hoc-анализ данных по продажам
description: 'Узнайте, как использовать режим анализа данных для анализа данных продаж.'
author: brentholtorf
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '516, 9300, 5119, 9301, 9305'
ms.date: 04/28/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="ad-hoc-analysis-of-sales-data"></a>Ad-hoc-анализ данных по продажам

В этой статье поясняется, как использовать функцию **Анализ данных** для анализа данных по продажам непосредственно со страниц списков и из запросов. Вам не нужно запускать отчет или переходить в другое приложение, такое как Excel. Эта функция представляет собой интерактивный и универсальный механизм для выполнения вычислений, подведения итогов и изучения данных. Вместо создания отчетов с использованием различных параметров и фильтров вы можете добавить несколько вкладок, представляющих различные задачи с данными или представления данных. Например, это может быть представление «Мои клиенты», «Статистика продаж» или любое другое представление, которое может вам понадобиться. Подробнее о том, как использовать функцию **Анализ данных**, см. в статье [Анализ данных списков и запросов в режиме анализа](analysis-mode.md).

Используйте следующие страницы списков для ad-hoc-анализа процессов продаж:

- [Заказы на продажу](https://businesscentral.dynamics.com/?page=9305)
- Операции главной книги
- [Операции книги клиентов](https://businesscentral.dynamics.com/?page=25)
- Операции книги товаров
- Учтенные счета продажи
- Заказы на возврат продажи

## <a name="sales-ad-hoc-analysis-scenarios"></a>Сценарии ad-hoc-анализа данных по продажам

Используйте функцию **Анализ данных** для быстрой проверки фактов и ad-hoc-анализа:

- Если вы не хотите запускать отчет.
- Если отчета для стоящей перед вами задачи не существует.
- Если вы хотите быстро перебрать несколько вариантов для рассмотрения какой-либо составляющей вашего бизнеса.

В следующих разделах представлены примеры сценариев продаж в [!INCLUDE [prod_short](includes/prod_short.md)].

| С областями | Задача | Открыть в режиме анализа эту страницу | С использованием этих полей |
| ---- | ----- | ------------------------------- |------------------- |
| [Продажи (ожидаемый объем продаж)](#example-sales-expected-sales-volume) | Проанализировать ожидаемый объем продаж. | [Заказы на продажу](https://businesscentral.dynamics.com/?page=9305) | **Название покупателя**, **№ клиента покупателя**, **№** , **Сумма**, **Дата документа (год)** и **Дата документа (месяц)**. |
| [Продажи (продажи клиентам по объему)](#example-sales-customer-sales-by-volume) | Получить представление о клиентах, которые больше всего у вас покупают либо имеют наибольшую задолженность. | [Операции книги клиентов](https://businesscentral.dynamics.com/?page=25) | **Имя/название клиента**, **№ документа**, **Сумма** и **Сумма остатка**. |
| [Финансы (дебиторская задолженность)](#example-finance-accounts-receivables) | Посмотреть, сколько вам должны ваши клиенты, например с разбивкой по временным интервалам, когда наступает срок уплаты сумм. | [Операции книги клиентов](https://businesscentral.dynamics.com/?page=25) | **Имя/название клиента**, **Срок оплаты** и **Сумма остатка**. |

## <a name="example-sales-expected-sales-volume"></a>Пример: продажи (ожидаемый объем продаж)

Чтобы проанализировать ожидаемый объем продаж и суммы продаж по неотгруженным заказам для каждого клиента по годам или месяцам, выполните следующие действия:

1. Откройте список [Заказы на продажу](https://businesscentral.dynamics.com/?page=9305) и включите режим анализа.
1. Откройте меню **Столбцы** и удалите все столбцы (выберите флажок рядом с полем **Поиск**).
1. Включите **Сводный режим** (прямо над полем **Поиск**).
1. Перетащите поля **Название покупателя**, **№ клиента покупателя** и **№** в область **Группы строк**. Перетаскивайте поля именно в этом порядке.
1. Перетащите поле **Сумма** в область **Значения**.
1. Перетащите поля **Дата документа (год)** и **Дата документа (месяц)** в область **Метки столбцов**. Перетаскивайте поля именно в этом порядке.
1. Чтобы выполнить анализ за определенный год или квартал, примените фильтр в меню **Дополнительные фильтры**. Это меню находится в правой части страницы, прямо под меню **Столбцы**.
1. Переименуйте вкладку анализа в **Ожидаемый объем продаж** (или дайте ей другое название, характеризующее этот анализ).

## <a name="example-sales-customer-sales-by-volume"></a>Пример: продажи (продажи клиентам по объему)

Чтобы получить представление о клиентах, которые больше всего у вас покупают либо имеют наибольшую задолженность, выполните следующие действия:

1. Откройте список [Операции книги клиентов](https://businesscentral.dynamics.com/?page=25) и включите режим анализа.
1. Откройте меню **Столбцы** и удалите все столбцы (выберите флажок рядом с полем **Поиск**).
1. Перетащите поле **Имя/название клиента** в область **Группы строк**, а поле **№ документа** так, чтобы оно находилось под ней.
1. Выберите поля **Сумма** и **Сумма остатка**.
1. Чтобы выполнить анализ за определенный год или квартал, примените фильтр в меню **Дополнительные фильтры**. Это меню находится в правой части страницы, прямо под меню **Столбцы**.
1. Переименуйте вкладку анализа в **Клиенты по объему продаж** (или дайте ей другое название, характеризующее этот анализ).

На следующем рисунке показан результат выполнения этих действий.

:::image type="content" source="media/data-analysis-customer-ledger-entries.png" alt-text="Пример выполнения анализа данных на странице «Операции книги клиентов»." lightbox="media/data-analysis-customer-ledger-entries.png":::

## <a name="example-finance-accounts-receivables"></a>Пример: финансы (дебиторская задолженность)

Чтобы увидеть, сколько вам должны ваши клиенты, — возможно, с разбивкой срока уплаты соответствующих сумм по временным интервалам — выполните следующие действия:

1. Откройте список [Операции книги клиентов](https://businesscentral.dynamics.com/?page=25) и включите режим анализа.
1. Откройте меню **Столбцы** и удалите все столбцы (выберите флажок рядом с полем **Поиск**).
1. Включите **Сводный режим** (прямо над полем **Поиск**).
1. Перетащите поле **Имя/название клиента** в область **Группы строк**, а также перетащите поле **Сумма остатка** в область **Значения**.
1. Перетащите поле **Срок оплаты (месяц)** в область **Метки столбцов**.
1. Чтобы выполнить анализ за определенный год или квартал, примените фильтр в меню **Дополнительные фильтры**. Это меню находится в правой части страницы, прямо под меню **Столбцы**.
1. Переименуйте вкладку анализа в **Задолженность по месяцам** (или дайте ей другое название, характеризующее этот анализ).

## <a name="data-foundation-for-ad-hoc-analysis-on-sales"></a>Данные, используемые для ad-hoc-анализа в продажах

После ввода информации в заказ на продажу и добавления всех строк заказа на продажу заказ можно учесть. При учете заказа создаются расходная накладная и счет. [!INCLUDE [prod_short](includes/prod_short.md)] обновляет счет клиента, главную книгу и операции книги товаров:

- По каждому заказу на продажу в таблице **Операция ГК** создается операция продажи. Операция создается также в счете клиента в таблице **Книга операций клиентов**, а операция ГК создается в соответствующем счете дебеторской задолженности. Кроме этого, в результате учета заказа может быть создана операция НДС и операция главной книги на сумму скидки.
- Для каждой строки заказа на продажу создается операция книги товаров в таблице **Операция книги товаров** (если строки продажи содержат номера товаров) или операция главной книги в таблице **Операция ГК** (если строки продажи содержат счет ГК). В дополнение к этому заказы продажи всегда записываются в таблицах **Заголовок расходной накладной** и **Заголовок счета продаж**.

Подробнее об учете продаж см. в статье [Учет продаж](ui-post-sales.md).

## <a name="see-also"></a>См. также

[Учет продаж](ui-post-sales.md)  
[Анализ данных списков и запросов в режиме анализа](analysis-mode.md)  
[Обзор аналитики продаж](sales-analytics-overview.md)  
[Обзор анализа, бизнес-аналитики и отчетности](reports-bi-reporting.md)  
[Обзор продаж](sales-manage-sales.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
