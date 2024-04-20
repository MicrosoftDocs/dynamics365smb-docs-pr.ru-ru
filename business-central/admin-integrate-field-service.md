---
title: Интеграция с Microsoft Dynamics 365 Field Service
description: 'Узнайте, как интегрировать Business Central c Field Service.'
ms.date: 02/21/2024
ms.topic: article
author: brentholtorf
ms.author: bholtorf
ms.reviewer: ivkoleti
ms.custom: bap-template
---

# <a name="integrate-with-microsoft-dynamics-365-field-service"></a>Интеграция с Microsoft Dynamics 365 Field Service

Сервисным организациям требуется сквозное приложение, в котором финансы, запасы и закупки тесно связаны с предоставлением услуг. Они генерируют финансовые данные при каждой транзакции. Каждый заказ на работу представляет собой затраты и доходы, а каждый ресурс генерирует прибыль и убытки. Взаимодействия с клиентами добавляют записи в главную книгу. Интеграция между [!INCLUDE [prod_short](includes/prod_short.md)] и [!INCLUDE [field-service-short](includes/field-service-short.md)] упрощает сквозной процесс управления операциями обслуживания и обеспечивает плавный поток информации между двумя системами.  

Вы можете легко создавать заказы на работу и управлять ими в [!INCLUDE [field-service-short](includes/field-service-short.md)], отслеживать ход выполнения сервисных задач, назначать ресурсы и собирать сведения о потреблении. Когда вы завершаете заказ на работу в [!INCLUDE [field-service-short](includes/field-service-short.md)], интеграция обеспечивает плавную передачу данных в [!INCLUDE [prod_short](includes/prod_short.md)] для дальнейшей обработки.  

Интеграция также упрощает выставление счетов и выполнение заказов на работу в [!INCLUDE [prod_short](includes/prod_short.md)]. Вы можете генерировать точные счета на основе оказанных услуг и потребления, записанных в [!INCLUDE [field-service-short](includes/field-service-short.md)].  

Благодаря интеграции [!INCLUDE [prod_short](includes/prod_short.md)] с [!INCLUDE [field-service-short](includes/field-service-short.md)] вам не придется вводить данные вручную или дублировать усилия. Интеграция также обеспечивает комплексное представление об операциях обслуживания и финансовых показателях, что позволяет лучше принимать решения и повышать операционную эффективность.

## <a name="prerequisites"></a>Предварительные требования

