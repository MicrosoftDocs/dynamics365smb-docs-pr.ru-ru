---
title: Сверьте затраты на инвентаризацию с главная книга
description: В конце учетных периодов должна выполняться последовательность задач аудита и управления себестоимостью для создания отчетов с правильной и сбалансированной стоимостью запасов.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'warehouse, stock'
ms.search.form: 9297
ms.date: 07/31/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# <a name="reconcile-inventory-costs-with-the-general-ledger"></a>Сверьте затраты на инвентаризацию с главная книга

При учете складских транзакций, таких как расходные накладные, счета покупки или корректировки запасов измененные значения себестоимости товаров записываются в операциях стоимости товаров. Чтобы отразить такое изменение стоимости запасов в финансовых книгах, себестоимость товаров автоматически учитывается на соответствующих счетах запасов в главной книге. Для каждой учитываемой складской транзакции учитываются соответствующие стоимости в товарном счете, счете коррекции и счете себестоимости продажи в главной книге.

Автоматический учет себестоимости определяется полем **Автомат. учет себест.** на странице **Настройка модуля "Запасы"**.

Даже несмотря на то что себестоимость запасов автоматически учитывается в главной книге, все равно необходимо обеспечить перенос себестоимости проданных товаров в соответствующие исходящие транзакции продаж. Это особенно важно в ситуациях, когда товары продаются до того, как на их покупку выставляется счет. Это называется корректировкой себестоимости. Себестоимость товаров автоматически корректируется при учете товарных транзакций, но себестоимость товаров также можно скорректировать вручную. Дополнительные сведения см. в разделе [Корректировка себестоимости товаров](inventory-how-adjust-item-costs.md).

## <a name="to-post-inventory-costs-manually"></a>Учет себестоимости товаров на складе вручную

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Учет себест. запасов в ГК**, а затем выберите связанную ссылку.
2. Учтите себестоимость товаров в главной книге вручную, выполнив пакетное задание. При запуске этого пакетного задания операции главной книги создаются на основе операций стоимости. Вы можете публиковать записи так, чтобы они были обобщены по группам публикаций.

> [!NOTE]  
> При запуске этого пакетного задания могут обнаружиться ошибки, связанные с отсутствием настройки или с неправильной настройкой измерений. Если обнаруживается ошибка в настройке измерения, пакетное задание игнорирует эти ошибки и использует измерения из операции стоимости. Если обнаруживаются другие ошибки, пакетное задание пропускает учет операций стоимости и включает их в виде списка в конце отчета в разделе “Пропущенные операции”. Чтобы учесть эти операции, необходимо исправить ошибки.

Чтобы просмотреть список ошибок перед выполнением пакетного задания, можно сформировать отчет **Учет себест. запасов в ГК - тест**. В тестовом отчете будут указаны все ошибки, которые произошли при тестовом учете. Затем эти ошибки можно исправить и выполнить пакетное задание учета себестоимости товаров на складе, не пропуская операции.

Если вы хотите получить обзор того, какие значения можно разместить в главная книга, не выполняя фактическую публикацию, вы можете запустить пакетное задание  **Разнести стоимость запасов в ГК**, не размещая значения в главная книга. Для этого следует снять флажок в поле **Учет** страницы запроса. Таким образом, при запуске пакетного задания создается отчет, показывающий значения, готовые к публикации в главная книга, но не опубликованные.

## <a name="to-audit-the-reconciliation-between-the-inventory-ledger-and-the-general-ledger"></a>Аудит выверки книги инвентаризации и главной книги
Страница **Склад - сверка с ГК** обеспечивает следующие возможности:

- Демонстрация различий выверки путем сравнения записей в ГК с содержимым книги инвентаризации (операции стоимости).
- Отображает несогласованные суммы затрат в записях стоимости в регистре учета запасов, как если бы они были сопоставлены с соответствующими счетами, связанными с запасами, в Главной книге, и сравнивает их с итоговыми суммами, зарегистрированными на тех же счетах в Главной книге.
- Отражение структуры двойной операции в ГК, путем визуального представления данных в соответствующем виде. Например, операции СПТ соответствует операция инвентаризации.
- Возможность детализации и просмотра операций, составляющих суммы себестоимости.
- Добавление фильтров для сокращения количества анализируемых данных по дате, товару и складу.
- Объяснение причин различий выверки в информативных сообщениях.


