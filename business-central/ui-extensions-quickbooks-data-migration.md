---
title: "Использование расширения для миграции данных QuickBooks | Microsoft Docs"
description: "Описывает, как использовать расширение для импорта клиентов, поставщиков, товаров и счетов из QuickBooks Desktop в Business Central."
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: ad1b888d475c0523c5a905e804a3f89ab4531b28
ms.openlocfilehash: c7348ff75e2f9660611d0d2aed0fa1beacfa259c
ms.contentlocale: ru-ru
ms.lasthandoff: 05/17/2018

---
# <a name="the-quickbooks-data-migration-extension-for-business-central"></a>Расширение "Миграция данных QuickBooks" для Business Central
Это расширение облегчает миграцию клиентов, поставщиков, товаров и счетов из QuickBooks в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Если сейчас ваша компания использует QuickBooks, вы можете экспортировать требуемую информацию, а затем открыть руководство по сопровождаемой настройке, чтобы загрузить данные в [!INCLUDE[d365fin](includes/d365fin_md.md)].  
Дополнительные сведения см. в разделе [Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md).

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
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  

