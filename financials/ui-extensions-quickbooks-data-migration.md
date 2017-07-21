---
title: "Использование расширения для миграции данных QuickBooks | Документы Майкрософт"
description: "Описывает, как использовать расширение для импорта клиентов, поставщиков, товаров и счетов из QuickBooks Desktop в Dynamics 365 for Financials."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 37d90316ea0be5489fb5abe33645de3fe0d3cf90
ms.contentlocale: ru-ru
ms.lasthandoff: 07/07/2017


---
# <a name="the-quickbooks-data-migration-extension-for-dynamics-365-for-financials"></a>Расширение для миграции данных QuickBooks для Dynamics 365 for Financials
Это расширение облегчает миграцию клиентов, поставщиков, товаров и счетов из QuickBooks в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Если сейчас ваша компания использует QuickBooks, вы можете экспортировать требуемую информацию, а затем открыть руководство по сопровождаемой настройке, чтобы загрузить данные в [!INCLUDE[d365fin](includes/d365fin_md.md)].  
Дополнительные сведения см. в разделе [Импорт бизнес-данных из других финансовых систем](upload-data.md).

## <a name="exporting-data-from-quickbooks"></a>Экспорт данных из QuickBooks
Вы должны были экспортировать часть или всех ваших существующих клиентов, поставщиков, складские товары и счета в файл Intuit Interchange Format (IIF). Расширение для миграции данных QuickBooks содержит сопоставление данных QuickBooks по умолчанию, чтобы вы могли использовать собственные данные для тестирования новой организации [!INCLUDE[d365fin](includes/d365fin_md.md)]. Сопоставления по умолчанию будет в большинстве случаев достаточно, но можно изменить его с помощью руководства по настройке.  
В QuickBooks в меню "Файл" есть служебная программа для экспорта списков. Для целей [!INCLUDE[d365fin](includes/d365fin_md.md)] можно экспортировать следующие списки:

* Список клиентов  
* Список поставщиков  
* Список товаров  
* Список счетов  

Экспортируемые данные сохраняются в виде файла IIF, который затем можно загрузить в [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="see-also"></a>См. также
[Импорт бизнес-данных из других финансовых систем](upload-data.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  

