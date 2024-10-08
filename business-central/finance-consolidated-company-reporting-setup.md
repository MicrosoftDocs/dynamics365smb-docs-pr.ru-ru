---
title: Настройка консолидации компании
description: 'Узнайте, как настроить, чтобы данные из разных компаний в Business Central передавались в консолидированную компанию.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.date: 06/12/2024
ms.custom: bap-template
ms.search.keywords: 'consolidation, subsidiaries, consolidate'
ms.search.form: '1826, 1827'
ms.service: dynamics-365-business-central
---

# <a name="set-up-company-consolidation"></a>Настройка консолидации организаций

Прежде чем вы сможете консолидировать операции книг учета двух или более отдельных организаций (дочерних компаний) в консолидированную организацию, вы должны подготовить планы счетов и консолидированную организацию.  

В зависимости от сложности ваших организаций, предусмотрено два способа настроить консолидацию:

* Если вам не требуются расширенные параметры, такие как включение организации, которой вы владеете только частично, можно использовать мастер настройки **Консолидация компаний** для быстрой настройки консолидации. Руководство помогает выполнить основные шаги.
* Если необходимы более сложные настройки, можно настроить консолидированную организацию и филиалы самостоятельно.
  * В каждом филиале укажите, какие счета главной книги должны быть включены в консолидацию, а также метод пересчета для каждого счета.
  * В консолидированной организации настройте карточку филиала для каждой организации, которая должна быть включена в консолидацию. Данная карточка содержит такие сведения, как даты финансового года филиала и процент каждого счета, который должен быть включен в консолидацию.

## <a name="simple-consolidation-setup"></a>Простая настройка консолидации

Если ваша консолидация простая, например потому что консолидируемые филиалы полностью находятся в вашей собственности, мастер настройки **Консолидация компаний** поможет выполнить следующие шаги:

* Создать новую консолидированную организацию или консолидировать уже созданную организацию. Эта организация не должна содержать транзакций.
* Просмотрите результаты. [!INCLUDE[prod_short](includes/prod_short.md)] проверяет, что основные данные и транзакции могут быть успешно перенесены в консолидированную организацию.

Для использовать руководство по сопровождаемой настройке, выполните следующие действия:

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Мастер настройки**, а затем выберите связанную ссылку.
2. Выберите **Обработка консолидаций**, а затем выполните каждый шаг в мастере настройки «Консолидация компаний».

## <a name="advanced-consolidation-setup"></a>Расширенная настройка консолидации

Если необходимо использовать более сложные настройки для консолидации, консолидацию можно настроить вручную. Например, если имеются организации, которые принадлежат вам лишь частично, или организации, которые не требуется включать в консолидацию.  

### <a name="set-up-the-consolidated-company"></a>Настройте консолидированную организацию

Необходимо сначала настроить консолидированную компанию. Консолидированную организацию можно настроить таким же образом, как и другие организации. Подробнее о создании организации см. в статье [Подготовьтесь к ведению бизнеса](ui-get-ready-business.md).  

Следующий список иллюстрирует ключевые аспекты консолидированной компании.

