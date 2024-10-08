---
title: Финансовая аналитика
description: 'Business Central позволяет собирать, анализировать и совместно использовать данные организации для получения бизнес-аналитики.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '103, 108, 198, 490'
ms.date: 03/27/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="financial-analytics"></a>Финансовая аналитика

Предприятия собирают огромное количество данных в ходе повседневной деятельности, что обеспечивает ценную бизнес-аналитику (BI) для лиц, принимающих решения:

- Цифры продаж
- Покупки
- Эксплуатационные расходы
- Зарплата сотрудников
- Бюджеты

[!INCLUDE[prod_short](includes/prod_short.md)] содержит множество функций, помогающих собирать, анализировать и совместно использовать финансовые данные организации:

- Бухгалтерская отчетность (для бухгалтерской отчетности и КПЭ)
- Ad-hoc-анализ списков
- Ad-hoc-анализ данных в Excel (с использованием открытия в Excel)
- Встроенные бухгалтерские отчеты

Каждая из этих функций имеет свои преимущества и недостатки в зависимости от типа анализа данных и роли пользователя. Чтобы узнать больше, перейдите к статье [Обзор аналитики, бизнес-аналитики и отчетности](reports-bi-reporting.md).

В этой статье рассказывается, как вы можете использовать эти аналитические функции для получения финансовой аналитики.

## <a name="analytics-needs-in-finance"></a>Потребности в аналитике в области финансов

Рассматривая потребности в аналитике в области финансов, имеет смысл использовать модель, основанную на высокоуровневых ролей пользователей и их потребностях в аналитике.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg" alt-text="Иллюстрация разных персонажей для аналитики" lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg":::

Люди, занимающие разные роли, имеют разные потребности в данных и используют их по-разному. Например, люди из финансовой сферы взаимодействуют с данными иначе, чем люди из отдела продаж.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg" alt-text="Иллюстрация того, как разные персонажи имеют разные потребности в аналитике." lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg":::

| Роль              | Агрегирование данных  | Типичные способы потребления данных                          | 
|-------------------|-------------------| ----------------------------------------------------- |
|Финансовый директор/генеральный директор          | Данные об эффективности  | КПЭ <br> Панели мониторинга <br> Бухгалтерские отчеты           |
|Управление финансами | Тенденции, сводки | Встроенные управленческие отчеты <br> Ad-hoc-анализ      | 
|Бухгалтер         | Подробные данные     | Встроенные операционные отчеты <br> Данные задачи на экране |

## <a name="finance-kpis"></a>Финансовые ключевые показатели эффективности

Ключевой показатель эффективности (КПЭ) — это измеримая величина, которая показывает, насколько эффективно вы достигаете своих целей. В сфере финансов люди часто используют следующие ключевые показатели эффективности для мониторинга финансового состояния своей организации:

- Коэф. вал. прибыли
- Чистая удельная прибыль
- Рабочий капитал
- Коэффициент текущей ликвидности/норма ликвидности
- Финансовое плечо, также известное как мультипликатор капитала
- Отношение заемного капитала к собственному
- Общий оборот активов
- Рентабельность капитала
- Рентабельность активов

<!-- Not ready to publish yet
For more information, see [Financial KPIs in Business Central](bi-finance-kpis.md) 
-->

## <a name="using-financial-reporting-to-produce-financial-statements-and-kpis"></a>Использование финансовой отчетности для создания финансовых отчетов и ключевых показателей эффективности

Функция **Финансовые отчеты** предоставляет аналитику финансовых данных, отображаемых в вашем плане счетов. Вы можете настроить финансовые отчеты для анализа цифры на счетах главной книги (ГК) и сравнивать операции главной книги с операциями бюджета. Результаты отображаются на диаграммах и в отчетах на домашней странице, таких как диаграмма движения денежных средств и отчет о прибылях и убытках или балансовый отчет.

