---
title: Обновление интеграции с Dynamics 365 Sales
description: Узнайте, как переместить интеграцию Dynamics 365 Business Central с Dynamics 365 Sales в последнюю версию.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, integrating
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 3bb6b26e011afc515fbd4f492f56b3090c56e860
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3922371"
---
# <a name="upgrading-an-integration-with-dynamics-365-sales"></a><span data-ttu-id="2a080-103">Обновление интеграции с Dynamics 365 Sales</span><span class="sxs-lookup"><span data-stu-id="2a080-103">Upgrading an Integration with Dynamics 365 Sales</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="2a080-104">интегрируется с [!INCLUDE[d365fin](includes/cds_long_md.md)], что позволяет легко подключать и синхронизировать данные с другими приложениями Dynamics 365, такими как [!INCLUDE[crm_md](includes/crm_md.md)], или даже с приложениями, которые вы создаете сами.</span><span class="sxs-lookup"><span data-stu-id="2a080-104">integrates with [!INCLUDE[d365fin](includes/cds_long_md.md)], which makes it easy to connect and synchronize data with other Dynamics 365 applications, such as [!INCLUDE[crm_md](includes/crm_md.md)], or even apps that you build yourself.</span></span> <span data-ttu-id="2a080-105">Если вы впервые выполняете интеграцию, мы рекомендуем сделать это через [!INCLUDE[d365fin](includes/cds_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="2a080-105">If you are integrating for the first time, we recommend that you do so through [!INCLUDE[d365fin](includes/cds_long_md.md)].</span></span> <span data-ttu-id="2a080-106">Дополнительные сведения см. в разделе [Интеграция с Common Data Service](admin-common-data-service.md).</span><span class="sxs-lookup"><span data-stu-id="2a080-106">For more information, see [Integration with Common Data Service](admin-common-data-service.md).</span></span>

<span data-ttu-id="2a080-107">Если вы уже интегрировали [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)], вы можете продолжить синхронизацию данных, используя ваши настройки.</span><span class="sxs-lookup"><span data-stu-id="2a080-107">If you have already integrated [!INCLUDE[crm_md](includes/crm_md.md)] with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can continue to synchronize data using your setup.</span></span> <span data-ttu-id="2a080-108">Однако, если вы обновите [!INCLUDE[d365fin](includes/d365fin_md.md)] или выключите интеграцию [!INCLUDE[crm_md](includes/crm_md.md)], чтобы включить его снова, вы должны подключиться через [!INCLUDE[d365fin](includes/cds_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="2a080-108">However, if you upgrade [!INCLUDE[d365fin](includes/d365fin_md.md)], or turn off your [!INCLUDE[crm_md](includes/crm_md.md)] integration, to turn it on again you must connect through [!INCLUDE[d365fin](includes/cds_long_md.md)].</span></span> 

> [!NOTE]
> <span data-ttu-id="2a080-109">При повторном подключении через [!INCLUDE[d365fin](includes/cds_long_md.md)] применяются настройки синхронизации по умолчанию и перезаписываются все ваши конфигурации.</span><span class="sxs-lookup"><span data-stu-id="2a080-109">Reconnecting through [!INCLUDE[d365fin](includes/cds_long_md.md)] will apply default synchronization settings, and will overwrite any configurations you have.</span></span> <span data-ttu-id="2a080-110">Например, будут применены сопоставления таблиц по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2a080-110">For example, the default table mappings will be applied.</span></span>

## <a name="to-upgrade-your-connection-to-use-common-data-service"></a><span data-ttu-id="2a080-111">Обновление подключения для использования Common Data Service</span><span class="sxs-lookup"><span data-stu-id="2a080-111">To upgrade your connection to use Common Data Service</span></span>
1. <span data-ttu-id="2a080-112">Откройте страницу **Настройка подключения Microsoft Dynamics 365**, выберите переключатель **Включено**, чтобы отключить существующее подключение к [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="2a080-112">Open the **Microsoft Dynamics 365 Connection Setup** page, choose the **Enable** toggle to turn off your existing connection to [!INCLUDE[crm_md](includes/crm_md.md)].</span></span>
2. <span data-ttu-id="2a080-113">Откройте страницу **Настройка подключения Common Data Service** и выберите переключатель **Включено**, чтобы включить подключение.</span><span class="sxs-lookup"><span data-stu-id="2a080-113">Open the **Common Data Service Connection Setup** page, and choose the **Enable** toggle to turn on the connection.</span></span>
  
   <span data-ttu-id="2a080-114">После включения соединения CDS базовое решение интеграции Business Central CDS развертывается в Common Data Service.</span><span class="sxs-lookup"><span data-stu-id="2a080-114">After you enable the CDS connection, the Business Central CDS Base Integration Solution is deployed to Common Data Service.</span></span>
3. <span data-ttu-id="2a080-115">Удалите решение интеграции Microsoft Dynamics 365 Business Central из Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="2a080-115">Uninstall the Microsoft Dynamics 365 Business Central Integration solution from your Dynamics 365 Sales.</span></span> <span data-ttu-id="2a080-116">Дополнительные сведения см. в разделе [Удаление темы решения](/powerapps/developer/common-data-service/uninstall-delete-solution).</span><span class="sxs-lookup"><span data-stu-id="2a080-116">For more information, see [Uninstall or delete a solution topic](/powerapps/developer/common-data-service/uninstall-delete-solution).</span></span> 

4. <span data-ttu-id="2a080-117">На странице **Настройка подключения Microsoft Dynamics 365** включите выключатель **Включено**, чтобы подключиться к [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="2a080-117">On the **Microsoft Dynamics 365 Connection Setup** page, turn on the **Enable** toggle to connect to [!INCLUDE[crm_md](includes/crm_md.md)].</span></span>
  
   <span data-ttu-id="2a080-118">После включения подключения Sales решение интеграции Business Central развертывается в Sales.</span><span class="sxs-lookup"><span data-stu-id="2a080-118">After you enable the Sales connection, the Business Central Integration Solution is deployed to Sales.</span></span> <span data-ttu-id="2a080-119">Это дает возможность интеграции с объектами, которые являются специфическими для [!INCLUDE[crm_md](includes/crm_md.md)], таким как заказы на продажу, предложения с расценками и счета.</span><span class="sxs-lookup"><span data-stu-id="2a080-119">This enables integration with entities that are specific to [!INCLUDE[crm_md](includes/crm_md.md)], such as sales orders, quotes, and invoices.</span></span>
5. <span data-ttu-id="2a080-120">На странице **Настройка подключения к Sales** выберите **Использовать настройку синхронизации по умолчанию**, чтобы инициализировать сопоставление таблиц интеграции для [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="2a080-120">On the **Sales Connection Setup** page, choose **Use Default Synchronization Setup** to initialize the integration table mappings for [!INCLUDE[crm_md](includes/crm_md.md)].</span></span>

## <a name="see-also"></a><span data-ttu-id="2a080-121">См. также</span><span class="sxs-lookup"><span data-stu-id="2a080-121">See Also</span></span>
[<span data-ttu-id="2a080-122">Интеграция с Dynamics 365 Sales</span><span class="sxs-lookup"><span data-stu-id="2a080-122">Integrating with Dynamics 365 Sales</span></span>](admin-prepare-dynamics-365-for-sales-for-integration.md)  
[<span data-ttu-id="2a080-123">Интеграция с Common Data Service</span><span class="sxs-lookup"><span data-stu-id="2a080-123">Integrating with Common Data Service</span></span>](admin-common-data-service.md)
