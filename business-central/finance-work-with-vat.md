---
title: Как работать с НДС по продажам и покупкам
description: 'В этой статье описываются различные способы работы с НДС, как вручную, так и с автоматической настройкой, чтобы помочь вам соблюдать правила конкретной страны/региона.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'VAT, sales, purchases'
ms.search.form: '7, 118, 130, 142, 459, 460, 525'
ms.date: 05/29/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="work-with-vat-on-sales-and-purchases"></a>Работа с НДС по продажам и покупкам

Если в вашей стране или регионе требуется, чтобы вы рассчитывали и сообщали налог на добавленную стоимость (НДС) по сделкам купли-продажи, вы можете настроить [!INCLUDE[prod_short](includes/prod_short.md)] для расчета НДС. Дополнительные сведения см. в разделе [Настройка методов расчета и учета налога на добавленную стоимость](finance-setup-vat.md).

Однако есть некоторые связанные с НДС задачи, которые можно выполнять вручную. Например, может потребоваться исправить учтенную сумму, если обнаружится, что поставщик использует другой метод округления.  

> [!TIP]
> Вы можете позволить [!INCLUDE[prod_short](includes/prod_short.md)] проверять ИНН и другую информацию о компании при создании или обновлении документов. Для получения дополнительной информации см. [Проверка номеров ИНН](finance-how-validate-vat-registration-number.md).

## <a name="calculating-and-displaying-vat-amounts-on-sales-and-purchase-documents"></a>Расчет и отображение сумм НДС в документах продаж и покупок

При выборе номенклатурного номера в поле **Номер** в документе купли-продажи, [!INCLUDE[prod_short](includes/prod_short.md)] заполняет поля **Цена единицы** и **Сумма строки**. Цена за единицу берется с карточки **Товар** или из цен, разрешенных для данного продукта и клиента. [!INCLUDE[prod_short](includes/prod_short.md)] рассчитывает сумму строки только после ввода количества в данную строку.  

