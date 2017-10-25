---
title: "Проверка и учет операции закрытия года | Документы Майкрософт"
description: "Описывается порядок открытия журнала, указанного в пакетном задании \"Закрытие отчета о прибылях и убытках\", и проверки и учета операции закрытия года."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 03/29/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 68017b8b031ee4bd368936b6fb4de157328d7030
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-post-the-year-end-closing-entry"></a>Практическое руководство: учет операции закрытия года
После использования пакетного задания **Закрытие отчета о прибылях и убытках** для создания закрывающей операции (операций) на конец года необходимо открыть журнал, указанный для пакетного задания, и затем просмотреть и учесть записи.

## <a name="to-post-the-year-end-closing-entry"></a>Учет операции закрытия года
1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Финансовый журнал**, а затем выберите связанную ссылку.
2. В окне **Финансовый журнал** в поле **Код раздела** выберите раздел, который содержит закрывающие операции.
3. Проверьте записи.
4. Чтобы учесть журнал, выберите действие **Учесть**.

> [!NOTE]  
>   При обнаружении ошибки отображается сообщение об ошибке. Если учет выполнен успешно, система удалит учтенные записи из журнала. После завершения учета запись учитывается во всех счетах прибылей и убытков, при этом ее сальдо становится нулевым, и результат года переносится в балансовый отчет.

## <a name="see-also"></a>См. также
[Практическое руководство. Закрытие учетных периодов](year-close-account-periods.md)  
[Закрытие книг](year-close-books.md)  
[Закрытие отчета о прибылях и убытках](year-close-income-statement.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

