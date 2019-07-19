---
title: Устранение ошибок синхронизации | Microsoft Docs
description: Предоставляет некоторые рекомендации по выявлению и устранению ошибок синхронизации.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/11/2019
ms.author: bholtorf
ms.openlocfilehash: bb6d0837f91240eb31abc7c02895cf2da420bf7d
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1726794"
---
# <a name="troubleshooting-synchronization-errors"></a><span data-ttu-id="efcbe-103">Устранение ошибок синхронизации</span><span class="sxs-lookup"><span data-stu-id="efcbe-103">Troubleshooting Synchronization Errors</span></span>
<span data-ttu-id="efcbe-104">Интеграция [!INCLUDE[d365fin](includes/d365fin_md.md)] с [!INCLUDE[crm_md](includes/crm_md.md)] — сложный процесс, и иногда что-то идет не так.</span><span class="sxs-lookup"><span data-stu-id="efcbe-104">There are lots of moving parts involved in integrating [!INCLUDE[d365fin](includes/d365fin_md.md)] with [!INCLUDE[crm_md](includes/crm_md.md)], and sometimes things go wrong.</span></span> <span data-ttu-id="efcbe-105">В этом разделе рассказывается о некоторых типичных ошибках, которые могут возникнуть, и даются советы о том, как их исправить.</span><span class="sxs-lookup"><span data-stu-id="efcbe-105">This topic points out some of the typical errors that occur and gives some pointers for how to fix them.</span></span>

<span data-ttu-id="efcbe-106">Ошибки часто возникают либо из-за того, что пользователь что-то сделал со связанными записями, либо из-за неправильной настройки интеграции.</span><span class="sxs-lookup"><span data-stu-id="efcbe-106">Errors often occur either because of something that a user has done to coupled records or something is wrong with how the integration is set up.</span></span> <span data-ttu-id="efcbe-107">Ошибки, относящиеся к связанным записям, пользователи могут устранить самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="efcbe-107">For errors related to coupled records, users can resolve those themselves.</span></span> <span data-ttu-id="efcbe-108">Эти ошибки вызваны такими действиями, как удаление записи в одном, но не в обоих бизнес-приложениях, с последующей синхронизацией.</span><span class="sxs-lookup"><span data-stu-id="efcbe-108">These errors are caused by actions such as deleting a record in one, but not both, business apps and then synchronizing.</span></span> <span data-ttu-id="efcbe-109">Для получения дополнительной информации см. раздел [Просмотр статуса синхронизации](admin-how-to-view-synchronization-status.md).</span><span class="sxs-lookup"><span data-stu-id="efcbe-109">For more information, see [View the Status of a Synchronization](admin-how-to-view-synchronization-status.md).</span></span>

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2097304]

<span data-ttu-id="efcbe-110">Ошибки, связанные с настройкой интеграции, обычно требуют участия администратора.</span><span class="sxs-lookup"><span data-stu-id="efcbe-110">Errors that are related to how the integration is set up typically require an administrator's attention.</span></span> <span data-ttu-id="efcbe-111">Вы можете просмотреть эти ошибки на странице **Ошибки синхронизации интеграции**.</span><span class="sxs-lookup"><span data-stu-id="efcbe-111">You can view these errors on the **Integration Synchronization Errors** page.</span></span> <span data-ttu-id="efcbe-112">Примеры некоторых типичных проблем:</span><span class="sxs-lookup"><span data-stu-id="efcbe-112">Examples of some typical issues include:</span></span>  
  
* <span data-ttu-id="efcbe-113">Права и роли, назначенные пользователям, неверны.</span><span class="sxs-lookup"><span data-stu-id="efcbe-113">The permissions and roles assigned to users are not correct.</span></span>  
* <span data-ttu-id="efcbe-114">Учетная запись администратора была указана в качестве пользователя интеграции.</span><span class="sxs-lookup"><span data-stu-id="efcbe-114">The administrator account was specified as the integration user.</span></span>  
* <span data-ttu-id="efcbe-115">Пароль пользователя интеграции настроен так, чтобы требовать смены при входе пользователя в систему.</span><span class="sxs-lookup"><span data-stu-id="efcbe-115">The integration user’s password is set to require a change when the user signs in.</span></span>  
* <span data-ttu-id="efcbe-116">Курсы обмена валют не указаны ни в одном, ни в другом приложении.</span><span class="sxs-lookup"><span data-stu-id="efcbe-116">The exchange rates for currencies are not specified in one or the other app.</span></span>  
  
