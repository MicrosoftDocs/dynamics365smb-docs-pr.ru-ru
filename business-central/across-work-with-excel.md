---
title: Просмотр и редактирование в Excel из Business Central | Документация Майкрософт
description: Узнайте, как открывать страницы в Microsoft Excel из Business Central для более тщательного анализа данных.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 10/24/2019
ms.author: jswymer
ms.openlocfilehash: 71b4e5b7124f929255f1374b38cfbe28c9f12d2b
ms.sourcegitcommit: c6e28db8f78fa21db064c9b8a8d742f49d7db3ae
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/31/2019
ms.locfileid: "2692804"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a>Просмотр и редактирование в Excel из Business Central

В случае страниц, на которых отображается список записей в строках и столбцах, например список клиентов, заказов на продажи или счетов, можно также просмотреть записи с помощью Microsoft Excel. Для этого существует два варианта. Можно выбрать действие **Открыть в Excel** или действие **Изменить в Excel** на странице. Различия между двумя действиями состоят в следующем:  

## <a name="open-in-excel"></a>Открыть в Excel

- С помощью этого действия Excel учитывает все фильтры на странице, которые ограничивают отображаемые записи. Это означает, что книга Excel будет содержать те же строки и столбцы, которые отображаются на странице в [!INCLUDE[prodshort](includes/prodshort.md)].

- Можно внести изменения в записи в Excel, но невозможно опубликовать изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)]. Можно только сохранить изменения в файл Microsoft Excel на компьютере. 

- Это действие работает как в Windows, так и в macOS. 

> [!NOTE]
> Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Открыть в Excel** доступно по умолчанию. Тем не менее, если вы настроили [!INCLUDE [prodshort](includes/prodshort.md)] On-premises для редактирования данных в Excel, то действие **Открыть в Excel** заменяется действием **Изменить в Excel**.

## <a name="edit-in-excel"></a>Изменить в Excel

- С помощью этого действия Excel учитывает большинство фильтров на странице, которые ограничивают отображаемые записи. Это означает, что книга Excel будет содержать почти те же записи и столбцы.

- Преимущество действия **Изменить в Excel** заключается в том, что оно позволяет внести изменения в записи в Excel, затем опубликовать эти изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)].

- Оно работает только в Windows, но не в macOS.

Это было улучшено в выпуске 2019 года, волна 2. Для получения дополнительной информации см. раздел [Улучшения интеграции с Excel](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration).

> [!NOTE]
> Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Изменить в Excel** доступно только в том случае, если ваш администратор настроил надстройку Excel. Для администраторов порядок установки надстройки Excel приведен в разделе [Настройка надстройки Excel для редактирования данных Business Central](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).

> [!NOTE]
> Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises эта функция доступна только для веб-клиента.

### <a name="see-the-differences-between-the-options"></a>См. разницу между параметрами 
> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-also"></a>См. также
[Работа с Business Central](ui-work-product.md)  
