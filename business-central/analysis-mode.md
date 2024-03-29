---
title: Анализ данных на страницах списков и в запросах с использованием режима анализа данных
description: 'Узнайте, как использовать режим анализа данных в Business Central для анализа данных.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: how-to
ms.date: 12/08/2023
ms.custom: bap-template
ms.service: dynamics-365-business-central
ms.search.form: '456, 457, 458, 459, 460, 461, 16, 22, 25, 26, 27, 31, 143, 144, 9300, 9301, 9303, 9304, 9305, 9306, 9307, 9309, 9310, 9311'
---
# <a name="analyze-list-page-and-query-data-using-data-analysis-mode"></a>Анализ данных на страницах списков и в запросах с использованием режима анализа данных

> **ОТНОСИТСЯ К:** общедоступной предварительной версии в волне 1 выпуска Business Central 2023 и выше в отношении анализа страниц списков; общей доступности в волне 2 выпуска Business Central 2023 в отношении анализа данных со страниц списков и из запросов.

Из этой статьи вы узнаете, как анализировать данные со страниц списков и из запросов, используя *режим анализа данных*. Режим анализа данных позволяет анализировать данные непосредственно со страницы без необходимости запускать отчет или переключаться на другое приложение, например Excel. Он обеспечивает интерактивный и универсальный способ для выполнения вычислений, подведения итогов и изучения данных. Вместо создания отчетов с использованием различных параметров и фильтров вы можете добавить несколько вкладок, представляющих различные задачи с данными или представления данных. Например, это могут быть «Мои клиенты», «Последующие товары», «Недавно добавленные поставщики», «Статистика продаж» или любое другое представление, которое вы сочтете нужным создать.

> [!TIP]
> Преимущество режима анализа данных заключается в том, что он не предполагает изменения никаких базовых данных страницы списка или запроса либо макета страницы или запроса, когда они не находятся в режиме анализа данных. Поэтому лучший способ узнать, что можно сделать в режиме анализа данных, — это попробовать.

## <a name="prerequisites"></a>Предварительные требования

- Если вы используете Business Central версии 22, режим анализа данных находится на этапе предварительной версии. Это значит, что прежде чем вы сможете его использовать, его должен включить администратор. Чтобы включить его, перейдите на страницу **Управление функциями** и включите **Обновление функции: режим анализа, быстрый анализ данных непосредственно в Business Central**. [Узнайте больше об управлении функциями](/dynamics365/business-central/dev-itpro/administration/feature-management).
- В версии 23 и более поздних версиях вашей учетной записи должен быть назначен набор разрешений **DATA ANALYSIS - EXEC** или разрешение на выполнение системного объекта **9640 Разрешить режим анализа данных**. Если вы администратор, вы можете исключить эти разрешения для пользователей, у которых не должно быть доступа к режиму анализа.

> [!NOTE]
> Вы можете заметить, что на некоторых страницах списков нет переключателя **Анализ** для перехода в режим анализа. Причина этого в том, что разработчики могут отключить режим анализа на определенных страницах, используя свойство [AnalysisModeEnabled](/dynamics365/business-central/dev-itpro/developer/properties/devenv-analysismodeenabled-property) в AL.

## <a name="get-started"></a>Начало работы

1. Откройте страницу списка или запрос.

   Например, для работы со страницей **Книга операций по клиентам** нажмите значок ![Лупа, которая открывает функцию «Что вы хотите сделать».](media/ui-search/search_small.png), (<kbd>Alt</kbd>+<kbd>Q</kbd>), введите *книга операций по клиентам*, а затем выберите связанную ссылку. 

