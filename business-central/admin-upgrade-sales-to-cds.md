---
title: Обновление интеграции с Dynamics 365 Sales
description: В этой теме рассказывается, как переместить интеграцию Dynamics 365 Business Central с Dynamics 365 Sales в последнюю версию.
author: bholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, integrating
ms.date: 06/14/2021
ms.author: bholtorf
ms.openlocfilehash: 977238383e7f4e4745e48a1966fe7714125406eb
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "8148802"
---
# <a name="upgrading-an-integration-with-dynamics-365-sales"></a>Обновление интеграции с Dynamics 365 Sales
[!INCLUDE[prod_short](includes/prod_short.md)] интегрируется с [!INCLUDE[prod_short](includes/cds_long_md.md)], что позволяет легко подключать и синхронизировать данные с другими приложениями Dynamics 365, такими как [!INCLUDE[crm_md](includes/crm_md.md)], или даже с приложениями, которые вы создаете сами. Если вы впервые выполняете интеграцию, мы рекомендуем сделать это через [!INCLUDE[prod_short](includes/cds_long_md.md)]. Дополнительные сведения см. в разделе [Интеграция с Dataverse](admin-common-data-service.md).

Если вы уже интегрировали [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[prod_short](includes/prod_short.md)], вы можете продолжить синхронизацию данных, используя ваши настройки. Однако, если вы обновите [!INCLUDE[prod_short](includes/prod_short.md)] или выключите интеграцию [!INCLUDE[crm_md](includes/crm_md.md)], чтобы включить его снова, вы должны подключиться через [!INCLUDE[prod_short](includes/cds_long_md.md)]. 

> [!NOTE]
> При повторном подключении через [!INCLUDE[prod_short](includes/cds_long_md.md)] применяются настройки синхронизации по умолчанию и перезаписываются все ваши конфигурации. Например, будут применены сопоставления таблиц по умолчанию.

## <a name="to-upgrade-your-connection-to-use-dataverse"></a>Обновление подключения для использования Dataverse
1. Откройте страницу **Настройка подключения Microsoft Dynamics 365** затем выключите переключатель **Включено**. Затем закройте страницу, чтобы отключиться от [!INCLUDE[crm_md](includes/crm_md.md)].
2. Откройте страницу **Настройка подключения Dataverse** и в поле **Модель ответственности** выберите **Человек**. Затем выберите переключатель **Включено**, чтобы включить подключение к [!INCLUDE[prod_short](includes/cds_long_md.md)].
  
   > [!NOTE]
   > После включения соединения решение интеграции Business Central развертывается в Dataverse.
4. На странице **Настройка подключения Microsoft Dynamics 365** выберите **Повторить развертывание решения интеграции**,чтобы переустановить решение интеграции Business Central.
5. Включите переключатель **Включено**, чтобы снова подключиться к [!INCLUDE[crm_md](includes/crm_md.md)].
  
   > [!NOTE]
   > После включения соединения решение интеграции Business Central развертывается в [!INCLUDE[prod_short](includes/prod_short.md)]. Это дает возможность интеграции с таблицами, которые являются специфическими для [!INCLUDE[crm_md](includes/crm_md.md)], таким как заказы на продажу, предложения с расценками и счета.
6. На странице **Настройка подключения к Sales** выберите **Использовать настройку синхронизации по умолчанию**, чтобы инициализировать сопоставление таблиц интеграции для [!INCLUDE[crm_md](includes/crm_md.md)].

   > [!IMPORTANT]
   > С помощью действия **Использовать настройку синхронизации по умолчанию** примените сопоставления таблиц интеграции по умолчанию. Все настраиваемые сопоставления будут перезаписаны. Если у вас есть настраиваемые сопоставления, которые вы хотите сохранить, мы рекомендуем вам экспортировать их в Excel или поговорить со своим партнером Майкрософт о других способах сохранения настраиваемых сопоставлений.    

## <a name="see-also"></a>См. также
[Интеграция с Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  
[Интеграция с Microsoft Dataverse](admin-common-data-service.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]