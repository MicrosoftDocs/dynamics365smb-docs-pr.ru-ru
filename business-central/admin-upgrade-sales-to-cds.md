---
title: Обновление интеграции с Dynamics 365 Sales | Документация Майкрософт
description: Узнайте, как подготовить Dynamics 365 Business Central к интеграции с Dynamics 365 Sales.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, integrating
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: 95098397bd9554be6c993b6107963eba9a99c067
ms.sourcegitcommit: d67328e1992c9a754b14c7267ab11312c80c38dd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3196886"
---
# <a name="upgrading-an-integration-with-dynamics-365-sales"></a>Обновление интеграции с Dynamics 365 Sales
[!INCLUDE[d365fin](includes/d365fin_md.md)] также интегрируется с [!INCLUDE[d365fin](includes/cds_long_md.md)], что позволяет легко подключать и синхронизировать данные с другими приложениями Dynamics 365, такими как [!INCLUDE[crm_md](includes/crm_md.md)], или даже с приложениями, которые вы создаете сами. Если вы впервые выполняете интеграцию, мы рекомендуем сделать это через [!INCLUDE[d365fin](includes/cds_long_md.md)]. Дополнительные сведения см. в разделе [Интеграция с Common Data Service](admin-common-data-service.md).

Если вы уже интегрировали [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)], вы можете продолжить синхронизацию данных, используя ваши настройки. Однако, если вы обновите [!INCLUDE[d365fin](includes/d365fin_md.md)] или выключите интеграцию [!INCLUDE[crm_md](includes/crm_md.md)], чтобы включить его снова, вы должны подключиться через [!INCLUDE[d365fin](includes/cds_long_md.md)]. 

> [!NOTE]
> При повторном подключении через [!INCLUDE[d365fin](includes/cds_long_md.md)] применяются настройки синхронизации по умолчанию и перезаписываются все ваши конфигурации. Например, будут применены сопоставления таблиц по умолчанию.

## <a name="to-upgrade-your-connection-to-use-common-data-service"></a>Обновление подключения для использования Common Data Service
1. Откройте страницу **Настройка подключения Microsoft Dynamics 365**, выберите переключатель **Включено**, чтобы отключить существующее подключение к [!INCLUDE[crm_md](includes/crm_md.md)].
2. Откройте страницу **Настройка подключения Common Data Service** и выберите переключатель **Включено**, чтобы включить подключение.
3. После включения соединения CDS базовое решение интеграции Business Central CDS развертывается в Common Data Service.
4. На странице настройки подключения Microsoft Dynamics 365 выберите переключатель "Включено", чтобы включить подключение к [!INCLUDE[crm_md](includes/crm_md.md)].
5. После включения подключения Sales решение интеграции Business Central развертывается в Sales. Это дает возможность интеграции с объектами, которые являются специфическими для [!INCLUDE[crm_md](includes/crm_md.md)], таким как заказы на продажу, предложения с расценками и счета.
6. На странице **Настройка подключения к Sales** выберите **Использовать настройку синхронизации по умолчанию**, чтобы инициализировать сопоставление таблиц интеграции для [!INCLUDE[crm_md](includes/crm_md.md)].
7. Теперь выберите **Повторить развертывание решения интеграции** ,чтобы установить и настроить обновленное решение интеграции Business Central.

## <a name="see-also"></a>См. также
[Интеграция с Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  
[Интеграция с Common Data Service](admin-common-data-service.md)