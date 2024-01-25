---
title: Введение в демонстрационные данные Contoso Coffee
description: 'Обзор сценариев, в которых демонстрационные данные Contoso Coffee могут помочь вам узнать, как использовать возможности Business Central.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.date: 09/20/2023
ms.topic: article
ms.service: dynamics-365-business-central
ms.search.form: '5194,'
ms.custom: bap-template
---

# <a name="introduction-to-contoso-coffee-demo-data"></a>Введение в демонстрационные данные Contoso Coffee

Contoso Coffee — вымышленная компания, производящая бытовые и коммерческие кофеварки. Приложения **Contoso Coffee** для [!INCLUDE [prod_short](../includes/prod_short.md)] предназначены для добавления демонстрационных данных, которые вы можете использовать для ознакомлений с возможностями [!INCLUDE [prod_short](../includes/prod_short.md)].  

## <a name="set-up-contoso-coffee-data"></a>Настройка данных Contoso Coffee

[!INCLUDE [contoso-coffee-app-install](../includes/contoso-coffee-app-install.md)]

После установки приложений на странице **Демонстрационные данные Contoso** используйте действие **Настроить**, чтобы подготовить следующие модули. Вы можете установить все доступные данные, включая конфигурационные и рабочие данные, или только конфигурационные данные.

 - **Общий модуль** для подготовки общих параметров, которые требуются [!INCLUDE [prod_short](../includes/prod_short.md)]. Например, к этим параметрам относятся серии номеров. 

Параметры рассматриваются в таблице ниже:  

|Поле  |Описанием  |
|---------|---------|
|**Начальный год** |Указывает первый год, который вы хотите использовать для демонстрационных данных Contoso Coffee. В зависимости от настройки компании год может быть либо календарным, либо финансовым годом.|
|**Код страны/региона**|Указывает код страны/региона для внутренних клиентов и поставщиков.|
|**Тип организации**    |Указывает, должна ли текущая компания сообщать НДС или налог с продаж. |
|**Ценовой фактор**     |Указывает коэффициент для конвертации цены из долларов США/евро в местную валюту. *1* означает, что цена — это одинаковая сумма в любой валюте. Для получения цены в местной валюте будет использоваться более высокое число. |
|**Точность Округления**  |Указывает точность округления, которую вы хотите использовать для создания демонстрационных данных.|

 - [Модуль «Производство»](manufacturing/contoso-coffee-manufacturing-intro.md), чтобы подготовиться к [производственным сценариям](manufacturing/contoso-coffee-manufacturing-intro.md#scenarios).
 - [Модуль «Складское хозяйство»](warehousing/contoso-coffee-warehousing-intro.md), чтобы подготовиться к [складским сценариям](warehousing/contoso-coffee-warehousing-intro.md#scenarios).
 - [Модуль «Сервис»](service/contoso-coffee-service-intro.md), чтобы подготовиться к [сервисным сценариям](service/contoso-coffee-service-intro.md#scenarios).

После настройки модулей, которые вы хотите опробовать, выберите действие **Создать**, чтобы создать для них демонстрационные данные.

## <a name="see-also"></a>См. также

[Производство](../production-manage-manufacturing.md)  
[Складское хозяйство](../warehouse-manage-warehouse.md)  
[Служба](../service-service.md)
<!-- [Projects and Jobs](../projects-manage-projects.md) -->

