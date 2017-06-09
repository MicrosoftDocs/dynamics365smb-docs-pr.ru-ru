---
title: "Практическое руководство. Включение операций книги в разных валютах | Документы Майкрософт"
description: "Узнайте, как можно применять операции книги в разных валютах."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, payment, reconcile
ms.date: 03/24/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 4f904d1600d56a83238581915726a7b7fd6cca38
ms.contentlocale: ru-ru
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-enable-application-of-ledger-entries-in-different-currencies"></a>Практическое руководство. Включение операций книги в разных валютах
В случае, если покупка у поставщика была произведена в одной валюте, а оплата проходит в другой валюте, то можно применить данную оплату к данной покупке.

Аналогично, если продажа клиенту осуществляется в одной валюте, а оплата от него поступает в другой валюте, оплату можно применить к счету продажи.

Далее описывается процедура настройки для операций книги поставщиков в окне **Настройка модуля "Покупки"**. Настройка аналогична для операций книги клиентов в **Настройка модуля "Продажи"**.

**Примечание**. Эта функция требует, чтобы было задано значение **Пакет**. Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a>Включение применения операций книги поставщиков в различных валютах
1. В правом вернем углу щелкните значок **Поиск страницы или отчета** ![Поиск страницы или отчета](media/ui-search/search_small.png "значок "Поиск страницы или отчета""), введите **Настройка модуля "Покупки"** и выберите связанную ссылку.
2. В поле **Применение между валютами** выберите один из следующих параметров.

| Параметр | Описание |
| --- | --- |
| Нет |Применение между валютами не разрешено. |
| Евро |Разрешено применение для валют стран ЕС. |
| Все |Разрешено применение для всех валют. |

## <a name="see-also"></a>См. также
[Управление кредиторской задолженностью](payables-manage-payables.md)  
[Управление дебиторской задолженностью](receivables-manage-receivables.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

