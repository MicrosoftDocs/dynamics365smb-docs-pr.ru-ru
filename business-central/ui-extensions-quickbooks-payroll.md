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
ms.openlocfilehash: eae93ea8cf81a2fad6af2c3810f94d5292eef93f
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4757096"
---
# <a name="the-quickbooks-payroll-file-import-extension"></a>Расширение импорта файла зарплаты QuickBooks
Используйте расширение импорта файла зарплаты QuickBooks для импорта транзакций зарплаты из QuickBooks в счета главной книги в [!INCLUDE[prod_short](includes/prod_short.md)]. Например, это может оказаться полезным при переходе с QuickBooks в [!INCLUDE[prod_short](includes/prod_short.md)] или если используются сторонние услуги расчета зарплаты, но вы хотите отслеживать зарплату в [!INCLUDE[prod_short](includes/prod_short.md)].

## <a name="steps-to-import-payroll-data"></a>Действия для импорта данных по зарплате
Первым шагом вы или, возможно, ваш бухгалтер, должны использовать функции экспорта в QuickBooks для экспорта данных зарплаты в файл IIF. На втором шаге необходимо открыть страницу **Финансовые журналы** в [!INCLUDE[prod_short](includes/prod_short.md)] и использовании действие **Импорт транзакций на зарплату** для импорта файла. Во время процесса импорта можно сопоставить счета главной книги из QuickBooks с соответствующими счетами в [!INCLUDE[prod_short](includes/prod_short.md)]. Последний шаг — это учет транзакции зарплаты в [!INCLUDE[prod_short](includes/prod_short.md)] в соответствии с сопоставлением счетов. 

Дополнительные сведения см. в разделе [Импорт транзакций зарплаты](finance-how-import-payroll-transactions.md).

## <a name="see-also"></a>См. также
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)] с помощью расширений](ui-extensions.md)    
[Финансы](finance.md)    
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]