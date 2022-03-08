---
title: Использование Business Central в Power BI | Документы Майкрософт
description: Можно сделать данные доступными в качестве источника данных в Power BI и создать мощные отчеты о состоянии вашего бизнеса.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 07/08/2019
ms.author: edupont
ms.openlocfilehash: c86f1c3c40f80ec993d0a3a89154047ddf9e8126
ms.sourcegitcommit: 519623f9a5134c9ffa97eeaed0841ae59835f453
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "1755245"
---
# <a name="using-prodlong-as-power-bi-data-source-for-building-reports"></a>Использование [!INCLUDE [prodlong](includes/prodlong.md)] как источника данных Power BI для создания отчетов

Можно сделать данные [!INCLUDE[prodlong](includes/prodlong.md)] доступными в качестве источника данных в Power BI и создать мощные отчеты о состоянии вашего бизнеса.  

Вы должны иметь допустимую учетную запись в [!INCLUDE[prodshort](includes/prodshort.md)] и в Power BI. Кроме того, необходимо скачать [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/). Для получения дополнительной информации см. раздел [Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data),  

## <a name="to-add-prodshort-as-a-data-source-in-power-bi-desktop"></a>Добавление [!INCLUDE[prodshort](includes/prodshort.md)] как источника данных в Power BI Desktop

1. В Power BI Desktop в левой области навигации выберите **Получить данные**.
2. На странице **Получить данные** выберите **Веб-службы**, выберите **Microsoft Dynamics 365 Business Central**, затем нажмите кнопку **Подключиться**.
3. Power BI отобразит мастер с руководством по процессу подключения. Будет предложено выполнить вход в [!INCLUDE [prodshort](includes/prodshort.md)]. Выберите **Войти** и выберите учетную запись для входа. Это должна быть та же учетная запись, которая использовалась для входа в [!INCLUDE [prodshort](includes/prodshort.md)].
4. Нажмите кнопку **Подключиться**, чтобы продолжить. Мастер Power BI отобразит список организаций и источников данных Microsoft [!INCLUDE[d365fin](includes/d365fin_md.md)]. Эти источники данных представляют все веб-службы, которые вы опубликовали из каждой организации в [!INCLUDE [prodshort](includes/prodshort.md)].

  ![powerbi_webservices.png](media/across-how-use-financials-data-source-powerbi/powerbi_webservices.png)

5. Либо создайте новый URL-адрес веб-службы в [!INCLUDE [prodshort](includes/prodshort.md)], используя действие **Создать набор данных** на странице **Веб-службы** с помощью руководства по сопровождаемой настройке **Настройка отчетов** либо используя действие **Изменить в Excel** в любом списке.
6. Укажите данные, которые требуется добавить в модель данных, а затем нажмите кнопку **Загрузить**.
7. Повторите предыдущие шаги для добавления дополнительных данных [!INCLUDE [prodshort](includes/prodshort.md)] или других данных в модель данных Power BI.

> [!NOTE]  
> После успешного подключения к [!INCLUDE [prodshort](includes/prodshort.md)] выполнять повторный вход не требуется.

После загрузки данные отобразятся в правой области навигации на странице. На этом шаге вы успешно подключились с данным [!INCLUDE [prodshort](includes/prodshort.md)] и готовы начать создание отчета Power BI.  

Перед построением отчета рекомендуется импортировать файлы темы [!INCLUDE [prodshort](includes/prodshort.md)].  Файл темы создаст цветовую палитру, чтобы можно было создавать отчеты с таким же цветовым стилем, что и приложения [!INCLUDE [prodshort](includes/prodshort.md)] без необходимости определения настраиваемых цветов для каждого визуального элемента.

Дополнительные сведения см. в разделе [Документация по Power BI](/power-bi/consumer/power-bi-consumer-landing/).

## <a name="see-also"></a>См. также

[Включение бизнес-данных для Power BI](admin-powerbi.md)  
[Бизнес-аналитика](bi.md)  
[Приступая к работе](product-get-started.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Финансы](finance.md)  
[Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