Измерения играют важную роль в бизнес-аналитике. Измерением называются данные, которые можно добавлять в операции в качестве параметра. Измерения позволяют группировать операции, имеющие схожие характеристики, для упрощения их анализа. Например, это могут быть группы клиентов, регионов, продуктов и менеджеров по продажам. Кроме того, измерения могут использоваться при определении аналитических представлений и создании бухгалтерских отчетов. Подробнее см. в статье [Работа с измерениями](finance-dimensions.md).

> [!TIP]
> Для быстрого анализа транзакционных данных можно фильтровать итоговые суммы в планах счетов и все операции на страницах **Операции** по измерениям. Найдите действие **Установить фильтр измерений**.  

В следующей таблице приводится последовательность задач в финансовой отчетности со ссылками на статьи, в которых они описываются.  

| По | Ссылка |
| --- | --- |
| Создание новых бухгалтерских отчетов для определения финансовых документов для отчетности или для отображения в виде диаграмм.| [Подготовка бухгалтерской отчетности с использованием финансовых данных и категорий счетов](bi-how-work-account-schedule.md)|
| Используйте статистические счета для добавления информации в финансовые отчеты. Статистические счета позволяют добавлять показатели, основанные на нетранзакционных данных. Вы можете добавить нетранзакционные данные в числовых единицах, например численность сотрудников, площадь в квадратных метрах или количество клиентов с просроченными счетами. | [Анализ данных с помощью статистических счетов](bi-use-statistical-accounts.md) |
| Узнайте, как настроить новый финансовый отчет на примерах. | [Пошаговое руководство. Использование бухгалтерской отчетности для создания прогнозов движения денежных средств](walkthrough-making-cash-flow-forecasts-by-using-account-schedules.md) |
| Анализ ваших финансовых показателей путем настройки ключевых показателей эффективности (КПЭ) на основе бухгалтерских отчетов с их последующей публикацией в виде веб-служб. Опубликованные КПЭ на основе бухгалтерских отчетов можно просматривать на веб-сайте или импортировать в Microsoft Excel с помощь веб-служб OData. |[Настройка и публикация веб-служб ключевых показателей эффективности, которые основаны на финансовых отчетах](bi-how-to-set-up-and-publish-kpi-web-services-based-on-account-schedules.md) |
| Настройка представлений для анализа данных с помощью измерений.|[Анализ данных по измерениям](bi-how-analyze-data-dimension.md)|
| Создание новых аналитических отчетов для продаж, покупок и запасов, а также настройка шаблонов анализа. |[Создание аналитических отчетов](bi-how-create-analysis-views-reports.md)|

## <a name="finance-reporting-across-business-units-or-legal-entities"></a>Бухгалтерская отчетность по филиалам или юридическим лицам

Некоторые организации используют [!INCLUDE [prod_short](includes/prod_short.md)] в нескольких бизнес-подразделениях или юридических лицах. Другие используют [!INCLUDE [prod_short](includes/prod_short.md)] в дочерних компаниях, которые должны отчитываться перед головными организациями. [!INCLUDE [prod_short](includes/prod_short.md)] предоставляет бухгалтерам инструменты для облегчения переноса операций главной книги из двух или более организаций (дочерних компаний) в консолидированную организацию.  

Чтобы узнать больше, перейдите в раздел [Консолидация компаний](finance-consolidated-company-reporting.md).

## <a name="ad-hoc-analysis-of-finance-data"></a>Ad-hoc-анализ финансовых данных

Иногда вам просто нужно проверить, правильно ли складываются цифры, или быстро подтвердить цифру. Следующие функции отлично подходят для специального анализа:

- Анализ данных на страницах списка книги учета
- Открытие списков в Excel

Функция анализа данных позволяет открыть практически любую страницу списка, например страницы "Операции главной книги", "Операции книги учета основных средств", "Операции книги учета чеков" или "Операции книги учета банковских счетов", перейти в режим анализа, а затем группировать, фильтровать и сводить данные так, как вам нужно.

