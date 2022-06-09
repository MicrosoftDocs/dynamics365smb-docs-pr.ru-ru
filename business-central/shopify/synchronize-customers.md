---
title: Синхронизация клиентов
description: Импорт клиентов из или экспорт в Shopify
ms.date: 05/11/2022
ms.topic: article
ms.service: dynamics365-business-central
author: edupont04
ms.author: andreipa
ms.reviewer: solsen
ms.openlocfilehash: 92ac46e9f7e69204b4c7edee4aa430a8786b6c0b
ms.sourcegitcommit: f071aef3660cc3202006e00f2f790faff849a240
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "8768158"
---
# <a name="synchronize-customers"></a>Синхронизация клиентов

При импорте заказа из Shopify информация о клиенте необходима для дальнейшей обработки документа в [!INCLUDE[prod_short](../includes/prod_short.md)]. Существует два основных варианта и их комбинации:

* Использование конкретного клиента для всех заказов.
* Импорт фактической информации о клиентах из Shopify. Этот параметр также доступен при первом экспорте клиента в Shopify из [!INCLUDE[prod_short](../includes/prod_short.md)].

## <a name="how-connector-chooses-which-customer-to-use"></a>Как соединитель выбирает, какого клиента использовать

Функция *Импорт заказа из Shopify* пытается выбрать клиента в следующем порядке:

1. Если **№ клиента по умолчанию** определяется в **Шаблоне клиента Shopify** для соответствующей страны, то используется **№ клиента по умолчанию** независимо от настроек параметров **Импорт клиентов из Shopify** и **Тип сопоставления клиентов**.
2. Если параметры **Импорт клиентов из Shopify** и **№ клиента по умолчанию** определены, то используется **№ клиента по умолчанию** .

Дальнейшие действия зависят от параметра **Тип сопоставления клиентов**.

* **Всегда брать клиента по умолчанию**, затем используйте клиента, определенного в поле **№ клиента по умолчанию** в окне **Карточка магазина Shopify**.
* **По электронной почте/телефону**, соединитель сначала пытается найти существующего клиента по идентификатору, затем по электронной почте, а затем по телефону. Если клиент не найден — соединитель создает нового клиента.
* **По информации о плательщике**, соединитель сначала пытается найти существующего клиента по идентификатору, а затем по информации об адресе для выставления счета. Если клиент не найден — соединитель создает нового клиента.

> [!NOTE]  
> Соединитель использует информацию из адреса для выставления счетов и создает клиента для выставления счетов в формате [!INCLUDE[prod_short](../includes/prod_short.md)]. Клиент, которому продают, соответствует клиенту, которому выставляют счет.

## <a name="important-settings-when-importing-customers-from-shopify"></a>Важные настройки при импорте клиентов из Shopify

Либо вы импортируете клиентов из Shopify оптом, либо вместе с импортом заказов, следующие настройки позволяют управлять процессом:

