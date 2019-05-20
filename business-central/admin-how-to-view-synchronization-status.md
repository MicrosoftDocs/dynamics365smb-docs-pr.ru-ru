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
ms.openlocfilehash: d55d8d5ab916cee6600deaf891702a625d76d7ee
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1245689"
---
# <a name="view-the-status-of-a-synchronization"></a>Просмотр статуса синхронизации
Можно просмотреть статус отдельных заданий синхронизации, запущенных для интеграции [!INCLUDE[crm_md](includes/crm_md.md)]. Сюда входят задания синхронизации, запущенные из очереди заданий и заданий ручной синхронизации, выполненные для записей из [!INCLUDE[d365fin](includes/d365fin_md.md)]. Это может оказаться полезным при устранении проблем синхронизации, поскольку при этом предоставляется доступ к подробным данным о конкретных ошибках.

### <a name="to-view-all-synchronization-issues"></a>Чтобы просмотреть все проблемы синхронизации
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Ошибки синхронизации связанных данных**, затем выберите связанную ссылку.
2. На странице **Ошибки синхронизации связанных данных** можно просмотреть все проблемы, которые произошли в синхронизации данных между [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)], фильтровать и сортировать записи на странице по таблицам, сообщения об ошибках и выполнять действия, такие как **Повторить** или **Удалить связь**, чтобы разрешать проблемы по одной или пакетом.

### <a name="to-view-synchronization-log-for-specific-manually-synchronized-record"></a>Просмотр журнала синхронизации для конкретной (синхронизированной вручную) записи
1. Откройте, например, запись клиента, товара или любую другую запись, которая синхронизирует данные между [!INCLUDE[d365fin](includes/d365fin_md.md)] и Sales
2. Выберите действие **Журнал синхронизации**, чтобы просмотреть журнал синхронизации для выбранной записи, например, определенного клиента, которого синхронизировали вручную

## <a name="see-also"></a>См. также  
[Настройка интеграции Dynamics 365 for Sales в Business Central](admin-setting-up-integration-with-dynamics-sales.md)  
[Использование Dynamics 365 for Sales из Business Central](marketing-integrate-dynamicscrm.md)
