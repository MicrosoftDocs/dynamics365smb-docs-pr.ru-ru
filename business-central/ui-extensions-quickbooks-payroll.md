---
title: Использование расширения "Импорт файла зарплаты QuickBooks" | Документация Майкрософт
description: В этой статье описывается использование расширения для импорта транзакция по зарплате из Quickbooks.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms. search.keywords: 'app, add-in, manifest, customize, salary, wage'
ms.date: 12/07/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# Расширение "Импорт файла зарплаты QuickBooks"
Используйте расширение импорта файла зарплаты QuickBooks для импорта транзакций зарплаты из QuickBooks в счета главной книги в [!INCLUDE[prod_short](includes/prod_short.md)]. Например, это может оказаться полезным при переходе с QuickBooks на [!INCLUDE[prod_short](includes/prod_short.md)] или если расчетом зарплаты для вас занимается внешняя организация, но вы хотите отслеживать зарплату в [!INCLUDE[prod_short](includes/prod_short.md)].

## Действия для импорта данных по зарплате
Первым шагом вы или, возможно, ваш бухгалтер, должны использовать функции экспорта в QuickBooks для экспорта данных зарплаты в файл IIF. На втором шаге необходимо открыть страницу **Финансовые журналы** в [!INCLUDE[prod_short](includes/prod_short.md)] и использовании действие **Импорт транзакций на зарплату** для импорта файла. В ходе импорта можно сопоставить счета главной книги из QuickBooks с соответствующими счетами в [!INCLUDE[prod_short](includes/prod_short.md)]. Последний шаг — это учет транзакции зарплаты в [!INCLUDE[prod_short](includes/prod_short.md)] в соответствии с сопоставлением счетов. 

Дополнительные сведения см. в разделе [Импорт транзакций зарплаты](finance-how-import-payroll-transactions.md).

## См. также
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)] с помощью расширений](ui-extensions.md)    
[Финансы](finance.md)    
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]