|Поле|Описанием|
|------|-----------|
|**Импорт клиентов из Shopify**|Выберите **Все клиенты**, если вы планируете импортировать клиентов из Shopify оптом; либо вручную с помощью действия **Синхронизировать клиентов**, либо через очередь заданий для повторяющихся обновлений. Независимо от выбора информация о клиенте всегда будет импортироваться вместе с заказом. Однако использование этой информации зависит от **шаблонов клиентов Shopify** и настроек поля **Тип сопоставления клиентов**.|
|**Тип сопоставления клиентов**|Определите, как вы хотите, чтобы соединитель выполнял сопоставление.<br>- **По электронной почте/телефону**, если вы хотите, чтобы соединитель сопоставлял импортированного клиента Shopify с существующим клиентом в [!INCLUDE[prod_short](../includes/prod_short.md)], используя электронную почту и телефон.</br>- **По информации о плательщике**, если вы хотите, чтобы соединитель сопоставлял импортированного клиента Shopify с существующим клиентом в [!INCLUDE[prod_short](../includes/prod_short.md)], используя адресную информацию стороны, которая получает счет.</br>Выберите **Всегда брать клиента по умолчанию**, если вы хотите, чтобы система использовала клиента из поля **№ клиента по умолчанию** . |
|**Shopify может обновлять клиентов**| Выберите этот параметр, если вы хотите, чтобы соединитель обновлял найденных клиентов, когда в поле **Тип сопоставления клиентов** выбраны параметры **По электронной почте/телефону** или **По информации о плательщике**.|
|**Автоматическое создание неизвестных клиентов**| Выберите этот параметр, если вы хотите, чтобы соединитель создавал отсутствующих клиентов, когда в поле **Тип сопоставления клиентов** выбраны параметры **По электронной почте/телефону** или **По информации о плательщике**. Новый клиент будет создан с использованием импортированных данных и **кода шаблона клиента**, определенного на страницах **Карточка магазина Shopify** или **Шаблон клиента Shopify**. Обратите внимание, что клиент Shopify должен иметь хотя бы один адрес. Если эта опция не включена, вам нужно будет создать клиента вручную и связать его с клиентом Shopify. Вы всегда можете инициировать создание клиента вручную со страницы **Заказ Shopify**.|
|**Код шаблона клиента**|Используется вместе с параметром **Автоматическое создание неизвестных клиентов**.<br> Выберите шаблон по умолчанию, который будет использоваться для автоматически созданных клиентов. Вы можете определить шаблоны для каждой страны или региона в окне **Шаблон клиентов Shopify**, которое удобно для правильного расчета налога. Дополнительные сведения см. в разделе [Примечания относительно налогов](synchronize-orders.md#tax-remarks).|

### <a name="customer-template-per-country"></a>Шаблон клиента для каждой страны

Некоторые настройки могут быть определены на уровне страны (региона) или на уровне штата (провинции). Настройки можно настроить в разделе [Отгрузка и доставка](https://www.shopify.com/admin/settings/shipping) в Shopify.

**Шаблон клиента Shopify** позволяет вам сделать следующее для каждой страны:

1. Указать **№ клиента по умолчанию**, который имеет приоритет над выбором в полях **Импорт клиентов из Shopify** и **Тип сопоставления клиентов**. Он используется в импортированном заказе на продажу.
2. Определить **Код шаблона клиента**, который используется для создания отсутствующих клиентов, если включен параметр **Автоматическое создание неизвестных клиентов**. Если **код шаблона клиента** не заполнен, то функция использует **код шаблона клиента**, определенный в **карточке магазина Shopify**.
3. В некоторых случаях **кода шаблона клиента** на страну недостаточно для правильного расчета налогов. Например, для стран, в которых действует налог с продаж.

> [!NOTE]  
> Коды стран — это коды стран по ISO 3166-1 alpha-2. Дополнительные сведения см. на веб-сайте [Коды стран](https://help.shopify.com/en/api/custom-storefronts/storefront-api/reference/enum/countrycode).

## <a name="export-customers-to-shopify"></a>Экспорт клиентов в Shopify

Существующие клиенты могут быть экспортированы в Shopify оптом. В результате создается клиент и один адрес по умолчанию. Вы можете управлять процессом с помощью следующих настроек:

|Поле|Описанием|
|------|-----------|
|**Экспорт клиентов в Shopify**|Выберите этот пункт, если вы планируете экспортировать всех клиентов с действительным адресом электронной почты из [!INCLUDE[prod_short](../includes/prod_short.md)] в Shopify оптом; либо вручную с помощью действия **Синхронизировать клиентов**, либо через очередь заданий для повторяющихся обновлений.|
|**Может обновлять клиентов Shopify**|Используется вместе с **Экспорт клиента в Shopify**. Включите его, если вы хотите генерировать обновления позже из [!INCLUDE[prod_short](../includes/prod_short.md)] для клиентов, которые уже существуют в Shopify.|

> [!NOTE]  
> Как только вы создали клиентов в Shopify, вы можете отправить клиентам прямые приглашения. Это побудит их активировать свою учетную запись.

### <a name="populate-customer-information-in-shopify"></a>Заполните информацию о клиенте в Shopify

Клиент в Shopify имеет имя, фамилию, адрес электронной почты и/или номер телефона. Вы можете заполнить имя и фамилию на основе данных из карточки клиента в [!INCLUDE[prod_short](../includes/prod_short.md)].

|Приоритет|Поле в карточке клиента|Описанием|
|------|------|-----------|
|1|**Имя контакта**|Имеет высший приоритет, если заполнено поле **Имя контакта**, а поле **Источник контакта** в **карточке магазина Shopify** содержит параметры *Имя и фамилия* или *Фамилия и имя*, определяющие, как разделить значения.|
|2|**Имя 2**|Если заполнено поле **Имя 2**, а поле **Источник имени 2** в **карточке магазина Shopify** содержит параметры *Имя и фамилия* или *Фамилия и имя*, определяющие, как разделить значения.|
|3|**Название**|Имеет низший приоритет, если заполнено поле **Имя**, а поле **Источник имени** в **карточке магазина Shopify** содержит параметры *Имя и фамилия* или *Фамилия и имя*, определяющие, как разделить значения.|

Клиент в Shopify также имеет адрес по умолчанию, который помимо имени, фамилии, электронной почты и/или телефона может содержать информацию о компании и адресе. Вы можете заполнить поле **Компания** на основе данных из карточки клиента в [!INCLUDE[prod_short](../includes/prod_short.md)].

|Приоритет|Поле в карточке клиента|Описанием|
|------|------|-----------|
|1|**Название**|Имеет высший приоритет, если поле **Источник имени** в **карточке магазина Shopify** содержит *Название компании*.|
|2|**Имя 2**|Имеет низший приоритет, если поле **Источник имени 2** в **карточке магазина Shopify** содержит *Название компании*.|

Для адресов, где используется страна или провинция, выберите *Код* или *Имя* в поле **Источник страны** в **карточке магазина Shopify**, чтобы указать, какой тип данных хранится в [!INCLUDE[prod_short](../includes/prod_short.md)] в поле **Страна**.

## <a name="sync-customers"></a>Синхронизация клиентов

1. Нажмите на значок поиска ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../media/ui-search/search_small.png "Что вы хотите сделать"), значок, введите **магазин Shopify** и выберите связанную ссылку.
2. Выберите магазин, для которого вы хотите синхронизировать клиентов, чтобы открыть страницу **Карточка магазина Shopify**.
3. Выберите действие **Синхронизировать клиентов**.

В качестве альтернативы вы можете использовать действие **Запустить синхронизацию клиентов** в окне **Клиенты Shopify** или поиск пакетного задания **Синхронизация клиентов**.

## <a name="see-also"></a>См. также

[Начало работы с соединителем для Shopify](get-started.md)  