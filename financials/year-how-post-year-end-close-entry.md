---
title: "Практическое руководство. Учет операции закрытия года | Документы Майкрософт"
description: "Описывает, как учитывать операцию закрытия года."
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
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: fe04f75ed84a959cbacd9e9d4806d43d41186edb
ms.contentlocale: ru-ru
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-post-year-end-closing-entry"></a>Практическое руководство. Учет операции закрытия года
После использования пакетного задания **Закрытие отчета о прибылях и убытках** для создания закрывающей операции (операций) на конец года необходимо открыть журнал, указанный для пакетного задания, и затем просмотреть и учесть записи.

## <a name="to-post-the-year-end-closing-entry"></a>Учет операции закрытия года
1. В правом вернем углу щелкните значок **Поиск страницы или отчета** ![Поиск страницы или отчета](media/ui-search/search_small.png "значок "Поиск страницы или отчета""), введите **Финансовый журнал** и выберите связанную ссылку.
2. В окне **Финансовый журнал** в поле **Код раздела** выберите раздел, который содержит закрывающие операции.
3. Проверьте записи.
4. Чтобы учесть журнал, выберите действие **Учесть**.

**Примечание**. При обнаружении ошибки отображается сообщение об ошибке. Если учет выполнен успешно, система удалит учтенные записи из журнала. После завершения учета запись учитывается во всех счетах прибылей и убытков, при этом ее сальдо становится нулевым, и результат года переносится в балансовый отчет.

## <a name="see-also"></a>См. также
[Практическое руководство. Закрытие учетных периодов](year-close-account-periods.md)  
[Закрытие книг](year-close-books.md)  
[Закрытие отчета о прибылях и убытках](year-close-income-statement.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

