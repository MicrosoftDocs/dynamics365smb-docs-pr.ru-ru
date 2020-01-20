---
title: Работа с финансовыми обзорами в Excel | Документация Майкрософт
description: Узнайте, как открывать финансовые отчеты в Microsoft Excel из Business Central для более тщательного их анализа.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 01/13/2020
ms.author: edupont
ms.openlocfilehash: 858116d656ef264c7c9445596c8b5345da944c8e
ms.sourcegitcommit: ead69ebe5b29927876a4fb23afb6c066f8854591
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2020
ms.locfileid: "2952581"
---
# <a name="analyzing-financial-statements-in-microsoft-excel"></a>Анализ финансовых отчетов в Microsoft Excel
В [!INCLUDE[d365fin](includes/d365fin_md.md)] можно просматривать ключевые коэффициенты эффективности и получать обзоры финансового состояния организации. Можно также открыть списки в Excel и анализировать данные в нем. Однако также можно экспортировать большие финансовые отчеты, такие как балансовый отчет или отчет о прибылях и убытках в Excel, проанализировать данные и напечатать отчеты.  

В ролевых центрах коммерческого директора и бухгалтера можно выбрать, какие финансовые отчеты просматривать в Excel из раскрывающегося меню в разделе "Отчеты" ленты. При выборе отчета он открывается в Excel или Excel Online. Надстройка связывает данные с [!INCLUDE[d365fin](includes/d365fin_md.md)]. Однако необходимо выполнить вход с теми же учетными данными, которые используются с [!INCLUDE[d365fin](includes/d365fin_md.md)].  

## <a name="getting-the-overview-and-the-details-in-excel"></a>Получение обзора и подробные сведений в Excel
На ленте выберите подходящий отчет Excel и дайте ему открыться, чтобы можно было просмотреть обзор, который вы искали. В этой версии [!INCLUDE[d365fin](includes/d365fin_md.md)] мы предлагаем следующие отчеты Excel:

- Балансовый отчет  
- Отч. о приб. и убыт.  
- Отчет о движении денежных средств  
- Отчет о нераспределенной прибыли  
- Кредиторская задолженность по срокам давности  
- Дебиторская задолженность по срокам давности  

Допустим, требуется подробнее изучить движение денежных средств. Из ролевого центра коммерческого директора или бухгалтера можно открыть отчет о движении денежных средств в Excel, но фактически производится экспорт соответствующих данных и создание книги Excel на основе заранее заданного шаблона. В зависимости от веб-браузера может быть предложено открыть или сохранить книгу.  

В Excel отображается вкладка с данными, скомпонованными на первом листе. Все экспортированные данные также присутствуют на других листах, если они вам потребуются. Можно сразу же напечатать отчет или можно изменить его, чтобы отображался требуемые вам обзорные и подробные сведения. Для дополнительной фильтрации данных и их анализа используйте надстройку [!INCLUDE[d365fin](includes/d365fin_md.md)] Excel.  

## <a name="the-included365finincludesd365fin_mdmd-excel-add-in"></a>Надстройка [!INCLUDE[d365fin](includes/d365fin_md.md)] Excel
Ваш [!INCLUDE[d365fin](includes/d365fin_md.md)] включает в себя надстройку для Excel. В зависимости от подписки, вход выполняется автоматически или необходимо указать те же данные для входа, что и для [!INCLUDE[d365fin](includes/d365fin_md.md)].  

С помощью надстройки можно получать обновленные данные из [!INCLUDE[d365fin](includes/d365fin_md.md)], а также передавать изменения в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Однако возможность передавать данные обратно в базу данных для перечисленных выше финансовых отчетов Excel отключена.  

## <a name="see-related-training-at-microsoft-learnlearnmodulesconfigure-powerbi-excel-dynamics-365-business-centralindex"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также
[Финансы](finance.md)  
[Настройка финансов](finance-setup-finance.md)  
[Главная книга и план счетов](finance-general-ledger.md)  
[Работа с Business Central](ui-work-product.md)  
