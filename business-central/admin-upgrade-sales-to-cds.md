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
# <a name="upgrading-an-integration-with-dynamics-365-sales"></a>Обновление интеграции с Dynamics 365 Sales
[!INCLUDE[d365fin](includes/d365fin_md.md)] интегрируется с [!INCLUDE[d365fin](includes/cds_long_md.md)], что позволяет легко подключать и синхронизировать данные с другими приложениями Dynamics 365, такими как [!INCLUDE[crm_md](includes/crm_md.md)], или даже с приложениями, которые вы создаете сами. Если вы впервые выполняете интеграцию, мы рекомендуем сделать это через [!INCLUDE[d365fin](includes/cds_long_md.md)]. Дополнительные сведения см. в разделе [Интеграция с Common Data Service](admin-common-data-service.md).

Если вы уже интегрировали [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)], вы можете продолжить синхронизацию данных, используя ваши настройки. Однако, если вы обновите [!INCLUDE[d365fin](includes/d365fin_md.md)] или выключите интеграцию [!INCLUDE[crm_md](includes/crm_md.md)], чтобы включить его снова, вы должны подключиться через [!INCLUDE[d365fin](includes/cds_long_md.md)]. 

> [!NOTE]
> При повторном подключении через [!INCLUDE[d365fin](includes/cds_long_md.md)] применяются настройки синхронизации по умолчанию и перезаписываются все ваши конфигурации. Например, будут применены сопоставления таблиц по умолчанию.

## <a name="to-upgrade-your-connection-to-use-common-data-service"></a>Обновление подключения для использования Common Data Service
1. Откройте страницу **Настройка подключения Microsoft Dynamics 365**, выберите переключатель **Включено**, чтобы отключить существующее подключение к [!INCLUDE[crm_md](includes/crm_md.md)].
2. Откройте страницу **Настройка подключения Common Data Service** и выберите переключатель **Включено**, чтобы включить подключение.
  
   После включения соединения CDS базовое решение интеграции Business Central CDS развертывается в Common Data Service.
3. Удалите решение интеграции Microsoft Dynamics 365 Business Central из Dynamics 365 Sales. Дополнительные сведения см. в разделе [Удаление темы решения](/powerapps/developer/common-data-service/uninstall-delete-solution). 

4. На странице **Настройка подключения Microsoft Dynamics 365** включите выключатель **Включено**, чтобы подключиться к [!INCLUDE[crm_md](includes/crm_md.md)].
  
   После включения подключения Sales решение интеграции Business Central развертывается в Sales. Это дает возможность интеграции с объектами, которые являются специфическими для [!INCLUDE[crm_md](includes/crm_md.md)], таким как заказы на продажу, предложения с расценками и счета.
5. На странице **Настройка подключения к Sales** выберите **Использовать настройку синхронизации по умолчанию**, чтобы инициализировать сопоставление таблиц интеграции для [!INCLUDE[crm_md](includes/crm_md.md)].

## <a name="see-also"></a>См. также
[Интеграция с Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  
[Интеграция с Common Data Service](admin-common-data-service.md)