:::image type="content" source="media/data-analysis-gl-entries.png" alt-text="Пример выполнения анализа данных на странице записей главной книги." lightbox="media/data-analysis-gl-entries.png":::

Аналогичным образом вы можете использовать действие **Открыть в Excel**, чтобы открыть страницу списка для записей книги учета, при необходимости отфильтровать список для получения подмножества данных, а затем использовать Excel для работы с данными. Например, с помощью таких функций, как «Анализ данных», «Анализ "что, если"» или «Таблица прогнозов».

:::image type="content" source="media/open-in-excel-gl-entries.png" alt-text="Пример выполнения анализа данных на данных записей главной книги в Excel." lightbox="media/open-in-excel-gl-entries.png":::

> [!TIP]
> Если у вас настроен OneDrive для системных функций, книга Excel открывается в браузере с помощью Excel для Интернета. 


Для получения дополнительной информации о том, как выполнять ad-hoc-анализ книг, см. статью [Ad-hoc-анализ финансовых данных](ad-hoc-analysis-finance.md). 

## <a name="built-in-reports-for-finance"></a>Встроенные отчеты для сферы финансов

[!INCLUDE [prod_short](includes/prod_short.md)] включает несколько встроенных отчетов, функции отслеживания и инструменты, чтобы помочь аудиторам или контролерам, которые несут ответственность за отчетность перед финансовым отделом.

Чтобы получить обзор доступных отчетов, выберите **Все отчеты** на верхней панели вашей домашней страницы. Откроется обозреватель ролей, в котором показаны только функции группы **Отчет и анализ**. Подробнее см. в статье [Поиск отчетов с помощью обозревателя ролей](ui-role-explorer.md).

:::image type="content" source="media/report-explorer-finance.png" alt-text="Пример отчетов в финансовом ролевом центре." lightbox="media/report-explorer-finance.png":::

Встроенные отчеты бывают двух видов:

- Предназначен для печати (pdf).
- Предназначен для анализа в Excel.

Для получения дополнительной информации см. следующие обзоры отчетов, имеющих отношение к финансам.

- [Встроенные бухгалтерские отчеты в формате Excel](finance-analyze-excel.md)
- [Встроенные основные бухгалтерские отчеты](finance-reports.md)
- [Встроенные отчеты по основным средствам](fa-reports.md)
- [Встроенные отчеты по расчетам с клиентами](receivables-reports.md)
- [Встроенные отчеты по расчетам с поставщиками](payables-reports.md)

<!-- TODO: add when we have these articles
* [Built-in Cost Accounting reports](cost-accounting-reports.md) 
* [Built-in Cash Management reports](cost-accounting-reports.md) 
* [Built-in Tax and VAT reports](tax-and-vat-reports.md) 
-->

## <a name="on-screen-finance-task-pages"></a>Страницы финансовых задач на экране

В [!INCLUDE [prod_short](includes/prod_short.md)] есть несколько страниц, на которых можно получить представление о ситуации в финансах и задачах, которые необходимо выполнить.

### <a name="show-general-ledger-entries-and-balances-from-the-chart-of-accounts-page"></a>Отображение записей и остатков главной книги на странице «План счетов»

На странице «План счетов» показаны все счета главной книги с агрегированными цифрами, учтенными в главной книге. На этой странице вы можете делать такие вещи, как:  

- Просмотреть отчеты, в которых отображаются операции главной книги и сальдо.  
- Просмотр списка учетных групп для этого счета.
- Просмотр отдельных дебетового сальдо и кредитового сальдо для одного счета.

:::image type="content" source="media/chart-of-accounts-page.png" alt-text="Пример того, как страница «План счетов» показывает финансовую аналитику" lightbox="media/chart-of-accounts-page.png":::

