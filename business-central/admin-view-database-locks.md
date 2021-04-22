---
title: Просмотр блокировок базы данных
description: Узнайте, как просмотреть информацию о любых блокировках базы данных прямо из клиентского интерфейса в Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: b53677ab57d6c48b015bb0dd47ea6e315f8e80c3
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776920"
---
# <a name="viewing-database-locks"></a>Просмотр блокировок базы данных

Блокировка базы данных контролирует доступ нескольких пользователей к одним и тем же данным одновременно. Чтобы защитить транзакцию от других транзакций, изменяющих те же данные, первая транзакция блокирует данные. Блокировка сохраняется до завершения транзакции.

Пользователи могут быть заблокированы от завершения транзакций с заблокированными данными. Как правило, они получают сообщение, которое указывает на состояние блокировки.

## <a name="to-view-database-locks"></a>Для просмотра блокировок базы данных

Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Блокировки базы данных**, затем выберите соответствующую ссылку.

Страница **Блокировки базы данных** дает снимок всех текущих блокировок базы данных.

Дополнительные сведения о блокировке базы данных см. в разделе [Мониторинг блокировок базы данных](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) в справке Business Central для разработчиков и ИТ-специалистов.

## <a name="see-also"></a>См. также

[Мониторинг блокировок базы данных](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) 


[!INCLUDE[footer-include](includes/footer-banner.md)]