---
title: Консолидация данных из нескольких организаций
description: 'В этой статье объясняется, как можно консолидировать операции главной книги для двух или более отдельных организаций (дочерних организаций) в одну консолидированную организацию.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.date: 06/27/2023
ms.custom: bap-template
ms.search.keywords: 'consolidation, subsidiaries, consolidate'
ms.search.form: '1826, 1827'
ms.service: dynamics-365-business-central
---

# <a name="consolidating-financial-data-from-multiple-companies"></a>Консолидация финансовых данных из нескольких организаций

Некоторые организации используют [!INCLUDE [prod_short](includes/prod_short.md)] в нескольких бизнес-подразделениях или юридических лицах. Другие используют [!INCLUDE [prod_short](includes/prod_short.md)] в дочерних компаниях, которые должны отчитываться перед головными организациями. [!INCLUDE [prod_short](includes/prod_short.md)] предоставляет бухгалтерам инструменты для облегчения переноса операций главной книги из двух или более организаций (дочерних компаний) в консолидированную организацию.  

Каждая организация, участвующая в консолидации, называется филиалом. Организация, в которой объединяются данные, называется консолидированной организацией.  

Вы можете перенести финансовые данные из дочерних организаций в консолидированную организацию, даже если дочерние организации используют [!INCLUDE [prod_short](includes/prod_short.md)] в разных средах. Подробнее о том, как подключаться к другим средам, см. в статье [Настройка консолидации организаций](finance-consolidated-company-reporting-setup.md#busunit).

Если финансовые отчеты филиала составляются в валюте, отличной от валюты консолидированной организации, необходимо настроить валютные курсы для консолидации. Подробнее об обменных курсах для консолидации см. в статье [Настройка консолидации организаций](finance-consolidated-company-reporting-setup.md#exchrates).  

Консолидация возможна следующими способами:  

* Между организациями с разными планами счетов.  
* Организации, которые используют различные финансовые годы и различные валюты.  
* По полному объему или проценту финансовых данных организации.
* С использованием различных обменных курсов валют для отдельных счетов ГК.
* организации, работающие в других программах бухгалтерского учета и управления бизнесом.
* организации в разных средах [!INCLUDE [prod_short](includes/prod_short.md)].

Консолидированную организацию можно настроить таким же образом, как и другие организации. План счетов не зависит от плана счетов в филиалах. Планы счетов в филиалах могут отличаться друг от друга. Подробнее о настройке консолидации см. в статье [Настройка консолидации организаций](finance-consolidated-company-reporting-setup.md).  

> [!TIP]
> Консолидация финансовых данных может быть особенно актуальна для межфирменных процессов. Подробнее о межфирменных функциях см. в статье [Управление межфирменными транзакциями](intercompany-manage.md).

## <a name="consolidate-data"></a>Консолидировать данные

Перед консолидацией рекомендуется протестировать данные перед их передачей в консолидированную организацию. [!INCLUDE[prod_short](includes/prod_short.md)] проверяет разницу между информацией в филиалах и в консолидированной организации. Например, отличаются ли номера счетов или коды измерений. Исправьте все обнаруженные ошибки, прежде чем запускать отчет. Можно протестировать базу данных или, если данные импортируются из файла XML, можно протестировать файл.

### <a name="test-the-data-before-you-consolidate"></a>Тестирование данных перед консолидацией

1. Откройте консолидированную организацию.  
2. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Филиалы**, а затем выберите связанную ссылку.  
3. Протестируйте файл и базу данных следующим образом:  

    * Для проверки файла выберите действие **Тестировать файл** введите имя проверяемого файла, затем выберите **Печать**.  
    * Для тестирования базы данных выберите **Тестировать базу данных**.  

### <a name="run-the-consolidation"></a>Выполнение консолидации

После проверки данных можно передать их в консолидированную организацию. Мастер настройки поможет вам это сделать.

> [!NOTE]
> При запуске консолидации вы можете выбрать организации для включения. Если у вашей консолидированной организации нет доступа к одной или нескольким дочерним организациям, мастер поможет вам предоставить к ним доступ.

1. Выполните вход в консолидированную организацию.  
2. На странице **Филиалы** выберите действие **Консолидировать**.  
3. Заполните обязательные поля.  

## <a name="use-the-consolidated-trial-balance-report"></a>Использование отчета "Консолидированный пробный баланс"

Отчет **Консолидированный пробный баланс** может дать общее преставление о финансовом состоянии вашего бизнеса в целом. Отчет объединяет операции главной книги для каждой из ваших организаций в новой организации, которую вы создали для консолидированных данных. Консолидированная организация — это просто контейнер для консолидированных данных, она не содержит никаких бизнес-данных в режиме реального времени. Организации, включенные в консолидированную организацию, в отчете отображаются как **Филиалы**. Если у вас есть четыре или менее филиалов, вы можете использовать отчет **Консолидированный пробный баланс (4)**.  

Данный отчет содержит строку для каждого счета и соблюдает структуру плана счетов. Если все суммы в строке равны нулю, счет не показывается. Для каждого счета в отчете показывается следующая информация:

* Номер счета и имя счета.
* Итоги по консолидированной компании и по каждому филиалу. В качестве итогов может отображаться оборот или сальдо на дату.
* Исключения, сделанные для консолидированной организации. Исключения всегда отображаются для периода, соответствующего финансовому году консолидированной организации.
* Итог для консолидированной организации после внесения исключений отображается как оборот или как сальдо на дату.

## <a name="eliminate-repeated-transactions"></a>Исключение повторных транзакций

После того как вы консолидировали организации, вы должны найти и исключить все транзакции, зарегистрированные в организациях более одного раза. Обработка исключений из консолидации — это выполняемый вручную процесс.  

Исключение повторных транзакций:

1. Найдите транзакции, которые, возможно, нуждаются в корректировке, и введите строки финансового журнала для их исключения.
2. Запустите отчет **Исключения консолидации ГК**, чтобы помочь оценить влияние строк финансового журнала перед учетом.
3. Выполните учет корректирующих транзакций.

В отчете **Исключения консолидации ГК** отображается предварительный пробный баланс, в котором можно моделировать последствия исключения операций. В этом отчете сравниваются операции в консолидированной компании с исключениями, введенными в финансовый журнал.

Чтобы филиал можно было включить в отчет, вы должны настроить его на странице **Филиалы**. Не забудьте перевести переключатель **Консолидировать** в положение «вкл.».

Для каждого счета создается строка в соответствии со структурой плана счетов. Если все суммы в строке равны нулю, счет не показывается. Для каждого счета в отчете показывается следующая информация:

* Номер счета.
* Название счета.
* Если вы выбрали один или несколько кодов филиалов в поле **Код филиала** на странице запроса, из общего итога, отображаемого для консолидированной организации, будут исключены выбранные филиалы и исключения. Если же поле **Код филиала** не заполнено, из общего итога для консолидированной организации будут исключены исключения.
* Если вы выбрали код филиала в поле **Код филиала** на странице запроса, будет показан общий итог для операций, импортированных из филиала. Если же поле **Код филиала** на заполнено, будет показан общий итог для учтенных исключений в консолидированной организации.
* Общий итог для консолидированной организации со всеми филиалами и всеми учтенными исключениями.
* Исключения, которые должны быть сделаны в консолидированной организации. То есть операции в финансовом журнале, который выбран на странице запроса.
* Текст проводки копируется из финансового журнала.
* Общий итог консолидированной организации после исключений, если они приняты к учету.

## <a name="export-and-import-consolidated-data-between-databases"></a>Экспорт и импорт консолидированных данных между базами данных

Если данные филиала находятся в другой базе данных, вы перенести их вручную в виде файла или автоматизировать процесс с помощью API. Подробнее об API см. в статье [Использование нашего API для автоматической передачи данных между средами](#use-our-api-to-automatically-share-data-across-environments).

В этом разделе описывается ручной процесс с использованием файла.

Прежде чем включать данные в консолидацию, экспортируйте их в файл. Экспортируйте каждую организацию отдельно, используя пакетное задание **Экспорт консолидации**.  

> [!TIP]
> Используйте этот же процесс для экспорта консолидированных данных, которые необходимо отправить в Dynamics 365 Finance. (Например, если филиал является дочерней организацией, а материнская организация использует Dynamics 365 Finance.)

После выполнения пакетного задания обрабатываются все записи в счетах Главной книги. Для каждой комбинации выбранных измерений и даты содержимое записей в полях **Сумма** суммируется и экспортируется. Обрабатывается следующая комбинация выбранных измерений и даты с тем же номером счета. Затем обрабатываются комбинации со следующим номером счета и так далее.  

Экспортированные записи содержат следующие поля: **Номер счета**, **Дата учета** и **Сумма**. Если данные об измерениях также были экспортированы, то включаются коды измерений и значения измерений.  

1. Для каждой экспортированной, если итог полей **Сумма** является дебетом, то номер счета, настроенный в поле **Консол. дебет. счет ГК** филиала, экспортируется в строку. Если итог относится к кредиту, соответствующее число в поле **Консол. кредит. счет ГК** экспортируется в строку.  
2. Дата, использованная для каждой экспортированной строки, является конечной датой периода или, если передача осуществляется ежедневно, точной датой расчета.  
3. Значение измерения, экспортированное для операции, станет значением измерения консолидированной организации, которая указана в поле **Код консолидации** для данного значения измерения. Если в поле **Код консолидации** для данного значения измерения ничего не введено, в строку экспортируется само значение измерения.  
4. Кроме того, файлы XML содержат курсы валют для данного периода консолидации. Эти курсы находятся в отдельном разделе в начале файла.  

## <a name="use-our-api-to-automatically-share-data-across-environments"></a>Использование нашего API для автоматической передачи данных между средами

В [!INCLUDE [prod_short](includes/prod_short.md)] предусмотрен API, который позволяет автоматизировать процесс обмена финансовыми данными между филиалами и консолидированной организацией. Этот API бесплатный, и настроить его достаточно просто. Он даже позволяет обмениваться данными между средами [!INCLUDE [prod_short](includes/prod_short.md)]. Обмен данными между средами может стать актуальным, например, если филиалы находятся в разных географических регионах Azure. Подробнее об использовании API для автоматизации процесса консолидации см. в статье [Настройка консолидации организаций](finance-consolidated-company-reporting-setup.md#busunit).

## <a name="see-also"></a>См. также

[Настройка консолидации организаций](finance-consolidated-company-reporting-setup.md)  
[Управление межфирменными транзакциями](intercompany-manage.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Экспорт бизнес-данных в Excel](about-export-data.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
