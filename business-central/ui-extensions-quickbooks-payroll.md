---
title: Использование расширения импорта файла зарплаты QuickBooks | Документация Майкрософт
description: В этом разделе описывается использование расширения для импорта транзакция по зарплате из Quickbooks.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, salary, wage
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: a63e2139ee4a3ac42e30724d8b7015cc0d968cd9
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3923474"
---
# <a name="the-quickbooks-payroll-file-import-extension"></a>Расширение импорта файла зарплаты QuickBooks
Используйте расширение импорта файла зарплаты QuickBooks для импорта транзакций зарплаты из QuickBooks в счета главной книги в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Например, это может оказаться полезным при переходе с QuickBooks в [!INCLUDE[d365fin](includes/d365fin_md.md)] или если используются сторонние услуги расчета зарплаты, но вы хотите отслеживать зарплату в [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="steps-to-import-payroll-data"></a>Действия для импорта данных по зарплате
Первым шагом вы или, возможно, ваш бухгалтер, должны использовать функции экспорта в QuickBooks для экспорта данных зарплаты в файл IIF. На втором шаге необходимо открыть страницу **Финансовые журналы** в [!INCLUDE[d365fin](includes/d365fin_md.md)] и использовании действие **Импорт транзакций на зарплату** для импорта файла. Во время процесса импорта можно сопоставить счета главной книги из QuickBooks с соответствующими счетами в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Последний шаг — это учет транзакции зарплаты в [!INCLUDE[d365fin](includes/d365fin_md.md)] в соответствии с сопоставлением счетов. 

Дополнительные сведения см. в разделе [Импорт транзакций зарплаты](finance-how-import-payroll-transactions.md).

## <a name="see-also"></a>См. также
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)    
[Финансы](finance.md)    
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