<span data-ttu-id="efcbe-117">Вы должны вручную устранить эти ошибки, но эта страница также может оказаться полезной.</span><span class="sxs-lookup"><span data-stu-id="efcbe-117">You must manually resolve the errors, but there are a few ways in which the page helps you.</span></span> <span data-ttu-id="efcbe-118">Например:</span><span class="sxs-lookup"><span data-stu-id="efcbe-118">For example:</span></span>  

* <span data-ttu-id="efcbe-119">Поля **Источник** и **Назначение** могут содержать ссылки на запись, в которой была обнаружена ошибка.</span><span class="sxs-lookup"><span data-stu-id="efcbe-119">The **Source** and **Destination** fields may contain links to the record where the error was found.</span></span> <span data-ttu-id="efcbe-120">Нажмите на ссылку, чтобы открыть запись и изучить проблему.</span><span class="sxs-lookup"><span data-stu-id="efcbe-120">Click the link to open the record and investigate the error.</span></span>  
* <span data-ttu-id="efcbe-121">Действия **Удалить записи старше 7 дней** и **Удалить все записи** помогут очистить список.</span><span class="sxs-lookup"><span data-stu-id="efcbe-121">The **Delete Entries Older than 7 Days** and the **Delete All Entries** actions will clean up the list.</span></span> <span data-ttu-id="efcbe-122">Как правило, эти действия используются после устранения причины ошибки, которая влияет на многие записи.</span><span class="sxs-lookup"><span data-stu-id="efcbe-122">Typically, you use these actions after you have resolved the cause of an error that affects many records.</span></span> <span data-ttu-id="efcbe-123">При этом следует соблюдать осторожность.</span><span class="sxs-lookup"><span data-stu-id="efcbe-123">Use caution, however.</span></span> <span data-ttu-id="efcbe-124">Эти действия могут удалить ошибки, которые все еще актуальны.</span><span class="sxs-lookup"><span data-stu-id="efcbe-124">These actions might delete errors that are still relevant.</span></span>

## <a name="see-also"></a><span data-ttu-id="efcbe-125">См. также</span><span class="sxs-lookup"><span data-stu-id="efcbe-125">See Also</span></span>
<span data-ttu-id="efcbe-126">[Интеграция с [!INCLUDE[crm_md](includes/crm_md.md)]](admin-prepare-dynamics-365-for-sales-for-integration.md)</span><span class="sxs-lookup"><span data-stu-id="efcbe-126">[Integrating with [!INCLUDE[crm_md](includes/crm_md.md)]](admin-prepare-dynamics-365-for-sales-for-integration.md)</span></span>  
<span data-ttu-id="efcbe-127">[Настройка учетных записей пользователя для интеграции с [!INCLUDE[crm_md](includes/crm_md.md)]](admin-setting-up-integration-with-dynamics-sales.md)</span><span class="sxs-lookup"><span data-stu-id="efcbe-127">[Setting Up User Accounts for Integrating with [!INCLUDE[crm_md](includes/crm_md.md)]](admin-setting-up-integration-with-dynamics-sales.md)</span></span>  
<span data-ttu-id="efcbe-128">[Настройка подключения к [!INCLUDE[crm_md](includes/crm_md.md)]](admin-how-to-set-up-a-dynamics-crm-connection.md)</span><span class="sxs-lookup"><span data-stu-id="efcbe-128">[Set Up a Connection to [!INCLUDE[crm_md](includes/crm_md.md)]](admin-how-to-set-up-a-dynamics-crm-connection.md)</span></span>  
[<span data-ttu-id="efcbe-129">Связывание и синхронизация записей вручную</span><span class="sxs-lookup"><span data-stu-id="efcbe-129">Couple and Synchronize Records Manually</span></span>](admin-how-to-couple-and-synchronize-records-manually.md)  
[<span data-ttu-id="efcbe-130">Просмотр статуса синхронизации</span><span class="sxs-lookup"><span data-stu-id="efcbe-130">View the Status of a Synchronization</span></span>](admin-how-to-view-synchronization-status.md)  