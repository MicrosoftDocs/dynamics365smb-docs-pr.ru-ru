---
title: 'Установите стоимость ресурсов проекта, цены и мощность'
description: 'Для использования ресурсов и функций управления проектами необходимо определить себестоимость и цены для отдельных ресурсов и групп ресурсов, а также задать производственную мощность ресурсов.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'project management, capacity, staff'
ms.search.form: '72, 76, 77, 203, 204'
ms.date: 08/19/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="set-up-resources-for-projects"></a>Настройка ресурсов для проектов

Для правильного управления деятельностью ресурсов необходимо настроить ресурсы, а также связанные с ними затраты и цены. Связанные с проектом цены, скидки и правила коэффициента себестоимости задаются в карточке проекта. Затраты и цены можно установить для каждого отдельного ресурса, группы ресурсов или всех доступных ресурсов организации.

При использовании или продаже ресурсов для проекта связанные с ними цены и затраты извлекаются из заданной вами информации.

Сумму в час, используемую по умолчанию, можно указать после создания ресурса. Например, при использовании в проекте определенной машины в течение пяти часов проект будет рассчитываться на основании суммы в час.

> [!NOTE]
> Вы не можете приобрести внешние ресурсы для конкретного проекта. Вместо этого мы рекомендуем использовать элементы типа «Услуга».

## <a name="to-set-up-a-resource"></a>Настройка ресурса

Создайте карточки для каждого ресурса, который требуется использовать в проектах.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Ресурсы**, а затем выберите связанную ссылку.
2. Выберите действие **Создать**.
3. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-set-up-a-resource-group"></a>Настройка группы ресурсов

Можно комбинировать несколько ресурсов в одной группе ресурсов. Все произв. мощности и бюджеты групп ресурсов суммируются для отдельных ресурсов. Можно также вводить произв. мощности групп ресурсов либо независимо от суммарных значений, либо в дополнение к ним.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Группы ресурсов**, а затем выберите связанную ссылку.
2. Выберите действие **Создать**.
3. Заполните соответствующим образом поля.

## <a name="to-set-capacity-for-a-resource"></a>Настройка производственной мощности ресурса

Чтобы рассчитать количество времени, которое ресурс может потратить на проекты, сначала необходимо настроить производственную мощность ресурса как доступное время на период в рабочем календаре. Эта настройка используется при заполнении строк планирования проекта, которые содержат ресурс. Дополнительные сведения см. в статье [Создание проектов](projects-how-create-jobs.md).

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Ресурсы**, а затем выберите связанную ссылку.
2. Откройте соответствующую карточку ресурса и выберите действие **Производственная мощность ресурсов**.
3. На странице **Производственная мощность ресурсов** в поле **Просмотр по** укажите продолжительность периода, например **День**, которая будет отображаться в столбцах на экспресс-вкладке **Матрица производственной мощности ресурсов**.
4. Для каждого ресурса в строке укажите для каждого периода в столбцах количество часов, в течение которых доступен ресурс.
5. Либо, чтобы детализировать еженедельную производственную мощность ресурса в пределах даты начала и даты окончания, выберите действие **Установить произв. мощность**.
6. На странице **Настройка произв. мощности ресурса** заполните требуемые поля.
7. Выберите действие **Обновить произв. мощность**. Страница **Производственная мощность ресурсов** обновится для отображения введенной производственной мощности.
8. Закройте страницу.

## <a name="to-set-up-alternate-resource-costs"></a>Настройка альтернативных затрат на ресурсы

В дополнение к себестоимости, указанной в карточке ресурса, можно задать альтернативные значения себестоимости для каждого ресурса. Например, если для конкретного сотрудника определена более высокая почасовая ставка за работу во внеурочное время, можно создать стоимость ресурса для ставки за работу во внеурочное время. Установленная для ресурса альтернативная стоимость при использовании этого ресурса в журнале ресурсов будет замещать стоимость, указанную в карточке ресурса.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Ресурсы**, а затем выберите связанную ссылку.  
2. Выберите ресурс, для которого нужно настроить одну или несколько альтернативных затрат, затем выберите действие **Затраты**.  
3. На странице **Стоимости ресурсов** заполните требуемые поля в строке.  
4. Повторите шаг 3 для каждой альтернативной себестоимости ресурса, которую необходимо настроить.

> [!NOTE]
> Чтобы настроить стоимость ресурсов, которая применяется ко всем ресурсам и группам ресурсов, откройте страницу **Стоимость ресурсов**  и заполните поля.

## <a name="to-set-up-alternate-resource-prices"></a>Настройка альтернативных цен ресурсов

В дополнение к цене, указанной в карточке ресурса, можно задать альтернативные цены для каждого ресурса. Эти альтернативные цены могут быть условными. Они могут зависеть от того, используются ли ресурсы с определенным типом проектов или типом работы.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Ресурсы**, а затем выберите связанную ссылку.
2. Выберите ресурс, для которого нужно настроить одну или несколько альтернативных цен, затем выберите действие **Цены**.
3. На странице **Цены ресурсов** заполните требуемые поля в строке.
4. Повторите шаг 3 для каждой альтернативной цены ресурса, которую необходимо настроить.

## <a name="to-adjust-resource-prices"></a>Корректировка цен ресурсов

Для изменения стоимости или цен большого количества ресурсов рекомендуется воспользоваться пакетным заданием.  

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок, введите **Коррекция цен/стоимостей ресурсов**, а затем выберите соответствующую связь.
2. Заполните поля в строке, как требуется, и нажмите кнопку **ОК**.

> [!NOTE]  
> Это пакетное задание не создает и не корректирует альтернативные затраты или цены на ресурсы. Это меняет только содержимое поля в карточке ресурса для поля **Коррекция поля**, выбранного в пакетном задании. Корректировка вступает в силу для ресурсов немедленно, поэтому проверьте коэффициенты корректировки перед запуском пакетного задания.

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a>Получения предложений по изменению цены ресурса на основе существующих альтернативных цен

Если вы уже настроили альтернативные цены на некоторые ресурсы, вы можете использовать пакетное задание для настройки нескольких альтернативных цен на ресурсы.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Изменение цен ресурсов**, а затем выберите связанную ссылку.
2. Выберите действие **Предлож. изменения цен ресурсов (цена)**, затем заполните поля, как требуется.
3. Нажмите кнопку **ОК**.  
4. После выполнения пакетного задания страница **Изменение цен ресурсов** показывает результаты пакетного задания.

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a>Получение предложений по изменению цены ресурса на основе стандартных цен

Если требуется настроить несколько альтернативных цен ресурсов на основе стандартных цен из карточек ресурсов, можно воспользоваться пакетным заданием.  

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Изменение цен ресурсов**, а затем выберите связанную ссылку.
2. Выберите действие **Предлож. изменение цен ресурсов (рес.)**, затем заполните поля, как требуется.  
3. Нажмите кнопку **ОК**.  
4. После выполнения пакетного задания откройте страницу **Изменение цен ресурсов** для просмотра результатов пакетного задания.

## <a name="see-also"></a>См. также

[Настройка управления проектами](projects-setup-projects.md)  
[Управление проектами](projects-manage-projects.md)  
[Финансы](finance.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Продажи](sales-manage-sales.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
