---
title: "Использование расширения для миграции данных QuickBooks | Документы Майкрософт"
description: "Описывает, как использовать расширение для импорта клиентов, поставщиков, товаров и счетов из QuickBooks Desktop в Dynamics 365 for Financials."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 4775c945a7721b8f4e52a187840a585396611e47
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="the-quickbooks-data-migration-extension-for-dynamics-365-for-financials"></a>Расширение для миграции данных QuickBooks для Dynamics 365 for Financials
Это расширение облегчает миграцию клиентов, поставщиков, товаров и счетов из QuickBooks Desktop в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Если сейчас ваша компания использует QuickBooks, вы можете экспортировать требуемую информацию, а затем открыть руководство по сопровождаемой настройке, чтобы загрузить данные в [!INCLUDE[d365fin](includes/d365fin_md.md)].  
Дополнительные сведения см. в разделе [Импорт бизнес-данных из других финансовых систем](upload-data.md).

## <a name="exporting-data-from-quickbooks-desktop"></a>Экспорт данных из QuickBooks Desktop
Вы должны были экспортировать часть или всех ваших существующих клиентов, поставщиков, складские товары и счета в файл Intuit Interchange Format (IIF). Расширение для миграции данных QuickBooks содержит сопоставление данных QuickBooks по умолчанию, чтобы вы могли использовать собственные данные для тестирования новой организации [!INCLUDE[d365fin](includes/d365fin_md.md)]. Сопоставления по умолчанию будет в большинстве случаев достаточно, но можно изменить его с помощью руководства по настройке.  
В QuickBooks в меню "Файл" есть служебная программа для экспорта списков. Для целей [!INCLUDE[d365fin](includes/d365fin_md.md)] можно экспортировать следующие списки:

* Список клиентов  
* Список поставщиков  
* Список товаров  
* Список счетов  

Экспортируемые данные сохраняются в виде файла IIF, который затем можно загрузить в [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="finding-the-quickbooks-data-migration-extension"></a>Поиск расширения для миграции данных QuickBooks
Расширение миграции данных QuickBooks установлено и готово к работе как составная часть мастер настройки миграции данных. Если вы готовы начать прямо сейчас и уже экспортировали свои данные из QuickBooks, выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Мастер настройки**, затем выберите связанную ссылку. Выберите **Миграция бизнес-данных**, затем выполните шаги в руководстве.  

## <a name="see-also"></a>См. также
[Импорт бизнес-данных из других финансовых систем](upload-data.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  

