---
title: Просмотр статуса заданий синхронизации | Документация Майкрософт
description: Узнайте, как просмотреть состояние после синхронизации связанных записей.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: a54ce7805deafa5d67c3e25b89606a1a40634ad6
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5378152"
---
# <a name="view-the-status-of-synchronization-jobs"></a><span data-ttu-id="da14d-103">Просмотр статуса заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="da14d-103">View the Status of Synchronization Jobs</span></span>
[!INCLUDE[prod_short](includes/cc_data_platform_banner.md)]

<span data-ttu-id="da14d-104">Используйте страницу **Ошибки синхронизации связанных данных** для просмотра состояния заданий синхронизации, которые были выполнены для связанных записей в интеграции Dataverse или [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="da14d-104">Use the **Coupled Data Synchronization Errors** page to view the status of synchronization jobs that have been run for coupled records in a Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)] integrations.</span></span> <span data-ttu-id="da14d-105">Сюда входят задания, запущенные из очереди заданий, и задания ручной синхронизации, выполненные для записей из [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="da14d-105">This includes jobs that were run from the job queue and manual synchronization jobs that ran on records from [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="da14d-106">Например, просмотр их статуса бывает полезен при устранении неполадок, поскольку он дает вам доступ к сведениям об ошибках, относящихся к связанным записям.</span><span class="sxs-lookup"><span data-stu-id="da14d-106">For example, viewing their status is helpful when troubleshooting because it gives you access to details about errors related to coupled records.</span></span> <span data-ttu-id="da14d-107">Как правило, эти ошибки вызваны действиями пользователя, например, когда:</span><span class="sxs-lookup"><span data-stu-id="da14d-107">Typically, these types of errors are caused by user actions, for example, when:</span></span>  

* <span data-ttu-id="da14d-108">Два человека внесли изменения в одни и те же данные в обоих бизнес-приложениях.</span><span class="sxs-lookup"><span data-stu-id="da14d-108">Two people made a change to the same data in both business apps.</span></span>
* <span data-ttu-id="da14d-109">Кто-то удалил данные в одном из приложений, но не в обоих.</span><span class="sxs-lookup"><span data-stu-id="da14d-109">Someone deleted data in one of the apps, but not both.</span></span>

> [!Note]
> <span data-ttu-id="da14d-110">На странице **Ошибки синхронизации связанных данных** отображается информация о заданиях, относящихся к связанным записям.</span><span class="sxs-lookup"><span data-stu-id="da14d-110">The **Coupled Data Synchronization Errors** page shows information about jobs related to coupled records.</span></span> <span data-ttu-id="da14d-111">Если вы устраните все ошибки, но записи по-прежнему не синхронизируются, это может быть связано с настройкой интеграции.</span><span class="sxs-lookup"><span data-stu-id="da14d-111">If you resolve all of the errors but records are still not synchronizing, it might have something to do with a setting for the integration.</span></span> <span data-ttu-id="da14d-112">Как правило, такие ошибки устраняет администратор.</span><span class="sxs-lookup"><span data-stu-id="da14d-112">Typically, your administrator will need to resolve those types of errors.</span></span>   

<!--

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098171]

-->

## <a name="to-view-and-resolve-synchronization-errors-for-coupled-records"></a><span data-ttu-id="da14d-113">Чтобы просмотреть и устранить ошибки синхронизации для связанных записей</span><span class="sxs-lookup"><span data-stu-id="da14d-113">To view and resolve synchronization errors for coupled records</span></span>
1. <span data-ttu-id="da14d-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Ошибки синхронизации связанных данных**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="da14d-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Coupled Data Synchronization Errors**, and then choose the related link.</span></span>
2. <span data-ttu-id="da14d-115">Страница **Ошибки синхронизации связанных данных** отображает проблемы, которые возникли при синхронизации связанных записей.</span><span class="sxs-lookup"><span data-stu-id="da14d-115">The **Coupled Data Synchronization Errors** page shows issues that occurred when you synchronized coupled records.</span></span> <span data-ttu-id="da14d-116">В следующей таблице приведены действия, которые вы можете использовать для последовательного решения проблем:</span><span class="sxs-lookup"><span data-stu-id="da14d-116">The following table includes actions that you can use to resolve issues one by one:</span></span>

|<span data-ttu-id="da14d-117">Действие</span><span class="sxs-lookup"><span data-stu-id="da14d-117">Action</span></span>|<span data-ttu-id="da14d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="da14d-118">Description</span></span>|
|----|----|
|<span data-ttu-id="da14d-119">**Удалить связь**</span><span class="sxs-lookup"><span data-stu-id="da14d-119">**Remove Coupling**</span></span>|<span data-ttu-id="da14d-120">Рассоединяет записи, и они больше не будут синхронизироваться.</span><span class="sxs-lookup"><span data-stu-id="da14d-120">Uncouples the records and they will no longer synchronize.</span></span> <span data-ttu-id="da14d-121">Чтобы возобновить синхронизацию, их нужно снова соединить.</span><span class="sxs-lookup"><span data-stu-id="da14d-121">To restart the synchronization you must couple them again.</span></span> |
|<span data-ttu-id="da14d-122">**Повторить** и **Повторить все**</span><span class="sxs-lookup"><span data-stu-id="da14d-122">**Retry** and **Retry All**</span></span>|<span data-ttu-id="da14d-123">Для каждой записи, где обнаружена ошибка, синхронизация пропускается, если вы не исправите проблему.</span><span class="sxs-lookup"><span data-stu-id="da14d-123">For each record where an error is found, synchronization is skipped unless you fix the issue.</span></span> <span data-ttu-id="da14d-124">"Повтор" включит выбранную запись в следующую синхронизацию, а **Повторить все** включает все записи.</span><span class="sxs-lookup"><span data-stu-id="da14d-124">Retry will include the selected record in the next synchronization, and **Retry All** includes all of the records.</span></span>|
|<span data-ttu-id="da14d-125">**Синхронизировать**</span><span class="sxs-lookup"><span data-stu-id="da14d-125">**Synchronize**</span></span>|<span data-ttu-id="da14d-126">Приложение попытается разрешить конфликт, если данные были изменены в обоих бизнес-приложениях.</span><span class="sxs-lookup"><span data-stu-id="da14d-126">The app will try to resolve a conflict where data was changed in both business apps.</span></span> <span data-ttu-id="da14d-127">Можно выбрать данные для использования.</span><span class="sxs-lookup"><span data-stu-id="da14d-127">You can choose the data to use.</span></span>|
|<span data-ttu-id="da14d-128">**Восстановить записи** и **Удалить записи**</span><span class="sxs-lookup"><span data-stu-id="da14d-128">**Restore Records** and **Delete Records**</span></span>|<span data-ttu-id="da14d-129">Это полезно, когда запись была удалена в одном из бизнес-приложений.</span><span class="sxs-lookup"><span data-stu-id="da14d-129">These are useful when a record was deleted in one of the business apps.</span></span> <span data-ttu-id="da14d-130">Операция "Удалить записи" удаляет запись или строку в приложении, где она еще существует.</span><span class="sxs-lookup"><span data-stu-id="da14d-130">Delete Records deletes the record or row in the app where it still exists.</span></span> <span data-ttu-id="da14d-131">Операция "Восстановить записи" воссоздает запись или строку в бизнес-приложении, где она была удалена.</span><span class="sxs-lookup"><span data-stu-id="da14d-131">Restore Records recreates the record or row in the business app where it was deleted.</span></span>|

> [!NOTE]
> <span data-ttu-id="da14d-132">Чтобы уменьшить количество конфликтов, которые необходимо разрешить, вы можете настроить сопоставления таблиц интеграции для автоматического применения этих действий.</span><span class="sxs-lookup"><span data-stu-id="da14d-132">To reduce the number of conflicts you need to resolve, you can set up your integration table mappings to apply these actions automatically.</span></span> <span data-ttu-id="da14d-133">Чтобы получить больше информации, см. [Сопоставление таблиц интеграции](admin-how-to-modify-table-mappings-for-synchronization.md#mapping-integration-tables).</span><span class="sxs-lookup"><span data-stu-id="da14d-133">For more information, [Mapping Integration Tables](admin-how-to-modify-table-mappings-for-synchronization.md#mapping-integration-tables).</span></span>

## <a name="to-view-the-synchronization-log-for-a-specific-manually-synchronized-record"></a><span data-ttu-id="da14d-134">Просмотр журнала синхронизации для конкретной (синхронизированной вручную) записи</span><span class="sxs-lookup"><span data-stu-id="da14d-134">To view the synchronization log for a specific (manually synchronized) record</span></span>
1. <span data-ttu-id="da14d-135">Откройте, например, запись клиента, товара или любую другую запись, которая синхронизирует данные между [!INCLUDE[prod_short](includes/prod_short.md)] и Dataverse или [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="da14d-135">Open, for example, a customer, item or any other record that is synchronizing data between [!INCLUDE[prod_short](includes/prod_short.md)] and Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)].</span></span>
2. <span data-ttu-id="da14d-136">Выберите действие **Журнал синхронизации** для просмотра журнала синхронизации для выбранной записи.</span><span class="sxs-lookup"><span data-stu-id="da14d-136">Choose the **Synchronization Log** action to view the synchronization log for a selected record.</span></span> <span data-ttu-id="da14d-137">Например, определенный клиент, которого вы синхронизировали вручную.</span><span class="sxs-lookup"><span data-stu-id="da14d-137">For example, a specific customer you synchronized manually.</span></span>

## <a name="see-also"></a><span data-ttu-id="da14d-138">См. также</span><span class="sxs-lookup"><span data-stu-id="da14d-138">See Also</span></span>  
[<span data-ttu-id="da14d-139">Настройка учетных записей пользователей для интеграции с Dynamics 365 Sales</span><span class="sxs-lookup"><span data-stu-id="da14d-139">Setting Up User Accounts for Integrating with Dynamics 365 Sales</span></span>](admin-setting-up-integration-with-dynamics-sales.md)  
[<span data-ttu-id="da14d-140">Использование Dynamics 365 Sales из Business Central</span><span class="sxs-lookup"><span data-stu-id="da14d-140">Using Dynamics 365 Sales from Business Central</span></span>](marketing-integrate-dynamicscrm.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]