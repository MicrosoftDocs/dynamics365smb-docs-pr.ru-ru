---
title: Ad-hoc-анализ данных запасов
description: 'Узнайте, как использовать режим анализа данных для анализа данных запасов.'
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '516, 9300, 5119, 9301, 9305'
ms.date: 05/03/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="ad-hoc-analysis-of-inventory-data"></a>Ad-hoc-анализ данных запасов

В этой статье поясняется, как использовать функцию **Анализ данных** для анализа данных по запасам непосредственно со страниц списков и из запросов. Вам не нужно запускать отчет или переходить в другое приложение, такое как Excel. Эта функция представляет собой интерактивный и универсальный механизм для выполнения вычислений, подведения итогов и изучения данных. Вместо создания отчетов с использованием различных параметров и фильтров вы можете добавить несколько вкладок, представляющих различные задачи с данными или представления данных. Например, это может быть представление «Запасы с истекающим сроком годности», «Товары, которые лучше всего продаются» или любое другое представление, которое может вам понадобиться. Подробнее о том, как использовать функцию **Анализ данных**, см. в статье [Анализ данных списков и запросов в режиме анализа](analysis-mode.md).

Используйте следующие страницы списков для ad-hoc-анализа процессов управления запасами:

- [Операции книги товаров](https://businesscentral.dynamics.com/?page=38)

## <a name="inventory-ad-hoc-analysis-scenarios"></a>Сценарии ad-hoc-анализа данных по запасам

Используйте функцию **Анализ данных** для быстрой проверки фактов и ad-hoc-анализа:

- Если вы не хотите запускать отчет.
- Если отчета для стоящей перед вами задачи не существует.
- Если вы хотите быстро перебрать несколько вариантов для рассмотрения какой-либо составляющей вашего бизнеса.

В следующих разделах представлены примеры сценариев управления запасами в [!INCLUDE [prod_short](includes/prod_short.md)].

| С областями | Задача | Открыть в режиме анализа эту страницу | С использованием этих полей |
| ---- | ----- | ------------------------------- |------------------- |
| [Запасы в наличии](#example-inventory-on-hand) | Получить представление о товарах, имеющихся в запасах. | [Операции книги товаров](https://businesscentral.dynamics.com/?page=38) | **№ товара**, **Оставшееся количество** |
|[Пример: отслеживание старых запасов или запасов с истекающим сроком годности](#example-track-expiring-or-old-stock) | Получить представление о товарах, которые находятся на складе в течение длительного времени и плохо продаются. | [Операции книги товаров](https://businesscentral.dynamics.com/?page=38) | **Дата учета (год)**, **Дата учета (месяц)**, **№ товара**, **Дата учета**, **Тип операции**, **Количество** и **Оставшееся количество**. |
| [Возвращенные товары по причине возврата](#example-returned-items-by-return-reason) | Получить представление о товарах, которые клиенты возвращают, с группированием по причинам возврата. Используется для контроля качества. | [Операции книги товаров](https://businesscentral.dynamics.com/?page=38) | **Код причины возврата**, **Дата учета (месяц)**, **Количество**, **Сумма себестоимости**, **Дата учета**, **Тип документа**, **№ товара** и **№ документа**. |
| Оборачиваемость запасов | Получить представление о закупках и продажах запасов по месяцам или кварталам. | [Операции книги товаров](https://businesscentral.dynamics.com/?page=38) | **Дата учета (год)**, **Дата учета (месяц)**, **№ товара**, **Количество**, **Сумма продаж**, **Сумма себестоимости (факт.)**, и **Дата учета (месяц)** |
| [Перемещения запасов] | Получить представление о том, как товары в запасах перемещаются между складами. | [Операции книги товаров](https://businesscentral.dynamics.com/?page=38) | **Код склада**, **Количество**, **Дата учета**, **№ товара** |

## <a name="example-inventory-on-hand"></a>Пример: запасы в наличии

Чтобы проанализировать товары, имеющиеся в наличии, выполните следующие действия:

1. Откройте список [Операции книги товаров](https://businesscentral.dynamics.com/?page=38) и выберите :::image type="content" source="media/analysis-mode-icon.png" alt-text="Перейти в режим анализа.":::, чтобы включить режим анализа.
1. Откройте меню **Столбцы** и удалите все столбцы (выберите флажок рядом с полем **Поиск**).
1. Перетащите поле **№ товара** в область **Группы строк**. Перетаскивайте поля именно в этом порядке.
1. Перетащите поле **Оставшееся количество** в область **Значения**.
1. Установите фильтр **Не равно** со значением **0** по полю **Оставшееся количество**. Если у вас не разрешены отрицательные уровни запасов, установите фильтр **Больше** со значением **0**.
1. При желании добавьте в анализ другие поля и, возможно, сведение по складу или другим полям.
1. Переименуйте вкладку анализа в **Запасы в наличии** (или дайте ей другое название, характеризующее этот анализ).

На следующем рисунке показан результат выполнения этих действий.

:::image type="content" source="media/data-analysis-inventory-on-hand.png" alt-text="Пример того, как проанализировать данные по наличию запасов." lightbox="media/data-analysis-inventory-on-hand.png":::

## <a name="example-track-expiring-or-old-stock"></a>Пример: отслеживание старых запасов или запасов с истекающим сроком годности

Чтобы проанализировать, какие товары находятся на складах в течение длительного времени и плохо продаются, выполните следующие действия:

1. Откройте список [Операции книги товаров](https://businesscentral.dynamics.com/?page=38) и выберите :::image type="content" source="media/analysis-mode-icon.png" alt-text="Перейти в режим анализа.":::, чтобы включить режим анализа.
1. Откройте меню **Столбцы** и удалите все столбцы (выберите флажок рядом с полем **Поиск** справа).
1. Перетащите поля **Дата учета (год)**, **Дата учета (месяц)** и **№ товара** в область **Группы строк**. Перетаскивайте поля именно в этом порядке.
1. В области **Столбцы** выберите поля **Дата учета**, **Тип операции**, **Количество** и **Оставшееся количество**.
1. Установите фильтр**Меньше** по полю **Дата учета**, чтобы определить, что вы понимаете под «старыми запасами».
1. Переименуйте вкладку анализа в **Старые запасы** (или дайте ей другое название, характеризующее этот анализ).

На следующем рисунке показан результат выполнения этих действий.

:::image type="content" source="media/data-analysis-inventory-dead-stock.png" alt-text="Пример проведения анализа для выявления залежалого товара на странице «Операции книги товаров»." lightbox="media/data-analysis-inventory-dead-stock.png":::

## <a name="example-returned-items-by-return-reason"></a>Пример: возвращенные товары по причине возврата

Чтобы проанализировать возвращенные товары и отсортировать их по причинам возврата, выполните следующие действия:

1. Откройте список [Операции книги товаров](https://businesscentral.dynamics.com/?page=38).
1. Добавьте поле **Код причины возврата** путем персонализации страницы. В меню **Настройки** выберите **Персонализация**.
1. Выйдите из режима персонализации.
1. Выберите :::image type="content" source="media/analysis-mode-icon.png" alt-text="Перейти в режим анализа."::: чтобы включить режим анализа.
1. Откройте меню **Столбцы** и удалите все столбцы (выберите флажок рядом с полем **Поиск** справа).
1. Перетащите поля **Код причины возврата** и **Дата учета (месяц)** в область **Группы строк**. Перетаскивайте поля именно в этом порядке.
1. Перетащите поля **Количество** и **Сумма себестоимости** в область **Значения**.
1. Добавьте любые другие поля, которые вы хотите использовать в анализе, и включите их в области **Столбцы**. Например, имеет смысл добавить поля **Дата учета**, **Тип документа**, **№ товара** и **№ документа**.
1. Переименуйте вкладку анализа в **Возвращенные товары по причине возврата** (или дайте ей другое название, характеризующее этот анализ).  

## <a name="example-inventory-throughput"></a>Пример: оборачиваемость запасов

1. Откройте список [Операции книги товаров](https://businesscentral.dynamics.com/?page=38) и выберите :::image type="content" source="media/analysis-mode-icon.png" alt-text="Перейти в режим анализа.":::, чтобы включить режим анализа.
1. Откройте меню **Столбцы** и удалите все столбцы (выберите флажок рядом с полем **Поиск** справа).
1. Включите **Сводный режим** (над полем **Поиск** справа).
1. Перетащите поля **Дата учета (год)**, **Дата учета (месяц)** и **№ товара** в область **Группы строк**.
1. Перетащите поля **Количество**, **Сумма продажи** и **Сумма себестоимости (факт.)** в область **Значения**.
1. Перетащите поле **Дата учета (месяц)** в область **Группы столбцов**.
1. Переименуйте вкладку анализа в **Оборачиваемость запасов по месяцам** (или дайте ей другое название, характеризующее этот анализ).  

## <a name="inventory-movements"></a>Перемещения запасов

Чтобы отслеживать перемещение запасов между складами, выполните следующие действия:

1. Откройте список [Операции книги товаров](https://businesscentral.dynamics.com/?page=38) и выберите :::image type="content" source="media/analysis-mode-icon.png" alt-text="Перейти в режим анализа.":::, чтобы включить режим анализа.
1. Откройте меню **Столбцы** и удалите все столбцы (выберите флажок рядом с полем **Поиск** справа).
1. Перетащите поле **Код склада** в область **Группы строк**.
1. Перетащите поле **Количество** в область **Значения**.
1. Добавьте любые другие поля, которые вы хотите использовать в анализе, и включите их в области **Столбцы**. Например, имеет смысл добавить поле **№ товара**.
1. Переименуйте вкладку анализа в **Перемещения запасов** (или дайте ей другое название, характеризующее этот анализ).  

   > [!TIP]
   > Если вы добавите поле «Дата учета», вы также сможете отслеживать перемещения в динамике.

## <a name="data-foundation-for-ad-hoc-analysis-on-inventory"></a>Данные, используемые для ad-hoc-анализа запасов

При учете заказа на продажу [!INCLUDE [prod_short](includes/prod_short.md)] обновляет счет клиента, главную книгу и операции книги товаров.

- Для каждой строки заказа на продажу создается операция книги товаров в таблице **Операция книги товаров** (если строки продаж содержат номера товаров). В дополнение к этому заказы продажи всегда записываются в таблицах **Заголовок расходной накладной** и **Заголовок счета продаж**. Подробнее об учете продаж см. в статье [Учет продаж](ui-post-sales.md).

При учете документа покупки [!INCLUDE [prod_short](includes/prod_short.md)] обновляет счет поставщика, главную книгу (ГК), операции книги товаров и операции книги ресурсов.

- Для каждой строки покупки, если это применимо, создаются операции в таблице **Операция книги товаров** (если строка покупки относится к типу «Товар»). Кроме того, документы покупки всегда записываются в таблицах **Прих. накладная покупки - заголовок** и **Заголовок счета покупки**. Подробнее см. в статье [Учет покупок](purchasing-how-record-purchases.md#posting-purchases).

## <a name="see-also"></a>См. также

[Анализ данных списков и запросов в режиме анализа](analysis-mode.md)  
[Обзор аналитики запасов](inventory-analytics-overview.md)  
[Обзор анализа, бизнес-аналитики и отчетности](reports-bi-reporting.md)  
[Обзор запасов](inventory-manage-inventory.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]