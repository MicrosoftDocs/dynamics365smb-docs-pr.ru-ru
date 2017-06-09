---
title: "Настройка маркетинговых кампаний в Financials | Документы Майкрософт"
description: "Описывается, как настроить и провести маркетинговые кампании в Dynamics 365 for Financials."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, campaign, promo, prospect
ms.date: 03/08/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 8f616382e28e29aab1ce7d9b45b8efb4ad374b96
ms.contentlocale: ru-ru
ms.lasthandoff: 05/04/2017


---
# <a name="managing-marketing-campaigns"></a>Управление маркетинговыми кампаниями
Наличие эффективного маркетингового плана помогает определять, привлекать и удерживать клиентов. Маркетинговый план состоит из различных кампаний и других видов взаимодействия, связанных с действиями по продажам и маркетингу. Планируя кампанию, необходимо решить, на какие контакты она будет ориентирована, какого она будет типа (скажем, специализированная выставка или прямая почтовая рассылка) и кто из менеджеров будет выполнять каждую задачу.

<!-- Each campaign consists of various activities or to-dos. Activities are large tasks that can be broken down into several smaller tasks or to-dos. To-dos are individual or team tasks that can be created within activities or individually and then be assigned to individual salespeople or groups of salespeople.-->

## <a name="defining-individual-campaigns"></a>Определение отдельных кампаний
Прежде чем создавать кампанию, необходимо настроить *коды статуса кампаний*. Их использование поможет управлять кампаниями путем назначения им статусов. Переходя от одного этапа кампании к другому, вы сможете видеть, на каком из них вы сейчас находитесь и какой этап следует за ним. Коды статуса кампаний настраиваются в окне **Статус кампании**.

Можно создать *карточку кампании* для каждой кампании, которую требуется отслеживать. Просмотр карточки кампании позволяет получить общие сведения о ней.
Можно удалить операции кампании, например, если некоторое действие в операции было зарегистрировано, но отменено. Можно удалить только отмененные операции кампаний.

### <a name="selecting-the-target-audience"></a>Выбор целевой аудитории
После создания кампании можно начинать создание сегментов, указывающих целевую аудиторию кампании. Дополнительные сведения см. в разделе [Управление сегментами](marketing-segments.md).

### <a name="registering-discount-percentages"></a>Регистрация процентов скидки
При настройке кампании определите, какие сегменты необходимы при работе с данной кампанией, и настройте дату начала и дату окончания. Затем выполните регистрацию процента скидки, которую получит клиент на отдельные товары в строках окна **Скидки строки продажи**. Можно также зарегистрировать цены продажи для отдельных товаров в строках в окне **Цены продажи**. Доступ к обоим окнам можно получить из карточки кампании.

 При настройке цены продажи/скидки строки и сегментов на карточке кампании необходимо их активизировать для отражения в строках цен/скидок кампании.

> [!NOTE]  
>  Для активации цены продажи/скидки строки необходимо указать, что входит в целевую аудиторию кампании: весь сегмент или только некоторые контакты. Если цены продажи/скидки строки охватывают все контакты в сегменте, выберите поле **Цель кампании** на экспресс-вкладке **Кампания** карточки **Сегмент**.
Если цены продажи/скидки строки предлагаются не всем контактам в сегменте, можно снять флажок в поле **Цель кампании** для соответствующих контактов. Если это поле не отображается, его можно добавить в представление. Дополнительные сведения см. в разделе [Персонализация пользователя](ui-user-personalization.md).

<!-- ## Conducting campaigns
As a campaign runs, all interactions with your contacts, or segment, are recorded so that you can get statistics and other information about the costs and success rates of the campaign.

Campaigns are conducted by salespeople, and you must create activities to represent each task and assign them to the relevant salespeople.  -->

## <a name="see-also"></a>См. также
[Управление контактами](marketing-contacts.md)  
[Управление сегментами](marketing-segments.md)  
[Управление возможностями продаж](marketing-manage-sales-opportunities.md)  
[Работа с Financials](ui-work-product.md)  

