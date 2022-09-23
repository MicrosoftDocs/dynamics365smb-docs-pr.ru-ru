---
title: Просмотр и редактирование в Excel из Business Central (содержит видео)
description: Узнайте, как открывать страницы в Microsoft Excel из Business Central для более тщательного анализа данных.
author: jswymer
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 82d08e1c072f74434ad50943a97baf77712cb171
ms.sourcegitcommit: 3acadf94fa34ca57fc137cb2296e644fbabc1a60
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2022
ms.locfileid: "9529411"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a>Просмотр и редактирование в Excel из Business Central

В случае страниц, на которых отображается список записей в строках и столбцах, например список клиентов, заказов на продажи или счетов, можно экспортировать список в Microsoft Excel и просмотреть его там. В зависимости от страницы у вас есть два варианта просмотра в Excel. Оба варианта доступны по значку **Поделиться** ![Поделиться страницей в другом приложении.](media/share-icon.png) вверху страницы. Можно выбрать действие **Открыть в Excel** или действие **Изменить в Excel** на странице. В этой статье объясняются различия между двумя действиями.

## <a name="open-in-excel"></a>Открыть в Excel

С помощью действия **Открыть в Excel** вы можете вносить изменения в записи в Excel, но не можете публиковать изменения обратно в [!INCLUDE[prod_short](includes/prod_short.md)]. Вы можете сохранить изменения только в файле Excel, не затрагивая данные в [!INCLUDE[prod_short](includes/prod_short.md)].

- С помощью этого действия Excel учитывает все фильтры на странице, которые ограничивают отображаемые записи. Книга Excel будет содержать те же строки и столбцы, которые отображаются на странице в [!INCLUDE[prod_short](includes/prod_short.md)].

- Это действие работает как в Windows, так и в macOS.

- Начиная с обновления 18.3, вы также можете просматривать списки, которые отображаются в частях страницы, например, в строках в заказе на продажу. 

> [!NOTE]
> Для [!INCLUDE[prod_short](includes/prod_short.md)] On-premises действие **Открыть в Excel** доступно по умолчанию. Тем не менее, если вы настроили [!INCLUDE[prod_short](includes/prod_short.md)] On-premises для редактирования данных в Excel, то действие **Открыть в Excel** заменяется действием **Изменить в Excel**.

[!INCLUDE [send-report-excel](includes/send-report-excel.md)]  

## <a name="edit-in-excel"></a>Изменить в Excel

Действие **Изменить в Excel** доступно в большинстве списков, но не во всех. С помощью действия **Изменить в Excel** вы можете вносить изменения в записи в Excel и публиковать изменения обратно в [!INCLUDE[prod_short](includes/prod_short.md)]. Когда откроется Excel, вы увидите область **Надстройка Excel** справа.

- Благодаря этому действию Excel учитывает большинство фильтров на странице, которые ограничивают отображаемые записи, поэтому книга Excel будет содержать почти те же записи и столбцы.

- Чтобы получить самые свежие данные из [!INCLUDE[prod_short](includes/prod_short.md)], выберите **Обновить** в области надстройки Excel.

- Вы можете сменить компанию, с которой вы работаете. Чтобы переключить компанию, выберите значок **Параметры** ![Параметры надстройки Excel.](media/cogwheel.png "Параметры надстроек Excel") на панели надстройки Excel, затем выберите компанию в поле **Компания**.  

    > [!IMPORTANT]
    > При смене компании убедитесь, что поле **Среда** не пустое. Если оно пустое, установите для него один из доступных параметров; в противном случае надстройка не будет работать правильно.  

Если вы вносите изменения в надстройку, вы должны перезагрузить ее, чтобы обновить подключение. Чтобы перезагрузить, используйте меню ![Меню надстроек Excel](media/excel-addin-menu.png "Меню надстроек Excel") в правом верхнем углу надстройки. Если вы не можете загрузить надстройку, обратитесь к администратору. Если вы администратор, см. [Получение надстройки Business Central для Excel](admin-deploy-excel-addin.md).

> [!NOTE]
> Надстройка работает с Excel в Интернете (онлайн) с любого устройства, если используется поддерживаемый браузер. Она также работает с приложением Excel для Windows (компьютер); но не для macOS.
>
> Для [!INCLUDE[prod_short](includes/prod_short.md)] On-premises действие **Изменить в Excel** доступно только в том случае, если ваш администратор настроил надстройку Excel, и доступна только для веб-клиента. Для администраторов порядок установки надстройки Excel приведен в разделе [Настройка надстройки Excel для редактирования данных Business Central](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).


<!-- Note for later: here we're immediately jumping to pretty advanced topics like changing company or reloading the addin. Fine to keep them for now. In the future, we will first need to explain in more detail the actual functionality of the addin, primarily these sub-sections:

Refreshing record data in Excel
Editing and publishing back to Business Central
Creating new records from Excel
Crafting your own editable Excel.
Point (4) is where it gets interesting for changing/specifying company, environment and other connection settings-->

### <a name="first-time-sign-in"></a>Первый вход

Действие **Изменить в Excel** требует, чтобы надстройка Business Central была установлена в Excel. В некоторых случаях ваш администратор мог настроить надстройку, чтобы приложение автоматически устанавливалось для вас. В этом случае вам просто нужно войти в Business Central в области **Надстройка Excel** с вашим именем пользователя и паролем. В противном случае открывается область **Новая надстройка Office**. Чтобы установить надстройку, выберите **Доверять этой надстройке**, что установит надстройку прямо из магазина Office.

Если по какой-то причине надстройка не устанавливается, обратитесь к администратору или попробуйте установить ее вручную. Для получения дополнительной информации см. [Установка надстройки вручную для собственного использования](admin-deploy-excel-addin.md#install).

## <a name="see-the-differences-between-the-options"></a>См. разницу между параметрами
<br><br>  

> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Анализ финансовых отчетов в Microsoft Excel](finance-analyze-excel.md)  
[Работа с Business Central](ui-work-product.md)  
[Улучшения интеграции с Excel в волне 2 выпуска 2019 года](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
