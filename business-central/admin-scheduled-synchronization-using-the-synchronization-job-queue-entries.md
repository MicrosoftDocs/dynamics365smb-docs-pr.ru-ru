---
title: Синхронизация Business Central и Dynamics 365 for Sales | Документы Майкрософт
description: Узнайте о синхронизации данных между Business Central и Dynamics 365 for Sales.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 07/16/2019
ms.author: bholtorf
ms.openlocfilehash: 9290730bb559d4ac03a437a49ed81b09f3c01853
ms.sourcegitcommit: 519623f9a5134c9ffa97eeaed0841ae59835f453
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "1755222"
---
# <a name="scheduling-a-synchronization-between-business-central-and-dynamics-365-for-sales"></a>Планирование синхронизации между Business Central и Dynamics 365 for Sales
Можно синхронизировать [!INCLUDE[d365fin](includes/d365fin_md.md)] с [!INCLUDE[crm_md](includes/crm_md.md)] для запланированных интервалов путем настройки заданий в очереди заданий. Задания синхронизации выполнят синхронизацию данных в записях [!INCLUDE[d365fin](includes/d365fin_md.md)] и записях [!INCLUDE[crm_md](includes/crm_md.md)], которые ранее были связаны. Или для записей, которые еще не связаны, в зависимости от направления синхронизации и правил, задания синхронизации могут создать и связать новые записи в целевой системе. Имеется несколько заданий синхронизации, которые доступны в готовом виде. Их можно просмотреть на странице **Операции очереди работ**. Дополнительные сведения см. в разделе [Использование очередей работ для планирования задач](admin-job-queues-schedule-tasks.md).
<!--
> [!Note]
> For the on-premeses version of [!INCLUDE[d365fin](includes/d365fin_md.md)], the synchronization jobs are run by codeunit **5339 Integration synch Job Runner**.--> 

## <a name="synchronization-process"></a>Процесс синхронизации  
Каждая операция очереди заданий синхронизации использует соответствующее сопоставление таблицы интеграции, задающее таблицу [!INCLUDE[d365fin](includes/d365fin_md.md)] и объект [!INCLUDE[crm_md](includes/crm_md.md)], которые должны быть синхронизированы. Сопоставления таблиц также включают ряд настроек, управляющих записями в таблице [!INCLUDE[d365fin](includes/d365fin_md.md)] и объекте [!INCLUDE[crm_md](includes/crm_md.md)], которые должны быть синхронизированы.  

Чтобы синхронизировать данные, записи объекта [!INCLUDE[crm_md](includes/crm_md.md)] должны быть связаны с записями [!INCLUDE[d365fin](includes/d365fin_md.md)]. Например, клиент [!INCLUDE[d365fin](includes/d365fin_md.md)] должен быть связан с организацией [!INCLUDE[crm_md](includes/crm_md.md)]. Связи можно настроить вручную перед выполнением заданий синхронизации или позволить заданиям синхронизации автоматически настроить связи. В следующем списке указан способ синхронизации данных между [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)] при использовании операций очереди заданий синхронизации. Дополнительные сведения см. в разделе [Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md). 

