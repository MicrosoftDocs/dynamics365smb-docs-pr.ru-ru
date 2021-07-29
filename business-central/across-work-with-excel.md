---
title: Просмотр и редактирование в Excel из Business Central
description: Узнайте, как открывать страницы в Microsoft Excel из Business Central для более тщательного анализа данных.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 6bf12f55f6bce843c4ed12f2a40db542367fffde
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "6443485"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a>Просмотр и редактирование в Excel из Business Central

В случае страниц, на которых отображается список записей в строках и столбцах, например список клиентов, заказов на продажи или счетов, можно также просмотреть записи с помощью Microsoft Excel. В зависимости от страницы у вас есть два варианта просмотра в Excel. Можно выбрать действие **Открыть в Excel** или действие **Изменить в Excel** на странице. В этой статье объясняются различия между двумя действиями.

## <a name="open-in-excel"></a>Открыть в Excel

С помощью действия **Открыть в Excel** вы можете вносить изменения в записи в Excel, но не можете публиковать изменения обратно в [!INCLUDE[prod_short](includes/prod_short.md)]. Можно только сохранить изменения в файл Microsoft Excel на компьютере.

- С помощью этого действия Excel учитывает все фильтры на странице, которые ограничивают отображаемые записи. Книга Excel будет содержать те же строки и столбцы, которые отображаются на странице в [!INCLUDE[prod_short](includes/prod_short.md)].

- Это действие работает как в Windows, так и в macOS.

- Начиная с обновления 18.3, вы также можете просматривать списки, которые отображаются в частях страницы, например, в строках в заказе на продажу. На данный момент эта возможность является дополнительной функцией, для которой необходимо включить **Экспорт какой-либо части списка в Excel** в **Управление функциями**. Для получения дополнительной информации см. [Раннее включение новых функций](/dynamics365/business-central/dev-itpro/administration/feature-management). 

> [!NOTE]
> Для [!INCLUDE[prod_short](includes/prod_short.md)] On-premises действие **Открыть в Excel** доступно по умолчанию. Тем не менее, если вы настроили [!INCLUDE[prod_short](includes/prod_short.md)] On-premises для редактирования данных в Excel, то действие **Открыть в Excel** заменяется действием **Изменить в Excel**.

[!INCLUDE [send-report-excel](includes/send-report-excel.md)]  

## <a name="edit-in-excel"></a>Изменить в Excel

С помощью действия **Изменить в Excel** вы можете вносить изменения в записи в Excel и публиковать изменения обратно в [!INCLUDE[prod_short](includes/prod_short.md)].

- Благодаря этому действию Excel учитывает большинство фильтров на странице, которые ограничивают отображаемые записи, поэтому книга Excel будет содержать почти те же записи и столбцы.

- Оно работает только в Windows, но не в macOS.

- Вы можете сменить компанию, с которой вы работаете. Чтобы переключить компанию, выберите значок **Параметры** ![Параметры надстройки Excel.](media/cogwheel.png "Параметры надстроек Excel") на панели надстройки Excel, затем выберите компанию в поле **Компания**.  

    > [!IMPORTANT]
    > При смене компании убедитесь, что поле **Среда** не пустое. Если оно пустое, установите для него один из доступных параметров; в противном случае надстройка не будет работать правильно.  

Если вы вносите изменения в надстройку, вы должны перезагрузить ее, чтобы обновить подключение. Чтобы перезагрузить, используйте меню ![Меню надстроек Excel](media/excel-addin-menu.png "Меню надстроек Excel") в правом верхнем углу надстройки. Если вы не можете загрузить надстройку, обратитесь к администратору. Если вы администратор, см. раздел [Настройка надстройки Excel для редактирования данных Business Central](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).

> [!NOTE]
> Для [!INCLUDE[prod_short](includes/prod_short.md)] On-premises действие **Изменить в Excel** доступно только в том случае, если ваш администратор настроил надстройку Excel, и доступна только для веб-клиента. Для администраторов порядок установки надстройки Excel приведен в разделе [Настройка надстройки Excel для редактирования данных Business Central](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).

### <a name="see-the-differences-between-the-options"></a>См. разницу между параметрами
<br><br>  

> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Анализ финансовых отчетов в Microsoft Excel](finance-analyze-excel.md)  
[Работа с Business Central](ui-work-product.md)  
[Улучшения интеграции с Excel в волне 2 выпуска 2019 года](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration)  


[!INCLUDE[footer-include](includes/footer-banner.md)]