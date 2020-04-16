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
ms.openlocfilehash: 1153ffc97d0f22c889ff23c5a27a8c0446b17018
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3196388"
---
# <a name="viewing-database-locks"></a>Просмотр блокировок базы данных

## <a name="about-locks"></a>Общие сведения о блокировках

Блокировка базы данных контролирует доступ нескольких пользователей к одним и тем же данным одновременно. Чтобы защитить транзакцию от других транзакций, изменяющих те же данные, первая транзакция блокирует данные. Блокировка сохраняется до завершения транзакции.

Пользователи могут быть заблокированы от завершения транзакций с заблокированными данными. Как правило, они получают сообщение, которое указывает на состояние блокировки.

## <a name="to-view-database-locks"></a>Для просмотра блокировок базы данных

Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Блокировки базы данных**, затем выберите соответствующую ссылку.

Страница **Блокировки базы данных** дает снимок всех текущих блокировок базы данных.

Дополнительные сведения о блокировке базы данных см. в разделе [Мониторинг блокировок базы данных](/dynamics365/business-central/a/dev-itpro/administration/monitor-database-locks) в справке Business Central для разработчиков и ИТ-специалистов.

## <a name="see-also"></a>См. также

[Мониторинг блокировок базы данных](/dynamics365/business-central/a/dev-itpro/administration/monitor-database-locks) 
