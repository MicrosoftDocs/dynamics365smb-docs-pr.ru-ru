---
title: 'Сведения о проектировании: входящий складской поток'
description: 'Узнайте, как оформлять приемку товаров на складе, регистрировать их и сопоставлять с входящими документами-источниками.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: warehouse
ms.date: 09/18/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="design-details-inbound-warehouse-flow"></a>Технические подробности: входящий складской поток

Входящий поток на складе начинается с прибытия товаров на склад компании из внешних источников или с другого склада компании. Можно получать физические и нескладируемые товары. Подробнее о приемке нескладируемых товаров см. в статье [Учет нескладируемых товаров](#post-non-inventory-items).

В принципе, процесс получения входящих заказов состоит из двух действий:

* Получение товаров в зоне приемки, где вы идентифицируете товары, сопоставляете их с исходным документом и регистрируете полученное количество.
* Размещение товаров на складе и регистрация места, где вы их разместили.

Исходными документами для входящего складского потока являются:

* Заказы на покупку  
* Входящие заказы на перемещение  
* Заказы на возврат продажи  

> [!NOTE]
> Выходные данные производства и сборки также представляют собой входящие исходные документы. Дополнительные сведения об обработке выводов производства и сборки для внутренних процессов см. в разделе [Сведения о проектировании: внутренние складские потоки](design-details-internal-warehouse-flows.md).  

В [!INCLUDE[prod_short](includes/prod_short.md)] получение и размещение происходит с использованием одного из четырех методов, как описано в следующей таблице.

|Метод|Входящий процесс|Требуется приемка|Требуется размещение|Уровень сложности (подробнее см. в разделе [Обзор Warehouse Management](design-details-warehouse-management.md))|  
|------------|---------------------|--------------|----------------|------------|  
|А|Выполните учет приемки и размещения из строки заказа|||Нет отдельной складской операции.|  
|Б|Выполните учет приемки и размещения из документа складского размещения||Включено|База: последовательно по каждому заказу.|  
|Т|Выполните учет приемки и размещения из документа складской приемки|Включено||База: объединенная проводка получения/отправки для нескольких заказов.|  
|Д|Выполните учет приемки из документа складской приемки и учет размещения из документа складского размещения|Включено|Включено|Дополнительно|  

Выбор подхода зависит от практик вашей организации и уровня организационной сложности. Ниже приведены некоторые примеры, которые могут помочь вам принять решение.

* В складской среде последовательного выполнения заказов, где большая часть персонала склада работает непосредственно с документами заказа, вы можете решить использовать метод А. 
* На складе с последовательным выполнением заказов, на котором выполняются более сложные процессы размещения или где сотрудники склада отделяют свои действия по размещению от документа заказа, можно использовать метод B.
* Организациям, которым требуется планирование обработки нескольких заказов, может быть полезно использовать документы складской приемки, методы В и Г.  

При использовании методов A, Б и В приемка и размещение объединены в один шаг при учете документов как полученных. При использовании метода Г сначала учитывается приемка для записи увеличения запасов и того, что товары доступны для продажи. Затем сотрудник склада регистрирует размещение, чтобы сделать товары доступными для подбора для исходящих заказов. 

> [!NOTE]
> Хотя размещения на складе и размещения запасов звучат похоже, это разные документы, которые используются в разных процессах.
> * Размещение запасов, используемое в методе B, вместе с регистрацией информации о размещении также принимает к учету получение исходного документа.
> * Размещение на складе, используемое в методе Г, не может быть проведено и только регистрирует размещение. Регистрация делает товары доступными для дальнейшей обработки, но не разносит приемку. Во входящем потоке для размещения на складе требуется складская приемка.

## <a name="no-dedicated-warehouse-activity"></a>Нет отдельной складской операции

В следующих статьях содержится информация о том, как обрабатывать поступления для исходных документов, если у вас нет выделенных складских заданий.

* [Регистрация покупок](purchasing-how-record-purchases.md)
* [Заказы на перемещение](inventory-how-transfer-between-locations.md)
* [Обработка заказов на возврат продажи](sales-how-process-sales-returns-orders.md)

## <a name="basic-warehouse-configurations"></a>Базовые конфигурации склада

В базовой конфигурации склада переключатель **Требуется размещение** включен, но переключатель **Требуется приемка** отключен на странице **Карточка склада** для склада.

На следующей схеме показаны входящие складские потоки по типам документов в базовых конфигурациях склада. Номер на схеме соответствует шагам в разделах после схемы.  

:::image type="content" source="media/design_details_warehouse_management_inbound_basic_flow.png" alt-text="Входящий поток в базовых конфигурациях склада.":::

### <a name="1-release-a-source-document-to-create-a-request-for-an-inventory-put-away"></a>1. Запрос размещения запасов путем выпуска исходного документа

При получении товаров выпустите исходный документ, например заказ на покупку или входящий заказ на перемещение. Выпуск документа делает товары доступными для размещения. Можно также создать документы размещения запасов для отдельных строк заказа в режиме распределения на основе ячеек и количеств для обработки.  

### <a name="2-create-an-inventory-put-away"></a>2. Создание размещения запасов

На странице **Размещение запасов** в режиме извлечения можно получить ожидающие строки исходного документа на основе входящих складских запросов. В режиме распределения также можно создавать строки размещения запасов при создании исходного документа.  

### <a name="3-post-an-inventory-put-away"></a>3. Учет размещения запасов

В каждой строке товаров, которые были полностью или частично размещены, работник склада заполняет поле **Количество**, а затем разносит размещение запасов. Документы-источники, связанные со складским размещением, учитываются как полученные.  

* Создаются положительные операции книги товаров.
* Складские операции создаются для складов, которым требуется код ячейки для всех операций с товарами.
* Запрос на размещение удаляется, если он полностью обработан. Например, обновляется поле **Полученное кол-во** во входящей строке документа-источника.
* Создается учтенный документ приемки, например, со сведениями о заказе на покупку и полученными товарами.  

## <a name="advanced-warehouse-configurations"></a>Расширенные конфигурации склада

Чтобы использовать расширенную конфигурацию склада, переведите в положение «вкл.» переключатель **Требуется приемка** на странице «Карточка склада» для склада. Переключатель **Требуется размещение** является необязательным.

На следующей схеме показан входящий складской поток по типу документов. Номер на схеме соответствует шагам в разделах после схемы.  

:::image type="content" source="media/design_details_warehouse_management_inbound_advanced_flow.png" alt-text="Расширенный входящий поток на складе.":::

### <a name="1-release-the-source-document"></a>1. Выпуск исходного документа

При получении товаров выпустите исходный документ, например заказ на покупку или входящий заказ на перемещение. Выпуск документа делает товары доступными для размещения. Размещение содержит ссылки на тип и номер исходного документа.

### <a name="2-create-a-warehouse-receipt"></a>2. Создание складской приемки

Строки исходного документа отображаются на странице **Складская приемка**. Несколько строк исходного документа можно объединить в один документ складской приемки. Заполните поле **Кол-во для обработки** и при необходимости выберите зону приемки и ячейку.  

### <a name="3-post-the-warehouse-receipt"></a>3. Учесть складскую приемку

Разнесите складскую приемку для создания положительных операции книги товаров. Поле **Полученное кол-во** в строке входящего исходного документа обновлено.  

Если переключатель **Требуется размещение** не включен в карточке склада, на этом процесс останавливается. В противном случае учет входящего исходного документа делает товары доступными для размещения. Размещение содержит ссылки на тип и номер исходного документа.  

### <a name="4-optional-generate-put-away-worksheet-lines"></a>4. Создание строк журнала размещения (необязательно)

Получите строки складского размещения в **журнале размещения** на основе учтенных складских приемок или операций, которые производят продукцию. В строках, которые вы собираетесь разместить на складе, укажите следующую информацию:

* Ячейки, из которых брать товары.
* Ячейки, в которые положить товары.
* Сколько единиц обрабатывать.

Ячейки могут быть предопределены настройкой местоположения склада или ресурса, выполнившего операцию.  

Если все размещения спланированы и присвоены складским рабочим, создайте документы складского размещения. Полностью назначенные строки размещения удаляются из **Журнала размещения**.  

> [!NOTE]  
> Если переключатель **Использовать журнал размещения** не включен в карточке склада, документы складского размещения создаются непосредственно на основе учтенных складских приемок. В этом случае этот шаг не нужен.  

### <a name="5-create-a-warehouse-put-away-document"></a>5. Создание документа складского размещения

Создайте документ складского размещения в режиме извлечения на основе учтенной складской приемки. В качестве альтернативы создайте документ складского размещения и назначьте работнику склада в режиме распределения.  

### <a name="6-register-a-warehouse-put-away"></a>6. Регистрация складского размещения

В каждой строке товаров, которые были полностью или частично размещены, заполните поле **Количество** на странице **Складское размещение**, а затем зарегистрируйте складское размещение.  

* Складские операции создаются для складов, которым требуется код ячейки для всех операций с товарами.
* Строки складского размещение удаляются, если они полностью обработаны.
* Документ складского размещения остается открытым до тех пор, пока вы не зарегистрируете все количество в соответствующей учтенной складской приходной накладной.
* Поле **Кол-во для размещения** в учтенных строках заказа складской приемки обновляется.

## <a name="related-tasks"></a>Связанные задачи

В следующей таблице приводится последовательность задач со ссылками на статьи, в которых они описываются.

|**Чтобы**|**Смотрите**|  
|------------|-------------|  
|Получение товаров на складах с оформлением складской приходной накладной для полностью или частично автоматизированной обработки складских операций.|[Приемка товаров](warehouse-how-receive-items.md)|
|Размещение товаров отдельно для каждого заказа и учет приемки в одном действии в базовых конфигурациях склада.|[Размещение товаров с помощью складского размещения](warehouse-how-to-put-items-away-with-inventory-put-aways.md)|  
|Размещайте товары, полученные от нескольких покупок, возвратов продаж, заказах на перемещение в расширенной конфигурации склада.|[Размещение товаров с использованием складских размещений](warehouse-how-to-put-items-away-with-warehouse-put-aways.md)|  

## <a name="post-non-inventory-items"></a>Учет нескладируемых товаров

[!INCLUDE [post-non-inventory-items](includes/post-non-inventory-items.md)]

## <a name="see-also"></a>См. также

[!INCLUDE[footer-include](includes/footer-banner.md)]
