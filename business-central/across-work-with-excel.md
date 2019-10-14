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
ms.date: 10/01/2019
ms.author: jswymer
ms.openlocfilehash: 2474f83fd9fa137b40756a3d07ac025208f3ac6c
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2308264"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a>Просмотр и редактирование в Excel из Business Central 

В случае страниц, на которых отображается список записей в строках и столбцах, например список клиентов, заказов на продажи или счетов, можно также просмотреть записи с помощью Microsoft Excel. Для этого существует два варианта. Можно выбрать действие **Открыть в Excel** или действие **Изменить в Excel** на странице. Различия между двумя действиями состоят в следующем:  

## <a name="open-in-excel"></a>Открыть в Excel

-    С помощью этого действия Excel учитывает все фильтры на странице для ограничения отображаемых записей. Это означает, что книга Excel будет содержать те же строки и столбцы, которые отображаются на странице в [!INCLUDE[prodshort](includes/prodshort.md)].

-    Можно внести изменения в записи в Excel, но невозможно опубликовать изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)]. Можно только сохранить изменения в файл Microsoft Excel на компьютере. 

-    Это действие работает как в Windows, так и в macOS. 

>[!NOTE]
>Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Открыть в Excel** недоступно, если имеется действие **Изменить в Excel**.

## <a name="edit-in-excel"></a>Изменить в Excel

-    С помощью этого действия книга Excel не будет учитывать фильтры на странице для ограничения отображаемых записей. Это означает, что книга Excel будет содержать все доступные учетные записи и столбцы, независимо от того, что отображается на странице. 

-    Преимущество действия **Изменить в Excel** заключается в том, что оно позволяет внести изменения в записи в Excel, затем опубликовать эти изменения обратно в [!INCLUDE[prodshort](includes/prodshort.md)].

-    Оно работает только в Windows, но не в macOS.

>[!NOTE]
>Для [!INCLUDE[prodshort](includes/prodshort.md)] On-premises действие **Изменить в Excel** доступно только в том случае, если ваш администратор установил надстройку Excel. Для администраторов порядок установки надстройки Excel приведен в разделе [Настройка надстройки Excel](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).

### <a name="see-the-differences-between-the-options"></a>См. разницу между параметрами 
> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-also"></a>См. также
[Работа с Business Central](ui-work-product.md)  
