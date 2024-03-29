---
title: Отчеты и аналитика по запасам и складу
description: 'Посмотрите, какие отчеты и аналитика по запасам и складу доступны в стандартной версии Business Central, чтобы вы могли отслеживать свой бизнес.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: 'Report_707, Report_716, Report_813, Report_1001, Report_5807, Report_5808, Report_5809, Report_7313, Report_7319, Report_7320'
ms.date: 04/13/2023
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

## <a name="see-also"></a>См. также

[Настройка запасов](inventory-setup-inventory.md)  
[Запасы](inventory-manage-inventory.md)  
[Настройка управления складом](warehouse-setup-warehouse.md)  
[Обзор управления складом](design-details-warehouse-management.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
