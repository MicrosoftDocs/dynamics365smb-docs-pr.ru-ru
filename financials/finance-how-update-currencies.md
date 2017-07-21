---
title: "Обновление валютных курсов | Документы Майкрософт"
description: "Для использования в бизнесе нескольких валют, можно настроить код по каждой используемой валюте и использовать внешний сервис валютного курса, например Yahoo."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, Yahoo
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: cc60569091b3aa37d17e981f1fae8f46c4a004df
ms.contentlocale: ru-ru
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-update-currency-exchange-rates"></a>Практическое руководство. Обновление валютных курсов
Следует настраивать код по каждой используемой валюте при покупке или продаже в валютах, отличных от местной валюты, при поступлениях или платежах в других валютах или при записи транзакций ГК в других валютах.  

> [!NOTE]  
>   Эта функция требует, чтобы было задано значение **Пакет**. Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).

Для обновления валютных курсов можно использовать внешнюю службу. Служба валютных курсов Yahoo предустановлена и готова к использованию.

## <a name="to-set-up-a-currency-exchange-rate-service"></a>Настройка служб валютных курсов
1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Службы валютных курсов**, а затем выберите связанную ссылку.
2. Выберите действие **Создать**.
3. В окне **Служба валютных курсов** заполните требуемые поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Установите флажок **Включено** для включения службы.

## <a name="to-update-currency-exchange-rates-through-a-service"></a>Обновление валютных курсов с использованием службы
1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Валюты**, а затем выберите связанную ссылку.
2. Выберите действие **Обновить валютные курсы**.

Значение в поле **Валютный курс** в окне **Валюты** обновляется до самого актуального валютного курса.

## <a name="see-also"></a>См. также
[Закрытие года и периодов](year-close-years-periods.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

