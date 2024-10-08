---
title: Использование табелей учета рабочего времени
description: 'Узнайте, как создавать, отправлять, утверждать и учитывать табели учета рабочего времени для ресурсов, проектов и услуг.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'project management, capacity, staff, resource, time sheets'
ms.search.form: '950, 951, 973'
ms.date: 02/05/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="use-time-sheets"></a>Использование табелей учета рабочего времени

В этой статье рассматривается, как использовать табели учета рабочего времени для отслеживания отсутствия, а также для отслеживания времени и ресурсов, затраченных на проект. Отслеживание времени позволяет на выявлять проблемы на ранних этапах, а также избегать задержек или перерасходов средств. Табели учета рабочего времени позволяют ресурсам легко отчитываться об использовании времени человеком или машиной, чтобы менеджеры могли проверять использование и распределение времени.

Можно скопировать и использовать в табеле строки планирования проекта. В этом способе необходимо только ввести информацию для одного места, и информация в строке всегда будет правильной. Подробнее см. в разделе [Копирование строк планирования проекта в табель учета рабочего времени](#copy-project-planning-lines-to-a-time-sheet).

После утверждения операций табеля для проекта их можно учесть в соответствующем журнале проектов или журнале ресурсов. Подробнее см. в разделах [Учет строк табеля в журнале проектов](#post-time-sheet-lines-in-a-project-journal) и [Учет строк табеля в журнале ресурсов](#post-time-sheet-lines-in-a-resource-journal).

Прежде чем использовать табели, необходимо настроить общую информацию и указать администратора и одного или нескольких утверждающих табелей. Подробнее о настройке табелей учета рабочего времени см. в статье [Настройка табелей учета рабочего времени](projects-how-setup-time-sheets.md).  

> [!TIP]
> Вы можете использовать табели учета рабочего времени на мобильном устройстве. Для этого вам может понадобиться перевести в положение «вкл.» переключатель **Использование нового интерфейса табелей учета рабочего времени** на странице [Настройка ресурсов](https://businesscentral.dynamics.com/?page=462).

## <a name="create-time-sheets"></a>Создание табелей учета рабочего времени

Вы можете использовать страницу **Создание табелей учета рабочего времени**, чтобы настроить табели для определенного количества периодов времени или недель. Затем владелец табеля может открыть его и записать время, которое было затрачено на задание. Вы также можете [запланировать автоматический запуск пакетного задания](ui-work-report.md#ScheduleReport).  

> [!IMPORTANT]
> Вы должны иметь разрешения на создание табелей. Подробнее о разрешениях см. в статье [Настройка табелей учета рабочего времени](projects-how-setup-time-sheets.md).

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") введите **Создать табели учета рабочего времени**, а затем выберите соответствующую ссылку.

    > [!TIP]
    > Вы также можете использовать действие **Создать табели учета рабочего времени** на странице списка **Ресурсы** и на странице **Карточка ресурса**.
2. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    > Прежде чем создавать табели учета рабочего времени для ресурса, убедитесь, что на странице **Карточка ресурса** для него заданы значения в полях **Использовать табель учета рабочего времени** и **Код пользователя владельца табеля**.

    При желании выберите действие **Расписание**, чтобы указать, как часто должна автоматически запускаться задача. Например, чтобы настроить запуск задачи еженедельно в течение четырех недель, на странице **Запланировать отчет — создать табели учета рабочего времени** в поле **Формула даты следующего запуска** введите **4W**. Подробнее о запуске отчетов по расписанию см. в статье [Планирование выполнения отчета](ui-work-report.md#ScheduleReport)  

Просмотреть созданные вами табели можно на странице **Табели учета рабочего времени**. Каждый табель учета рабочего времени состоит из одной или нескольких строк, которая определяет время, которое вы хотите отправить на утверждение. В следующей таблице описаны типы строк, которые можно добавить в табель учета рабочего времени.

| **Поле** | **Описание** |
|---|---|
| | Используйте, чтобы добавить примечание или отметку в поле **Описание** строки табеля учета рабочего времени. Например, это поле можно использовать для категоризации операций табеля. Если оставить поле **Тип** пустым для строки табеля, ввести значения времени в поля дней недели в этой строке будет нельзя. |
| Простой | Используется для регистрации времени, в течение которого вы отсутствуете во время рабочей недели. Чтобы предоставить информацию для строки, укажите тип отсутствия в поле **Код причины отсутствия**. |
| Заказ на сборку | Используется для регистрации времени для заказов на сборку. Строка табеля данного типа создается во время учета строк заказа на сборку, для которых ресурс настроен на использование табелей. Вручную выбрать строку этого типа невозможно. |
| Проекты | Используйте для регистрации распределения времени для проекта. Чтобы предоставить информацию для строки, укажите номер проекта и номер задачи проекта, время для которой вы хотите зарегистрировать. Можно регистрировать время для строк, которые не входят в график.|
| Ресурсы | Используйте для регистрации распределения времени для ресурса. Чтобы предоставить информацию для строки, введите описание работы. |
| Сервис | Используйте для регистрации распределения времени для сервисной кредит-ноты или сервисного заказа. |

Например, вы хотите отправить табель учета рабочего времени за неделю, когда вы выполняли работу по уборке и у вас был отгул для похода на прием к врачу. В следующей таблице показано, как вы в этом случае добавите строки в табель учета рабочего времени.

| Тип | Описание | Код вида работы | Код типа отсутствия |
|--|--|--|--|
| Ресурсы | Рабочие часы | Уборка |  |
| Простой | Выходной |  | Работоспособность |
|  | Мне пришлось взять выходной во вторник из-за приема у врача. |  |  |

В этом гипотетическом примере вы затем сможете зарегистрировать соответствующие часы в соответствующие дни для каждого дня недели.  

> [!TIP]
> В большинстве случаев у вашей компании есть предопределенные типы работы для различных типов строк. В таких случаях вы просто выбираете соответствующий тип работы из списка, а затем добавляете свое собственное описание.  
>
> Выберите вид работы, выбрав кнопку :::image type="icon" source="media/assist-edit-icon.png" border="false"::: в поле **Описание**, выбрав действие **Сведения о действии**, а затем указав его на открывшейся странице или выбрав его в поле **Код типа работы** или **Код типа отсутствия** соответственно. В этом случае вы можете игнорировать раздел [Определение видов работ и добавление вида работ в табель](#define-work-types-and-add-one-to-a-time-sheet).  

## <a name="reuse-time-sheet-lines-in-other-time-sheets"></a>Повторное использование строк табелей в других табелях

Если информация табеля не меняется от периода к периоду, скопируйте строки из предыдущего периода, чтобы сэкономить время. Затем просто вводите свое время работы для нового периода.

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок, введите **Табели учета рабочего времени**, а затем выберите связанную ссылку.  
2. Откройте табель дата периода, более позднего, чем период для существующего табеля со строками.  
3. Выберите действие **Копировать строки из предыдущих табелей**.

Строки копируются, включая подробную информацию, такую как тип и описание. Например, если строка связана с проектом, то поле **№ проекта** копируется. Все скопированные строки имеют статус **Открыто**. Теперь строки можно изменять, как требуется.

## <a name="copy-project-planning-lines-to-a-time-sheet"></a>Копирование строк планирования проекта в табель учета времени

Ниже описывается процедура быстрого добавления строк планирования проекта в табель.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Табели учета рабочего времени**, а затем выберите связанную ссылку.  
2. На странице **Табели учета рабочего времени** выберите табель учета рабочего времени для соответствующего периода времени.  
3. Выберите действие **Создать строки из планирования проекта**. Все строки планирования проекта в периоде времени табеля копируются в табель для человека или машины в поле **№ ресурса** табеля учета рабочего времени.

## <a name="define-work-types-and-add-one-to-a-time-sheet"></a>Определение видов работ и добавление вида работ в табель

Для всех строк табелей для сервисных заказов, проектных заказов и ресурсов можно задать вид работ. Таким образом можно добавить информацию, которая необходима, чтобы выставить счет клиенту за различные типы работ.  

1. На странице **Табели учета рабочего времени** выберите соответствующий табель.
2. В первой строке в разделе **Строки** выберите поле **Тип**, а затем выберите соответствующий тип, например *Ресурс*.  
3. Выберите поле **Описание**, а затем на странице **Сведения о ресурсе строки табеля учета рабочего времени** заполните поля. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  
    1. Если видов работ нет, выберите действие **Создать**.
    2. На странице **Типы работ** заполните поля по мере необходимости, затем вернитесь к табелю учета рабочего времени.
4. Заполните остальные поля табеля учета рабочего времени. Для получения дополнительной информации см. раздел [Заполнение строк табелей и отправка на утверждение](#fill-in-time-sheet-lines-and-submit-for-approval).  

> [!TIP]
> Определить коды отсутствия можно аналогичным образом.

## <a name="fill-in-time-sheet-lines-and-submit-for-approval"></a>Заполнение строк табелей и отправка на утверждение

Регистрация табеля отслеживается в часах (стандартной базовой единице измерения для ресурсов). По умолчанию в табеле отображаются общие рабочие дни с понедельника по пятницу.  

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Табели учета рабочего времени**, а затем выберите связанную ссылку.  
2. Выберите табель учета рабочего времени на соответствующий период.
3. Заполните поля в строке по мере необходимости. Введите количество часов, использованных ресурсом, для каждого дня недели.  

    В большинстве случаев для отслеживания работы вы добавляете строку типа *Ресурс*, а затем регистрируете часы, затрачиваемые каждый день. Если вы хотите зарегистрировать отсутствие, добавьте строку типа *Отсутствие*.  

    > [!TIP]  
    > Сумму введенных часов по табелю можно просмотреть на информационной панели **Сводка по фактическим и бюджетным суммам**.  
4. Повторите шаг 3 для других видов работ, которые выполняет ресурс.  

    Затем решите, хотите ли вы отправить все строки в табеле или только выбранные.  

    * Чтобы отправить табель для одной или нескольких строк, выберите соответствующую строку, а затем выберите действие **Отправить**.

        На странице отправки выберите вариант **Только выбранные строки**. Состояние строки меняется с **Открыто** на **Отправлено**.
    * Чтобы отправить табель учета рабочего времени для всех открытых строк, выберите действие **Отправить** в верхней части страницы **Табель учета рабочего времени**.  

        Подтвердите, что вы хотите отправить все открытые строки в текущем табеле.  

    > [!NOTE]  
    > Вы можете отправлять только строки табеля, для которых введено время.  
5. Чтобы изменить информацию в строке, для которой установлено значение **Представляется**, выделите строку и выберите действие **Открыть**.

    > [!NOTE]  
    > Менеджер может отклонить отправленную на утверждение строку табеля. Если строка имеет статус **Отклонено**, вы можете внести изменения в строку, а затем выбрать **Отправить** еще раз.  
6. Нажмите кнопку **ОК**.

## <a name="approve-or-reject-a-time-sheet"></a>Утверждение или отклонение табеля

Табель должны быть отправлен для утверждения, прежде чем его можно будет использовать. Вы можете утвердить или отклонить отдельные строки в табеле либо отправить их обратно отправителю. Утвердить табель можно двумя способами:

* Администратор табелей может утвердить любой табель.
* Лицо, указанное в поле **Код пользователя, утверждающего табель** в карточке ресурса, может утвердить табели этого ресурса. Подробнее о настройке утверждения см. в статье [Настройка табелей учета рабочего времени](projects-how-setup-time-sheets.md).

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок, введите **Табели учета рабочего времени для менеджера**, а затем выберите связанную ссылку.
2. Выберите табель в списке.  
3. На странице **Табель учета рабочего времени**: 
    1. Выберите действие **Обработка**, затем выберите действие **Утвердить**.
    2. Выберите действие **Все отправленные строки**, чтобы утвердить все строки, или действие **Только выбранные строки** для утверждения только строк, которые выбраны на странице **Табель учета рабочего времени**.
4. Нажмите кнопку **ОК**.  
5. Можно также выбрать действие **Отклонить** и выполнить шаги с 4 по 5.  

> [!TIP]  
> Используйте информационные панели **Статус табеля** и **Сводка по фактическим и бюджетным суммам** для общего просмотра сведений о табеле учета рабочего времени.

После утверждения или отклонения табеля его нельзя изменить, пока он не будет повторно открыт. В следующей процедуре объясняется, как повторно открыть утвержденный или отклоненный табель.

## <a name="reopen-a-time-sheet"></a>Повторное открытие табеля

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Табели учета рабочего времени для менеджера** или **Табели учета рабочего времени**, а затем выберите связанную ссылку.
2. Откройте табель из списка.  

    > [!NOTE]  
    > Повторно можно открыть только строки с состоянием **Утверждено**. Повторно открыть строки со статусом **Отклонено** или учтенные строки невозможно.  
3. На странице **Табель учета рабочего времени** выберите действие **Открыть повторно**, затем выберите действие **Все отправленные строки** для повторного открытия всех строк или действие **Только выбранные строки** для повторного открытия только строк, которые выбраны на странице **Табель учета рабочего времени**.
4. Нажмите кнопку **ОК**. Статус строки или строк табелей изменяется на **Представляется**.  

## <a name="view-and-approve-time-sheets-by-project"></a>Просмотр и утверждение табелей учета рабочего времени по проектам

В проекте можно определить человека, который является ответственным за этот проект. Эта информация связывается со строками табеля учета рабочего времени. Эта связь позволяет менеджерам проектов получить список табелей учета рабочего времени, которые необходимо утвердить. Например, менеджер команды проекта может быть ответственным за некоторые проекты в вашей организации. В этом случае менеджер должен быть обозначен как **Ответственное лицо** на странице «Карточка проекта». В этом представлении информации из табеля можно просмотреть задачи проекта, связанные с проектом, и израсходованное количество часов.

> [!NOTE]
> Чтобы утверждать табели учета времени на странице **Табели менеджера по проектам**, необходимо сначала установить флажок **Табель по утверждению проекта** на странице **Настройка модуля «Ресурсы»**. О том, как настраивать утверждения для ресурсов, см. в статье [Настройка ресурсов](projects-how-setup-resources.md).

### <a name="approve-or-reject-a-time-sheet-by-project"></a>Утверждение или отклонение табеля учета рабочего времени по проекту

1. В поле **Поиск** введите **Табели менеджера по проектам**, а затем выберите соответствующую ссылку. [!INCLUDE[prod_short](includes/prod_short.md)] отображает список строк табелей учета рабочего времени, связанных с проектами, за которые вы отвечаете.
2. Выберите действие **Утвердить**, затем выберите действие **Все отправленные строки** для утверждения всех строк или действие **Только выбранные строки** для утверждения только строк, которые выбраны на странице **Табель учета рабочего времени**.

    > [!NOTE]
    > Утвердить можно только те табели, которые имеют статус **Отправлено**.

3. Чтобы предоставить дополнительную информацию об утверждении или отклонении, выберите действие **Связанный**, затем выберите **Комментарии** и **Комментарии к строке**.
4. Нажмите кнопку **ОК**.

> [!NOTE]
> После утверждения или отклонения строки табеля по проекту его нельзя будет заново открыть или изменить на странице **Табель учета рабочего времени**.

## <a name="post-time-sheet-lines-in-a-resource-journal"></a>Учет строк табеля в журнале ресурсов

После утверждения операций табеля для ресурса можно выполнять их учет в соответствующем журнале ресурсов.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Журналы ресурсов**, а затем выберите связанную ссылку.  
2. Выберите действие **Предлагать строки из табелей**.  
3. На странице **Предложить строки журнала ресурсов** заполните требуемые поля. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)] 
4. Нажмите кнопку **ОК**. Операции для использования создаются в журнале ресурсов, в котором можно изменить информацию как нужно.  
5. Выберите действие **Учет**.  
6. Чтобы проверить учет, выберите действие **Книга операций**. Открывается страница **Операции книги ресурсов** с результатом учета журнала ресурсов.

## <a name="post-time-sheet-lines-in-a-project-journal"></a>Учет строк табеля в журнале проектов

После утверждения операций табеля для проекта можно учесть их в соответствующем журнале проектов.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") введите **Журналы проектов**, а затем выберите соответствующую ссылку.  
2. Выберите действие **Предлагать строки из табелей**.  
3. На странице **Предложить строки журнала проектов** заполните требуемые поля. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)] 
4. Нажмите кнопку **ОК**. Операции использования создаются в журнале проектов, где вы может внести в информацию необходимые изменения.  

    > [!NOTE]  
    > Информация о виде работы и о том, оплачивается ли эта работа, копируется из строки табеля. Если необходимо, можно сократить количество и выполнить частичный учет. Если уменьшить количество, то при следующем выборе действия **Предлагать строки из табелей** строка будет содержать оставшееся количество часов.  
5. Выберите действие **Учет**.  
6. Чтобы проверить учет, выберите действие **Книга операций**. Открывается страница **Операции книги проектов** с результатом учета журнала ресурсов.

## <a name="archive-time-sheets"></a>Архивация табелей учета рабочего времени

После учета табелей их можно поместить в архив для обращения к ним в будущем. Прежде чем архивировать табель, необходимо учесть все строки в нем.

> [!NOTE]  
> При архивации табель учета рабочего времени удаляется из списков на страницах **Табели учета рабочего времени** и **Табели учета рабочего времени для менеджера**.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Табели учета рабочего времени**, а затем выберите связанную ссылку.
2. Выберите действие **Переместить табели учета рабочего времени в архив**.  
3. На странице **Переместить табели учета рабочего времени в архив** заполните поля, как требуется, и нажмите кнопку **ОК**.  
4. Чтобы просмотреть архивированные табели учета рабочего времени, выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Архивы табелей учета рабочего времени** или **Архивы табелей учета рабочего времени для менеджера**, а затем выберите связанную ссылку.

## <a name="see-also"></a>См. также

[Управление проектами](projects-manage-projects.md)  
[Настройка управления проектами](projects-setup-projects.md)  
[Финансы](finance.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Продажи](sales-manage-sales.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
