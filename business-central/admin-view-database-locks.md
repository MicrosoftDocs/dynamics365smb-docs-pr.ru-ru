---
title: Просмотр блокировок базы данных
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 04/01/2020
ms.author: jswymer
ms.openlocfilehash: abee0f31d66f648f4b0be567d8599b31c536a193
ms.sourcegitcommit: 7d54d8abe52e0546378cf760f5082f46e8441b90
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/30/2020
ms.locfileid: "3324106"
---
# <a name="viewing-database-locks"></a>Просмотр блокировок базы данных

## <a name="about-locks"></a>Общие сведения о блокировках

Блокировка базы данных контролирует доступ нескольких пользователей к одним и тем же данным одновременно. Чтобы защитить транзакцию от других транзакций, изменяющих те же данные, первая транзакция блокирует данные. Блокировка сохраняется до завершения транзакции.

Пользователи могут быть заблокированы от завершения транзакций с заблокированными данными. Как правило, они получают сообщение, которое указывает на состояние блокировки.

## <a name="to-view-database-locks"></a>Для просмотра блокировок базы данных

Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Блокировки базы данных**, затем выберите соответствующую ссылку.

Страница **Блокировки базы данных** дает снимок всех текущих блокировок базы данных.

Дополнительные сведения о блокировке базы данных см. в разделе [Мониторинг блокировок базы данных](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) в справке Business Central для разработчиков и ИТ-специалистов.

## <a name="see-also"></a>См. также

[Мониторинг блокировок базы данных](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) 
