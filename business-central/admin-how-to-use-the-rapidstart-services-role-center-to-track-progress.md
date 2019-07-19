---
title: Использование ролевого центра "Внедряющий мастер служб RapidStart Services" | Документы Майкрософт
description: При использовании служб RapidStart Services рекомендуется отслеживать свою работу и использовать ролевой центр «Внедряющий мастер служб RapidStart Services», так как он предоставляет правильный контекст для вашей работы по конфигурации.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: /dynamics365/business-central/admin-set-up-company-configuration
ROBOTS: NOINDEX
ms.openlocfilehash: e1cfcc47d5fb1112c4422be93ab49a345e9a30ec
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1726909"
---
# <a name="use-the-rapidstart-services-implementer-role-center"></a>Использование ролевого центра «Внедряющий мастер служб RapidStart Services»
При использовании служб RapidStart Services рекомендуется использовать ролевой центр «Внедряющий мастер служб RapidStart Services», так как он предоставляет правильный контекст для вашей работы по конфигурации. Дополнительные сведения см. в разделе [Изменение ролевого центра](ui-change-basic-settings.md#to-change-role-center).

Во время работы вы можете назначить каждой таблице статус, который отражает текущее состояние работ. В этом случае [!INCLUDE[d365fin](includes/d365fin_md.md)] отслеживает статус таблицы в части **Действия** в ролевом центре.  

По умолчанию при добавлении таблицы в журнал конфигураций ее статус устанавливается пустым. Это означает, что конфигурация таблицы не началась. Это отражено в количестве **Не запущено** на плитке **Действия**.  

## <a name="to-update-the-status-of-a-configuration-table"></a>Обновление статуса таблицы конфигурации  
1.  Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал конфигураций**, затем выберите связанную ссылку.  
2.  Выберите действие **Изменить список**.  
3.  Выберите таблицу, а затем в поле **Статус** выберите подходящий статус.  
4.  Нажмите кнопку **ОК**.  

При возврате в ролевой центр плитки в части **Действия** обновляются, чтобы отразить внесенные изменения.  

## <a name="to-track-the-status-of-a-configuration-project"></a>Трассировка статуса проекта конфигурации  
- Откройте ролевой центр RapidStart Services.  

В разделе **Области конфигурации** отображается статистику завершения для областей и групп, которые вы настроили. Если не были заданы области или группы, то в этой части данные отсутствуют.  

## <a name="to-see-a-filtered-view-of-table-status"></a>Просмотр отфильтрованного представления статуса таблицы  
1. Выберите действие **Таблицы**.  
2. Выберите подходящее представление с фильтром.  

## <a name="see-also"></a>См. также  
[Настройка организации со службами RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Администрация](admin-setup-and-administration.md)
