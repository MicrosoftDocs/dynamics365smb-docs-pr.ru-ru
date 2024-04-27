---
title: Отслеживание коррекций себестоимости товаров
description: 'Узнайте, как отслеживание коррекции себестоимости товаров может помочь вам обеспечить точность данных о себестоимости товаров.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: how-to
ms.search.keywords: null
ms.search.form: null
ms.date: 03/08/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="track-item-cost-adjustments"></a>Отслеживание коррекций себестоимости товаров

Очень важно поддерживать точность себестоимости товаров и сокращать время между учетом операции и моментом отражения ее себестоимости в главной книге. Вы можете отслеживать результаты коррекции себестоимости для отдельных запусков коррекции и отдельных товаров. В случае возникновения ошибок вы можете выявить проблемные товары и внести исправления. Например, вы можете исключить такие товары из расчетов во избежание нарушения коррекции для других товаров. Вы можете корректировать себестоимость для отдельных товаров или создавать пакеты товаров и корректировать их все одновременно.

## <a name="start-tracking-cost-adjustments"></a>Как приступить к отслеживанию коррекции себестоимости

Начать использовать эту функцию несложно. На странице **Настройка модуля «Запасы»** в поле **Ведение журнала коррекции себестоимости** предусмотрено несколько вариантов:

* **Отключено** означает, что журнал запусков коррекции себестоимости не ведется.
* **Только ошибки** означает, что в журнал заносятся только запуски, которые завершились сбоем.
* **Все** означает, что в журнал заносятся все запуски.

> [!NOTE]
> Чтобы минимизировать размер журнала, [!INCLUDE [prod_short](includes/prod_short.md)] не регистрирует коррекции, которая происходят автоматически, когда кто-то учитывает товар.

Вам также необходимо настроить операцию очереди заданий **Учет себестоимости запасов в ГК (1002)**. Эта операция очереди заданий автоматически корректирует себестоимость в соответствии с графиком. Подробнее об операциях очереди заданий см. в статье [Использование очередей заданий для планирования задач](admin-job-queues-schedule-tasks.md).

## <a name="manage-cost-adjustments"></a>Управление коррекциями себестоимости

Для управления процессом коррекции себестоимости и его мониторинга используется страница **Коррекция себестоимости запасов**. На этой странице отображаются товары вместе со своими параметрами учета себестоимости и статусом коррекции себестоимости. Вы можете отфильтровать список, чтобы сосредоточиться на товарах, требующих коррекции или исключенных из процесса коррекции себестоимости.

### <a name="about-item-batches"></a>О пакетах товаров

Вы можете корректировать себестоимость товаров, группируя их в пакеты. Пакеты позволяют легко корректировать некоторые товары по отдельности, например потому, что их коррекция занимает больше времени. Пакеты также могут помочь в выявлении товаров с проблемами.

Чтобы создать пакет, на странице **Коррекция себестоимости запасов** выполните одно из следующих действий:

* Выберите товары в списке, выберите **Запустить коррекцию себестоимости**, а затем выберите **Добавить пакет**.
* Чтобы создать пакет и сразу же запустить коррекцию себестоимости, выберите товары в списке, выберите **Запустить коррекцию себестоимости**, а затем выберите **Добавить пакет и запустить**.
* Выберите **Запустить коррекцию себестоимости**, выберите **Пакеты товаров** и введите фильтр в поле **Фильтр по товару**.
  
> [!TIP]
> Чтобы быстро создать еще один пакет для всех товаров, которые еще не включены ни в один пакет, на странице **Коррекция себестоимости - пакеты товаров** выберите **Добавить отсутствующие товары**.

После завершения обработки пакета пакет имеет один из следующих статусов на странице **Пакеты товаров**:

* **Успех** : коррекция себестоимости прошла успешно.
* **Сбой**: если коррекция себестоимости завершилась сбоем, [!INCLUDE [prod_short](includes/prod_short.md)] определяет товар, из-за которого возникла ошибка, а затем разбивает текущий пакет на две части. В один пакет входит проблемный товар, а во второй — все остальные товары. Коррекция себестоимости запускается снова для пакета с оставшимися товарами. Если снова произойдет сбой, процесс повторяется. Максимальное количество разбиений задается в поле **Макс. количество повторных попыток**. По умолчанию максимальное количество повторных попыток равно 10, но вы можете изменить это ограничение.
* **Истекло время ожидания** : если коррекция себестоимости для пакета не завершается в течение периода, указанного в поле **Время ожидания (минут)** (в диапазоне от 1 до 720 минут), сеанс завершается и изменения откатываются. [!INCLUDE [prod_short](includes/prod_short.md)] затем разбивает текущий пакет пополам и повторно запускает процесс коррекции себестоимости для каждой половины. Этот процесс продолжается до тех пор, пока коррекция себестоимости не завершится успешно или пока не будет достигнуто максимальное количество повторных попыток.

> [СОВЕТ!] Каждый пакет обрабатывается в отдельном сеансе. Чтобы отслеживать ход выполнения, используйте действие **Обновить**.

### <a name="run-cost-adjustment"></a>Запустить коррекцию себестоимости