2. В строке действий в верхней части страницы включите переключатель **Анализ**.

    Активируется режим анализа данных, и данные будут открыты в интерфейсе, оптимизированном для анализа данных.  В режиме анализа данных вместо обычной строки действий отображается специальная строка режима анализа данных. На следующем рисунке показаны различные области страницы в режиме анализа данных.

   [![Показывает обзор страницы в режиме анализа данных](media/analysis-mode-overview-2.png)](media/analysis-mode-overview-2.png#lightbox)

   Каждая область объясняется в последующих разделах.

3. Различные области страницы предназначены для обработки, суммирования и анализа данных. Подробные сведения см. в последующих разделах.

4. Если вы хотите выйти из режима анализа, выключите переключатель **Анализ**.

   Добавленные вами вкладки анализа будут оставаться до тех пор, пока вы их не удалите. Поэтому, если вы снова вернетесь в режим анализа данных, вы увидите их точно в том же виде, в каком оставили.

> [!NOTE]
> Отображением данных в режиме анализа можно управлять с помощью фильтров или представлений, настраиваемых на странице списка. Это позволяет предварительно отфильтровать данные перед входом в режим анализа.

## <a name="work-with-data-analysis-mode"></a>Работа в режиме анализа данных

В режиме анализа данных страница делится на две области:

- Основная область, которая состоит из области данных (1), строки сводки (2) и строки вкладок (5).
- Область обработки данных, которая состоит из двух панелей: столбцов (3) и фильтров анализа (4).

### <a name="data-area-1"></a>Область данных (1)

В области данных отображаются строки и столбцы из запроса страницы списка, и подводятся итоги данных. Область данных предоставляет универсальный способ управления расположением столбцов и быстрый способ получить сводку данных. Для столбцов, содержащих числовые значения, в последней строке отображается сумма всех значений в столбце, если вы не определили группы строк. В последнем случае суммы отображаются в виде промежуточных итогов для групп.  

![Показывает обзор области данных на странице в режиме анализа данных](media/analysis-mode-data-area.png)

- Чтобы переместить столбец, выберите его и перетащите в то место, где он наиболее уместен для вашего анализа.
- Чтобы отсортировать данные по столбцу, выберите заголовок столбца. Чтобы отсортировать данные по нескольким столбцам, нажмите клавишу <kbd>Shift</kbd> и, удерживая ее, выбирайте заголовки столбцов, по которым вы хотите отсортировать данные.
- Щелкните правой кнопкой мыши столбец или наведите на него курсор и выберите значок меню ![Показывает значок в столбце в режиме анализа данных, который открывает меню действий](media/analysis-mode-column-menu-icon.png) для доступа к ряду действий, которые можно выполнить над столбцами. Например:

  - Чтобы закрепить столбец слева или справа от области данных, чтобы он не скрывался за пределами экрана при прокрутке, нажмите элемент столбца ![Показывает значок в столбце в режиме анализа данных, который открывает меню действий](media/analysis-mode-column-menu-icon.png) > **Закрепить столбец** > **Закрепить слева**.
  - Определите фильтры данных непосредственно в определении столбца, не переходя на панели **Фильтры анализа**. Вы по-прежнему можете просмотреть сведения о связанных данных для каждой строки, а также открыть карточку, чтобы узнать больше о конкретном объекте.
- Используйте область данных для взаимодействия с данными. Для столбцов, содержащих числовые значения, допускающие суммирование, можно получить описательную статистику по набору полей, пометив их. Статистика отображается в строке состояния (2) внизу страницы.
- Экспортируйте данные в формате Excel или CSV. Щелкните правой кнопкой мыши область данных или выбранные ячейки, чтобы экспортировать данные.

### <a name="summary-bar-2"></a>Строка сводки (2)

Строка сводки находится в нижней части страницы и служит для отображения статистики по данным на странице списка или в запросе. В ходе работы со столбцами, значения которых можно суммировать (например, при выборе нескольких строк в столбце, в котором отображаются суммы), данные обновляются.

![Показывает обзор строки сводки в режиме анализа данных](media/analysis-mode-totals-row.png)

В следующей таблице описаны различные числовые значения, отображаемые в области итогов:

|Номер|Описание|
|-|-|
|Строки|Количество выбранных строк как часть общего количества доступных строк. |
|Всего строк|Количество строк в нефильтрованном списке или запросе.|
|Отфильтровано|Количество строк, отображаемых в результате применения фильтров к списку или запросу.|
|По средней|Среднее значение по всем выбранным суммируемым полям.|
|Число|Количество выбранных строк.|
|Мин.|Минимальное значение по всем выбранным суммируемым полям.|
|Макс.|Максимальное значение по всем выбранным суммируемым полям.|
|Сумма|Сумма всех значений в выбранных суммируемых полях.|

### <a name="columns-3"></a>Столбцы (3)

**Столбцы** — это одна из двух панелей, которые вместе определяют ваш анализ. Другой областью является панель **Фильтры анализа**. Панель **Столбцы** используется для суммирования данных. Используя панель **Столбцы**, вы определяете, какие столбцы следует включить в анализ.

![Показывает обзор панели столбцов в режиме анализа данных](media/analysis-mode-columns-2.png)

|Области|Описание|
|-|-|
|Поиск/установка или снятие всех флажков|Можно производить поиск столбцов. Установите флажок, чтобы выбрать или отменить выбор всех столбцов.|
|Флажки|Эта область содержит флажок для каждого поля в исходной таблицы списка или запроса. С помощью этой области вы можете выбирать, какие столбцы должны отображаться. Если нужно, чтобы на странице отображался столбец для данного поля, установите флажок; если столбец нужно скрыть, снимите флажок. |
|Группы строк|Используйте эту область для группирования и суммирования данных по одному или нескольким полям. Вы можете включать только нечисловые поля, такие как текстовые поля, а также поля даты и времени. Группы строк часто используются в сводном режиме.|
|Значения|Используя эту область, укажите поля, сумму значений которых вы хотите получить. Вы можете включать только поля, содержащие числовые значения, которые можно складывать друг с другом. Нельзя, например, выбирать текстовые поля либо поля даты/времени.|

Чтобы переместить поле из одной области в другую, выберите значок перетаскивания ![Показывает обзор страницы в режиме анализа](media/column-grab-icon.png) рядом со столбцом в списке и перетащите поле в требуемую область. При этом вы не сможете переместить поле в область, где это поле недопустимо.

### <a name="analysis-filters-4"></a>Фильтры анализа (4)

На панели **Фильтры анализа** для столбцов можно задать дополнительные фильтры данных, чтобы ограничить количество записей в списке. Задайте фильтры для столбцов, чтобы ограничить количество записей в списке и последующее суммирование только интересующими вас записями на основе заданных вами критериев. Предположим, например, что вас интересуют только данные по конкретному клиенту или заказы на продажу, превышающие определенную сумму. Чтобы установить фильтр, выберите столбец, выберите операцию сравнения из списка (например, **Равно** или **Начинается с**), а затем введите значение.

![Показывает обзор панели фильтров в режиме анализа данных](media/analysis-mode-filters.png)

> [!NOTE]
> Дополнительные фильтры применяются только к текущей вкладке анализа. Это позволяет точно определить дополнительную фильтрацию данных, необходимую для конкретного анализа.

### <a name="tabs-5"></a>Вкладки (5)

В области вкладок вверху вы можете создавать различные конфигурации (столбцы и фильтры анализа) на отдельных вкладках, после чего вы можете работать с данными на вкладках независимо друг от друга. Всегда есть как минимум одна вкладка, которая по умолчанию называется **Анализ 1**. Вы можете добавлять дополнительные вкладки, что удобно для сохранения часто используемых конфигураций анализа некоторого набора данных. Например, у вас могут быть вкладки для анализа данных в сводном режиме и другие вкладки с отфильтрованными подмножествами строк. На некоторых вкладках может отображаться подробное представление со множеством столбцов, а на других — только несколько основных столбцов.

Вот несколько советов по работе с несколькими вкладками анализа:

- Чтобы добавить новую вкладку, нажмите крупный значок **+** рядом с последней вкладкой анализа.
- Щелкните указывающую вниз стрелку на вкладке, чтобы открыть список действий, которые можно выполнить с вкладкой (переименовать, дублировать, удалить, переместить и т. п.).

   - **Удалить** — удаляется открытая в данный момент вкладка. **Удалить все** — удаляются все добавленные вами вкладки, кроме вкладки по умолчанию **Анализ 1**.
- Вы не можете полностью удалить вкладку **Анализ 1**, но можете ее переименовать с помощью действия **Переименовать**, а также сбросить внесенные вами изменения с помощью действия **Удалить** или **Удалить все**.  

- Добавленные и настроенные вами вкладки анализа будут оставаться до тех пор, пока вы их не удалите. Поэтому, если вы снова вернетесь в режим анализа данных, вы увидите их точно в том же виде, в каком оставили.

   > [!TIP]
   > Настроенные вами вкладки видны только вам. Другие пользователи будут видеть только те вкладки, которые настроили они.
- Вкладки анализа можно копировать. Копирование может быть удобно, если вы хотите поэкспериментировать с вкладкой, не изменяя оригинал, или если вы хотите создать различные варианты одного и того же анализа.


## <a name="date-hierarchies"></a>Иерархии дат

В режиме анализа поля дат в наборе данных генерируются в виде иерархии «год-квартал-месяц», состоящей из трех отдельных полей. Эта иерархия основана на обычном календаре, а не на финансовых календарях, определенных в Business Central.

Дополнительные поля называются _\<field name\> - год_, _\<field name\> - квартал_ и _\<field name\> - месяц_. Например, если набор данных включает поле с именем _Дата учета_, то соответствующая иерархия дат состоит из полей с именами _Дата учета - год_, _Дата учета - квартал_ и _Дата учета - месяц_.

> [!NOTE]
> Иерархия дат в настоящее время применяется только к полям типа «дата», но не к полям типа «дата/время».

## <a name="pivot-mode"></a>Сводный режим

Вы можете использовать сводный режим для анализа большого количества числовых данных, а также суммирования данных по категориям и подкатегориям. Сводный режим аналогичен [сводным таблицам в Microsoft Excel](https://support.microsoft.com/office/create-a-pivottable-to-analyze-worksheet-data-a9a84538-bfe9-40a9-a8e9-f99134456576).

Чтобы включить или выключить сводный режим, сдвиньте переключатель **Сводный режим** на панели **Столбцы** (3). При включении сводного режима на панели появляется область **Метки столбцов**. Используя область **Метки столбцов**, можно группировать итоговые значения для строк по категориям. Поля, добавляемые вами в область **Метки столбцов**, отображаются как столбцы в области данных (1).

Настройка анализа данных в сводном режиме включает в том числе перемещение полей в три области: **Группы строк**, **Метки столбцов** и **Значения**. На следующем рисунке показано, где поля сопоставляются с областью данных (1) (`sum` — это вычисляемые данные и, возможно, **Значения**).

<table>
<tr><th></th><th>Метка столбца</th><th></th><th>Метка столбца</th><th></th></tr>
<tr><th>Группа строк</th><th>Значение</th><th>Значение</th><th>Значение</th><th>Значение</th></tr>
<tr><td>строка</td><td>sum</td><td>sum</td><td>sum</td><td>sum</td></tr>
<tr><td>строка</td><td>sum</td><td>sum</td><td>sum</td><td>sum</td></tr>
<tr><td>строка</td><td>sum</td><td>sum</td><td>sum</td><td>sum</td></tr>
<tr><td>строка</td><td>sum</td><td>sum</td><td>sum</td><td>sum</td></tr>
</table>

> [!TIP]
> Столбцы с несколькими возможными значениями лучше всего подходят для использования в столбце **Значения**.


## <a name="analyze-large-amounts-of-data"></a>Анализ больших объемов данных

Если размер набора данных, который вы хотите проанализировать, превышает 100 000 строк, система предложит вам перейти в режим анализа, оптимизированный для больших наборов данных. В настоящее время существует два ограничения при переключении в этот режим: 

- Форматирование полей следующих четырех типов данных может измениться: 

   - Валюта 
   - Десятичные дроби (они всегда отображаются с двумя десятичными знаками) 
   - Даты (они всегда отображаются в формате ГГГГ-ММ-ДД)
   - Часовые пояса
- Поля, которые используются в режиме сводной таблицы и добавляются в метки столбцов, должны иметь небольшое количество различных значений.

   Если вы включите режим сводной таблицы и перетащите поле в область **Метки столбцов**, однако данные в этом поле имеют слишком много различных значений, вкладка браузера может перестать отвечать на запросы и в конечном итоге закроется, так что вам придется начать заново в новом сеансе. В этом случае либо не выполняйте свертывание по этому полю, либо установите фильтр на это поле, прежде чем добавлять его в область **Метки столбцов**.

## <a name="share-data-analysis"></a>Как поделиться анализом данных

После того как вы подготовили анализ на вкладке, вы можете поделиться им в виде ссылки с коллегами и другими сотрудниками вашей организации непосредственно из клиента. Ссылку смогут использовать только получатели, у которых есть разрешение на доступ к этой организации и этим данным.

1. На вкладке «Анализ» щелкните стрелку вниз, а затем выберите **Копировать ссылку**.

   ![Показано действие для копирования анализа](media/copy-analysis.svg)

   Откроется диалоговое окно **Ссылка на \<tab name\>**.

1. По умолчанию анализ, которым вы делитесь, будет ссылаться на страницу или запрос в организации, в которой вы сейчас работаете, что можно понять по фрагменту `company=<company_name>` в поле URL-адреса рядом с кнопкой **Копировать**. Если вы хотите отправить ссылку на анализ, не связанный с конкретной организацией, установите в поле **Организация:** значение **Не связывать с конкретной организацией**.

   ![Показано диалоговое окно копирования ссылки для вкладки анализа](media/analysis-link-copied.svg)

1. Выберите **Копировать**.

1. Вставьте ссылку в выбранное вами приложение для связи, например Word, Outlook, Teams, OneNote и т. д. 

2. Получатели смогут выбрать ссылку и открыть анализ для страницы или запроса в Business Central. Им будет предложено указать имя для новой вкладки анализа, которая будет создана.  

## <a name="limitations-in-2023-release-wave-1-preview"></a>Ограничения в волне 1 выпуска 2023 г. (предварительная версия)

Общедоступная предварительная версия этой функции имеет следующие ограничения:

- Представление режима анализа может содержать не более 100 000 строк. Если вы превысите этот лимит, отобразится соответствующее сообщение. Чтобы обойти это ограничение, установите фильтры на странице, прежде чем переключаться в режим анализа, если это возможно. Например, вы можете проанализировать определенную группу клиентов или данные только за текущий год. Вы также можете выбрать предустановленное представление, если оно подходит для вашего анализа.
- Функция «Поделиться» для анализа данных недоступна.
- Возможность сохранять предпочтительные варианты анализа данных на страницах списков и сохранять меню анализа для каждой вкладки анализа в настоящее время недоступна.

## <a name="see-also"></a>См. также

[Ad-hoc-анализ данных](reports-adhoc-analysis.md)  
[Просмотр и редактирование в Excel](across-work-with-excel.md)  
