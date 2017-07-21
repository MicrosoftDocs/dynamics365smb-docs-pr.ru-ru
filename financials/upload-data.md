---
title: "Импорт устаревших бизнес-данных в Financials | Документы Майкрософт"
description: "Вы можете перенести данные по клиентам, поставщикам и запасам, например из Excel, QuickBooks или Dynamics GP, в Financials."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: migrate, initialize, implement
ms.date: 07/05/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 2a38dc36cb9ff609c5582acd489841b20013d4bc
ms.openlocfilehash: dd6eb5a6b19bf4c8fd92674a48e8cd29ce912eee
ms.contentlocale: ru-ru
ms.lasthandoff: 07/07/2017


---
# <a name="importing-business-data-from-other-finance-systems"></a>Импорт бизнес-данных из других финансовых систем
При регистрации в [!INCLUDE[d365fin](includes/d365fin_md.md)] вы можете создать пустую организации, чтоб загрузить собственные данные и протестировать новую организацию [!INCLUDE[d365fin](includes/d365fin_md.md)]. В зависимости от финансового решения, которое вы используете сейчас, вы можете перенести информацию о клиентах, поставщиках, запасах и банковских счетах.  

На начальной странице вы можете запустить руководство по настройке, помогающее перенести бизнес-данные из файла Excel или из других форматов. Тип файлов, которые можно загружать, зависит от доступных расширений. Например, вы можете перенести данные из QuickBooks, поскольку [!INCLUDE[d365fin](includes/d365fin_md.md)] включает расширение, которое обрабатывает преобразование из QuickBooks. Если вам нужно перенести данные из других финансовых решений, вы должны проверить, есть ли расширение для этого решения, или импортировать из Excel.  

[!INCLUDE[d365fin](includes/d365fin_md.md)] включает шаблоны для счетов, клиентов, поставщиков и складских товаров, которые можно выбрать для применения при импорте данных.  

## <a name="importing-data-from-quickbooks-or-dynamics-gp"></a>Импорт данных из QuickBooks или Dynamics GP
Если ваша организация использует QuickBooks или Dynamics GP, вы можете экспортировать требуемую информацию в файл. Затем вы сможете открыть руководство по сопровождаемой настройке для переноса данных.
Например, если ваш файл включает информацию о клиентах и поставщиках, вы можете остановиться на переносе только данных о клиентах. Остальную информацию можно будет перенести позже.  

Сопровождаемая настройка позволяет изменить конфигурацию переноса по умолчанию, однако рекомендуется использовать эти расширенные возможности, только если вы знакомы с таблицами баз данных. Для большинства организацией сопоставление QuickBooks или Dynamics GP с [!INCLUDE[d365fin](includes/d365fin_md.md)] по умолчанию позволяет перенести все нужные данные.  

Дополнительные сведения см. в разделе [Миграция данных QuickBooks](ui-extensions-quickbooks-data-migration.md) или [Миграция данных Dynamics GP](ui-extensions-dynamicsgp-data-migration.md).

## <a name="importing-data-from-configuration-packages"></a>Импорт данных из пакетов конфигураций
[!INCLUDE[d365fin](includes/d365fin_md.md)] включает пакет конфигурации, который можно экспортировать в Excel, а затем настроить там данные. После этого можно импортировать данные обратно из Excel. Пакет состоит из 27 таблиц, включая основные данные, такие как клиенты, поставщики, товары и счета, другие таблицы настройки, такие как методы отгрузки, и таблицы транзакций, такие как заголовок и строки продаж.  

> [!NOTE]  
>   Работа с пакетами конфигураций — расширенная функция, и рекомендуется связаться с администратором. Дополнительные сведения см. в разделе [Импорт данных из устаревшего ПО учета с использованием пакета конфигурации](across-import-data-configuration-packages.md).  

## <a name="see-also"></a>См. также
[Финансы](finance.md)  
[Импорт данных из устаревшего ПО учета с использованием пакета конфигурации](across-import-data-configuration-packages.md)  
[Миграция данных QuickBooks](ui-extensions-quickbooks-data-migration.md)  
[Миграция данных Dynamics GP](ui-extensions-dynamicsgp-data-migration.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)   
[Установка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)

## [!INCLUDE[d365fin](includes/free_trial_md.md)]