Для получения дополнительных сведений перейдите в раздел [План счетов](finance-general-ledger.md#the-chart-of-accounts).

### <a name="view-actual-amounts-compared-to-budgeted-amounts-for-all-accounts-and-for-several-periods"></a>Просмотр фактических сумм в сравнении с суммами бюджетов для всех счетов и для нескольких периодов

В процессе сбора, анализа и предоставления доступа к данным своей организации может потребоваться просмотреть фактические суммы в сравнении с суммами бюджета для всех счетов и для различных периодов. Выполнить это сравнение можно на странице **План счетов**, выбрав действие **Сальдо/бюджет ГК**.

Для получения дополнительных сведений перейдите в раздел [Анализ фактических сумм в сравнении с суммами бюджета](bi-how-analyze-actual-versus-budget.md).

### <a name="analyze-data-by-dimensions"></a>Анализ данных по измерениям

Измерения — это значения, которые классифицируют операции для их отслеживания и анализа в документах, таких как заказы на продажу. Измерения могут, например, указывать проект или отдел, который является источником операции.  

Поэтому вместо того, чтобы настраивать отдельные счета главной книги для каждого отдела и проекта, вы можете использовать измерения в качестве основы для анализа и избежать необходимости создавать сложную структуру плана счетов.

В финансовом анализе измерением называются данные, которые можно добавить в операцию главной книги в качестве своего рода маркера. Эти данные используются для группировки операций главной книги со сходными характеристиками, такими как клиенты, регионы, товары или менеджеры, и удобного извлечениях этих групп для анализа. Вы можете использовать измерения в операциях в журналах, документах и бюджетах. Дополнительные сведения см. в разделе [Анализ данных по измерениям](bi-how-analyze-data-dimension.md)

### <a name="analyzing-cash-flow"></a>Анализ движения денежных средств

На домашней странице бухгалтера в разделе **Финансовое исполнение** диаграммы "Цикл кассы", "Движение денежных средств" и "Доходы и расходы" предлагают способы анализа движения денежных средств:

- Просмотрите цифры за период с помощью слайдера временной шкалы.
- Отфильтруйте диаграмму, выбрав источник в легенде.
- Измените продолжительность периода или перейдите к предыдущему либо следующему периоду, выбрав параметры в раскрывающемся меню Финансовое исполнение.

:::image type="content" source="media/cashflow-accountant-rolecentre.png" alt-text="Пример того, как визуальные элементы движения денежных средств выглядят в ролевом центре бухгалтера" lightbox="media/cashflow-accountant-rolecentre.png":::

Чтобы проверить прогноз в дополнение к операциям прогноза, можно также просмотреть журнал движения денежных средств. Например, можно посмотреть, как в прогнозе:

- Обрабатываются подтвержденные продажи и покупки.
- Вычитается кредиторская задолженность и добавляется дебиторская задолженность.
- Пропускаются дублирующие заказы на продажу и заказы на покупку.

Для получения дополнительных сведений перейдите в раздел [Анализ движения денежных средств в организации](finance-analyze-cash-flow.md).

## <a name="see-also"></a>См. также

[Ведение бухгалтерской отчетности по филиалам или юридическим лицам](finance-consolidated-company-reporting.md)  
<!-- [Financial KPIs in Business Central](bi-finance-kpis.md)    -->
[Подготовка бухгалтерской отчетности с использованием финансовых данных и категорий счетов](bi-how-work-account-schedule.md)  
[Ad-hoc-анализ финансовых данных](ad-hoc-analysis-finance.md)   
[Общие сведения о плане счетов](finance-general-ledger.md#the-chart-of-accounts)  
[Встроенные бухгалтерские отчеты в формате Excel](finance-analyze-excel.md)  
[Встроенные основные бухгалтерские отчеты](finance-reports.md)  
[Встроенные отчеты по основным средствам](fa-reports.md)  
[Встроенные отчеты по расчетам с клиентами](receivables-reports.md)  
[Встроенные отчеты по расчетам с поставщиками](payables-reports.md)  
[Обзор финансов](finance.md)  
[Обзор анализа, бизнес-аналитики и отчетности](reports-bi-reporting.md)   
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
