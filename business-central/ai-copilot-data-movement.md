---
title: Перемещение данных Copilot по географическим регионам
description: 'Узнайте, как данные, используемые в функциях Copilot в Dynamics 365 Business Central, перемещается по географическим регионам, где служба Azure OpenAI по умолчанию недоступна.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: conceptual
ms.date: 04/16/2024
ms.custom: bap-template
ms.collection:
  - bap-ai-copilot
---

# Перемещение данных Copilot по географическим регионам 

Copilot доступен во всех поддерживаемых [странах/регионах Business Central](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations). Однако Copilot использует службу Microsoft Azure OpenAI, которая в настоящее время доступна для Business Central только в некоторых географических регионах. Это означает, что если ваша среда расположена в другом месте, данные функций Copilot и генеративного искусственного интеллекта должны передаваться за пределы вашего географического региона и могут обрабатываться и храниться за пределами границ вашего соответствия требованиям. Данные включают в себя подсказки ИИ и ваши бизнес-данные, которые используются или генерируются Copilot. В этом случае вам необходимо разрешить перемещение данных в службе Azure OpenAI в другой географический регион. <!--For a list of geographies, refer to the [Azure OpenAI Service geographies](#azure-openai-service-geographies) section that follows.-->

> [!IMPORTANT]
> Если ваша среда находится в том же регионе Azure, что и служба Azure OpenAI, она автоматически подключается к службе Azure OpenAI, без вариантов; никакая разовая настройка не требуется.

> [!NOTE]
> Отдельные функции Copilot и генеративного ИИ могут быть доступны не во всех странах/регионах сред Business Central. Чтобы узнать о доступности, проконсультируйтесь с издателем каждой возможности.
> 
> Функции Copilot и генеративного ИИ от издателей, не принадлежащих Microsoft, например, возникшие в результате настроек или из приложений AppSource, которые вы устанавливаете, каждая определяет свой собственный регион службы Azure OpenAI. Проконсультируйтесь с издателем расширения, чтобы узнать, какие региональные службы Azure используются расширением. 

### Географические регионы службы Azure OpenAI

В следующей таблице приведены географические регионы службы Azure OpenAI, используемые Copilot, в зависимости от региона Azure среды Business Central. Эта информация важна при принятии решения о том, следует ли соглашаться на перемещение данных между регионами. Узнать регион Azure своей среды вы можете в центре администрирования Business Central (см. статью [Управление средами в центре администрирования](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments)).

| Среда региона Azure| Географический регион службы Azure OpenAI|Действие администратора, необходимое для включения Copilot| 
| - | - | - |
|Азия (Восточная, Юго-Восточная) |Соединенные Штаты|Да|
|Австралия (Юго-Восточная)| Австралия |Нет |
|Бразилия (Южная) |Соединенные Штаты|Да|
|Канада (Центральная, Восточная)|Соединенные Штаты|Да|
|Европа (Западная, Северная)| Швеция или Швейцария |Нет\*|
|Франция (Центральная, Южная)| Швеция или Швейцария |Да|
|Германия (Северная, Центрально-Западная)| Швеция или Швейцария |Да|
|Индия (Центральная, Южная)|Индия|Нет|
|Япония (Восточная, Западная)|Соединенные Штаты|Да|
|Республика Корея (Центральная, Южная)|Соединенные Штаты|Да|
|Норвегия (Восток, Запад)|Швеция или Швейцария |Да|
|ЮАР (Север, Запад)|Соединенные Штаты|Да|
|Швейцария (Северная, Западная) |Швеция или Швейцария |Да|
|ОАЭ (Север, Запад)|Соединенные Штаты|Да|
|Соединенное Королевство (Юг, Запад)|Соединенное Королевство|Нет|
|США (Центр, Восток, Северный Центральный, Южный Центральный, Запад) |Соединенные Штаты|Нет|

\* Для сред в регионах Azure «Западная Европа» и «Северная Европа» в Business Central автоматически разрешено перемещение данных между регионами, однако администраторы могут в любой момент от этого отказаться.

> [!NOTE]
> После того как служба Azure OpenAI станет доступной в вашем регионе Business Central, ваша среда автоматически перейдет на использование этой службы Azure OpenAI и согласие на участие не будет требоваться, и даже предоставить его будет невозможно.
<!--

BC geos base on https://dynamics.microsoft.com/en-us/availability-reports/georeport/
case "AUSTRALIAEAST":
            case "AUSTRALIASOUTHEAST":
                return new CapiRegion("au", 2);
            case "BRAZILSOUTH":
                return new CapiRegion("br", 2);
            case "CANADACENTRAL":
            case "CANADAEAST":
                return new CapiRegion("ca", 2);
            case "CENTRALINDIA":
            case "SOUTHINDIA":
                return new CapiRegion("in", 1);
            case "EASTASIA":
                return new CapiRegion("as", 2);
            case "EASTUS":
            case "EASTUS2":
            case "SOUTHCENTRALUS":
            case "CENTRALUS":
            case "NORTHCENTRALUS":
            case "WESTUS":
            case "US":
                return new CapiRegion("us", 9, HasGpt4InGeo: true, HasTurboInGeo: true);
            case "FRANCECENTRAL":
            case "FRANCESOUTH":
                return new CapiRegion("fr", 1);
            case "GERMANYNORTH":
            case "GERMANYWESTCENTRAL":
                return new CapiRegion("de", 1);
            case "JAPANEAST":
            case "JAPANWEST":
                return new CapiRegion("jp", 1);
            case "KOREACENTRAL":
            case "KOREASOUTH":
                return new CapiRegion("kr", 1);
            case "NORWAYEAST":
            case "NORWAYWEST":
                return new CapiRegion("no", 1);
            case "SOUTHAFRICANORTH":
            case "SOUTHWESTAFRICA":
                return new CapiRegion("za", 1);
            case "SOUTHEASTASIA":
                return new CapiRegion("sg", 1);
            case "SWITZERLANDNORTH":
            case "SWITZERLANDWEST":
                return new CapiRegion("ch", 1, HasTurboInGeo: true);
            case "UKSOUTH":
            case "UKWEST":
                return new CapiRegion("uk", 2);
            case "NORTHEUROPE":
            case "WESTEUROPE":
                return new CapiRegion("eu", 10);
            case "UAENORTH":
            case "UAECENTRAL":
                return new CapiRegion("ae", 1);

-->

## Дальнейшие шаги

Вы соглашаетесь на перемещение данных между регионами (или отказываетесь от него) на странице [Возможности Copilot и ИИ](https://businesscentral.dynamics.com/?page=7775). Чтобы узнать больше, перейдите в раздел [Разрешение перемещения данных между географическими регионами](enable-ai.md#allow-data-movement-across-geographies).
