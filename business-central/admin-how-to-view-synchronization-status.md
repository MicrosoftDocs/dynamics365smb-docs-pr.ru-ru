---
title: Просмотр статуса синхронизации | Документы Майкрософт
description: Узнайте, как просмотреть статус индивидуального задания синхронизации.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: 11e29674c2d12031fdf4e7f66e767be4fcc74795
ms.sourcegitcommit: 04581558f6c5488c705a7ac392cf297be10b5f4f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2019
ms.locfileid: "1620888"
---
# <a name="view-the-status-of-a-synchronization"></a>Просмотр статуса синхронизации
Можно просмотреть статус отдельных заданий синхронизации, запущенных для интеграции [!INCLUDE[crm_md](includes/crm_md.md)]. Сюда входят задания синхронизации, запущенные из очереди заданий и заданий ручной синхронизации, выполненные для записей из [!INCLUDE[d365fin](includes/d365fin_md.md)]. Это может оказаться полезным при устранении проблем синхронизации, поскольку при этом предоставляется доступ к подробным данным о конкретных ошибках.

### <a name="to-view-synchronization-issues-for-coupled-records"></a>Просмотр проблем синхронизации для связанных записей
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Ошибки синхронизации связанных данных**, затем выберите связанную ссылку.
2. Страница **Ошибки синхронизации связанных данных** отображает проблемы, которые возникли при синхронизации связанных записей. Можно фильтровать и сортировать записи и выполнять действия, такие как **Восстановить** или **Удалить записи**, чтобы устранить проблемы одну за одной.

### <a name="to-view-synchronization-log-for-specific-manually-synchronized-record"></a>Просмотр журнала синхронизации для конкретной (синхронизированной вручную) записи
1. Откройте, например, запись клиента, товара или любую другую запись, которая синхронизирует данные между [!INCLUDE[d365fin](includes/d365fin_md.md)] и Sales.
2. Выберите действие **Журнал синхронизации** для просмотра журнала синхронизации для выбранной записи. Например, определенный клиент, которого вы синхронизировали вручную.

## <a name="see-also"></a>См. также  
[Настройка интеграции Dynamics 365 for Sales в Business Central](admin-setting-up-integration-with-dynamics-sales.md)  
[Использование Dynamics 365 for Sales из Business Central](marketing-integrate-dynamicscrm.md)