Для запуска коррекций используется страница **Коррекция себестоимости запасов**.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") введите **Коррекция себестоимости запасов**, а затем выберите соответствующую ссылку.
1. В зависимости от того, что вы хотите сделать, используйте один из следующих вариантов:

  * Чтобы скорректировать себестоимость одного или нескольких товаров сразу же, выберите товар(ы) в списке и выберите **Запустить коррекцию себестоимости**.
  * Для пакетов используйте один из следующих вариантов:

    * Чтобы создать пакет и сразу же скорректировать себестоимость, выберите товары в списке, выберите **Запустить коррекцию себестоимости**, а затем **Добавить пакет и запустить**.
    * Чтобы запустить коррекцию для всех пакетов, выберите **Запустить коррекцию себестоимости**, **Пакеты товаров**, а затем выберите **Запустить**.
    
    Подробнее о пакетах см. в разделе [О пакетах товаров](#about-item-batches).

### <a name="explore-item-details"></a>Изучение сведений о товаре

Для доступа к информации о коррекциях себестоимости для выбранного товара используется меню **Товар**.

* **Операции книги товаров**: выводит список товарных операций для товара. Действие **Пометить для коррекции** позволяет принудительно перезапустить коррекцию себестоимости для товаров, прямо или косвенно связанных с выбранными вами входящими операциями. Принудительный перезапуск может быть полезным, если предыдущие запуски привели к неверной себестоимости.
* **Операции стоимости**: выводит список операций стоимости для товара.
* **Точки входа коррекции себест.**: открывает страницу **Точка ввода коррекции средней себест.**, которая используется главным образом для расчета средней стоимости. На этой странице отображаются сочетания товаров, складов, вариантов и дат оценки, для которых выполняется или должна быть выполнена коррекция себестоимости.
* **Заказы с коррекцией себест.**: открывает страницу **Операция коррекции запасов - заказы**, где осуществляется коррекция производственных заказов и заказов на сборку. На ней отображаются заказы, которые были скорректированы или требуют коррекции.

### <a name="view-the-outcome"></a>Просмотр результата

Для просмотра результатов коррекции себестоимости используется меню **Журнал по**:

* **Запуск**: отображает журналы коррекции себестоимости по каждому запуску. Журнал включает данные о фильтре по товарам, статусе (успех/сбой/истекло время ожидания), дате/времени начала и окончания, продолжительности и разницах в себестоимости, возникших в результате запуска.
* **Товар**: отображает подробную информацию о процессе коррекции для выбранного товара.

### <a name="include-or-exclude-items-from-adjustments"></a>Включение или исключение товаров из коррекций

Если коррекция себестоимости для одного или нескольких товаров завершается сбоем, вы можете исключить эти товары из запуска коррекции, а затем включить их в последующие запуски. В меню **Функции** выберите один из следующих вариантов:

* **Исключить товар из коррекции** и **Включить товар в коррекцию**: позволяют временно отключить, а затем снова включить коррекцию себестоимости для выбранного товара. Коррекция себестоимости продолжит обеспечивать точность себестоимости других товаров, пока вы исследуете проблему с конкретным товаром.

## <a name="post-adjusted-costs-to-the-general-ledger"></a>Учет скорректированной себестоимости в главной книге

Обычно новые операции стоимости учитываются в главной книге в соответствии с графиком операции очереди заданий **Учет себестоимости запасов в ГК (1002)**. Тем не менее вы можете учесть коррекцию в главной книге сразу же со страницы **Коррекция себестоимости запасов**. В меню **Функции** выберите **Учет себестоимости запасов в ГК**.

## <a name="troubleshoot-cost-adjustments"></a>Устранение неполадок с коррекцией себестоимости

Для устранения неполадок при коррекции себестоимости используются следующие команды в меню **Диагностика**.

* **Экспорт данных о товарах**: экспорт связанных с товарами данных в текстовый файл. Этот файл можно использовать для дальнейшего анализа в среде-песочнице или прикрепить его к запросу в службу поддержки при исследовании проблем с расчетом себестоимости.
* **Импорт данных о товарах**: импорт ранее экспортированного текстового файла обратно в базу данных. Это действие доступно только средах-песочницах или пробных организациях.
* **Сбросить флаг «Себестоимость скорректирована»**: сбрасывает флаг **Себестоимость скорректирована** для товаров, производственных заказов или заказов на сборку. Этот параметр позволяет принудительно перезапустить для них коррекцию себестоимости.
* **Отчет для обнаружения проблем расчета себестоимости**: диагностика типичных проблем с данными, вызывающих ошибки расчета при калькуляции себестоимости. Этот отчет позволяет проверить правильность операций книги товаров, операций стоимости, операций применения товаров и операции книги производственных мощностей.
* **Удаление данных о товарах**: очищает все связанные с товаром таблицы в базе данных. Это действие доступно только средах-песочницах или пробных организациях.

## <a name="see-also"></a>См. также

[Коррекция себестоимости товаров](inventory-how-adjust-item-costs.md)  
[Технические подробности: коррекция себестоимости](design-details-cost-adjustment.md)  