Поскольку [!INCLUDE [field-service-short](includes/field-service-short.md)] построен на основе Dynamics 365 Sales, необходимо [настроить подключение к Dataverse](/dynamics365/business-central/admin-how-to-set-up-a-dynamics-crm-connection#to-use-the-dataverse-connection-setup-assisted-setup-guide) и [включить интеграцию с Dynamics 365 Sales](/dynamics365/business-central/admin-prepare-dynamics-365-for-sales-for-integration#connection-settings-in-the-setup-guide).

### <a name="permissions-and-security-roles-for-user-accounts"></a>Разрешения и роли безопасности для учетных записей пользователей

При установке решения интеграции разрешения для учетной записи пользователя интеграции настраиваются. Если эти разрешения изменились, вам может потребоваться сбросить их. Для этого заново установите решение интеграции со страницы **Настройка подключения Dynamics 365**, выбрав **Повторить развертывание решения интеграции**. В следующих разделах перечислены разрешения и роли безопасности, которые решение развертывает для каждого приложения.

#### <a name="sales"></a>Продажа

* Администратор интеграции Dynamics 365 [!INCLUDE [prod_short](includes/prod_short.md)]/
* Пользователь интеграции с Dynamics 365 [!INCLUDE [prod_short](includes/prod_short.md)]
* Пользователь наличия товара Dynamics 365 [!INCLUDE [prod_short](includes/prod_short.md)]

#### <a name="business-central"></a>Business Central

Пользователи, разносящие журналы проектов, должны иметь следующий набор разрешений:

* Интеграция с Dynamics 365 Sales

#### <a name="field-service"></a>Выездное обслуживание

Чтобы использовать интегрированные данные, пользователи должны иметь следующую роль безопасности:

* Интеграция Business Central с Field Service

Например, пользователи должны иметь эту роль, чтобы подключать заказы на работу к [!INCLUDE [prod_short](includes/prod_short.md)] для обработки.

> [!NOTE]
> Убедитесь, что пользователям назначены стандартные роли и профили безопасности в [!INCLUDE [field-service-short](includes/field-service-short.md)].  
>
> Чтобы узнать больше о профилях безопасности столбцов в [!INCLUDE [field-service-short](includes/field-service-short.md)], перейдите к разделу [Роли безопасности Field Service](/dynamics365/field-service/users-licenses-permissions#field-service-security-roles).
>
> Администраторы должны добавить один из соответствующих профилей безопасности столбцов для пользователей в Power Platform. Чтобы узнать больше, перейдите к разделу [Добавление групп или пользователей в профиль безопасности столбцов для управления доступом](/power-platform/admin/add-teams-users-field-security-profile).

> [!NOTE]
> Для использования действия **Открыть в Business Central** в Sales у вас должны быть следующие привилегии в отношении следующих таблиц:

У вас должны быть разрешения на **чтение** в отношении таблицы **Подключение к Dynamics 365 Business Central** (nav_connection).
У вас должны быть разрешения на **чтение**, **запись** и **удаление** в отношении таблицы **Подключение к Dynamics 365 Business Central по умолчанию** (nav_defaultconnection).

### <a name="other-settings-in-field-service"></a>Другие настройки в Field Service

На странице **Настройки Field Service** выполните следующие настройки:

* На вкладке **Покупка** очистите поле **Использование продуктов, отсутствующих в наличии**. В противном случае вы можете получить предупреждение об отсутствии на складе при выборе продукта, которого нет в наличии в [!INCLUDE [field-service-short](includes/field-service-short.md)], но который есть в наличии в [!INCLUDE [prod_short](includes/prod_short.md)].
* На вкладке **Заказ на работу/Резервирование** отключите выключатели **Рассчитать цену** и **Рассчитать себестоимость**. В поле **Создание счета по заказу на работу** выберите **Никогда**.

> [!NOTE]
> Настройка подключения к [!INCLUDE [field-service-short](includes/field-service-short.md)] удаляет связь между ресурсами и продуктами. Чтобы сделать номенклатуры [!INCLUDE [prod_short](includes/prod_short.md)] доступными в [!INCLUDE [field-service-short](includes/field-service-short.md)], обновите поле **Тип продукта Field Service**, чтобы оно соответствовало полю **Тип** в номенкелатурах в [!INCLUDE [prod_short](includes/prod_short.md)]. Чтобы узнать больше, перейдите к разделу [Создание продукта или услуги](/dynamics365/field-service/create-product-or-service#create-a-product-or-service).

## <a name="set-up-the-integration-in-business-central"></a>Настройка интеграции в Business Central

После подключения к Dataverse и Sales вы можете настроить интеграцию с [!INCLUDE [field-service-short](includes/field-service-short.md)]. На странице **Мастер настройки** в [!INCLUDE [prod_short](includes/prod_short.md)] выберите **Настроить интеграцию с Dynamics 365 Field Service**, чтобы запустить руководство мастера настройки. В этом разделе описаны ключевые настройки в руководстве.

Чтобы люди могли разносить потребление товаров и услуг в заказах на работу [!INCLUDE [field-service-short](includes/field-service-short.md)], укажите **Шаблон журнала проекта** и **Пакет журнала проекта** для разноски потребления продуктов и услуг.

Поскольку услуги выражаются в продолжительности в [!INCLUDE [field-service-short](includes/field-service-short.md)], укажите **Единицу измерения «часы»**, чтобы использовать ее для преобразования длительности в количества в [!INCLUDE [prod_short](includes/prod_short.md)].

Можно также указать, когда синхронизировать строки продуктов и услуг по заказам на работу с [!INCLUDE [prod_short](includes/prod_short.md)]. Например, они могут синхронизироваться при использовании строк заказа на работу или когда кто-то выполняет заказ на работу. Выберите подходящий вариант в поле **Синхронизировать продукты/услуги заказа на работу**.

После того как продукты и услуги заказов на работу синхронизируются с журналами проектов в [!INCLUDE [prod_short](includes/prod_short.md)], вы можете выбрать, следует ли разносить журналы проектов вручную. Выберите подходящий вариант в поле **Автоматически разносить строки журналов проектов**:

* При завершении заказа на работу.
* Когда используются продукты или услуги заказов на работу.

После завершения настройки запустите полную синхронизацию со страницы **Настройка интеграции Dynamics 365 Field Service**. Это действие синхронизирует сопоставления таблиц для таких вещей, как:

* Задачи проекта для проектов с установленным флажком **Применить связь использования**. Эта синхронизация делает проекты [!INCLUDE [prod_short](includes/prod_short.md)] доступными для выбора в [!INCLUDE [field-service-short](includes/field-service-short.md)].
* Ресурсы, которые не заблокированы, не имеют выбранного флажка **Использовать табель** и имеют **Часы**, указанные как единица измерения, на странице **Настройка интеграции Dynamics 365 Field Service**.
* Сервисные номенклатуры (требуется, чтобы вы используете премиум-версию в [!INCLUDE [prod_short](includes/prod_short.md)]).

## <a name="standard-field-service-entity-mapping-for-synchronization"></a>Сопоставление стандартных сущностей Field Service для синхронизации

Основой синхронизации данных является сопоставление таблиц и полей в [!INCLUDE [prod_short](includes/prod_short.md)] с таблицами и столбцами в Dataverse, чтобы они могли обмениваться данными. Сопоставление происходит через таблицы интеграции. Чтобы узнать больше о сопоставлениях таблиц, перейдите к разделу [Сопоставление таблиц и полей для синхронизации](/dynamics365/business-central/admin-how-to-modify-table-mappings-for-synchronization).

Интеграция с [!INCLUDE [field-service-short](includes/field-service-short.md)] представляет следующие стандартные сопоставления таблиц интеграции.

* **PJLINE-WORDERPRODUCT** — сопоставляет продукты заказа на работу в [!INCLUDE [field-service-short](includes/field-service-short.md)] со строками журнала проекта в [!INCLUDE [prod_short](includes/prod_short.md)].
* **PJLINE-WORDERSERVICE** — сопоставляет услуги заказа на работу в [!INCLUDE [field-service-short](includes/field-service-short.md)] со строками журнала проекта в [!INCLUDE [prod_short](includes/prod_short.md)].
* **PROJECTTASK** — сопоставляет проекты и задачи проекта в [!INCLUDE [prod_short](includes/prod_short.md)] с продуктами во внешних проектах в [!INCLUDE [field-service-short](includes/field-service-short.md)].
* **RESOURCE-BOOKABLERSC** — сопоставляет ресурсы в [!INCLUDE [prod_short](includes/prod_short.md)] с резервируемыми ресурсами в [!INCLUDE [field-service-short](includes/field-service-short.md)].
* **SVCITEM-CUSTASSET** — (только премиум-интерфейс) сопоставляет сервисные номенклатуры в [!INCLUDE [prod_short](includes/prod_short.md)] с активами клиента в [!INCLUDE [field-service-short](includes/field-service-short.md)].

## <a name="use-data-in-both-applications"></a>Использование данных в обоих приложениях

В следующих разделах описаны функции, в которых можно использовать данные из [!INCLUDE [prod_short](includes/prod_short.md)] и [!INCLUDE [field-service-short](includes/field-service-short.md)].

### <a name="field-service-1"></a>Выездное обслуживание

Вы можете [создавать **Заказы на работу**](/dynamics365/field-service/create-work-order) с помощью **Учетной записи службы** и **Учетная запись для выставления счетов** из [!INCLUDE [prod_short](includes/prod_short.md)]. В заказах на работу необходимо выбрать **Задача проекта Business Central** в поле **Внешний проект**. Выбор проекта позволяет синхронизировать продукты и услуги заказа на работу с соответствующей задачей проекта в [!INCLUDE [prod_short](includes/prod_short.md)].

Вы можете добавлять запасы и не относящиеся к запасам номенклатуры как **Продукты заказа на работу** в заказы на работу и получать количество в наличии, а также себестоимость и цены из [!INCLUDE [prod_short](includes/prod_short.md)]. Чтобы узнать больше, перейдите к разделу [Создание заказа на работу из формы заказа на работу и списка записей](/dynamics365/field-service/create-work-order#create-a-work-order-from-the-work-order-form-and-record-list).

Вы можете добавить номенклатур типа услуга как **Услуги по заказам на работу** и получать себестоимость и цены из [!INCLUDE [prod_short](includes/prod_short.md)]. Чтобы узнать больше, перейдите в раздел [Вкладка продуктов и услуг](/dynamics365/field-service/work-order-experience#products-and-services-tab).

> [!NOTE]
> Когда статус продукта или услуги в заказе на работу меняется с **Оценено** на **Использовано** в [!INCLUDE [field-service-short](includes/field-service-short.md)], они будут синхронизированы со строками журнала проекта в [!INCLUDE [prod_short](includes/prod_short.md)].

Вы можете зарезервировать ресурс и связать **Резервирования** с услугами заказов на работу, используя **Резервируемый ресурс** из [!INCLUDE [prod_short](includes/prod_short.md)].

### <a name="business-central-1"></a>Business Central

В зависимости от ваших настроек на странице **Настройка интеграции Field Service**, когда заказы на работу включают продукты и услуги, информация о потреблении переносится и разносится с использованием **Журнала проекта** в [!INCLUDE [prod_short](includes/prod_short.md)].

Значения **Количество для выставления счета** и **Длительность для выставления счета** копируются в поле **Кол-во - для переноса в счет**. На основе этих значений вы можете создавать и разносить счета-фактуры по продажам в [!INCLUDE [prod_short](includes/prod_short.md)] , чтобы выставить счет клиенту. После того как счет-фактура разнесен или потребление обработано в [!INCLUDE [prod_short](includes/prod_short.md)], выставленное в счете количество и потребленное количество отображаются на вкладке [!INCLUDE [prod_short](includes/prod_short.md)] на страницах **Продукт заказа на работу** и **Услуга заказа на работу**.  

Используйте страницу **Строки планирования проекта**, чтобы отслеживать разноски и выставление счетов за потребление по заказам на работу. На странице **Строки планирования проекта** можно создавать и разносить счета-фактуры по продажам в [!INCLUDE [prod_short](includes/prod_short.md)]. После этого вы можете синхронизировать их с [!INCLUDE [field-service-short](includes/field-service-short.md)] и отслеживать статус счетов.

> [!NOTE]
> Услуги заказов на работу с резервированием, использующим резервируемый ресурс, связанный с ресурсом [!INCLUDE [prod_short](includes/prod_short.md)], синхронизируются с двумя строками журнала проекта. Одна строка типа **Бюджет** для связанного ресурса и другая строка типа **Оплачиваемый** для обслуживаемого элемента.
>
> Продукт, выбранный в услуге заказа на работу, должен быть связан с номенклатурой типа **Услуга** в [!INCLUDE [prod_short](includes/prod_short.md)]. Кроме того, базовая единица измерения для номенклатуры должна быть установлена ​​на **Единица измерения «часы»**, выбранную на странице **Настройки интеграции Dynamics 365 Field Service**.
>
> Вы можете создать счет для номенклатуры типа **Услуга** из строки планирования оплачиваемого проекта и использовать строку планирования бюджетного проекта для регистрации затрат в ресурсе.

## <a name="see-also"></a>См. также

[Интеграция с Microsoft Dataverse посредством синхронизации данных](admin-common-data-service.md)  
[Сопоставление таблиц и полей для синхронизации](admin-how-to-modify-table-mappings-for-synchronization.md)
