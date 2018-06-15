---
title: "Создание входящего сальдо журнала | Microsoft Docs"
description: "Business Central включает несколько пакетных заданий, которые помогают перенести предыдущие сальдо счетов в заново настроенную организацию. Можно легко перенести эти данные с помощью учета в журналах."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/06/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: fc8e8f34220643b7cd3fd357aea3807641cee911
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="create-journal-opening-balances"></a>Создание входящего сальдо журнала
[!INCLUDE[d365fin](includes/d365fin_md.md)] включает несколько пакетных заданий, которые помогают перенести предыдущие сальдо счетов в заново настроенную организацию. Можно легко перенести эти данные с помощью журнала клиентов, журнала поставщиков, журнала товаров или журнала ГК.

Первым этапом является создание пакета конфигурации, включающего таблицы настройки таких журналов. Следующая процедура предполагает, что этот шаг выполнен. Дополнительные сведения см. в разделе [Настройка конфигурации организации](admin-set-up-company-configuration.md). Эта процедура описывает последовательные действия, в число которых включается применение пакета, предоставленного партнером.  

Перед началом убедитесь, что вы находитесь на странице ролевого центра «Внедряющий мастер служб RapidStart Services», так как она дает правильный контекст для вашей работы по конфигурации. Дополнительные сведения см. в разделе [Изменение базовых настроек](ui-change-basic-settings.md).

## <a name="to-apply-the-entries-in-a-journal-to-a-new-company"></a>Применение журнальных записей к новой организации  
1. Настройте новую организацию и примените к ней пакет конфигурации. Дополнительные сведения см. в разделе [Настройка организации с помощью мастера RapidStart Services](admin-how-to-configure-a-company-with-the-rapidstart-wizard.md).  

    Новая организация не содержит информацию о входящем сальдо журнала.  

2. Откройте журнал конфигураций и импортируйте существующие данные о товарах, клиентах, поставщиках и Главной книге. Дополнительные сведения см. в разделе [Миграция данных клиента](admin-migrate-customer-data.md).  
3. Выберите, например действие **Создать строки журнала ГК**.  
4. Заполните экспресс-вкладку **Параметры** должным образом и по мере необходимости настройте фильтры. Например, в поле **Шаблон журнала** введите описательное имя шаблона.  
5. Нажмите кнопку **ОК**. Записи теперь находятся в журнале, но суммы не указаны.  
6. Экспортируйте таблицу журнала в Excel и вручную введите информацию об учете и балансирующем счете из унаследованных данных.
7. Импортируйте и примените информацию о таблице в новой организации. Строки журнала готовы к учету.  
8. В журнале конфигураций выберите таблицу строки журнала, затем выберите действие **Данные базы данных**.  
9. Проверьте информацию, затем выберите действие **Учет**.  
10. Повторите эти шаги для импорта и учета всех других начальных балансов.  

## <a name="see-also"></a>См. также  
[Применение конфигураций к новым организациям](admin-apply-configuration-to-new-companies.md)  
[Настройка компании с помощью служб RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Администрация](admin-setup-and-administration.md)
