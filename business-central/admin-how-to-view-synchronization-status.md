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
# <a name="view-the-status-of-a-synchronization"></a><span data-ttu-id="cdddb-103">Просмотр статуса синхронизации</span><span class="sxs-lookup"><span data-stu-id="cdddb-103">View the Status of a Synchronization</span></span>
<span data-ttu-id="cdddb-104">Можно просмотреть статус отдельных заданий синхронизации, запущенных для интеграции [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="cdddb-104">You can view the status of the individual synchronization jobs that have been run for [!INCLUDE[crm_md](includes/crm_md.md)] integration.</span></span> <span data-ttu-id="cdddb-105">Сюда входят задания синхронизации, запущенные из очереди заданий и заданий ручной синхронизации, выполненные для записей из [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="cdddb-105">This includes synchronization jobs that have been run from the job queue and manual synchronization jobs that were performed on records from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="cdddb-106">Это может оказаться полезным при устранении проблем синхронизации, поскольку при этом предоставляется доступ к подробным данным о конкретных ошибках.</span><span class="sxs-lookup"><span data-stu-id="cdddb-106">This is helpful when troubleshooting synchronization problems because it gives you access to details about specific errors.</span></span>

### <a name="to-view-all-synchronization-issues"></a><span data-ttu-id="cdddb-107">Чтобы просмотреть все проблемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="cdddb-107">To view all synchronization issues</span></span>
1. <span data-ttu-id="cdddb-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Ошибки синхронизации связанных данных**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="cdddb-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Coupled Data Synchronization Errors**, and then choose the related link.</span></span>
2. <span data-ttu-id="cdddb-109">На странице **Ошибки синхронизации связанных данных** можно просмотреть все проблемы, которые произошли в синхронизации данных между [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)], фильтровать и сортировать записи на странице по таблицам, сообщения об ошибках и выполнять действия, такие как **Повторить** или **Удалить связь**, чтобы разрешать проблемы по одной или пакетом.</span><span class="sxs-lookup"><span data-stu-id="cdddb-109">On the **Coupled Data Synchronization Errors** page you can view of all issues that occurred in synchronization of data between [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[d365fin](includes/d365fin_md.md)], filter and sort records in the page by table, error message and take actions such as **Retry** or **Remove Coupling** to resolve issues one by one or in bulk.</span></span>

### <a name="to-view-synchronization-log-for-specific-manually-synchronized-record"></a><span data-ttu-id="cdddb-110">Просмотр журнала синхронизации для конкретной (синхронизированной вручную) записи</span><span class="sxs-lookup"><span data-stu-id="cdddb-110">To view synchronization log for specific (manually synchronized) record</span></span>
1. <span data-ttu-id="cdddb-111">Откройте, например, запись клиента, товара или любую другую запись, которая синхронизирует данные между [!INCLUDE[d365fin](includes/d365fin_md.md)] и Sales</span><span class="sxs-lookup"><span data-stu-id="cdddb-111">Open, for example, customer, item or any other record that is synchronizing data between [!INCLUDE[d365fin](includes/d365fin_md.md)] and Sales</span></span>
2. <span data-ttu-id="cdddb-112">Выберите действие **Журнал синхронизации**, чтобы просмотреть журнал синхронизации для выбранной записи, например, определенного клиента, которого синхронизировали вручную</span><span class="sxs-lookup"><span data-stu-id="cdddb-112">Choose **Synchronization Log** action to view the synchronization log for selected record, for example, specific customer you synchronized manually</span></span>

## <a name="see-also"></a><span data-ttu-id="cdddb-113">См. также</span><span class="sxs-lookup"><span data-stu-id="cdddb-113">See Also</span></span>  
[<span data-ttu-id="cdddb-114">Настройка интеграции Dynamics 365 for Sales в Business Central</span><span class="sxs-lookup"><span data-stu-id="cdddb-114">Setting Up Dynamics 365 for Sales Integration in Business Central</span></span>](admin-setting-up-integration-with-dynamics-sales.md)  
[<span data-ttu-id="cdddb-115">Использование Dynamics 365 for Sales из Business Central</span><span class="sxs-lookup"><span data-stu-id="cdddb-115">Using Dynamics 365 for Sales from Business Central</span></span>](marketing-integrate-dynamicscrm.md)
