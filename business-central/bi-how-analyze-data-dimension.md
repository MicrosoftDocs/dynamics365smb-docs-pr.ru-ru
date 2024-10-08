---
title: Анализ данных по измерениям
description: 'В этой статье описывается, как анализировать бизнес-данные по измерениям для лучшего понимания ваших бизнес-процессов.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '545, 555, 556, 557, 558, 9372, 9370, 9371'
ms.date: 04/19/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="analyze-data-by-dimensions"></a>Анализ данных по измерениям

В финансовом анализе измерением называются данные, которые можно добавить в операцию в качестве своего рода маркера для группировки операций с аналогичными характеристиками. Например, в измерениях часто группируются записи по клиентам, регионам, продуктам и продавцам. Группы позволяют легко получать данные о них для анализа. Вы можете использовать измерения в операциях в журналах, документах и бюджетах.

Каждое измерение описывает, что именно анализируется. Например, примером двумерного анализа могут быть продажи по регионам. Используя более двух измерений при создании записи, вы можете выполнить более сложный анализ. Примером комплексного анализа является изучение продаж по каждой торговой кампании по группам клиентов по регионам. Это дает возможность осуществлять более глубокое исследование бизнес-процессов для анализа того, насколько успешно ваша организация ведет деятельность, в каких областях наблюдается рост, а в каких нет и куда стоит направить дополнительные ресурсы. Это понимание поможет вам принимать более обоснованные бизнес-решения. Подробнее см. в статье [Работа с измерениями](finance-dimensions.md).

> [!TIP]
> Для быстрого анализа транзакционных данных по измерениям можно фильтровать итоговые суммы в планах счетов и операциии на всех страницах **Операции** по измерениям. Найдите действие **Установить фильтр измерений**.

> [!NOTE]
> Если вы обнаружите, что в учтенных операциях главной книги используется неверное значение измерения, вы можете исправить его и обновить аналитические представления. Подробнее см. в статье [Устранение неполадок и исправление измерений](finance-troubleshooting-correcting-dimensions.md#changing-dimension-assignments-after-posting).

## <a name="set-up-an-analysis-view"></a>Настройка аналитического представления

В анализе по измерениям используется выбранная комбинация измерений. Для сохранения, извлечения и обновления этого набора измерений используется карточка **Аналитическое представление**.

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Аналитические представления**, а затем выберите соответствующую ссылку.  
2. На странице **Список представлений анализа** выберите действие **Создать**.
3. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Чтобы к четырем кодам измерений на экспресс-вкладке **Измерения** добавить другие коды, щелкните действие **Фильтр**, заполните поля и нажмите кнопку **ОК**.  
5. Чтобы обновить представление, выберите действие **Обновить**.

## <a name="analyze-by-dimensions"></a>Анализ по измерениям

Матрицу **Анализ по измерениям** можно использовать для просмотра сумм в главной книге с использованием уже настроенных аналитических предсталвений.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") введите **Аналитические представления**, а затем выберите соответствующую ссылку.  
2. Выберите соответствующее аналитическое представление и выберите действие **Анализ по измерениям**.
3. На странице **Анализ по измерениям** заполните поля, чтобы определить, какие данные и как отображать.
4. Выберите действие **Показать**, чтобы открыть страницу матрицы для аналитического представления.
5. Чтобы получить доступ к подробной информации о сумме на странице матрицы, выберите сумму.  

- В столбцах слева содержится информация, зависящая от варианта, выбранного в поле **Показывать в строках** в заголовке.  
- В столбцах справа содержится информация, зависящая от варианта, выбранного в поле **Показывать в столбцах** в заголовке.

> [!IMPORTANT]  
> Продолжительность периода не может быть меньше, чем указано для сжатия по дате в карточке **Аналитический отчет**. Действия **Следующий набор** и **Предыдущий набор** недоступны, если вы выбрали в поле **Показывать в строках** или **Показывать в столбцах** вариант **Период**.  

> [!NOTE]  
> Отчет **Измерения - подробно** используется для отображения детальной классификации использования измерений в операциях за определенный промежуток времени. Для отображения только значений сумм может использоваться отчет **Измерения - всего**.  

> [!TIP]  
> Представление также можно изменитьп путем изменения содержимого полей **Показывать в строках** и **Показывать в столбцах**. Чтобы обратить параметры просмотра, выберите действие **Поменять местами строки и столбцы**.

## <a name="update-an-analysis-view"></a>Обновление аналитического представления

Суммы на странице **Анализ по измерениям** представляют собой картину состояния организации на дату последнего обновления. Чтобы получить текущее состояние, запустите действие обновления, чтобы обновить представление анализа.

Для обновления аналитического представления со страницы **Анализ по измерениям** используйте следующую процедуру. Аналогичным обраом можно обновить страницы **Карточка аналитического представления** и **Cписок аналитических представлений**.  

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Аналитические представления**, а затем выберите соответствующую ссылку.
2. Выберите соответствующее аналитическое представление и выберите действие **Анализ по измерениям**.
3. На странице **Анализ по измерениям** выберите поле **Код представления анализа**.  
4. Выберите строку с соответствующим аналитическим отчетом.  
5. На странице **Аналитические представления** выберите аналитическео преставление, затем выберите действие **Обновить**.  

> [!TIP]  
> При установке флажка **Обновлять при учете** на карточке аналитического представления представление автоматически обновляется, когда кто-то выполняет учет соответствующей транзакции.

> [!NOTE]  
> Чтобы одновременно изменить некоторые или все аналитические отчеты, воспользуйтесь пакетным заданием **Обновление представлений анализа**.  

## <a name="see-also"></a>См. также

[Финансовая бизнес-аналитика](bi.md)  
[Финансы](finance.md)  
[Настройка финансов](finance-setup-finance.md)  
[Главная книга и план счетов](finance-general-ledger.md)  
[Работа с измерениями](finance-dimensions.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
