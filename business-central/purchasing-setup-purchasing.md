---
title: Обзор задач по настройке покупок
description: Описывает задачи по определению политик закупки организации и настройки процессы покупки.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: overview
ms.devlang: al
ms.search.keywords: 'procurement, supply, vendor order'
ms.search.form: '175, 176, 177, 178, 456, 460, 5727, 5729'
ms.date: 06/10/2024
ms.service: dynamics-365-business-central
---
# <a name="setting-up-purchasing"></a>Настройка покупок

Прежде чем приступать к управлению процессами закупки, необходимо настроить правила и значения, которые определяют политики закупок в организации.

Вы должны определить общую настройку на странице **Настройка модуля "Покупки и кредиторская задолженность"**, что обычно делается один раз во время первоначального внедрения. Узнайте больше в следующем разделе, [Настройка модуля «Покупки и кредиторская задолженность»](#purchases-and-payables-setup).

Отдельная серия задач, связанных с регистрацией новых поставщиков, заключается в регистрации любых соглашений по цене и предоставлению скидок, заключенных с каждым поставщиком.

Настройка параметров покупок, связанных с финансами, например способов оплаты и валют, рассмотрены в разделе настройки финансов. Узнайте больше в разделе [Настройка Finance](finance-setup-finance.md). Точно так же настройки покупки, связанные с запасами, такие как единицы измерения и коды отслеживания товаров, можно найти в[разделе "Настройка инвентаря"](inventory-setup-inventory.md).

## <a name="purchases-and-payables-setup"></a>Настройка модуля "Покупки и поставщики"

Перед работой с закупками и кредиторской задолженностью уточните на странице **Настройка модуля "Покупки и кредиторская задолженность"**, как разносятся стоимости покупок, и серии номеров, используемые для поставщиков и документов покупки.

### <a name="general-settings"></a>Общие настройки

На экспресс-вкладке **Общее** определяются такие параметры, как способ расчета и учета скидок, а также потребность в округлении счетов. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].

Некоторые поля требуют особого внимания, например, поле **Расчет скидки по счету для ид. НДС**, которое указывает, рассчитывается ли скидка по счету в соответствии с идентификатором налога или общей суммой счета. Узнайте больше в разделе [Объединение НДС учетных групп в настройках учета НДС](finance-setup-vat.md#combine-vat-posting-groups-in-vat-posting-setups).

Точно так же поле **Применение между валютами** может привести к небольшой разнице округления при применении записей в разных валютах друг к другу. Подробнее см. в разделе [Включение операций книги в разных валютах](finance-how-enable-application-ledger-entries-different-currencies.md).

Кроме того, некоторые поля меняют свое поведение или зависят от того, как установлены другие поля. Например, функция **Проверять предоплату при учете** зависит от того, как задано поле **Автоматическое обновление предоплаты** установлено для проверки ожидающих предоплат.

Подробности о полях [**Номер внеш. документа обязателен**](#external-document-number) и [**Точный возврат себест. обязат.**](#exact-cost-reversing) приведены в следующих разделах в этой статье.

### <a name="number-series-settings"></a>Параметры серий номеров

На экспресс-вкладке **Серии номеров** необходимо указать уникальные идентификационные коды, которые будут использоваться для поставщиков, счетов и других документов покупки. Нумерация важна не только для внутренних процессов, но может также требоваться для соблюдения требований местных регуляторов. Так что, возможно, стоит подумать о настройке всех серий на странице **Серия номеров** заранее, вместо того, чтобы создавать новые из пункта **Настройка модуля "Покупки и кредиторская задолженность"**. Дополнительные сведения см. в разделе [Создание серий номеров](ui-create-number-series.md).

## <a name="external-document-number"></a>Номер внешнего документа

[!INCLUDE [ext-doc-no-purch](includes/ext-doc-no-purch.md)]

## <a name="exact-cost-reversing"></a>Точное сторнирование себестоимости

Функция **Точный возврат себест. обязат.** помогает гарантировать, что возвращенные товары оцениваются по той же стоимости, что и при их первоначальном извлечении из запасов, с использованием фиксированного применения, а не по методу средней себестоимости или «первым пришел — первым вышел» (FIFO). Узнайте больше в разделе [Сведения о проектировании: фиксированное применение](design-details-item-application.md#fixed-application). Если в дальнейшем к первоначальной покупке будет добавлена дополнительная стоимость, то стоимость возвращенной покупки будет соответствующим образом обновлена.

Когда эта функция включена, транзакция возврата может быть учтена только путем указания номера операции журнала товаров в поле **Примен. к товарной операции** строки заказа на возврат покупки. По умолчанию это поле не отображается на экспресс-вкладке **Строки**. О том, как добавлять поля на страницы, см. в разделе [Персонализация рабочей области](ui-personalization-user.md#start-personalizing-by-using-the-personalization-mode).

[!INCLUDE[local-functionality](includes/local-functionality.md)]

## <a name="more-purchasing-setups"></a>Дополнительные настройки покупки

| По | Ссылка |
| --- | --- |
| Создание карточки поставщика для каждого поставщика, у которого производится покупка. |[Регистрация новых поставщиков](purchasing-how-register-new-vendors.md) |
| Назначение приоритетов поставщикам. |[Назначение приоритетов поставщикам](purchasing-how-prioritize-vendors.md) |
| Введите информацию о банковском счете, &mdash; включая коды IBAN и SWIFT, &mdash; в карточку поставщика. | [Настройка банковских счетов поставщика](purchasing-how-set-up-vendors-bank-accounts.md) |
| Настройте покупателей, назначьте им поставщиков и коды для отслеживания статистики. |[Настройка менеджеров по закупкам](purchasing-how-setup-purchasers.md) |
| Введите различные скидки и специальные цена, которые предлагает поставщик в зависимости от товара, количества или даты. |[Регистрация соглашений о цене покупки, скидках и платежах](purchasing-how-record-purchase-price-discount-payment-agreements.md) |
| Определите, сколько вы платите за товары и услуги, приобретаемые вашей компанией.  | [Настройка цен и скидок](across-prices-and-discounts.md) |
| Создайте стандартные строки для вставки в типовые документы покупки. | [Настройка типовых строк покупок](purchasing-how-work-recurring-purchase-lines.md) |
| Создавайте последовательности задач для соединения процессов, выполняемых разными пользователями, таких как запрос и утверждение заказов на покупку. | [Настройка рабочих процессов утверждения покупок](across-set-up-workflows.md) |
| Управляйте бизнес-взаимодействиями с вашими поставщиками, импортируйте полученные документы счетов и регистрируйте новых поставщиков с помощью почтового клиента Outlook. | [Настройка надстройки Business Central для Outlook](admin-outlook.md) |
| Просматривайте квитанции о расходах, преобразовывайте бумажные и электронные документы в строки журнала и оцифровывайте бумажные счета от поставщиков. | [Настройка входящих документов](across-how-setup-income-documents.md) |
| Укажите отчеты по умолчанию, которые будут использоваться для различных типов документов. |[Выбор отчета в Business Central](across-report-selections.md)|
|Укажите, разрешено ли пользователям принимать к учету счета-фактуры покупки и должны ли они принимать их к учету вместе с отгрузкой. |[Определение политики учета счетов для пользователей](admin-setup-invoice-posting-policy.md)|

## <a name="see-also"></a>См. также

[Покупки](purchasing-manage-purchasing.md)  
[Обзор настройки](setup.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