В крайнем левом столбце **Название** содержится список различных типов счетов ГК, связанных с запасами.

В столбцах **Запасы**, **Запасы (промежут.)** и **Запасы НЗП** отображаются итоги с выставленными счетами, без выставленных счетов и по НЗП для каждого типа счета ГК. Они рассчитываются на основе записей значений, то есть они проецируются на типы счетов ГК, где они будут находиться, когда в конечном итоге будут учтены в ГК.

В столбце **Всего** указывается сумма (полужирным шрифтом) величин операций стоимости в трех столбцах запасов.

В столбце **Итого по ГК** указываются суммы (полужирным шрифтом) для каждого типа счета ГК, который существует в ГК. Они вычисляются на основе операций ГК, то есть соответствуют себестоимости запасов, уже учтенной в ГК.

В столбце **Разница** представлена разница между значениями в полях **Итого по ГК** и **Всего**.

В верхней части страницы **Склад - сверка с ГК** можно ввести фильтры для ограничения, например, периода времени, за который отображаются данные.

Если флажок **Показывать предупреждение** установлен и есть расхождения между итогами по запасам и итогами по ГК, приложение отображает в поле **Предупреждение** сетки сообщения с объяснением причины расхождения. Если выбрать поле "Предупреждение", приложение выдаст дополнительные сведения о том, что означает предупреждение.

После ввода всех требуемых фильтров выберите действие **Показать матрицу**. Это приведет к вычислению данных и отображению страницы матрицы.

В левом крайнем столбце сетки отображаются различные типы счетов главной книги, связанных с товарами. Сетка отображает итоги по товарам с выставленными счетами, без счетов (с промежуточными счетами) и НЗП для каждого типа счета. Эти суммы вычисляются с помощью операций стоимости.

В следующих столбцах отображаются итоги для тех же типов счетов, рассчитанные на основе операций Главной книги.

Выберите сумму в любом из полей итогов, чтобы просмотреть операции отчета по запасам, которые использовались для расчета итогов. Для итогов по запасам операции отчета по запасам являются суммами операций стоимости для товаров. Для итогов по ГК операции отчета по запасам представляют собой суммы операций Главной книги.

## <a name="reporting-costs-and-reconciling-with-the-general-ledger"></a>Отчет о затратах и выверка с главной книгой
Другие отчеты, функции отслеживания и специальный инструмент выверки доступны аудитору или контроллеру, ответственному за сообщение точной и сбалансированной стоимости запасов в финансовый отдел.

В следующей таблице приводится их описание.    

|**Задача**|**Раздел**|  
|------------|-------------|  
|Просмотр стоимости запасов для выбранных товаров, включая сведения о количестве и стоимости увеличения и уменьшения запасов за выбранный период.|Отчет **Оценка стоимости товаров**|  
|Просмотр стоимости запасов для выбранных заказов на производство в НЗП (незавершенном производстве), таких как количество и стоимость потребления, использование производственных мощностей и выход по текущим производственным заказам.|Отчет **Оценка стоимости запасов - НЗП**|  
|Просмотр стоимости запасов для выбранных товаров, включая их фактическую и ожидаемую себестоимость на заданную дату.|Отчет **Оценка запасов - специф. себест.**|  
|Использование отчета для анализа причин отклонения себестоимости или анализа доли себестоимости для проданных товаров (себестоимости продажи).|Отчет **Анализ структуры себестоимости**|  

## <a name="see-also"></a>См. также
[Управление себестоимостью товаров](finance-manage-inventory-costs.md)    
[Покупки](purchasing-manage-purchasing.md)    
[Продажи](sales-manage-sales.md)    
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)    
[Общая бизнес-функциональность](ui-across-business-areas.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