-   По умолчанию синхронизируются только записи в [!INCLUDE[d365fin](includes/d365fin_md.md)], связанные с записями в [!INCLUDE[crm_md](includes/crm_md.md)]. Сопоставление таблицы между операцией [!INCLUDE[crm_md](includes/crm_md.md)] и таблицей [!INCLUDE[d365fin](includes/d365fin_md.md)] можно изменить, чтобы задания синхронизации интеграции создавали новые записи в целевой базе данных для каждой записи в исходной базе, которая не связана. Новые записи также связываются с соответствующими записями в источнике. Например, при синхронизации клиентов с организациями [!INCLUDE[crm_md](includes/crm_md.md)] создается новая запись организации для каждого клиента в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Новые счета автоматически связываются с клиентами в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Поскольку синхронизация в этом случае является двунаправленной, новый клиент создается и связывается для каждой организации [!INCLUDE[crm_md](includes/crm_md.md)], которая еще не связана.  

    > [!NOTE]  
    > Имеются правила и фильтры, которые определяют, какие данные синхронизируются. Для получения дополнительной информации см. [Правила синхронизации](admin-synchronizing-business-central-and-sales.md#synchronization-rules).

-   Когда новые записи создаются в [!INCLUDE[d365fin](includes/d365fin_md.md)], записи используют шаблон, определенный для сопоставления таблиц интеграции, или шаблон по умолчанию, доступный для этого типа записей. Поля заполняются данными из [!INCLUDE[d365fin](includes/d365fin_md.md)] или [!INCLUDE[crm_md](includes/crm_md.md)] в зависимости от направления синхронизации. Дополнительные сведения см. в разделе [Практическое руководство. Изменение сопоставлений таблицы для синхронизации](admin-how-to-modify-table-mappings-for-synchronization.md).  

-   При последующих синхронизациях обновляются только те записи, которые были изменены или добавлены после последнего успешного задания синхронизации.  

     Новые записи в [!INCLUDE[crm_md](includes/crm_md.md)] добавляются в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Если данные в полях в записях [!INCLUDE[crm_md](includes/crm_md.md)] изменены, данные копируются в соответствующее поле в [!INCLUDE[d365fin](includes/d365fin_md.md)].  

-   При двунаправленной синхронизации задание выполняет синхронизацию из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)], а затем из [!INCLUDE[crm_md](includes/crm_md.md)] в [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="default-synchronization-job-queue-entries"></a>Операции очереди заданий синхронизации по умолчанию  
В следующей таблице описываются задания синхронизации по умолчанию.  

|Операция очереди работ|Описанием|Направление|Сопоставление таблиц интеграции|  
|---------------------|---------------------------------------|---------------|-------------------------------|  
|Задание синхронизации КОНТАКТ — Dynamics 365 for Sales|Синхронизирует контакты [!INCLUDE[crm_md](includes/crm_md.md)] с контактами [!INCLUDE[d365fin](includes/d365fin_md.md)].|Двунаправленная|КОНТАКТ|  
|Задание синхронизации ВАЛЮТА — Dynamics 365 for Sales|Синхронизирует валюты транзакций [!INCLUDE[crm_md](includes/crm_md.md)] с валютами [!INCLUDE[d365fin](includes/d365fin_md.md)].|Из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|ВАЛЮТА|  
|Задание синхронизации КЛИЕНТ — Dynamics 365 for Sales|Синхронизирует организации [!INCLUDE[crm_md](includes/crm_md.md)] с клиентами [!INCLUDE[d365fin](includes/d365fin_md.md)].|Двунаправленная|КЛИЕНТ|  
|Задание синхронизации CUSTPRCGRP-PRICE — Dynamics 365 for Sales|Синхронизирует прайс-листы продаж [!INCLUDE[crm_md](includes/crm_md.md)] с ценовыми группами клиентов [!INCLUDE[d365fin](includes/d365fin_md.md)].| |ЦЕНОВЫЕ ГРУППЫ КЛИЕНТОВ — ПРАЙС-ЛИСТЫ ПРОДАЖ|
|Задание синхронизации ТОВАР - ПРОДУКТ — Dynamics 365 for Sales|Синхронизирует продукты [!INCLUDE[crm_md](includes/crm_md.md)] с товарами [!INCLUDE[d365fin](includes/d365fin_md.md)].|Из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|ТОВАР-ПРОДУКТ|
|Задание синхронизации POSTEDSALESINV-INV — Dynamics 365 for Sales|Синхронизирует счета [!INCLUDE[crm_md](includes/crm_md.md)] с учтенными счетами продаж [!INCLUDE[d365fin](includes/d365fin_md.md)].|Из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|СЧЕТА — УЧТЕННЫЕ СЧЕТА ПРОДАЖ|
|Задание синхронизации "РЕСУРС-ПРОДУКТ — Dynamics 365 for Sales"|Синхронизирует продукты [!INCLUDE[crm_md](includes/crm_md.md)] с ресурсами [!INCLUDE[d365fin](includes/d365fin_md.md)].|Из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|РЕСУРС-ПРОДУКТ|  
|Задание синхронизации "ПРОДАВЦЫ — Dynamics 365 for Sales"|Синхронизирует продавцов [!INCLUDE[d365fin](includes/d365fin_md.md)] с пользователями [!INCLUDE[crm_md](includes/crm_md.md)].|Из [!INCLUDE[crm_md](includes/crm_md.md)] в [!INCLUDE[d365fin](includes/d365fin_md.md)]|ПРОДАВЦЫ|
|Задание синхронизации SALESPRC-PRODUCTPRICE — Dynamics 365 for Sales|Синхронизирует цены продуктов [!INCLUDE[crm_md](includes/crm_md.md)] с ценами продажи [!INCLUDE[d365fin](includes/d365fin_md.md)].||ЦЕНА ПРОДУКТА — ЦЕНА ПРОДАЖ|
|Задание синхронизации "ЕДИНИЦА ИЗМЕРЕНИЯ — Dynamics 365 for Sales"|Синхронизирует группы единиц [!INCLUDE[crm_md](includes/crm_md.md)] с единицами измерения [!INCLUDE[d365fin](includes/d365fin_md.md)].|Из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|ЕДИНИЦА ИЗМЕРЕНИЯ|  
|Синхронизация статистики по клиенту — Dynamics 365 for Sales|Обновление организаций [!INCLUDE[crm_md](includes/crm_md.md)] с новейшими данными клиентов [!INCLUDE[d365fin](includes/d365fin_md.md)]. В [!INCLUDE[crm_md](includes/crm_md.md)] данная информация отображается в форме быстрого просмотра **Статистика организации Business Central** организаций, которые связаны с клиентами [!INCLUDE[d365fin](includes/d365fin_md.md)].<br /><br /> Эти данные можно также обновлять вручную из каждой записи клиента. Дополнительные сведения см. в разделе [Практическое руководство. Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md). </BR></BR>**Примечание.** Эта запись очереди заданий используется только в случае установки решения интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [О решении интеграции Business Central](admin-prepare-dynamics-365-for-sales-for-integration.md#about-the-business-central-integration-solution).|Неприменимо.|Неприменимо.|   

## <a name="to-view-the-synchronization-job-log"></a>Просмотр журнала заданий синхронизации  
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал синхронизации интеграции**, затем выберите связанную ссылку.
2.  Если при выполнении задания синхронизации произошла одна или несколько ошибок, количество ошибок отображается в столбце **Ошибки**. Для просмотра ошибок по заданию выберите номер.  

    > [!TIP]  
    > Можно просмотреть все ошибки задания синхронизации, открыв журнал ошибок задания синхронизации вручную.

## <a name="to-view-the-synchronization-job-log-from-the-table-mappings"></a>Просмотр журнала заданий синхронизации из сопоставлений таблиц  
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сопоставления таблиц интеграции**, затем выберите связанную ссылку.
2.  На странице **Сопоставления таблиц интеграции** выберите запись, затем выберите **Журнал заданий синхронизации интеграции**.  

## <a name="to-view-the-synchronization-error-log"></a>Просмотр журнала ошибок синхронизации  
* Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Ошибки синхронизации интеграции**, затем выберите связанную ссылку.

## <a name="see-also"></a>См. также  
[Синхронизация данных в Business Central и Dynamics 365 for Sales](admin-synchronizing-business-central-and-sales.md)  
[Ручная синхронизация сопоставлений таблиц](admin-manual-synchronization-of-table-mappings.md)  
[Планирование синхронизации между Business Central и Dynamics 365 for Sales](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)  
[Об интеграции Dynamics 365 Business Central с Dynamics 365 for Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  



