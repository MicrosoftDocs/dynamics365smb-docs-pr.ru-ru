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
ms.openlocfilehash: 6528a05d0d2b43d39f0f2fafa26d71b03d0d2511
ms.sourcegitcommit: 311e86d6abb9b59a5483324d8bb4cd1be7949248
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "5013721"
---
# <a name="upgrading-an-integration-with-dynamics-365-sales"></a><span data-ttu-id="5c4fc-103">Обновление интеграции с Dynamics 365 Sales</span><span class="sxs-lookup"><span data-stu-id="5c4fc-103">Upgrading an Integration with Dynamics 365 Sales</span></span>
[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="5c4fc-104">интегрируется с [!INCLUDE[prod_short](includes/cds_long_md.md)], что позволяет легко подключать и синхронизировать данные с другими приложениями Dynamics 365, такими как [!INCLUDE[crm_md](includes/crm_md.md)], или даже с приложениями, которые вы создаете сами.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-104">integrates with [!INCLUDE[prod_short](includes/cds_long_md.md)], which makes it easy to connect and synchronize data with other Dynamics 365 applications, such as [!INCLUDE[crm_md](includes/crm_md.md)], or even apps that you build yourself.</span></span> <span data-ttu-id="5c4fc-105">Если вы впервые выполняете интеграцию, мы рекомендуем сделать это через [!INCLUDE[prod_short](includes/cds_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5c4fc-105">If you are integrating for the first time, we recommend that you do so through [!INCLUDE[prod_short](includes/cds_long_md.md)].</span></span> <span data-ttu-id="5c4fc-106">Дополнительные сведения см. в разделе [Интеграция с Dataverse](admin-common-data-service.md).</span><span class="sxs-lookup"><span data-stu-id="5c4fc-106">For more information, see [Integration with Dataverse](admin-common-data-service.md).</span></span>

<span data-ttu-id="5c4fc-107">Если вы уже интегрировали [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[prod_short](includes/prod_short.md)], вы можете продолжить синхронизацию данных, используя ваши настройки.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-107">If you have already integrated [!INCLUDE[crm_md](includes/crm_md.md)] with [!INCLUDE[prod_short](includes/prod_short.md)], you can continue to synchronize data using your setup.</span></span> <span data-ttu-id="5c4fc-108">Однако, если вы обновите [!INCLUDE[prod_short](includes/prod_short.md)] или выключите интеграцию [!INCLUDE[crm_md](includes/crm_md.md)], чтобы включить его снова, вы должны подключиться через [!INCLUDE[prod_short](includes/cds_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5c4fc-108">However, if you upgrade [!INCLUDE[prod_short](includes/prod_short.md)], or turn off your [!INCLUDE[crm_md](includes/crm_md.md)] integration, to turn it on again you must connect through [!INCLUDE[prod_short](includes/cds_long_md.md)].</span></span> 

> [!NOTE]
> <span data-ttu-id="5c4fc-109">При повторном подключении через [!INCLUDE[prod_short](includes/cds_long_md.md)] применяются настройки синхронизации по умолчанию и перезаписываются все ваши конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-109">Reconnecting through [!INCLUDE[prod_short](includes/cds_long_md.md)] will apply default synchronization settings, and will overwrite any configurations you have.</span></span> <span data-ttu-id="5c4fc-110">Например, будут применены сопоставления таблиц по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-110">For example, the default table mappings will be applied.</span></span>

## <a name="to-upgrade-your-connection-to-use-dataverse"></a><span data-ttu-id="5c4fc-111">Обновление подключения для использования Dataverse</span><span class="sxs-lookup"><span data-stu-id="5c4fc-111">To upgrade your connection to use Dataverse</span></span>
1. <span data-ttu-id="5c4fc-112">Откройте страницу **Настройка подключения Microsoft Dynamics 365**, затем выключите выключатель **Включено**, чтобы отключиться от [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5c4fc-112">Open the **Microsoft Dynamics 365 Connection Setup** page, and then turn off the **Enabled** toggle to disconnect from [!INCLUDE[crm_md](includes/crm_md.md)].</span></span>
2. <span data-ttu-id="5c4fc-113">Откройте страницу **Настройка подключения Dataverse** и выберите переключатель **Включено**, чтобы включить подключение к [!INCLUDE[prod_short](includes/cds_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5c4fc-113">Open the **Dataverse Connection Setup** page, and choose the **Enabled** toggle to turn on the connection to [!INCLUDE[prod_short](includes/cds_long_md.md)].</span></span>
  
   <span data-ttu-id="5c4fc-114">После включения соединения решение интеграции Business Central развертывается в Dataverse.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-114">After you enable the connection, the Business Central Integration Solution is deployed to Dataverse.</span></span>
3. <span data-ttu-id="5c4fc-115">Выберите **Повторить развертывание решения интеграции**, чтобы заново установить решение интеграции Business Central.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-115">Choose **Redeploy Integration Solution** to reinstall the Business Central Integration Solution.</span></span>
4. <span data-ttu-id="5c4fc-116">На странице **Настройка подключения Microsoft Dynamics 365** включите выключатель **Включено**, чтобы снова подключиться к [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5c4fc-116">On the **Microsoft Dynamics 365 Connection Setup** page, turn on the **Enabled** toggle to reconnect to [!INCLUDE[crm_md](includes/crm_md.md)].</span></span>
  
   <span data-ttu-id="5c4fc-117">Это дает возможность интеграции с таблицами, которые являются специфическими для [!INCLUDE[crm_md](includes/crm_md.md)], таким как заказы на продажу, предложения с расценками и счета.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-117">This enables integration with tables that are specific to [!INCLUDE[crm_md](includes/crm_md.md)], such as sales orders, quotes, and invoices.</span></span>
5. <span data-ttu-id="5c4fc-118">На странице **Настройка подключения к Sales** выберите **Использовать настройку синхронизации по умолчанию**, чтобы инициализировать сопоставление таблиц интеграции для [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5c4fc-118">On the **Sales Connection Setup** page, choose **Use Default Synchronization Setup** to initialize the integration table mappings for [!INCLUDE[crm_md](includes/crm_md.md)].</span></span>

## <a name="see-also"></a><span data-ttu-id="5c4fc-119">См. также</span><span class="sxs-lookup"><span data-stu-id="5c4fc-119">See Also</span></span>
[<span data-ttu-id="5c4fc-120">Интеграция с Dynamics 365 Sales</span><span class="sxs-lookup"><span data-stu-id="5c4fc-120">Integrating with Dynamics 365 Sales</span></span>](admin-prepare-dynamics-365-for-sales-for-integration.md)  
[<span data-ttu-id="5c4fc-121">Интеграция с Microsoft Dataverse</span><span class="sxs-lookup"><span data-stu-id="5c4fc-121">Integrating with Microsoft Dataverse</span></span>](admin-common-data-service.md)
