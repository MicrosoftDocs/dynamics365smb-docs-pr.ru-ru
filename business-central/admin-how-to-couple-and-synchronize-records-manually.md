---
title: Связывание и синхронизация записей вручную | Документы Майкрософт
description: Синхронизация сопоставления таблиц интеграции позволяет синхронизировать данные во всех записях в таблице в Business Central и объекте Dynamics 365 for Sales, которые связаны.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: crm, sales, couple, decouple, synchronize
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: 6d1248ac77208e382c5594af57335df6ff824630
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1726771"
---
# <a name="couple-and-synchronize-records-manually"></a>Связывание и синхронизация записей вручную
В этом разделе описана процедура связывания одной или нескольких записей [!INCLUDE[d365fin](includes/d365fin_md.md)] с записями в [!INCLUDE[crm_md](includes/crm_md.md)]. Связывание записей позволяет просматривать сведения [!INCLUDE[crm_md](includes/crm_md.md)] из [!INCLUDE[d365fin](includes/d365fin_md.md)] и наоборот. Связывание также позволяет синхронизировать данные между записями. Можно связать существующие записи или создать и связать новые записи.

> [!Note]
> Связывание и синхронизация данных с [!INCLUDE[crm_md](includes/crm_md.md)] доступны только в том случае, если системный администратор создал подключение между [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)]. Быстрый способ проверить — это открыть карточку **Клиент** и найти действие **Настроить связывание**. Если действие доступно, приложения подключены.   

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098376]

## <a name="to-couple-a-record"></a>Связывание записи  
1.  В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте карточку для записи, которую требуется связать. Например, карточка клиента или контакта.  

    Можно также открыть страницу списка и выбрать запись, которую следует связать.  

2.  Выберите действие **Настроить связывание**.  
3.  Заполните поля, затем выберите **ОК**.  

## <a name="to-synchronize-a-single-record"></a>Синхронизация одной записи  
1.  В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте карточку для записи, которую требуется связать. Например, карточка клиента или контакта.  
2.  Выберите действие **Синхронизировать сейчас**.  
3.  Если запись можно синхронизировать из [!INCLUDE[d365fin](includes/d365fin_md.md)] с [!INCLUDE[crm_md](includes/crm_md.md)] или из [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)], выберите параметр, определяющий направление обновления данных, а затем нажмите кнопку **ОК**.  

## <a name="to-synchronize-multiple-records"></a>Синхронизация нескольких записей  
1.  В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте страницу списка для записи, например страницы списка "Клиенты" или "Контакты".  
2.  Выберите записи, который требуется синхронизировать, затем выберите действие **Синхронизировать сейчас**.  
3.  Если записи можно синхронизировать из [!INCLUDE[d365fin](includes/d365fin_md.md)] с [!INCLUDE[crm_md](includes/crm_md.md)] или из [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)], выберите параметр, определяющий направление обновления данных, а затем нажмите кнопку **ОК**.  

## <a name="see-also"></a>См. также  
[Использование Dynamics 365 for Sales из Business Central](marketing-integrate-dynamicscrm.md)
