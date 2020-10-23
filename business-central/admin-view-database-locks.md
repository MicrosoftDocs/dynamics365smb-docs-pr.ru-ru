---
title: Просмотр блокировок базы данных
description: Узнайте, как просмотреть информацию о любых блокировках базы данных прямо из клиентского интерфейса в Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: 6880ffa9a2ab42c1af7c22f9cace64697c9f905b
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3922321"
---
# <a name="viewing-database-locks"></a><span data-ttu-id="a2cb0-103">Просмотр блокировок базы данных</span><span class="sxs-lookup"><span data-stu-id="a2cb0-103">Viewing Database Locks</span></span>

<span data-ttu-id="a2cb0-104">Блокировка базы данных контролирует доступ нескольких пользователей к одним и тем же данным одновременно.</span><span class="sxs-lookup"><span data-stu-id="a2cb0-104">Database locking controls access by multiple users to the same data at the same time.</span></span> <span data-ttu-id="a2cb0-105">Чтобы защитить транзакцию от других транзакций, изменяющих те же данные, первая транзакция блокирует данные.</span><span class="sxs-lookup"><span data-stu-id="a2cb0-105">To protect a transaction against other transactions modifying the same data, the first transaction puts a lock on the data.</span></span> <span data-ttu-id="a2cb0-106">Блокировка сохраняется до завершения транзакции.</span><span class="sxs-lookup"><span data-stu-id="a2cb0-106">The lock remains until the transaction's done.</span></span>

<span data-ttu-id="a2cb0-107">Пользователи могут быть заблокированы от завершения транзакций с заблокированными данными.</span><span class="sxs-lookup"><span data-stu-id="a2cb0-107">Users may be blocked from completing transactions on the locked data.</span></span> <span data-ttu-id="a2cb0-108">Как правило, они получают сообщение, которое указывает на состояние блокировки.</span><span class="sxs-lookup"><span data-stu-id="a2cb0-108">They'll typically get a message that indicates the lock condition.</span></span>

## <a name="to-view-database-locks"></a><span data-ttu-id="a2cb0-109">Для просмотра блокировок базы данных</span><span class="sxs-lookup"><span data-stu-id="a2cb0-109">To view database locks</span></span>

<span data-ttu-id="a2cb0-110">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Блокировки базы данных**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="a2cb0-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Database Locks**, and then choose the related link.</span></span>

<span data-ttu-id="a2cb0-111">Страница **Блокировки базы данных** дает снимок всех текущих блокировок базы данных.</span><span class="sxs-lookup"><span data-stu-id="a2cb0-111">The **Database Locks** page gives snapshot of all current database locks.</span></span>

<span data-ttu-id="a2cb0-112">Дополнительные сведения о блокировке базы данных см. в разделе [Мониторинг блокировок базы данных](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) в справке Business Central для разработчиков и ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="a2cb0-112">For more information about database locking, see [Monitoring Database Locks](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) in the Business Central Developer and IT Pro help.</span></span>

## <a name="see-also"></a><span data-ttu-id="a2cb0-113">См. также</span><span class="sxs-lookup"><span data-stu-id="a2cb0-113">See Also</span></span>

[<span data-ttu-id="a2cb0-114">Мониторинг блокировок базы данных</span><span class="sxs-lookup"><span data-stu-id="a2cb0-114">Monitor Database Locks</span></span>](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) 
