---
title: Связывание и синхронизация записей вручную | Документация Майкрософт
description: Синхронизация сопоставления таблиц интеграции позволяет синхронизировать данные во всех записях в связанных таблице Business Central и объекте Dynamics 365 Sales.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: crm, sales, couple, decouple, synchronize
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: d8140f71709208a271eff5c8de415b0e95736072
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3911409"
---
# <a name="couple-and-synchronize-records-manually"></a>Связывание и синхронизация записей вручную
В этом разделе описана процедура связывания одной или нескольких записей [!INCLUDE[d365fin](includes/d365fin_md.md)] с записями в Common Data Service или [!INCLUDE[crm_md](includes/crm_md.md)]. Связывание записей позволяет просматривать сведения Common Data Service из [!INCLUDE[d365fin](includes/d365fin_md.md)] и наоборот. Связывание также позволяет синхронизировать данные между записями. Можно связать существующие записи или создать и связать новые записи.

> [!Note]
> Связывание и синхронизация данных доступны только в том случае, если системный администратор создал подключение между [!INCLUDE[d365fin](includes/d365fin_md.md)] и Common Data Service или [!INCLUDE[crm_md](includes/crm_md.md)]. Быстрый способ проверить — это открыть карточку **Клиент** и найти действие **Настроить связывание**. Если действие доступно, приложения подключены.   

## <a name="video-example"></a>Видео с примером

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098376]

## <a name="to-couple-a-record"></a>Связывание записи  
1.  В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте карточку для записи, которую требуется связать. Например, карточка клиента или контакта.  

    Можно также открыть страницу списка и выбрать запись, которую следует связать.  

2.  Выберите действие **Настроить связывание**.  
3.  Заполните поля, затем выберите **ОК**.  

## <a name="to-synchronize-a-single-record"></a>Синхронизация одной записи  
1.  В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте карточку для записи, которую требуется связать. Например, карточка клиента или контакта.  
2.  Выберите действие **Синхронизировать сейчас**.  
3.  Если запись можно синхронизировать в одном направлении, выберите параметр, определяющий направление обновления данных, затем выберите **ОК**.  

## <a name="to-synchronize-a-single-record-from-crm_md"></a>Синхронизация одной записи из [!INCLUDE[crm_md](includes/crm_md.md)]  
1.  В [!INCLUDE[crm_md](includes/crm_md.md)] откройте форму для записи, которую требуется связать. Например, форма карточки организации или карточки контакта.  
2.  Выберите действие **[!INCLUDE[d365fin](includes/d365fin_md.md)]** на ленте, чтобы открыть и связать запись автоматически.

> [!Note]
> Вы можете синхронизировать одну запись из [!INCLUDE[crm_md](includes/crm_md.md)] автоматически, только когда параметр **Синхр. только связанные записи** отключен, и установлено направление синхронизации "Двунаправленная" или "Из таблицы интеграции" на странице **Сопоставление таблиц интеграции** для записи. Дополнительные сведения см. в разделе [Сопоставление таблиц и полей для синхронизации](admin-how-to-modify-table-mappings-for-synchronization.md#creating-new-records).     

## <a name="to-synchronize-multiple-records"></a>Синхронизация нескольких записей  
1.  В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте страницу списка для записи, например страницы списка "Клиенты" или "Контакты".  
2.  Выберите записи, который требуется синхронизировать, затем выберите действие **Синхронизировать сейчас**.  
3.  Если записи можно синхронизировать в одном направлении, выберите параметр, определяющий направление, затем выберите **ОК**.  

## <a name="see-also"></a>См. также  
[Использование Dynamics 365 Sales из Business Central](marketing-integrate-dynamicscrm.md)
