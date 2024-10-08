---
title: Отчеты и аналитика по запасам и складу
description: 'Посмотрите, какие отчеты и аналитика по запасам и складу доступны в стандартной версии Business Central, чтобы вы могли отслеживать свой бизнес.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: 'Report_707, Report_716, Report_813, Report_1001, Report_5807, Report_5808, Report_5809, Report_7313, Report_7319, Report_7320'
ms.date: 08/15/2024
ms.custom: bap-template
ms.service: dynamics-365-business-central
---
# <a name="inventory-and-warehouse-reports-and-analytics"></a>Отчеты и аналитика по запасам и складу

Отчетность по запасам и складу в [!INCLUDE [prod_short](includes/prod_short.md)] позволяет специалистам по управлению запасами и другим бизнес-пользователям получать информацию и статистические данные о текущей и прошлой деятельности по запасам и складу.  

## <a name="reports"></a>Отчеты

[!INCLUDE [inventory_WMS_reports](includes/inventory-WMS-reports-include.md)]

## <a name="tasks"></a>Задачи

В следующих статьях описываются некоторые ключевые задачи анализа состояния вашего бизнеса:

* [Создание аналитических отчетов](bi-how-create-analysis-views-reports.md)  
* [Просмотр наличия товаров](inventory-how-availability-overview.md)

## <a name="print-and-scan-barcodes"></a>Печать и сканирование штрихкодов

Использование штрихкодов помогает оптимизировать входящие, исходящие и внутренние складские процессы. 

[!INCLUDE [barcode-mobile-app](includes/barcode-mobile-app.md)]

После установки приложения вы можете использовать действие **Печать этикетки** для печати линейных и двумерных штрихкодов со страниц, перечисленных в следующей таблице.

|Стр.  |штрихкоды значений полей могут включать  |
|---------|---------|
|Товары, Карточка товара     |№ товара, Описание, Код GTIN         |
|Список ссылок на товар, Ссылка на товар     |№ товара, Описание, Единица измерения, № ссылки         |
|Информационный список номеров партий, Этикетка с № партии     |№ товара, Описание, Номер партии       |
|Этикетка с серийным №     |№, Описание, Серийный номер         |

> [!NOTE]
> Некоторые принтеры и форматы штрихкодов/QR-кодов требуют специальной реализации. Возможно, вам придется загрузить другой шаблон Word или клонировать отчет, чтобы создать свою собственную версию.
>
> Обратитесь к поставщику оборудования, чтобы узнать, как печатать документы Word на вашем устройстве.  

## <a name="explore-inventory-reports-with-report-explorer"></a>Знакомство с отчетами по запасам с помощью обозревателя отчетов

Чтобы ознакомиться с доступными отчетами для управления запасами, выберите **Все отчеты** на своей домашней странице. Откроется обозреватель ролей, в котором показаны только функции группы **Отчет и анализ**. Под заголовком **Продажи и маркетинг** выберите **Обзор**.

:::image type="content" source="media/report-explorer-sales.png" alt-text="Пример отчетов в финансовом ролевом центре." lightbox="media/report-explorer-sales.png":::

Подробнее см. в статье [Поиск отчетов с помощью обозревателя ролей](ui-role-explorer.md).

## <a name="see-also"></a>См. также

[Ad-hoc-анализ данных запасов](ad-hoc-analysis-inventory.md)  
[Обзор аналитики запасов](inventory-analytics-overview.md)  
[Настройка запасов](inventory-setup-inventory.md)  
[Запасы](inventory-manage-inventory.md)  
[Настройка управления складом](warehouse-setup-warehouse.md)  
[Обзор управления складом](design-details-warehouse-management.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