1. Настройте план счетов.

    Подробнее о настройке плана счетов см. в статье [Настройка или изменение плана счетов](finance-setup-chart-accounts.md).  

    Планы счетов могут быть идентичными для бизнес-единицы и консолидированной компании, или консолидированная компания может иметь другой план счетов. Если план счетов филиала отличается от плана счетов консолидированной организации, вы должны сопоставить счета со счетами в филиале. Подробнее см. в статье [Подготовка счетов главной книги для консолидации](#glacc).

2. Добавьте филиалы.

    Чтобы консолидировать данные нескольких организаций, необходимо настроить дочерние организации как филиалы и указать, какую часть их сальдо следует включать в консолидацию. Подробнее о филиалах см. в статье [Добавление филиалов](#busunit).

3. При необходимости укажите обменные курсы.

    Указывать обменные курсы необходимо, если вы будете консолидировать данные для филиалов, в которых используются разные валюты. Можно использовать три обменных курса: **Средний курс (вручную)**, **Курс закрытия** и **Последний курс закрытия**. Подробнее об обменных курсах см. в разделе [Задание обменных курсов для консолидаций](#exchrates).

4. Консолидируйте информацию в измерениях и счета главной книги.

    Подробнее см. в разделе [Включение или исключение измерений](#dim).

### <a name="add-business-units"></a><a name="busunit"></a>Добавление бизнес-подразделений

В консолидированной организации каждую организацию, данные из которой вы хотите консолидировать, необходимо настроить как филиал. Прежде чем запускать консолидацию и создавать отчет о консолидации, желательно проверить финансовые данные в каждом филиале.

Существенная часть создания филиала заключается в указании того, как филиал будет передавать свои финансовые данные в консолидированную организацию. Существуют ручной и автоматические варианты:

* Чтобы использовать ручной процесс, для [!INCLUDE [prod_short](includes/prod_short.md)] Online и в локальной версии можно экспортировать файл.xml, содержащий операции главной книги филиала. Затем импортируйте файл в консолидированную компанию.
* Для автоматизации обмена данными в [!INCLUDE [prod_short](includes/prod_short.md)] Online можно использовать предусмотренный в [!INCLUDE [prod_short](includes/prod_short.md)] API, который обеспечивает обмен данными между средами. Если ваши организации находятся в одной среде, вы можете использовать вариант **База данных**.

> [!NOTE]
> Вариант с API также позволяет передавать операции главной книги из других сред [!INCLUDE [prod_short](includes/prod_short.md)]. Для использования варианта с API пользователь, настраивающий консолидацию, должен иметь разрешение на доступ к операциям главной книги. Например, такой доступ обеспечивают наборы разрешений «D365 Базовый» и «D365 Чтение».

#### <a name="set-up-business-unit-currencies"></a>Настройка валют филиала

При выполнении консолидации филиалов в иностранной валюте обращайте внимание на обменные курсы, используемые на различных этапах процесса. Это особенно актуально при повторном запуске консолидации. Используйте страницу **Настройка валют филиала**, чтобы легко отслеживать курсы.

На странице **Настройка валют филиала** отображаются последние курсы для среднего курса, курса закрытия и последнего курса закрытия. Вы можете посмотреть обменные курсы в таблице курсов обмена валют, что упрощает проверку курсов. Вы можете изменить ставки для текущего прогона, введя значения или скопировав их из предыдущих прогонов. Чтобы скопировать курсы, выберите **Выбрать из предыдущей консолидации**. Эта страница особенно полезна, когда вы хотите повторно запустить более раннюю консолидацию и использовать более ранний курс закрытия. Этот шаг необходим для правильной переоценки статей балансового отчета. Страница **Выбрать из предыдущей консолидации** также полезна, если вы просто хотите просмотреть курсы, которые использовались, например, при устранении неполадок. Страница фильтруется по запускам, включающим выбранный филиал.

Вы запускаете пакетное задание **Выполнить консолидацию** со страницы списка **Филиалы** . Вы также можете найти страницу **Настройка валют филиала**, выбрав действие **Курсы обмена**.

> [!NOTE]
> Страницы настройки обменного курса для среднего курса, курса закрытия и последнего курса закрытия, которые в настоящее время доступны на карточке **Филиала**, в будущей версии станут устаревшими. Однако вы все равно можете сохранить эти курсы, если у вас есть филиалы, которые вы импортируете через файлы.

#### <a name="create-a-business-unit"></a>Создание подразделения

1. Выполните вход в консолидированную организацию.
2. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок введите **Филиалы**, а затем выберите связанную ссылку.  
3. Выберите **Создать**, а затем заполните необходимые поля на экспресс-вкладках **Общие сведения** и **Счета ГК**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!IMPORTANT]
    > При заполнении полей **Дата начала** и **Дата окончания** убедитесь, что вы соответствуете общепризнанным принципам бухгалтерского учета (GAAP) в отношении финансовых периодов филиала по сравнению с родительской организацией.
4. На экспресс-вкладке **Импорт данных** в поле **Импорт данных по умолчанию** укажите, как вы будете передавать операции главной книги в консолидированную организацию:

   * Для совместного использования данных между организациями в одной среде выберите **База данных**.
   * Для совместного использования данных между организациями в разных средах, выберите **API**, а затем заполните поле **Конечная точка API**.
        
        Чтобы узнать URL-адрес конечной точки, в [!INCLUDE [prod_short](includes/prod_short.md)] филиала откройте страницу **Настройка консолидации** и проверьте значение поля «Конечная точка API текущей среды». 
   * Чтобы экспортировать файл.xml и передать его вручную, выберите **Файловый формат**.

### <a name="prepare-general-ledger-accounts-for-consolidation"></a><a name="glacc"></a>Подготовка счетов главной книги для консолидации

План счетов организации, которую вы будете консолидировать, должен определять счета для консолидации. Для каждого учетного счета ГК в каждой организации необходимо указать счет ГК в консолидированной организации, на который будет переноситься сальдо. Это сопоставление позволяет консолидировать организации, имеющие разные планы счетов.

Если план счетов в филиале отличается от плана счетов в консолидированной организации, следует подготовить счета главной книги для консолидации. Можно указать счета для учета дебета и кредита, и метод, используемый для преобразования валют в консолидированной организации.

1. В каждом [!INCLUDE [prod_short](includes/prod_short.md)] бизнес-подразделения выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **План счетов**, а затем выберите связанную ссылку.  
2. Откройте карточку для счета, затем заполните поля на экспресс-вкладке **Консолидация**. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

> [!NOTE]
> Если вы не заполните поля **Консол. дебет. счет ГК** и **Консол. кредит. счет ГК**, [!INCLUDE [prod_short](includes/prod_short.md)] предполагает, что они сопоставлены с такими же счетами в консолидированной организации.

> [!TIP]
> Возможны сценарии, в которых включать тот или иной счет в консолидацию не требуется. Например, если вы хотите, чтобы ваша консолидированная организация отражала только балансовые отчеты дочерних организаций. Чтобы исключить счет из консолидации, включите переключатель **Исключить из консолидации** для этого счета.

### <a name="specify-exchange-rates-for-consolidations"></a><a name="exchrates"></a>Задание обменных курсов для консолидации

Если филиал использует валюту, отличную от валюты консолидированной организации, следует указать методы обмена валют для каждого счета до консолидации. Для каждого счета содержимое поля **Метод пересчета при консолидации** определяет валютный курс. В каждой консолидированной компании в каждой карточке филиала в поле **Таблица обменных курсов** задается, какие валютные курсы используются при консолидации: филиала или консолидированной организации. При использовании валютных курсов консолидированной организации можно изменять валютные курсы филиала. Для филиалов если в поле **Таблица обменных курсов** карточки филиала содержится значение **Локально**, можно изменить валютный курс из карточки филиала. Валютные курсы копируются из таблицы **Курс валюты**, но их можно изменить перед консолидацией.

В следующей таблице описываются способы задания валютных курсов, которые можно использовать для счетов.

|Валютный курс | Типичное использование |
|---|---|
|Средний курс (вручную) | Вы вручную вычисляете средний курс для периода консолидации. Средний курс вычисляется как арифметическое среднее или как лучшая оценка и результат указывается для каждого филиала. Используется для счетов отчета о прибылях и убытках.|
|Курс закрытия | Используется для счетов балансового отчета.|
|Последний курс закрытия | Курс, который действовал на валютном рынке на дату, для которой подготавливается отчет по балансу или отчет о прибылях. Этот курс вводится для каждого филиала. Используется для счетов балансового отчета.|
|Статистический курс | Валютный кур, который действовал на момент транзакции.|
|Составной курс | Суммы текущего периода переводятся по среднему курсу и добавляются к ранее записанному балансу в консолидированной организации. Обычно этот метод используется для счетов нераспределенной прибыли. Эти счета включают суммы за разные периоды, поэтому они содержат суммы, пересчитанные с использованием разных обменных курсов.|
|Справедливый курс | Этот вариант аналогичен варианту **Составной**. Разницы учитываются на отдельных счетах главной книги.|

Чтобы задать обменные курсы для филиала, выполните следующие действия:

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок введите **Филиалы**, а затем выберите связанную ссылку.  
2. На странице **Список филиалов** выберите филиал, а затем выберите действие **Валютные курсы**.  
3. На странице **Настройка валют филиала** заполните требуемые поля. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

### <a name="include-or-exclude-dimensions"></a><a name="dim"></a>Включить или исключить измерения

Возможна консолидация как данных измерений, так и счетов главной книги.

* В измерениях задайте значение в поле **Код консолидации** или оставьте его пустым.
  * Чтобы исключить измерение из консолидации, оставьте поле **Код консолидации** для измерения пустым, и не выбирайте измерения в полях **Копировать измерения** поля в функциях консолидации или отчетах.
  * Чтобы включить информацию об измерениях в консолидацию, оставьте поле **Код консолидации** пустым. Однако консолидация будет работать, только если значения измерений в филиале точно такие же, как в консолидированной организации.
  * Чтобы консолидировать код значения измерения в филиале с другим кодом значения измерения в консолидированной организации, заполните поле **Код консолидации** для соответствующих измерений.  
* Добавьте измерения к счетам главной книги.

### <a name="exclude-a-company-from-consolidation"></a><a name="exclude"></a>Исключение организации из консолидации

Если не требуется включать филиал в консолидацию, его можно исключить. Чтобы это сделать, перейдите на карточку филиала и снимите флажок **Консолидировать**.

### <a name="include-a-partially-owned-company-in-consolidation"></a><a name="include"></a>Включение в консолидацию организации с частичным участием

Если вы владеете только частью организации, можно включать в консолидацию процент каждой транзакции, соответствующий доле вашего участия в организации. Например, если вы владеете 70% организации, в консолидацию будут включены $70 из счета на $100. Чтобы указать долю собственности в организации, перейдите на карточку филиала и введите значение в процентах в поле **Консолидация (%)**.  

## <a name="see-also"></a>См. также

[Консолидация финансовых данных из нескольких организаций](finance-consolidated-company-reporting.md)  
[Управление межфирменными транзакциями](intercompany-manage.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Экспорт бизнес-данных в Excel](about-export-data.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