Если вы хотите, чтобы цены за единицу и суммы строк включали НДС — например, если вы продаете розничным потребителям — установите в документе флажок **Цены с учетом НДС**. Для получения дополнительной информации см. [Включение или исключение НДС в ценах и суммах строк](#including-or-excluding-vat-in-prices-and-line-amounts). 

Суммы НДС в документах продажи и покупки можно рассчитывать и отображать по-разному. Разница зависит от типа клиента или поставщика, с которым вы имеете дело. Можно также изменить рассчитанную сумму НДС вручную, например, для ее соответствия сумме НДС, рассчитанной поставщиком для данной транзакции.

### <a name="including-or-excluding-vat-in-prices-and-line-amounts"></a>Включение или исключение НДС в ценах и суммах строк

Если в документах на продажу установлен флажок **Цены с учетом НДС**, поля **Цена единицы** и **Сумма строки** включают НДС. По умолчанию значения в этих полях НДС не включают. Названия полей отражают, включают ли цены НДС.  

Можно настроить значение по умолчанию **Цены с учетом НДС** для всех документов продажи, передаваемых клиенту, в поле **Цены с учетом НДС** в карточке **Клиент**. Можно также настроить цены товаров с НДС или без НДС. Как правило, цены в карточке товара не включают НДС.

В следующей таблице показано, как приложение вычисляет цену за единицу для документа продажи, когда цены не настроены на странице **Цены продажи**:  

|**Поле Цена с НДС в карточке товара**|**Поле Цены с учетом НДС**|**Выполняемое действие**|  
|-----------------------------------------------|----------------------------------------------------|--------------------------|  
|Не включено|Не включено|**Цена единицы** в карточке продукта копируется в поле **Цена за ед. без НДС** в строках документа продажи.|  
|Не включено|Включено|Приложение вычисляет сумму НДС на единицу и прибавляет ее к значению **Цена единицы** на карточке товара. Итоговая цена за единицу затем вводится в поле **Цена за ед. с НДС** в строках продажи.|  
|Включено|Не включено|Приложение вычисляет сумму НДС, включенную в поле **Цена единицы** в **карточке товара**, используя процент НДС, связанный с комбинацией значений "НДС бизнес-группа (цена)" и "НДС товарная группа". **Цена единицы** на карточке продукта, уменьшенная на сумму НДС, вводится затем в поле **Цена за ед. без НДС** в строках документа продажи. Для получения дополнительной информации см. [Использование учетных бизнес-групп НДС и групп цен клиентов](finance-work-with-vat.md#using-vat-business-posting-groups-and-customer-price-groups).|  
|Включено|Включено|**Цена единицы** в карточке продукта копируется в поле **Цена за ед. с НДС** в строках документа продажи.|

#### <a name="using-vat-business-posting-groups-and-customer-price-groups"></a>Использование учетных бизнес-групп НДС и ценовых групп клиентов

Если вы хотите, чтобы цены включали НДС, вы можете использовать учетные бизнес-группы НДС для расчета суммы на основе настройки учета НДС для группы. Дополнительные сведения см. в разделе [Настройка НДС бизнес-групп](finance-setup-vat.md#set-up-vat-business-posting-groups).

В зависимости от того, что вы хотите сделать, вы можете назначить учетную бизнес-группу НДС клиентам или торговым документам следующими способами:

* Чтобы использовать одинаковую ставку НДС для всех клиентов, вы можете выбрать группу в поле **Учетная бизнес-группа НДС (Цена)** на странице **Настройка модуля "Продажи и дебитор. задолж."**.
* Чтобы использовать ставку НДС для конкретного клиента, вы можете выбрать группу в поле **Учетная бизнес-группа НДС (Цена)** на странице **Карточка клиента**. 
* Чтобы использовать ставку НДС для конкретных клиентов, вы можете выбрать группу в поле **Учетная бизнес-группа НДС (Цена)** на странице **Ценовая группа клиента**. Это удобно делать, например, когда вы хотите, чтобы цена применялась ко всем клиентам в определенном географическом регионе или в определенной отрасли.
* Во всех документах продажи в поле **Учетная бизнес-группа НДС**. Сумма НДС, указанная для группы, используется только для документа, над которым вы сейчас работаете.

> [!NOTE]
> Если вы не укажете группу в поле **Учетная бизнес-группа НДС (Цена)**, НДС не будет включен в цены.

#### <a name="examples"></a>Примеры

Такие факторы, как страна или регион, где вы продаете товары, или отрасль, предприятия которой являются вашими покупателями, могут влиять на сумму НДС, которую вы должны учитывать. Например, с ресторана может взиматься 6% НДС за блюда в помещении и 17% за еду на вынос. Для этого вы создаете одну учетную бизнес-группу учета НДС (цена) для помещения и другую для еды на вынос.

## <a name="working-with-vat-date"></a>Работа с датой НДС

### <a name="vat-date-in-documents"></a>Дата НДС в документах

Когда вы создаете новые документы продажи или покупки, **Дата НДС** основывается на настройке в поле **Дата НДС по умолчанию** на странице **Настройка ГК**. Это значение по умолчанию может быть таким же, как **Дата учета** или **Дата документа**. Если вам нужна другая дата НДС, вы можете вручную изменить значение в поле **Дата НДС**. Когда вы учитываете документ, **Дата НДС** отображается в учитываемом документе, а также в операциях НДС и ГК.

> [!NOTE]
> Если поле **Дата НДС** недоступно в ваших документах или журналах, это означает, что **Не использовать функциональность даты НДС** выбрано в поле **Использование даты НДС** на странице **Настройка главной книги** .  

> [!IMPORTANT]
> Если вы настроите **Управлять периодом НДС** в **Настройках главной книги** как **Блокировать учет в закрытом периоде** или **Блокировать учет в закрытом периоде и предупреждать за выпущенные в период проводки**, вы можете учесть документ или журнал, только если дата в поле **Дата НДС** не находится в закрытом периоде в разделе **Периоды возврата НДС**. Даже если период в разделе **Периоды возврата НДС** открыт, вы можете получить предупреждение на основе **Статуса возврата НДС** и настройки в **Управлять периодом НДС**.

> [!IMPORTANT]
> Начиная с версии 23.1 вы можете запретить или разрешить учет **Даты НДС** для определенного диапазона данных, используя поля **Разрешить дату НДС от** и **Разрешить дату НДС до** на страницах **Настройка НДС** и **Настройка пользователей**. Если вы используете более старые версии, вы можете запретить или разрешить учет **Даты НДС** для определенного диапазона данных, используя поля **Разрешить учет с** и **Разрешить учет по** на страницах **Настройка ГК** и **Настройка пользователей**.  

> [!NOTE]
> Если оставить поле **Дата НДС** пустым, [!INCLUDE [prod_short](includes/prod_short.md)] будет использовать настройку по умолчанию из **Дата НДС по умолчанию** в **Настройка главной книги** как **Дата НДС** в учтенной транзакции.  

### <a name="modifying-the-vat-date-in-posted-entries"></a>Изменение даты НДС в учтенных записях

При необходимости можно изменить дату НДС в учтенных документах. Чтобы изменить дату в поле **Дата НДС** для учтенных документов, необходимо выполнить следующие действия:

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок, введите **Операции НДС**, а затем выберите связанную ссылку. 
2. Найдите запись с неправильной датой НДС.  
3. Нажмите действие **Редактировать список** и введите правильную дату в поле **Дата НДС**.  
4. После того как вы закроете страницу, дата НДС в соответствующих **операциях ГК** и в учтенном документе меняется.  

> [!NOTE]
> Вы можете изменить поле **Дата НДС** в **Записях НДС**, только если ваша текущая дата не относится к закрытому периоду отчета по НДС. Даже если период в поле **Периоды возврата НДС** открыт, вы можете получить предупреждение на основе **Статуса возврата НДС**.  

> [!NOTE]
> Если в вашем документе несколько **Записей по НДС**, вам нужно изменить только значение в поле **Дата НДС** в одной записи, относящейся к документу. Чтобы обеспечить согласованность записей, [!INCLUDE[prod_short](includes/prod_short.md)] автоматически изменяет дату НДС в записях НДС, связанных с этой транзакцией. [!INCLUDE [prod_short](includes/prod_short.md)] обновит **Дату НДС** в других таблицах (Записи главной книги и документы), но только связанные с этой транзакцией.  

## <a name="correcting-vat-amounts-manually-on-sales-and-purchase-documents"></a>Ручная корректировка сумм НДС в документах продаж и покупок

Уже учтенные операции НДС можно корректировать, чтобы изменять общие суммы НДС по покупкам и продажам без изменения базы начисления НДС. Например, если вы получили счет-фактуру от поставщика с неправильной суммой НДС.  

Хотя вы можете настроить одну или несколько комбинаций для обработки импортного НДС, необходимо настроить хотя бы одну товарную учетную группу НДС. Например, можно присвоить название **ПРАВИЛЬНЫЙ** в целях корректировки за исключением случаев, когда вы будете использовать один и тот же счет Главной книги в поле **Счет НДС покупки** на строке настройки учета НДС. Дополнительные сведения см. в разделе [Настройка методов расчета и учета налога на добавленную стоимость](finance-setup-vat.md).

Если скидка по оплате была вычислена на основе суммы счета, включающей НДС, при предоставлении скидки по оплате сторнируется та часть суммы скидки, которая относится к сумме НДС. Необходимо активировать функцию **Коррекция для скидки оплаты** как в настройке ГК вообще, так и в настройке учета НДС для конкретных сочетаний НДС бизнес-группы и НДС товарной группы.  

### <a name="to-set-the-system-up-for-manual-vat-entry-in-sales-documents"></a>Чтобы настроить систему для ручного ввода НДС в торговых документах

Чтобы включить возможность изменения НДС вручную в документах продажи, выполните следующие действия. Шаги аналогичны шагам на странице **Настройка модуля "Покупки и кредиторская задолженность"**.

1. На странице **Настройка ГК** укажите значение параметра **Максимальная разрешенная разница НДС** между суммой, рассчитанной приложением и вручную.  
2. На странице **Настройка модуля «Продажи»** включите переключатель **Разрешить разницу НДС**.  

### <a name="to-adjust-vat-for-a-sales-document"></a>Корректировка НДС для документа продажи

1. Откройте соответствующий заказ на продажу.  
2. Выберите действие **Статистика**.  
3. На экспресс-вкладке **Выставление счетов** выберите значение в поле **Число строк налога**.
4. Измените поле **Сумма НДС**.   

> [!NOTE]  
> Общая сумма НДС по счету, сгруппированная по идентификатору НДС, отображается в строках. Сумму можно откорректировать вручную в поле **Сумма НДС** по строкам для каждого идентификатора НДС. При изменении поля **Сумма НДС** приложение проверяет, не был ли НДС изменен на сумму, превышающую указанную в качестве максимально допустимой разницы. Если сумма выходит за пределы **Максимальная разрешенная разница НДС**, появится предупреждающее сообщение с указанием максимальной допустимой разницы. Продолжить работу можно будет только после корректировки суммы до приемлемого значения. Щелкните **ОК** и введите другую **Сумма НДС**, находящуюся в допустимом диапазоне. Если разница НДС равна или меньше допустимого максимума, НДС будет поделен пропорционально между строками документа с одинаковым идентификатором НДС.  

## <a name="calculating-vat-manually-using-journals"></a>Расчет НДС вручную с использованием журналов

Можно также корректировать суммы НДС в финансовом журнале, журнале продаж и журнале покупок. Например, коррекция может понадобиться при вводе счета поставщика в журнал, если имеется разница между суммой НДС, рассчитанной [!INCLUDE[prod_short](includes/prod_short.md)], и суммой НДС, указанной в счете поставщика.  

### <a name="to-set-the-system-up-for-manual-vat-entry-in-general-journals"></a>Настройка системы для ручного ввода НДС в финансовых журналах

Необходимо выполнить следующие шаги, прежде чем вручную вводить НДС в финансовый журнал.  

1. На странице **Настройка ГК** укажите значение параметра **Максимальная разрешенная разница НДС** между суммой, рассчитанной приложением и вручную.  
2. На странице **Шаблоны финансового журнала** установите флажок **Разрешить разницу НДС** для соответствующего журнала.  

### <a name="to-set-the-system-up-for-manual-vat-entry-in-a-sales-and-purchase-journals"></a>Чтобы настроить систему для ручного ввода НДС в журналы продаж и покупок

Необходимо выполнить следующие шаги, прежде чем вручную вводить НДС в журнал продаж или покупок.

1. На странице **Настройка модуля "Покупки"** установите флажок **Разрешить разницу НДС**.  
2. Повторите шаг 1 для страницы **Настройка модуля "Продажи и дебитор. задолж."**.
3. По окончании настройки вы сможете корректировать поле **Сумма НДС** в строке финансового журнала или поле **Бал. - сумма НДС** в строке журнала продаж или покупок. [!INCLUDE[prod_short](includes/prod_short.md)] проверяет, не превышает ли разница заданное максимальное значение.  

> [!NOTE]  
> Если разница больше, отображается предупреждающее сообщение с указанием максимально допустимой разницы. Чтобы продолжить, нужно скорректировать сумму. Выберите **ОК**, затем введите сумму, соответствующую допустимому диапазону. Если разница НДС равна или меньше допустимого максимума, [!INCLUDE[prod_short](includes/prod_short.md)] покажет разницу в поле **Разница НДС**.  

## <a name="posting-import-vat-with-purchase-invoices"></a>Учет НДС на импорт со счетами покупки
Вместо использования журналов для учета счета НДС для импорта можно использовать счет покупки.  

### <a name="to-set-up-purchasing-for-posting-import-vat-invoices"></a>Настройка процесса покупки для учета счетов по импортному НДС

1. Настройте карточку поставщика для ответственного за импорт органа, который отправляет вам счета НДС для импорта. Необходимо настроить параметры **Общая бизнес-группа** и **НДС бизнес-группа** таким же образом, как и счет главной книги для НДС импорта.  
2. Создайте **Общую товарную группу** для НДС для импорта и настройте для НДС для импорта **стандартную товарную группу НДС** для связанной **Общей товарной группы**.  
3. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **План счетов**, а затем выберите связанную ссылку.  
4. Выберите счет главной книги НДС импорта, а затем выберите действие **Изменить**.  
5. На экспресс-вкладке **Учет** выберите настройку **Общая товарная группа** для НДС импорта. [!INCLUDE[prod_short](includes/prod_short.md)] автоматически заполнит поле **НДС товарная группа**.  
6. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок, введите **Общая настройка учета**, а затем выберите связанную ссылку.  
7. Создайте комбинацию **Общая бизнес-группа** для налогового органа НДС и **Общая товарная группа** для НДС импорта. Для этой комбинации в поле **Счет покупки** выберите счет импортного НДС главной книги.  

### <a name="to-create-a-new-invoice-for-the-import-authority-vendor-after-you-complete-the-setup"></a>Создание нового счета для поставщика, ответственного за импорт, по завершении настройки

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок введите **Счета покупки**, а затем выберите связанную ссылку.  
2. Создать новый счет покупки.  
3. В поле **Код поставщика (продавца)** выберите поставщика, ответственного за импорт, и затем нажмите кнопку **ОК**.  
4. В строке покупки в поле **Тип** выберите **Счет ГК** и в поле **Номер** выберите счет ГК НДС импорта.  
5. В поле **Кол-во** введите **1**.  
6. В поле **Прямая себест. единицы НДС** задайте сумму НДС.  
7. Учет счета.  

## <a name="processing-certificates-of-supply"></a>Обработка сертификатов поставки

При продаже товаров клиенту в другой стране или регионе ЕС, необходимо послать клиенту сертификат поставки, который клиент должен подписать и вернуть вам. В следующих процедурах показана обработка сертификатов поставки для расходных накладных продаж, однако те же шаги применимы к сервисным накладным продаж на товары и расходным накладным возврата поставщикам.  

### <a name="to-view-certificate-of-supply-details"></a>Просмотр сведений о сертификате поставки
1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок введите **Учтенные расходные накладные**, а затем выберите связанную ссылку.  
2. Выберите соответствующую расх. накладную продажи клиенту в другом регионе или стране ЕС.  
3. Выберите **Подробности сертификата поставки**.  
4. По умолчанию если в настройке группы учета НДС для клиента установлен флажок **Требуется сертификат поставки**, поле **Статус** имеет значение **Требуется**. Вы можете изменить значение поля, чтобы указать, вернул ли клиент сертификат.  

> [!Note]  
>  Если в настройке "Группа учета НДС" не установлен флажок **Требуется сертификат поставки**, создается запись, в поле **Статус** настраивается значение **Не применимо**. Можно обновить поле, чтобы отразить правильные сведения о статусе. Можно вручную изменить статус c **Не применимо** на **Требуется**, и с **Требуется** на **Не применимо**, как нужно.  

   При обновлении поля **Статус** на **Требуется**, **Получено** или **Не получено**, создается сертификат.  

> [!TIP]  
>  Можно использовать страницу **Сертификаты поставки** для получения представления о статусе всех учтенных отгрузок, для которых был создан сертификат поставки.  

5. Выберите **Печать сертификата поставки**.  

> [!Note]  
> Можно просмотреть или напечатать документ. При выборе **Печать сертификата поставки** и печати документа автоматически устанавливается флажок **Напечатано**. Кроме того, если еще не задано, статус сертификата обновляется на **Требуется**. Если требуется, напечатанный сертификат прилагается к отгрузке.  

### <a name="to-print-a-certificate-of-supply"></a>Печать сертификата поставки

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Учтенные расходные накладные**, а затем выберите связанную ссылку.  
2. Выберите соответствующую расх. накладную продажи клиенту в другом регионе или стране ЕС.  
3. Выберите действие **Печать сертификата поставки**.  

> [!NOTE]  
> Кроме того, можно напечатать сертификат со страницы **Сертификат поставки**.  

4. Для включения информации из строк в документе отгрузки в сертификат включите переключатель **Печать сведений о строке**.  
5. Чтобы дать [!INCLUDE[prod_short](includes/prod_short.md)] указание создавать сертификаты для учтенных расходных накладных, у которых их нет, включите переключатель **Создать сертификаты поставки, если они еще не созданы**. После включения этого переключателя новые сертификаты будут создаваться для всех учтенных расходных накладных без сертификатов в пределах выбранного диапазона.  
6. По умолчанию параметры фильтра соответствуют выбранному документу отгрузки. Заполните сведения о фильтре, чтобы выбрать конкретный сертификат поставки для печати.  
7. На странице **Сертификат поставки** выберите действие **Печать**, чтобы напечатать отчет, или действие **Предварительный просмотр**, чтобы просмотреть его на экране.  

   > [!Note]  
   > Поле **Статус сертификата поставки** и поле **Напечатано** обновляются для отгрузки на странице **Сертификаты поставок**.  

8. Отправьте напечатанный сертификат поставки клиенту на подпись.  

### <a name="to-update-the-status-of-a-certificate-of-supply-for-a-shipment"></a>Обновление статуса сертификата поставки для отгрузки

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), значок введите **Учтенные расходные накладные**, а затем выберите связанную ссылку.  
2. Выберите соответствующую расх. накладную продажи клиенту в другом регионе или стране ЕС.  
3. В поле **Статус** выберите соответствующий параметр.  

   Если клиент вернул подписанный сертификат поставки, выберите **Получен**. Поле **Дата прихода** обновляется. По умолчанию дата приемки назначается текущей рабочей датой.  

   Можно изменить дату, чтобы отразить дату получения подписанного клиентом сертификата поставки. Можно также добавить ссылку на подписанный сертификат, используя стандартную связь [!INCLUDE[prod_short](includes/prod_short.md)].  

   Если клиент не возвращает подписанный сертификат поставки, выберите **Не получен**. Затем необходимо отправить клиенту новый счет с НДС, поскольку первоначальный счет не будет принят налоговым органом.  

Для просмотра группы сертификатов откройте страницу **Сертификаты поставки**, а затем обновите информацию о статусе недостающих сертификатов по мере их возвращения клиентами. Обновленная информация может быть полезна, если вы хотите найти все сертификаты с определенным статусом, например **Требуется**, для которых нужно изменить статус на **Не получено**.  

### <a name="to-update-the-status-of-a-group-of-certificates-of-supply"></a>Обновление статуса группы сертификатов поставки

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Сертификаты поставки**, а затем выберите связанную ссылку.  
2. Фильтруйте поле **Статус** по нужному значению, чтобы создать список сертификатов, которыми требуется управлять.  
3. Для обновления информации о статусе выберите **Изменить список**.  
4. В поле **Статус** выберите соответствующий вариант.  

   Если клиент вернул подписанный сертификат поставки, выберите **Получен**. Поле **Дата прихода** обновляется. По умолчанию дата приемки назначается текущей рабочей датой.  

   Можно изменить дату, чтобы отразить дату получения подписанного сертификата поставки. Можно также добавить ссылку на подписанный сертификат, используя стандартную связь документа [!INCLUDE[prod_short](includes/prod_short.md)].  

> [!NOTE]
> Невозможно создать новый сертификат поставки на странице **Сертификат поставки** при осуществлении навигации с использованием этой процедуры. Чтобы создать сертификат для расходной накладной, не настроенной требовать такой сертификат, откройте учтенную расходную накладную продажи и воспользуйтесь любой из двух описанных выше процедур.  
>
> * Создание сертификата поставки вручную  
> * Печать сертификата поставки.

## <a name="see-also"></a>См. также

[Настройка методов расчета и учета налога на добавленную стоимость](finance-setup-vat.md)  
[Подача отчета об НДС в налоговый орган](finance-how-report-vat.md)  
[Проверка ИНН](finance-how-validate-vat-registration-number.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
